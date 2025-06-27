Directory structure:
└── rhydon1337-windows-kernel-dll-injector/
    ├── README.md
    └── DLLInjector/
        ├── DLLInjector.sln
        ├── DLLInjector/
        │   ├── apc.cpp
        │   ├── apc.h
        │   ├── common.h
        │   ├── consts.h
        │   ├── device_handlers.cpp
        │   ├── device_handlers.h
        │   ├── dll_injection.cpp
        │   ├── dll_injection.h
        │   ├── DLLInjector.inf
        │   ├── DLLInjector.vcxproj
        │   ├── DLLInjector.vcxproj.filters
        │   ├── main.cpp
        │   ├── pe.cpp
        │   ├── pe.h
        │   ├── process.cpp
        │   ├── process.h
        │   ├── ProcessReference.cpp
        │   └── ProcessReference.h
        └── DLLInjectorCom/
            ├── DLLInjectorCom.cpp
            ├── DLLInjectorCom.vcxproj
            └── DLLInjectorCom.vcxproj.filters


Files Content:

================================================
FILE: README.md
================================================
# windows-kernel-dll-injector
## TL;DR
Windows kernel mode to user mode dll injection

Tested on Windows x64 1909

Inject a dll to target process from kernel driver

## How its works
The injection process is divided into several stages:

1. Attach current kernel thread to the virtual address space of the target process (KeStackAttachProcess)
2. Parse kernel32.dll PE header and locate LoadLibraryW function address
	* Get current process PEB (PsGetProcessPeb)
	* Iterate over all loaded modules and find kernel32.dll
	* Parse kernel32.dll PE header in order to find the address of LoadLibraryW
3. Allocate and copy to target process the APC callback arguments RW (ZwAllocateVirtualMemory)
4. Allocate and copy to target process the APC callback RWX (ZwAllocateVirtualMemory)
5. Detach from target process address space (KeUnstackDetachProcess)
6. Find all target process threads
	* ZwQuerySystemInformation(SystemProcessInformation...)
	* Iterate over all processes and find the target process by its id
	* Return all threads id of the target process
7. Inject APC to target process in order to execute our APC callback which loads the dll (KeInitializeApc & KeInsertQueueApc)

The whole process described above happens in the kernel driver. The only things that the kernel module needs are: target pid, dll file path.

## Limitations
* The current version supports only in x64 binaries
* The current version doesn't release the APC callback or the APC callback arguments allocations

## Usage

sc create DllInjector binPath= {driver_path} type= kernel

sc start DllInjector

DLLInjectorCom.exe {dll_path} {pid}

DONE!!!



================================================
FILE: DLLInjector/DLLInjector.sln
================================================
﻿
Microsoft Visual Studio Solution File, Format Version 12.00
# Visual Studio Version 16
VisualStudioVersion = 16.0.30907.101
MinimumVisualStudioVersion = 10.0.40219.1
Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "DLLInjector", "DLLInjector\DLLInjector.vcxproj", "{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}"
EndProject
Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "DLLInjectorCom", "DLLInjectorCom\DLLInjectorCom.vcxproj", "{3B559C45-3EBD-4B6C-A434-9E03BA55C797}"
EndProject
Global
	GlobalSection(SolutionConfigurationPlatforms) = preSolution
		Debug|ARM = Debug|ARM
		Debug|ARM64 = Debug|ARM64
		Debug|x64 = Debug|x64
		Debug|x86 = Debug|x86
		Release|ARM = Release|ARM
		Release|ARM64 = Release|ARM64
		Release|x64 = Release|x64
		Release|x86 = Release|x86
	EndGlobalSection
	GlobalSection(ProjectConfigurationPlatforms) = postSolution
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM.ActiveCfg = Debug|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM.Build.0 = Debug|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM.Deploy.0 = Debug|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM64.Build.0 = Debug|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|ARM64.Deploy.0 = Debug|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x64.ActiveCfg = Debug|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x64.Build.0 = Debug|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x64.Deploy.0 = Debug|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x86.ActiveCfg = Debug|Win32
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x86.Build.0 = Debug|Win32
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Debug|x86.Deploy.0 = Debug|Win32
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM.ActiveCfg = Release|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM.Build.0 = Release|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM.Deploy.0 = Release|ARM
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM64.ActiveCfg = Release|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM64.Build.0 = Release|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|ARM64.Deploy.0 = Release|ARM64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x64.ActiveCfg = Release|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x64.Build.0 = Release|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x64.Deploy.0 = Release|x64
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x86.ActiveCfg = Release|Win32
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x86.Build.0 = Release|Win32
		{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}.Release|x86.Deploy.0 = Release|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|ARM.ActiveCfg = Debug|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|ARM64.ActiveCfg = Debug|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|x64.ActiveCfg = Debug|x64
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|x64.Build.0 = Debug|x64
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|x86.ActiveCfg = Debug|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Debug|x86.Build.0 = Debug|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|ARM.ActiveCfg = Release|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|ARM64.ActiveCfg = Release|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|x64.ActiveCfg = Release|x64
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|x64.Build.0 = Release|x64
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|x86.ActiveCfg = Release|Win32
		{3B559C45-3EBD-4B6C-A434-9E03BA55C797}.Release|x86.Build.0 = Release|Win32
	EndGlobalSection
	GlobalSection(SolutionProperties) = preSolution
		HideSolutionNode = FALSE
	EndGlobalSection
	GlobalSection(ExtensibilityGlobals) = postSolution
		SolutionGuid = {3A47E694-3390-40C4-9923-73A6A58F54E7}
	EndGlobalSection
EndGlobal



================================================
FILE: DLLInjector/DLLInjector/apc.cpp
================================================
#include "apc.h"

VOID KernelAPC(PVOID, PVOID, PVOID, PVOID, PVOID) {
}

NTSTATUS call_apc(PKTHREAD target_thread, PVOID target_function, PVOID params) {
    KAPC* apc = static_cast<KAPC*>(ExAllocatePool(NonPagedPool, sizeof(KAPC)));
    if (nullptr == apc) {
        return STATUS_UNSUCCESSFUL;
    }
    KeInitializeApc(apc,
        target_thread,
        OriginalApcEnvironment,
        reinterpret_cast<PKKERNEL_ROUTINE>(KernelAPC),
        nullptr,
        reinterpret_cast<PKNORMAL_ROUTINE>(target_function),
        UserMode,
        params);

    if (!KeInsertQueueApc(apc, nullptr, nullptr, 0)) {
        ExFreePool(apc);
    	return STATUS_UNSUCCESSFUL;
    }
	return STATUS_SUCCESS;
}


================================================
FILE: DLLInjector/DLLInjector/apc.h
================================================
#pragma once

#include <ntifs.h>

typedef enum _KAPC_ENVIRONMENT {
    OriginalApcEnvironment,
    AttachedApcEnvironment,
    CurrentApcEnvironment,
    InsertApcEnvironment
} KAPC_ENVIRONMENT, * PKAPC_ENVIRONMENT;

typedef VOID(NTAPI* PKNORMAL_ROUTINE)(
    _In_ PVOID NormalContext,
    _In_ PVOID SystemArgument1,
    _In_ PVOID SystemArgument2
    );

typedef VOID KKERNEL_ROUTINE(
    _In_ PRKAPC Apc,
    _Inout_opt_ PKNORMAL_ROUTINE* NormalRoutine,
    _Inout_opt_ PVOID* NormalContext,
    _Inout_ PVOID* SystemArgument1,
    _Inout_ PVOID* SystemArgument2
);

typedef KKERNEL_ROUTINE(NTAPI* PKKERNEL_ROUTINE);

typedef VOID(NTAPI* PKRUNDOWN_ROUTINE)(_In_ PRKAPC Apc);

extern "C" VOID NTAPI KeInitializeApc(
    _Out_ PRKAPC Apc,
    _In_ PRKTHREAD Thread,
    _In_ KAPC_ENVIRONMENT Environment,
    _In_ PKKERNEL_ROUTINE KernelRoutine,
    _In_opt_ PKRUNDOWN_ROUTINE RundownRoutine,
    _In_opt_ PKNORMAL_ROUTINE NormalRoutine,
    _In_opt_ KPROCESSOR_MODE ProcessorMode,
    _In_opt_ PVOID NormalContext
);

extern "C" BOOLEAN NTAPI KeInsertQueueApc(
    _Inout_ PRKAPC Apc,
    _In_opt_ PVOID SystemArgument1,
    _In_opt_ PVOID SystemArgument2,
    _In_ KPRIORITY Increment
);

NTSTATUS call_apc(PKTHREAD target_thread, PVOID target_function, PVOID params);



================================================
FILE: DLLInjector/DLLInjector/common.h
================================================
#pragma once

struct InjectDllArgs {
	size_t pid;
	wchar_t dll_path[256];
};

#define INJECT_DLL_IOCTL CTL_CODE(FILE_DEVICE_UNKNOWN, 0x1337, METHOD_BUFFERED, FILE_WRITE_DATA)


================================================
FILE: DLLInjector/DLLInjector/consts.h
================================================
#pragma once

#define NT_DEVICE_NAME L"\\Device\\DLLInjector"
#define DOS_DEVICE_NAME L"\\DosDevices\\DLLInjector"

#define CHECK(ntstatus) if (!NT_SUCCESS(ntstatus)) { return ntstatus;}

#define DELETE_DEFAULT_CTORS(class_name) \
	class_name(class_name const&) = delete; \
	class_name& operator =(class_name const&) = delete; \
	class_name(class_name&&) = delete; \
	class_name& operator=(class_name&&) = delete \


================================================
FILE: DLLInjector/DLLInjector/device_handlers.cpp
================================================
#include "device_handlers.h"

#include "common.h"
#include "dll_injection.h"

NTSTATUS device_create_close(PDEVICE_OBJECT device_object, PIRP irp) {
	UNREFERENCED_PARAMETER(device_object);
	irp->IoStatus.Status = STATUS_SUCCESS;
	irp->IoStatus.Information = 0;

	IoCompleteRequest(irp, IO_NO_INCREMENT);

	return STATUS_SUCCESS;
}

NTSTATUS device_ioctl(PDEVICE_OBJECT device_object, PIRP irp) {
	UNREFERENCED_PARAMETER(device_object);

	NTSTATUS nt_status;
	PIO_STACK_LOCATION  irp_stack_location = IoGetCurrentIrpStackLocation(irp);
	size_t input_buffer_length = irp_stack_location->Parameters.DeviceIoControl.InputBufferLength;

	switch (irp_stack_location->Parameters.DeviceIoControl.IoControlCode) {
	case INJECT_DLL_IOCTL:
	{
		if (input_buffer_length != sizeof InjectDllArgs) {
			nt_status = STATUS_INVALID_PARAMETER;
			break;
		}
		auto args = static_cast<InjectDllArgs*>(irp->AssociatedIrp.SystemBuffer);
		nt_status = inject_dll(*args);
	}
	break;
	default:
	{
		nt_status = STATUS_INVALID_DEVICE_REQUEST;
	}
	break;
	}

	irp->IoStatus.Status = nt_status;
	IoCompleteRequest(irp, IO_NO_INCREMENT);
	return nt_status;
}



================================================
FILE: DLLInjector/DLLInjector/device_handlers.h
================================================
#pragma once
#include <ntifs.h>


NTSTATUS device_create_close(PDEVICE_OBJECT device_object, PIRP irp);

NTSTATUS device_ioctl(PDEVICE_OBJECT device_object, PIRP irp);


================================================
FILE: DLLInjector/DLLInjector/dll_injection.cpp
================================================
#include "dll_injection.h"

#include <ntifs.h>

#include "consts.h"
#include "ProcessReference.h"
#include "apc.h"
#include "process.h"
#include "pe.h"

using LoadLibraryW = HANDLE(*)(LPCWSTR lpLibFileName);

struct UserApcArgs {
	wchar_t dll_path[256];
	LoadLibraryW load_library;
};

#pragma optimize("", off)
#pragma runtime_checks("", off )
void user_mode_apc_callback(UserApcArgs* args, PVOID, PVOID) {
	args->load_library(args->dll_path);
}

void user_mode_apc_callback_end() {}
#pragma runtime_checks("", restore)
#pragma optimize("", on)


NTSTATUS inject_dll(const InjectDllArgs& inject_dll_args) {
	PVOID injected_apc_args = nullptr;
	PVOID injected_apc_callback = nullptr;
	ProcessInfo process_info;
	PKTHREAD target_thread;
	{
		// Attack to target process
		ProcessReference process_reference;
		CHECK(process_reference.init(inject_dll_args.pid, true));

		UserApcArgs user_apc_args;
		memcpy(&user_apc_args.dll_path, &inject_dll_args.dll_path, 256);
		user_apc_args.load_library = (LoadLibraryW)get_module_symbol_address((wchar_t*)L"KERNEL32.DLL", "LoadLibraryW");
		if (nullptr == user_apc_args.load_library) {
			return STATUS_UNSUCCESSFUL;
		}

		// Allocate and copy the dll path to target process
		SIZE_T apc_args_allocation_size = sizeof(UserApcArgs);
		CHECK(ZwAllocateVirtualMemory(NtCurrentProcess(), &injected_apc_args, 0, &apc_args_allocation_size, MEM_COMMIT, PAGE_READWRITE));
		RtlCopyMemory(injected_apc_args, &user_apc_args, sizeof(UserApcArgs));

		// Allocate and copy the apc user mode callback code to target process
		SIZE_T code_size = reinterpret_cast<ULONG_PTR>(user_mode_apc_callback_end) - reinterpret_cast<ULONG_PTR>(user_mode_apc_callback);
		if (!NT_SUCCESS(ZwAllocateVirtualMemory(NtCurrentProcess(), &injected_apc_callback, NULL, &code_size, MEM_COMMIT, PAGE_EXECUTE_READWRITE))) {
			ZwFreeVirtualMemory(NtCurrentProcess(), &injected_apc_args, &apc_args_allocation_size, MEM_RELEASE);
			return STATUS_UNSUCCESSFUL;
		}

		RtlCopyMemory(injected_apc_callback, &user_mode_apc_callback, reinterpret_cast<ULONG_PTR>(user_mode_apc_callback_end) - reinterpret_cast<ULONG_PTR>(user_mode_apc_callback));
	}

	CHECK(get_process_info_by_pid(inject_dll_args.pid, &process_info));

	for (size_t i = 0; i < process_info.number_of_threads; i++) {
		if (!NT_SUCCESS(PsLookupThreadByThreadId((HANDLE)process_info.threads_id[i], &target_thread))) {
			ExFreePool(process_info.threads_id);
			return STATUS_UNSUCCESSFUL;
		}

		// Execute LoadLibrary in the target process in order to load our dll
		call_apc(target_thread, injected_apc_callback, injected_apc_args);
		ObDereferenceObject(target_thread);
	}
	return STATUS_SUCCESS;
}



================================================
FILE: DLLInjector/DLLInjector/dll_injection.h
================================================
#pragma once
#include <ntdef.h>

#include "common.h"

NTSTATUS inject_dll(const InjectDllArgs& inject_dll_args);


================================================
FILE: DLLInjector/DLLInjector/DLLInjector.inf
================================================
;
; DLLInjector.inf
;

[Version]
Signature="$WINDOWS NT$"
Class=System
ClassGuid={4d36e97d-e325-11ce-bfc1-08002be10318}
Provider=%ManufacturerName%
DriverVer=
CatalogFile=DLLInjector.cat

[DestinationDirs]
DefaultDestDir = 12


[SourceDisksNames]
1 = %DiskName%,,,""

[SourceDisksFiles]


[Manufacturer]
%ManufacturerName%=Standard,NT$ARCH$

[Standard.NT$ARCH$]


[Strings]
ManufacturerName="<Your manufacturer name>" ;TODO: Replace with your manufacturer name
ClassName=""
DiskName="DLLInjector Source Disk"



================================================
FILE: DLLInjector/DLLInjector/DLLInjector.vcxproj
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<Project DefaultTargets="Build" ToolsVersion="12.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <ItemGroup Label="ProjectConfigurations">
    <ProjectConfiguration Include="Debug|Win32">
      <Configuration>Debug</Configuration>
      <Platform>Win32</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|Win32">
      <Configuration>Release</Configuration>
      <Platform>Win32</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Debug|x64">
      <Configuration>Debug</Configuration>
      <Platform>x64</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|x64">
      <Configuration>Release</Configuration>
      <Platform>x64</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Debug|ARM">
      <Configuration>Debug</Configuration>
      <Platform>ARM</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|ARM">
      <Configuration>Release</Configuration>
      <Platform>ARM</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Debug|ARM64">
      <Configuration>Debug</Configuration>
      <Platform>ARM64</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|ARM64">
      <Configuration>Release</Configuration>
      <Platform>ARM64</Platform>
    </ProjectConfiguration>
  </ItemGroup>
  <PropertyGroup Label="Globals">
    <ProjectGuid>{3CAA899B-B384-42CA-ABB1-7FEEE57B31BB}</ProjectGuid>
    <TemplateGuid>{dd38f7fc-d7bd-488b-9242-7d8754cde80d}</TemplateGuid>
    <TargetFrameworkVersion>v4.5</TargetFrameworkVersion>
    <MinimumVisualStudioVersion>12.0</MinimumVisualStudioVersion>
    <Configuration>Debug</Configuration>
    <Platform Condition="'$(Platform)' == ''">Win32</Platform>
    <RootNamespace>DLLInjector</RootNamespace>
  </PropertyGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props" />
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|ARM'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|ARM'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|ARM64'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|ARM64'" Label="Configuration">
    <TargetVersion>Windows10</TargetVersion>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>WindowsKernelModeDriver10.0</PlatformToolset>
    <ConfigurationType>Driver</ConfigurationType>
    <DriverType>WDM</DriverType>
  </PropertyGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props" />
  <ImportGroup Label="ExtensionSettings">
  </ImportGroup>
  <ImportGroup Label="PropertySheets">
    <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform" />
  </ImportGroup>
  <PropertyGroup Label="UserMacros" />
  <PropertyGroup />
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|ARM'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|ARM'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|ARM64'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|ARM64'">
    <DebuggerFlavor>DbgengKernelDebugger</DebuggerFlavor>
  </PropertyGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <ClCompile>
      <BufferSecurityCheck>false</BufferSecurityCheck>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <ClCompile>
      <ControlFlowGuard>false</ControlFlowGuard>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <ClCompile>
      <FunctionLevelLinking>false</FunctionLevelLinking>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <ClCompile>
      <BufferSecurityCheck>false</BufferSecurityCheck>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <ClCompile>
      <ControlFlowGuard>false</ControlFlowGuard>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <ClCompile>
      <FunctionLevelLinking>false</FunctionLevelLinking>
    </ClCompile>
  </ItemDefinitionGroup>
  <ItemGroup>
    <Inf Include="DLLInjector.inf" />
  </ItemGroup>
  <ItemGroup>
    <FilesToPackage Include="$(TargetPath)" />
  </ItemGroup>
  <ItemGroup>
    <ClCompile Include="apc.cpp" />
    <ClCompile Include="device_handlers.cpp" />
    <ClCompile Include="dll_injection.cpp" />
    <ClCompile Include="main.cpp" />
    <ClCompile Include="pe.cpp" />
    <ClCompile Include="process.cpp" />
    <ClCompile Include="ProcessReference.cpp" />
  </ItemGroup>
  <ItemGroup>
    <ClInclude Include="apc.h" />
    <ClInclude Include="common.h" />
    <ClInclude Include="consts.h" />
    <ClInclude Include="device_handlers.h" />
    <ClInclude Include="dll_injection.h" />
    <ClInclude Include="pe.h" />
    <ClInclude Include="process.h" />
    <ClInclude Include="ProcessReference.h" />
  </ItemGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets" />
  <ImportGroup Label="ExtensionTargets">
  </ImportGroup>
</Project>


================================================
FILE: DLLInjector/DLLInjector/DLLInjector.vcxproj.filters
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <ItemGroup>
    <Filter Include="Source Files">
      <UniqueIdentifier>{4FC737F1-C7A5-4376-A066-2A32D752A2FF}</UniqueIdentifier>
      <Extensions>cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx</Extensions>
    </Filter>
    <Filter Include="Header Files">
      <UniqueIdentifier>{93995380-89BD-4b04-88EB-625FBE52EBFB}</UniqueIdentifier>
      <Extensions>h;hpp;hxx;hm;inl;inc;xsd</Extensions>
    </Filter>
    <Filter Include="Resource Files">
      <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
    </Filter>
    <Filter Include="Driver Files">
      <UniqueIdentifier>{8E41214B-6785-4CFE-B992-037D68949A14}</UniqueIdentifier>
      <Extensions>inf;inv;inx;mof;mc;</Extensions>
    </Filter>
  </ItemGroup>
  <ItemGroup>
    <Inf Include="DLLInjector.inf">
      <Filter>Driver Files</Filter>
    </Inf>
  </ItemGroup>
  <ItemGroup>
    <ClCompile Include="main.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="device_handlers.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="dll_injection.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="ProcessReference.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="apc.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="process.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="pe.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
  </ItemGroup>
  <ItemGroup>
    <ClInclude Include="consts.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="device_handlers.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="common.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="dll_injection.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="ProcessReference.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="apc.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="process.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="pe.h">
      <Filter>Header Files</Filter>
    </ClInclude>
  </ItemGroup>
</Project>


================================================
FILE: DLLInjector/DLLInjector/main.cpp
================================================
#include <ntifs.h>

#include "device_handlers.h"
#include "consts.h"

void driver_unload(PDRIVER_OBJECT driver_object) {
	UNICODE_STRING  win32_name;
	RtlInitUnicodeString(&win32_name, DOS_DEVICE_NAME);
	IoDeleteSymbolicLink(&win32_name);
	if (nullptr != driver_object->DeviceObject) {
		IoDeleteDevice(driver_object->DeviceObject);
	}
}

extern "C" NTSTATUS DriverEntry(PDRIVER_OBJECT DriverObject, PUNICODE_STRING RegistryPath) {
	UNREFERENCED_PARAMETER(RegistryPath);

	DbgPrint("Hello from driver entry\n");

	UNICODE_STRING  nt_name;
	UNICODE_STRING  win32_name;
	PDEVICE_OBJECT  device_object = nullptr;

	RtlInitUnicodeString(&nt_name, NT_DEVICE_NAME);
	NTSTATUS nt_status = IoCreateDevice(DriverObject, 0, &nt_name,
		FILE_DEVICE_UNKNOWN, FILE_DEVICE_SECURE_OPEN,
		TRUE, &device_object);

	if (!NT_SUCCESS(nt_status)) {
		DbgPrint("Couldn't create the device object\n");
		return nt_status;
	}

	DriverObject->MajorFunction[IRP_MJ_CREATE] = device_create_close;
	DriverObject->MajorFunction[IRP_MJ_CLOSE] = device_create_close;
	DriverObject->MajorFunction[IRP_MJ_DEVICE_CONTROL] = device_ioctl;
	DriverObject->DriverUnload = driver_unload;

	RtlInitUnicodeString(&win32_name, DOS_DEVICE_NAME);

	nt_status = IoCreateSymbolicLink(&win32_name, &nt_name);
	if (!NT_SUCCESS(nt_status)) {
		DbgPrint("Couldn't create symbolic link\n");
		IoDeleteDevice(device_object);
	}

	return nt_status;
}


================================================
FILE: DLLInjector/DLLInjector/pe.cpp
================================================
#include "pe.h"

#define IMAGE_NUMBEROF_DIRECTORY_ENTRIES 16
#define IMAGE_DIRECTORY_ENTRY_EXPORT 0

typedef unsigned long       DWORD;
typedef int                 BOOL;
typedef unsigned char       BYTE;
typedef unsigned short      WORD;

typedef struct _PEB_LDR_DATA {
	ULONG                   Length;
	BOOLEAN                 Initialized;
	PVOID                   SsHandle;
	LIST_ENTRY              InLoadOrderModuleList;
	LIST_ENTRY              InMemoryOrderModuleList;
	LIST_ENTRY              InInitializationOrderModuleList;
} PEB_LDR_DATA, * PPEB_LDR_DATA;


typedef struct _PEB {
	BYTE Reserved1[2];
	BYTE BeingDebugged;
	BYTE Reserved2[1];
	PVOID Reserved3[2];
	PPEB_LDR_DATA Ldr;
	PVOID ProcessParameters;
	PVOID Reserved4[3];
	PVOID AtlThunkSListPtr;
	PVOID Reserved5;
	ULONG Reserved6;
	PVOID Reserved7;
	ULONG Reserved8;
	ULONG AtlThunkSListPtr32;
	PVOID Reserved9[45];
	BYTE Reserved10[96];
	PVOID PostProcessInitRoutine;
	BYTE Reserved11[128];
	PVOID Reserved12[1];
	ULONG SessionId;
} PEB, * PPEB;

//0x110 bytes (sizeof)
struct LDR_DATA_TABLE_ENTRY {
	struct _LIST_ENTRY InLoadOrderLinks;                                    //0x0
	struct _LIST_ENTRY InMemoryOrderLinks;                                  //0x10
	union
	{
		struct _LIST_ENTRY InInitializationOrderLinks;                      //0x20
		struct _LIST_ENTRY InProgressLinks;                                 //0x20
	};
	VOID* DllBase;                                                          //0x30
	VOID* EntryPoint;                                                       //0x38
	ULONG SizeOfImage;                                                      //0x40
	struct _UNICODE_STRING FullDllName;                                     //0x48
	struct _UNICODE_STRING BaseDllName;                                     //0x58
	union
	{
		UCHAR FlagGroup[4];                                                 //0x68
		ULONG Flags;                                                        //0x68
		struct
		{
			ULONG PackagedBinary : 1;                                         //0x68
			ULONG MarkedForRemoval : 1;                                       //0x68
			ULONG ImageDll : 1;                                               //0x68
			ULONG LoadNotificationsSent : 1;                                  //0x68
			ULONG TelemetryEntryProcessed : 1;                                //0x68
			ULONG ProcessStaticImport : 1;                                    //0x68
			ULONG InLegacyLists : 1;                                          //0x68
			ULONG InIndexes : 1;                                              //0x68
			ULONG ShimDll : 1;                                                //0x68
			ULONG InExceptionTable : 1;                                       //0x68
			ULONG ReservedFlags1 : 2;                                         //0x68
			ULONG LoadInProgress : 1;                                         //0x68
			ULONG ReservedFlags2 : 1;                                         //0x68
			ULONG EntryProcessed : 1;                                         //0x68
			ULONG ReservedFlags3 : 3;                                         //0x68
			ULONG DontCallForThreads : 1;                                     //0x68
			ULONG ProcessAttachCalled : 1;                                    //0x68
			ULONG ProcessAttachFailed : 1;                                    //0x68
			ULONG CorDeferredValidate : 1;                                    //0x68
			ULONG CorImage : 1;                                               //0x68
			ULONG DontRelocate : 1;                                           //0x68
			ULONG CorILOnly : 1;                                              //0x68
			ULONG ReservedFlags5 : 3;                                         //0x68
			ULONG Redirected : 1;                                             //0x68
			ULONG ReservedFlags6 : 2;                                         //0x68
			ULONG CompatDatabaseProcessed : 1;                                //0x68
		}A;
	};
	USHORT ObsoleteLoadCount;                                               //0x6c
	USHORT TlsIndex;                                                        //0x6e
	struct _LIST_ENTRY HashLinks;                                           //0x70
	ULONG TimeDateStamp;                                                    //0x80
	struct _ACTIVATION_CONTEXT* EntryPointActivationContext;                //0x88
	VOID* PatchInformation;                                                 //0x90
	struct _LDR_DDAG_NODE* DdagNode;                                        //0x98
	struct _LIST_ENTRY NodeModuleLink;                                      //0xa0
	struct _LDRP_DLL_SNAP_CONTEXT* SnapContext;                             //0xb0
	VOID* ParentDllBase;                                                    //0xb8
	VOID* SwitchBackContext;                                                //0xc0
	struct _RTL_BALANCED_NODE BaseAddressIndexNode;                         //0xc8
	struct _RTL_BALANCED_NODE MappingInfoIndexNode;                         //0xe0
	ULONGLONG OriginalBase;                                                 //0xf8
	union _LARGE_INTEGER LoadTime;                                          //0x100
	ULONG BaseNameHashValue;                                                //0x108
	enum _LDR_DLL_LOAD_REASON LoadReason;                                   //0x10c
};

typedef struct _IMAGE_DOS_HEADER
{
	WORD e_magic;
	WORD e_cblp;
	WORD e_cp;
	WORD e_crlc;
	WORD e_cparhdr;
	WORD e_minalloc;
	WORD e_maxalloc;
	WORD e_ss;
	WORD e_sp;
	WORD e_csum;
	WORD e_ip;
	WORD e_cs;
	WORD e_lfarlc;
	WORD e_ovno;
	WORD e_res[4];
	WORD e_oemid;
	WORD e_oeminfo;
	WORD e_res2[10];
	LONG e_lfanew;
} IMAGE_DOS_HEADER, * PIMAGE_DOS_HEADER;

typedef struct _IMAGE_FILE_HEADER {
	WORD  Machine;
	WORD  NumberOfSections;
	DWORD TimeDateStamp;
	DWORD PointerToSymbolTable;
	DWORD NumberOfSymbols;
	WORD  SizeOfOptionalHeader;
	WORD  Characteristics;
} IMAGE_FILE_HEADER, * PIMAGE_FILE_HEADER;

typedef struct _IMAGE_DATA_DIRECTORY {
	DWORD VirtualAddress;
	DWORD Size;
} IMAGE_DATA_DIRECTORY, * PIMAGE_DATA_DIRECTORY;

typedef struct _IMAGE_OPTIONAL_HEADER64 {
	WORD                 Magic;
	BYTE                 MajorLinkerVersion;
	BYTE                 MinorLinkerVersion;
	DWORD                SizeOfCode;
	DWORD                SizeOfInitializedData;
	DWORD                SizeOfUninitializedData;
	DWORD                AddressOfEntryPoint;
	DWORD                BaseOfCode;
	ULONGLONG            ImageBase;
	DWORD                SectionAlignment;
	DWORD                FileAlignment;
	WORD                 MajorOperatingSystemVersion;
	WORD                 MinorOperatingSystemVersion;
	WORD                 MajorImageVersion;
	WORD                 MinorImageVersion;
	WORD                 MajorSubsystemVersion;
	WORD                 MinorSubsystemVersion;
	DWORD                Win32VersionValue;
	DWORD                SizeOfImage;
	DWORD                SizeOfHeaders;
	DWORD                CheckSum;
	WORD                 Subsystem;
	WORD                 DllCharacteristics;
	ULONGLONG            SizeOfStackReserve;
	ULONGLONG            SizeOfStackCommit;
	ULONGLONG            SizeOfHeapReserve;
	ULONGLONG            SizeOfHeapCommit;
	DWORD                LoaderFlags;
	DWORD                NumberOfRvaAndSizes;
	IMAGE_DATA_DIRECTORY DataDirectory[IMAGE_NUMBEROF_DIRECTORY_ENTRIES];
} IMAGE_OPTIONAL_HEADER64, * PIMAGE_OPTIONAL_HEADER64;

typedef struct _IMAGE_NT_HEADERS64 {
	DWORD                   Signature;
	IMAGE_FILE_HEADER       FileHeader;
	IMAGE_OPTIONAL_HEADER64 OptionalHeader;
} IMAGE_NT_HEADERS64, * PIMAGE_NT_HEADERS64;

typedef struct _IMAGE_EXPORT_DIRECTORY {
	ULONG Characteristics;
	ULONG TimeDateStamp;
	USHORT MajorVersion;
	USHORT MinorVersion;
	ULONG Name;
	ULONG Base;
	ULONG NumberOfFunctions;
	ULONG NumberOfNames;
	ULONG AddressOfFunctions;
	ULONG AddressOfNames;
	ULONG AddressOfNameOrdinals;
} IMAGE_EXPORT_DIRECTORY, * PIMAGE_EXPORT_DIRECTORY;

extern "C" PPEB NTAPI PsGetProcessPeb(IN PEPROCESS Process);

PVOID find_symbol_address(BYTE* module_address, char* symbol_name) {
	auto dos_header = (IMAGE_DOS_HEADER*)module_address;
	auto nt_headers64 = (IMAGE_NT_HEADERS64*)(module_address + dos_header->e_lfanew);
	auto optional_header = (IMAGE_OPTIONAL_HEADER64*)&nt_headers64->OptionalHeader;
	auto export_directory = &optional_header->DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT];
	auto export_table = (IMAGE_EXPORT_DIRECTORY*)(module_address + export_directory->VirtualAddress);
	for (size_t i = 0; i < export_table->NumberOfNames; i++) {
		auto function_name_offset = *(ULONG*)(module_address + export_table->AddressOfNames + (sizeof(export_table->AddressOfNames) * i));
		auto function_name = (char*)module_address + (size_t)function_name_offset;
		if (0 == strcmp(function_name, symbol_name)) {
			return module_address + *(ULONG*)(module_address + export_table->AddressOfFunctions + (sizeof(export_table->AddressOfFunctions) * i));
		}
	}
	return nullptr;
}

PVOID get_module_symbol_address(wchar_t* module_name, char* symbol_name) {
	PPEB peb = PsGetProcessPeb(PsGetCurrentProcess());
	auto module_entry = (LDR_DATA_TABLE_ENTRY*)((char*)peb->Ldr->InLoadOrderModuleList.Flink);
	do {
		if (nullptr != wcsstr(module_entry->FullDllName.Buffer, module_name)) {
			return find_symbol_address((BYTE*)module_entry->DllBase, symbol_name);
		}
		module_entry = (LDR_DATA_TABLE_ENTRY*)((char*)module_entry->InLoadOrderLinks.Flink);
	}
	while (module_entry != nullptr);
	return nullptr;
}


================================================
FILE: DLLInjector/DLLInjector/pe.h
================================================
#pragma once

#include <wdm.h>

PVOID get_module_symbol_address(wchar_t* module_name, char* symbol_name);


================================================
FILE: DLLInjector/DLLInjector/process.cpp
================================================
#include "process.h"

#include <wdm.h>

#define SystemProcessInformation 5

extern "C" NTSTATUS NTAPI ZwQuerySystemInformation(IN size_t SystemInformationClass,
                                                   OUT PVOID SystemInformation,
                                                   IN ULONG SystemInformationLength,
                                                   OUT PULONG ReturnLength OPTIONAL);
typedef struct _VM_COUNTERS {
    SIZE_T PeakVirtualSize;
    SIZE_T VirtualSize;
    ULONG PageFaultCount;
    // Padding here in 64-bit
    SIZE_T PeakWorkingSetSize;
    SIZE_T WorkingSetSize;
    SIZE_T QuotaPeakPagedPoolUsage;
    SIZE_T QuotaPagedPoolUsage;
    SIZE_T QuotaPeakNonPagedPoolUsage;
    SIZE_T QuotaNonPagedPoolUsage;
    SIZE_T PagefileUsage;
    SIZE_T PeakPagefileUsage;
} VM_COUNTERS;

struct SYSTEM_THREAD_INFORMATION {
    ULONGLONG KernelTime;
    ULONGLONG UserTime;
    ULONGLONG CreateTime;
    ULONG WaitTime;
    // Padding here in 64-bit
    PVOID StartAddress;
    CLIENT_ID ClientId;
    KPRIORITY Priority;
    LONG BasePriority;
    ULONG ContextSwitchCount;
    ULONG State;
    KWAIT_REASON WaitReason;
};

typedef struct _IO_COUNTERS {
    ULONGLONG ReadOperationCount;
    ULONGLONG WriteOperationCount;
    ULONGLONG OtherOperationCount;
    ULONGLONG ReadTransferCount;
    ULONGLONG WriteTransferCount;
    ULONGLONG OtherTransferCount;
} IO_COUNTERS;

struct SYSTEM_PROCESS_INFORMATION {
    ULONG NextEntryOffset;
    ULONG NumberOfThreads;
    ULONGLONG WorkingSetPrivateSize;
    ULONG HardFaultCount;
    ULONG Reserved1;
    ULONGLONG CycleTime;
    ULONGLONG CreateTime;
    ULONGLONG UserTime;
    ULONGLONG KernelTime;
    UNICODE_STRING ImageName;
    KPRIORITY BasePriority;
    HANDLE ProcessId;
    HANDLE ParentProcessId;
    ULONG HandleCount;
    ULONG Reserved2[2];
    // Padding here in 64-bit
    VM_COUNTERS VirtualMemoryCounters;
    size_t Reserved3;
    IO_COUNTERS IoCounters;
    SYSTEM_THREAD_INFORMATION Threads[1];
};

PVOID get_all_processes() {
    size_t processes_allocation_size = 0;
    PVOID processes_pool = nullptr;

    while (true) {
        processes_allocation_size += 0x10000;
        processes_pool = ExAllocatePool(PagedPool, processes_allocation_size);

        auto status = ZwQuerySystemInformation(SystemProcessInformation, processes_pool, (ULONG)processes_allocation_size, nullptr);
        if (status == STATUS_INFO_LENGTH_MISMATCH) {
            ExFreePool(processes_pool);
        }
        else {
            break;
        }
    }
    return processes_pool;
}

NTSTATUS get_process_info_by_pid(size_t pid, ProcessInfo* process_info) {
    size_t number_of_processes = 0;
    ProcessInfo* processes = get_processes_info(&number_of_processes);
    if (nullptr == processes) {
        return STATUS_UNSUCCESSFUL;
    }
    for (size_t i = 0; i < number_of_processes; i++) {
	    if (pid == (processes + i)->process_id) {
            *process_info = *(processes + i);
            (processes + i)->threads_id = nullptr;
	    }
    }
    for (size_t i = 0; i < number_of_processes; i++) {
    	if (nullptr != (processes + i)->threads_id && (processes + i)->number_of_threads > 0) {
            ExFreePool((processes + i)->threads_id);
    	}
    }
    ExFreePool(processes);
	return STATUS_SUCCESS;
}

ProcessInfo* get_processes_info(size_t* number_of_processes) {
    PVOID all_processes = get_all_processes();
    if (nullptr == all_processes) {
        return nullptr;
    }
    *number_of_processes = 0;
    for (auto process = (SYSTEM_PROCESS_INFORMATION*)all_processes; process->NextEntryOffset != 0;
        process = (SYSTEM_PROCESS_INFORMATION*)((char*)process + process->NextEntryOffset)) {
        *number_of_processes += 1;
    }

    auto processes_info = (ProcessInfo*)ExAllocatePool(PagedPool, sizeof(ProcessInfo) * *number_of_processes);

    size_t i = 0;
    for (auto process = (SYSTEM_PROCESS_INFORMATION*)all_processes; process->NextEntryOffset != 0;
        process = (SYSTEM_PROCESS_INFORMATION*)((char*)process + process->NextEntryOffset), ++i) {
        (processes_info + i)->process_id = (size_t)process->ProcessId;
		(processes_info + i)->number_of_threads = (size_t)process->NumberOfThreads;
        if (0 == process->NumberOfThreads) {
            continue;
        }
    	(processes_info + i)->threads_id = (size_t*)ExAllocatePool(PagedPool, sizeof(size_t) * process->NumberOfThreads);
    	for (size_t j = 0; j < process->NumberOfThreads; j++) {
            *(((ProcessInfo*)(processes_info + i))->threads_id + j) = (size_t)process->Threads[j].ClientId.UniqueThread;
        }
    }

    ExFreePool(all_processes);
    return processes_info;
}



================================================
FILE: DLLInjector/DLLInjector/process.h
================================================
#pragma once
#include <wdm.h>

struct ProcessInfo {
	size_t process_id;
	size_t number_of_threads;
	size_t* threads_id;
};

ProcessInfo* get_processes_info(size_t* number_of_processes);

NTSTATUS get_process_info_by_pid(size_t pid, ProcessInfo* process_info);


================================================
FILE: DLLInjector/DLLInjector/ProcessReference.cpp
================================================
#include "ProcessReference.h"

ProcessReference::ProcessReference()
	: m_process(nullptr) {
}

ProcessReference::~ProcessReference() {
	if (nullptr != m_process) {
		ObDereferenceObject(m_process);
		if (m_attach) {
			KeUnstackDetachProcess(m_apc_state);
			ExFreePool(m_apc_state);
		}
	}

}

NTSTATUS ProcessReference::init(size_t pid, bool attach) {
	CHECK(PsLookupProcessByProcessId(reinterpret_cast<HANDLE>(pid), &m_process));
	m_attach = attach;
	if (attach) {
		m_apc_state = (KAPC_STATE*)ExAllocatePool(NonPagedPool, sizeof(KAPC_STATE));
		KeStackAttachProcess(m_process, m_apc_state);
	}
	return STATUS_SUCCESS;
}



================================================
FILE: DLLInjector/DLLInjector/ProcessReference.h
================================================
#pragma once

#include <ntifs.h>

#include "consts.h"

class ProcessReference {
public:
	ProcessReference();
	~ProcessReference();

	NTSTATUS init(size_t pid, bool attach);

	DELETE_DEFAULT_CTORS(ProcessReference);
private:
	PEPROCESS m_process;
	bool m_attach{};
	KAPC_STATE* m_apc_state;
};




================================================
FILE: DLLInjector/DLLInjectorCom/DLLInjectorCom.cpp
================================================
#include <Windows.h>
#include <iostream>
#include <string>

#include "../DLLInjector/common.h"

int wmain(int, wchar_t** argv) {
    std::cout << "Hello World!\n";
	HANDLE driver = CreateFileA("\\\\.\\DLLInjector", GENERIC_ALL, 0,
		nullptr, OPEN_EXISTING, FILE_ATTRIBUTE_NORMAL, nullptr);
    if (INVALID_HANDLE_VALUE == driver) {
		return 1;
    }
	InjectDllArgs args = {};
	memcpy(args.dll_path, argv[1], wcslen(argv[1]) * sizeof(wchar_t));
	args.pid = std::stoi(argv[2]);

	DeviceIoControl(driver, INJECT_DLL_IOCTL, &args, sizeof(InjectDllArgs),
		nullptr, 0, nullptr, nullptr);

	CloseHandle(driver);
	return 0;
}


================================================
FILE: DLLInjector/DLLInjectorCom/DLLInjectorCom.vcxproj
================================================
<?xml version="1.0" encoding="utf-8"?>
<Project DefaultTargets="Build" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <ItemGroup Label="ProjectConfigurations">
    <ProjectConfiguration Include="Debug|Win32">
      <Configuration>Debug</Configuration>
      <Platform>Win32</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|Win32">
      <Configuration>Release</Configuration>
      <Platform>Win32</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Debug|x64">
      <Configuration>Debug</Configuration>
      <Platform>x64</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|x64">
      <Configuration>Release</Configuration>
      <Platform>x64</Platform>
    </ProjectConfiguration>
  </ItemGroup>
  <PropertyGroup Label="Globals">
    <VCProjectVersion>16.0</VCProjectVersion>
    <Keyword>Win32Proj</Keyword>
    <ProjectGuid>{3b559c45-3ebd-4b6c-a434-9e03ba55c797}</ProjectGuid>
    <RootNamespace>DLLInjectorCom</RootNamespace>
    <WindowsTargetPlatformVersion>10.0</WindowsTargetPlatformVersion>
  </PropertyGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props" />
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
    <ConfigurationType>Application</ConfigurationType>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>v142</PlatformToolset>
    <CharacterSet>Unicode</CharacterSet>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
    <ConfigurationType>Application</ConfigurationType>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>v142</PlatformToolset>
    <WholeProgramOptimization>true</WholeProgramOptimization>
    <CharacterSet>Unicode</CharacterSet>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
    <ConfigurationType>Application</ConfigurationType>
    <UseDebugLibraries>true</UseDebugLibraries>
    <PlatformToolset>v142</PlatformToolset>
    <CharacterSet>Unicode</CharacterSet>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
    <ConfigurationType>Application</ConfigurationType>
    <UseDebugLibraries>false</UseDebugLibraries>
    <PlatformToolset>v142</PlatformToolset>
    <WholeProgramOptimization>true</WholeProgramOptimization>
    <CharacterSet>Unicode</CharacterSet>
  </PropertyGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props" />
  <ImportGroup Label="ExtensionSettings">
  </ImportGroup>
  <ImportGroup Label="Shared">
  </ImportGroup>
  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
    <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform" />
  </ImportGroup>
  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform" />
  </ImportGroup>
  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform" />
  </ImportGroup>
  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform" />
  </ImportGroup>
  <PropertyGroup Label="UserMacros" />
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
    <LinkIncremental>true</LinkIncremental>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <LinkIncremental>false</LinkIncremental>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <LinkIncremental>true</LinkIncremental>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <LinkIncremental>false</LinkIncremental>
  </PropertyGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
    <ClCompile>
      <WarningLevel>Level3</WarningLevel>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Console</SubSystem>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <ClCompile>
      <WarningLevel>Level3</WarningLevel>
      <FunctionLevelLinking>true</FunctionLevelLinking>
      <IntrinsicFunctions>true</IntrinsicFunctions>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Console</SubSystem>
      <EnableCOMDATFolding>true</EnableCOMDATFolding>
      <OptimizeReferences>true</OptimizeReferences>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <ClCompile>
      <WarningLevel>Level3</WarningLevel>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
      <RuntimeLibrary>MultiThreadedDebug</RuntimeLibrary>
    </ClCompile>
    <Link>
      <SubSystem>Console</SubSystem>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <ClCompile>
      <WarningLevel>Level3</WarningLevel>
      <FunctionLevelLinking>true</FunctionLevelLinking>
      <IntrinsicFunctions>true</IntrinsicFunctions>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
      <RuntimeLibrary>MultiThreaded</RuntimeLibrary>
    </ClCompile>
    <Link>
      <SubSystem>Console</SubSystem>
      <EnableCOMDATFolding>true</EnableCOMDATFolding>
      <OptimizeReferences>true</OptimizeReferences>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
  </ItemDefinitionGroup>
  <ItemGroup>
    <ClCompile Include="DLLInjectorCom.cpp" />
  </ItemGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets" />
  <ImportGroup Label="ExtensionTargets">
  </ImportGroup>
</Project>


================================================
FILE: DLLInjector/DLLInjectorCom/DLLInjectorCom.vcxproj.filters
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <ItemGroup>
    <Filter Include="Source Files">
      <UniqueIdentifier>{4FC737F1-C7A5-4376-A066-2A32D752A2FF}</UniqueIdentifier>
      <Extensions>cpp;c;cc;cxx;c++;cppm;ixx;def;odl;idl;hpj;bat;asm;asmx</Extensions>
    </Filter>
    <Filter Include="Header Files">
      <UniqueIdentifier>{93995380-89BD-4b04-88EB-625FBE52EBFB}</UniqueIdentifier>
      <Extensions>h;hh;hpp;hxx;h++;hm;inl;inc;ipp;xsd</Extensions>
    </Filter>
    <Filter Include="Resource Files">
      <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
    </Filter>
  </ItemGroup>
  <ItemGroup>
    <ClCompile Include="DLLInjectorCom.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
  </ItemGroup>
</Project>

