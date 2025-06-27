Directory structure:
└── gange666-xvmp/
    ├── README.md
    ├── build.sh
    ├── examples/
    │   ├── test1/
    │   │   ├── README.md
    │   │   └── test1.c
    │   ├── test2/
    │   │   ├── README.md
    │   │   └── test2.c
    │   └── test3/
    │       ├── README.md
    │       ├── test3_foo.c
    │       ├── test3_foo.h
    │       └── test3_main.c
    ├── scripts/
    │   ├── interpreter-ir2str.py
    │   └── rebuild-with-interpreter.sh
    ├── src/
    │   ├── llvm.spec.in
    │   ├── RELEASE_TESTERS.TXT
    │   ├── bindings/
    │   │   ├── LLVMBuild.txt
    │   │   ├── README.txt
    │   │   ├── go/
    │   │   │   ├── build.sh
    │   │   │   ├── conftest.go
    │   │   │   ├── README.txt
    │   │   │   └── llvm/
    │   │   │       ├── analysis.go
    │   │   │       ├── bitreader.go
    │   │   │       ├── bitwriter.go
    │   │   │       ├── dibuilder.go
    │   │   │       ├── executionengine.go
    │   │   │       ├── executionengine_test.go
    │   │   │       ├── InstrumentationBindings.cpp
    │   │   │       ├── InstrumentationBindings.h
    │   │   │       ├── ir.go
    │   │   │       ├── ir_test.go
    │   │   │       ├── IRBindings.cpp
    │   │   │       ├── IRBindings.h
    │   │   │       ├── linker.go
    │   │   │       ├── llvm_config.go.in
    │   │   │       ├── llvm_dep.go
    │   │   │       ├── string.go
    │   │   │       ├── string_test.go
    │   │   │       ├── support.go
    │   │   │       ├── SupportBindings.cpp
    │   │   │       ├── SupportBindings.h
    │   │   │       ├── target.go
    │   │   │       ├── transforms_coroutines.go
    │   │   │       ├── transforms_instrumentation.go
    │   │   │       ├── transforms_ipo.go
    │   │   │       ├── transforms_pmbuilder.go
    │   │   │       ├── transforms_scalar.go
    │   │   │       └── version.go
    │   │   ├── ocaml/
    │   │   │   ├── CMakeLists.txt
    │   │   │   ├── README.txt
    │   │   │   ├── all_backends/
    │   │   │   │   ├── all_backends_ocaml.c
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_all_backends.ml
    │   │   │   │   └── llvm_all_backends.mli
    │   │   │   ├── analysis/
    │   │   │   │   ├── analysis_ocaml.c
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_analysis.ml
    │   │   │   │   └── llvm_analysis.mli
    │   │   │   ├── backends/
    │   │   │   │   ├── backend_ocaml.c
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_backend.ml.in
    │   │   │   │   ├── llvm_backend.mli.in
    │   │   │   │   └── META.llvm_backend.in
    │   │   │   ├── bitreader/
    │   │   │   │   ├── bitreader_ocaml.c
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_bitreader.ml
    │   │   │   │   └── llvm_bitreader.mli
    │   │   │   ├── bitwriter/
    │   │   │   │   ├── bitwriter_ocaml.c
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_bitwriter.ml
    │   │   │   │   └── llvm_bitwriter.mli
    │   │   │   ├── executionengine/
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── executionengine_ocaml.c
    │   │   │   │   ├── llvm_executionengine.ml
    │   │   │   │   └── llvm_executionengine.mli
    │   │   │   ├── irreader/
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── irreader_ocaml.c
    │   │   │   │   ├── llvm_irreader.ml
    │   │   │   │   └── llvm_irreader.mli
    │   │   │   ├── linker/
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── linker_ocaml.c
    │   │   │   │   ├── llvm_linker.ml
    │   │   │   │   └── llvm_linker.mli
    │   │   │   ├── llvm/
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm.ml
    │   │   │   │   ├── llvm.mli
    │   │   │   │   ├── llvm_ocaml.c
    │   │   │   │   └── META.llvm.in
    │   │   │   ├── target/
    │   │   │   │   ├── CMakeLists.txt
    │   │   │   │   ├── llvm_target.ml
    │   │   │   │   ├── llvm_target.mli
    │   │   │   │   └── target_ocaml.c
    │   │   │   └── transforms/
    │   │   │       ├── CMakeLists.txt
    │   │   │       ├── ipo/
    │   │   │       │   ├── CMakeLists.txt
    │   │   │       │   ├── ipo_ocaml.c
    │   │   │       │   ├── llvm_ipo.ml
    │   │   │       │   └── llvm_ipo.mli
    │   │   │       ├── passmgr_builder/
    │   │   │       │   ├── CMakeLists.txt
    │   │   │       │   ├── llvm_passmgr_builder.ml
    │   │   │       │   ├── llvm_passmgr_builder.mli
    │   │   │       │   └── passmgr_builder_ocaml.c
    │   │   │       ├── scalar_opts/
    │   │   │       │   ├── CMakeLists.txt
    │   │   │       │   ├── llvm_scalar_opts.ml
    │   │   │       │   ├── llvm_scalar_opts.mli
    │   │   │       │   └── scalar_opts_ocaml.c
    │   │   │       ├── utils/
    │   │   │       │   ├── CMakeLists.txt
    │   │   │       │   ├── llvm_transform_utils.ml
    │   │   │       │   ├── llvm_transform_utils.mli
    │   │   │       │   └── transform_utils_ocaml.c
    │   │   │       └── vectorize/
    │   │   │           ├── CMakeLists.txt
    │   │   │           ├── llvm_vectorize.ml
    │   │   │           ├── llvm_vectorize.mli
    │   │   │           └── vectorize_ocaml.c
    │   │   └── python/
    │   │       ├── README.txt
    │   │       └── llvm/
    │   │           ├── __init__.py
    │   │           ├── bit_reader.py
    │   │           ├── common.py
    │   │           ├── core.py
    │   │           ├── disassembler.py
    │   │           ├── enumerations.py
    │   │           ├── object.py
    │   │           └── tests/
    │   │               ├── __init__.py
    │   │               ├── base.py
    │   │               ├── test.bc
    │   │               ├── test_bitreader.py
    │   │               ├── test_core.py
    │   │               ├── test_disassembler.py
    │   │               ├── test_file
    │   │               └── test_object.py
    │   ├── docs/
    │   │   ├── AdvancedBuilds.rst
    │   │   ├── AliasAnalysis.rst
    │   │   ├── AMDGPUInstructionNotation.rst
    │   │   ├── AMDGPUInstructionSyntax.rst
    │   │   ├── AMDGPUModifierSyntax.rst
    │   │   ├── AMDGPUOperandSyntax.rst
    │   │   ├── AMDGPUUsage.rst
    │   │   ├── Atomics.rst
    │   │   ├── Benchmarking.rst
    │   │   ├── BigEndianNEON.rst
    │   │   ├── BitCodeFormat.rst
    │   │   ├── BlockFrequencyTerminology.rst
    │   │   ├── BranchWeightMetadata.rst
    │   │   ├── BugLifeCycle.rst
    │   │   ├── Bugpoint.rst
    │   │   ├── CFIVerify.rst
    │   │   ├── CMake.rst
    │   │   ├── CMakeLists.txt
    │   │   ├── CMakePrimer.rst
    │   │   ├── CodeGenerator.rst
    │   │   ├── CodeOfConduct.rst
    │   │   ├── CodingStandards.rst
    │   │   ├── CommandLine.rst
    │   │   ├── CompileCudaWithLLVM.rst
    │   │   ├── CompilerWriterInfo.rst
    │   │   ├── conf.py
    │   │   ├── Contributing.rst
    │   │   ├── Coroutines.rst
    │   │   ├── CoverageMappingFormat.rst
    │   │   ├── DebuggingJITedCode.rst
    │   │   ├── DeveloperPolicy.rst
    │   │   ├── Docker.rst
    │   │   ├── doxygen-mainpage.dox
    │   │   ├── doxygen.cfg.in
    │   │   ├── ExceptionHandling.rst
    │   │   ├── ExtendedIntegerResults.txt
    │   │   ├── ExtendingLLVM.rst
    │   │   ├── Extensions.rst
    │   │   ├── FAQ.rst
    │   │   ├── FaultMaps.rst
    │   │   ├── FuzzingLLVM.rst
    │   │   ├── GarbageCollection.rst
    │   │   ├── GetElementPtr.rst
    │   │   ├── GettingStarted.rst
    │   │   ├── GettingStartedVS.rst
    │   │   ├── GlobalISel.rst
    │   │   ├── GoldPlugin.rst
    │   │   ├── HowToAddABuilder.rst
    │   │   ├── HowToBuildOnARM.rst
    │   │   ├── HowToBuildWithPGO.rst
    │   │   ├── HowToCrossCompileBuiltinsOnArm.rst
    │   │   ├── HowToCrossCompileLLVM.rst
    │   │   ├── HowToReleaseLLVM.rst
    │   │   ├── HowToSetUpLLVMStyleRTTI.rst
    │   │   ├── HowToSubmitABug.rst
    │   │   ├── HowToUseAttributes.rst
    │   │   ├── HowToUseInstrMappings.rst
    │   │   ├── InAlloca.rst
    │   │   ├── index.rst
    │   │   ├── LangRef.rst
    │   │   ├── Lexicon.rst
    │   │   ├── LibFuzzer.rst
    │   │   ├── LinkTimeOptimization.rst
    │   │   ├── llvm-objdump.1
    │   │   ├── LLVMBuild.rst
    │   │   ├── LLVMBuild.txt
    │   │   ├── make.bat
    │   │   ├── Makefile.sphinx
    │   │   ├── MarkdownQuickstartTemplate.md
    │   │   ├── MarkedUpDisassembly.rst
    │   │   ├── MCJITDesignAndImplementation.rst
    │   │   ├── MemorySSA.rst
    │   │   ├── MergeFunctions.rst
    │   │   ├── MIRLangRef.rst
    │   │   ├── NVPTXUsage.rst
    │   │   ├── OptBisect.rst
    │   │   ├── Packaging.rst
    │   │   ├── Passes.rst
    │   │   ├── Phabricator.rst
    │   │   ├── ProgrammersManual.rst
    │   │   ├── Projects.rst
    │   │   ├── re_format.7
    │   │   ├── README.txt
    │   │   ├── ReleaseNotes.rst
    │   │   ├── ReleaseProcess.rst
    │   │   ├── ReportingGuide.rst
    │   │   ├── ScudoHardenedAllocator.rst
    │   │   ├── SegmentedStacks.rst
    │   │   ├── SourceLevelDebugging.rst
    │   │   ├── SpeculativeLoadHardening.md
    │   │   ├── SphinxQuickstartTemplate.rst
    │   │   ├── StackMaps.rst
    │   │   ├── StackSafetyAnalysis.rst
    │   │   ├── Statepoints.rst
    │   │   ├── SupportLibrary.rst
    │   │   ├── SystemLibrary.rst
    │   │   ├── TableGenFundamentals.rst
    │   │   ├── TestingGuide.rst
    │   │   ├── TestSuiteGuide.md
    │   │   ├── TestSuiteMakefileGuide.rst
    │   │   ├── TransformMetadata.rst
    │   │   ├── TypeMetadata.rst
    │   │   ├── Vectorizers.rst
    │   │   ├── WritingAnLLVMBackend.rst
    │   │   ├── WritingAnLLVMPass.rst
    │   │   ├── XRay.rst
    │   │   ├── XRayExample.rst
    │   │   ├── XRayFDRFormat.rst
    │   │   ├── yaml2obj.rst
    │   │   ├── YamlIO.rst
    │   │   ├── _ocamldoc/
    │   │   │   └── style.css
    │   │   ├── _static/
    │   │   │   └── llvm.css
    │   │   ├── _templates/
    │   │   │   ├── indexsidebar.html
    │   │   │   └── layout.html
    │   │   ├── _themes/
    │   │   │   └── llvm-theme/
    │   │   │       ├── layout.html
    │   │   │       ├── theme.conf
    │   │   │       └── static/
    │   │   │           └── llvm-theme.css
    │   │   ├── AMDGPU/
    │   │   │   ├── AMDGPUAsmGFX7.rst
    │   │   │   ├── AMDGPUAsmGFX8.rst
    │   │   │   ├── AMDGPUAsmGFX9.rst
    │   │   │   ├── gfx7_addr_buf.rst
    │   │   │   ├── gfx7_addr_ds.rst
    │   │   │   ├── gfx7_addr_flat.rst
    │   │   │   ├── gfx7_addr_mimg.rst
    │   │   │   ├── gfx7_attr.rst
    │   │   │   ├── gfx7_base_smem_addr.rst
    │   │   │   ├── gfx7_base_smem_buf.rst
    │   │   │   ├── gfx7_bimm16.rst
    │   │   │   ├── gfx7_bimm32.rst
    │   │   │   ├── gfx7_data_buf_atomic128.rst
    │   │   │   ├── gfx7_data_buf_atomic32.rst
    │   │   │   ├── gfx7_data_buf_atomic64.rst
    │   │   │   ├── gfx7_data_mimg_atomic_cmp.rst
    │   │   │   ├── gfx7_data_mimg_atomic_reg.rst
    │   │   │   ├── gfx7_data_mimg_store.rst
    │   │   │   ├── gfx7_dst_buf_128.rst
    │   │   │   ├── gfx7_dst_buf_64.rst
    │   │   │   ├── gfx7_dst_buf_96.rst
    │   │   │   ├── gfx7_dst_buf_lds.rst
    │   │   │   ├── gfx7_dst_flat_atomic32.rst
    │   │   │   ├── gfx7_dst_flat_atomic64.rst
    │   │   │   ├── gfx7_dst_mimg_gather4.rst
    │   │   │   ├── gfx7_dst_mimg_regular.rst
    │   │   │   ├── gfx7_fimm32.rst
    │   │   │   ├── gfx7_hwreg.rst
    │   │   │   ├── gfx7_label.rst
    │   │   │   ├── gfx7_mod.rst
    │   │   │   ├── gfx7_msg.rst
    │   │   │   ├── gfx7_offset_buf.rst
    │   │   │   ├── gfx7_offset_smem.rst
    │   │   │   ├── gfx7_opt.rst
    │   │   │   ├── gfx7_param.rst
    │   │   │   ├── gfx7_ret.rst
    │   │   │   ├── gfx7_rsrc_buf.rst
    │   │   │   ├── gfx7_rsrc_mimg.rst
    │   │   │   ├── gfx7_samp_mimg.rst
    │   │   │   ├── gfx7_sdst128_0.rst
    │   │   │   ├── gfx7_sdst256_0.rst
    │   │   │   ├── gfx7_sdst32_0.rst
    │   │   │   ├── gfx7_sdst32_1.rst
    │   │   │   ├── gfx7_sdst32_2.rst
    │   │   │   ├── gfx7_sdst512_0.rst
    │   │   │   ├── gfx7_sdst64_0.rst
    │   │   │   ├── gfx7_sdst64_1.rst
    │   │   │   ├── gfx7_simm16.rst
    │   │   │   ├── gfx7_src32_0.rst
    │   │   │   ├── gfx7_src32_1.rst
    │   │   │   ├── gfx7_src32_2.rst
    │   │   │   ├── gfx7_src32_3.rst
    │   │   │   ├── gfx7_src64_0.rst
    │   │   │   ├── gfx7_src64_1.rst
    │   │   │   ├── gfx7_src64_2.rst
    │   │   │   ├── gfx7_src_exp.rst
    │   │   │   ├── gfx7_ssrc32_0.rst
    │   │   │   ├── gfx7_ssrc32_1.rst
    │   │   │   ├── gfx7_ssrc32_2.rst
    │   │   │   ├── gfx7_ssrc32_3.rst
    │   │   │   ├── gfx7_ssrc32_4.rst
    │   │   │   ├── gfx7_ssrc64_0.rst
    │   │   │   ├── gfx7_ssrc64_1.rst
    │   │   │   ├── gfx7_ssrc64_2.rst
    │   │   │   ├── gfx7_ssrc64_3.rst
    │   │   │   ├── gfx7_tgt.rst
    │   │   │   ├── gfx7_type_dev.rst
    │   │   │   ├── gfx7_uimm16.rst
    │   │   │   ├── gfx7_vcc_64.rst
    │   │   │   ├── gfx7_vdata128_0.rst
    │   │   │   ├── gfx7_vdata32_0.rst
    │   │   │   ├── gfx7_vdata64_0.rst
    │   │   │   ├── gfx7_vdata96_0.rst
    │   │   │   ├── gfx7_vdst128_0.rst
    │   │   │   ├── gfx7_vdst32_0.rst
    │   │   │   ├── gfx7_vdst64_0.rst
    │   │   │   ├── gfx7_vdst96_0.rst
    │   │   │   ├── gfx7_vsrc128_0.rst
    │   │   │   ├── gfx7_vsrc32_0.rst
    │   │   │   ├── gfx7_vsrc64_0.rst
    │   │   │   ├── gfx7_waitcnt.rst
    │   │   │   ├── gfx8_addr_buf.rst
    │   │   │   ├── gfx8_addr_ds.rst
    │   │   │   ├── gfx8_addr_flat.rst
    │   │   │   ├── gfx8_addr_mimg.rst
    │   │   │   ├── gfx8_attr.rst
    │   │   │   ├── gfx8_base_smem_addr.rst
    │   │   │   ├── gfx8_base_smem_buf.rst
    │   │   │   ├── gfx8_bimm16.rst
    │   │   │   ├── gfx8_bimm32.rst
    │   │   │   ├── gfx8_data_buf_atomic128.rst
    │   │   │   ├── gfx8_data_buf_atomic32.rst
    │   │   │   ├── gfx8_data_buf_atomic64.rst
    │   │   │   ├── gfx8_data_buf_d16_128.rst
    │   │   │   ├── gfx8_data_buf_d16_32.rst
    │   │   │   ├── gfx8_data_buf_d16_64.rst
    │   │   │   ├── gfx8_data_buf_d16_96.rst
    │   │   │   ├── gfx8_data_mimg_atomic_cmp.rst
    │   │   │   ├── gfx8_data_mimg_atomic_reg.rst
    │   │   │   ├── gfx8_data_mimg_store.rst
    │   │   │   ├── gfx8_data_mimg_store_d16.rst
    │   │   │   ├── gfx8_dst_buf_128.rst
    │   │   │   ├── gfx8_dst_buf_64.rst
    │   │   │   ├── gfx8_dst_buf_96.rst
    │   │   │   ├── gfx8_dst_buf_d16_128.rst
    │   │   │   ├── gfx8_dst_buf_d16_32.rst
    │   │   │   ├── gfx8_dst_buf_d16_64.rst
    │   │   │   ├── gfx8_dst_buf_d16_96.rst
    │   │   │   ├── gfx8_dst_buf_lds.rst
    │   │   │   ├── gfx8_dst_flat_atomic32.rst
    │   │   │   ├── gfx8_dst_flat_atomic64.rst
    │   │   │   ├── gfx8_dst_mimg_gather4.rst
    │   │   │   ├── gfx8_dst_mimg_regular.rst
    │   │   │   ├── gfx8_dst_mimg_regular_d16.rst
    │   │   │   ├── gfx8_fimm16.rst
    │   │   │   ├── gfx8_fimm32.rst
    │   │   │   ├── gfx8_hwreg.rst
    │   │   │   ├── gfx8_imm4.rst
    │   │   │   ├── gfx8_label.rst
    │   │   │   ├── gfx8_mod_dpp_sdwa_abs_neg.rst
    │   │   │   ├── gfx8_mod_sdwa_sext.rst
    │   │   │   ├── gfx8_mod_vop3_abs_neg.rst
    │   │   │   ├── gfx8_msg.rst
    │   │   │   ├── gfx8_offset_buf.rst
    │   │   │   ├── gfx8_offset_smem_load.rst
    │   │   │   ├── gfx8_offset_smem_store.rst
    │   │   │   ├── gfx8_opt.rst
    │   │   │   ├── gfx8_param.rst
    │   │   │   ├── gfx8_perm_smem.rst
    │   │   │   ├── gfx8_ret.rst
    │   │   │   ├── gfx8_rsrc_buf.rst
    │   │   │   ├── gfx8_rsrc_mimg.rst
    │   │   │   ├── gfx8_samp_mimg.rst
    │   │   │   ├── gfx8_sdata128_0.rst
    │   │   │   ├── gfx8_sdata32_0.rst
    │   │   │   ├── gfx8_sdata64_0.rst
    │   │   │   ├── gfx8_sdst128_0.rst
    │   │   │   ├── gfx8_sdst256_0.rst
    │   │   │   ├── gfx8_sdst32_0.rst
    │   │   │   ├── gfx8_sdst32_1.rst
    │   │   │   ├── gfx8_sdst32_2.rst
    │   │   │   ├── gfx8_sdst512_0.rst
    │   │   │   ├── gfx8_sdst64_0.rst
    │   │   │   ├── gfx8_sdst64_1.rst
    │   │   │   ├── gfx8_simm16.rst
    │   │   │   ├── gfx8_src32_0.rst
    │   │   │   ├── gfx8_src32_1.rst
    │   │   │   ├── gfx8_src64_0.rst
    │   │   │   ├── gfx8_src64_1.rst
    │   │   │   ├── gfx8_src_exp.rst
    │   │   │   ├── gfx8_ssrc32_0.rst
    │   │   │   ├── gfx8_ssrc32_1.rst
    │   │   │   ├── gfx8_ssrc32_2.rst
    │   │   │   ├── gfx8_ssrc32_3.rst
    │   │   │   ├── gfx8_ssrc32_4.rst
    │   │   │   ├── gfx8_ssrc64_0.rst
    │   │   │   ├── gfx8_ssrc64_1.rst
    │   │   │   ├── gfx8_ssrc64_2.rst
    │   │   │   ├── gfx8_ssrc64_3.rst
    │   │   │   ├── gfx8_tgt.rst
    │   │   │   ├── gfx8_type_dev.rst
    │   │   │   ├── gfx8_uimm16.rst
    │   │   │   ├── gfx8_vcc_64.rst
    │   │   │   ├── gfx8_vdata128_0.rst
    │   │   │   ├── gfx8_vdata32_0.rst
    │   │   │   ├── gfx8_vdata64_0.rst
    │   │   │   ├── gfx8_vdata96_0.rst
    │   │   │   ├── gfx8_vdst128_0.rst
    │   │   │   ├── gfx8_vdst32_0.rst
    │   │   │   ├── gfx8_vdst64_0.rst
    │   │   │   ├── gfx8_vdst96_0.rst
    │   │   │   ├── gfx8_vsrc128_0.rst
    │   │   │   ├── gfx8_vsrc32_0.rst
    │   │   │   ├── gfx8_vsrc64_0.rst
    │   │   │   ├── gfx8_waitcnt.rst
    │   │   │   ├── gfx9_addr_buf.rst
    │   │   │   ├── gfx9_addr_ds.rst
    │   │   │   ├── gfx9_addr_flat.rst
    │   │   │   ├── gfx9_addr_mimg.rst
    │   │   │   ├── gfx9_attr.rst
    │   │   │   ├── gfx9_base_smem_addr.rst
    │   │   │   ├── gfx9_base_smem_buf.rst
    │   │   │   ├── gfx9_base_smem_scratch.rst
    │   │   │   ├── gfx9_bimm16.rst
    │   │   │   ├── gfx9_bimm32.rst
    │   │   │   ├── gfx9_data_buf_atomic128.rst
    │   │   │   ├── gfx9_data_buf_atomic32.rst
    │   │   │   ├── gfx9_data_buf_atomic64.rst
    │   │   │   ├── gfx9_data_mimg_atomic_cmp.rst
    │   │   │   ├── gfx9_data_mimg_atomic_reg.rst
    │   │   │   ├── gfx9_data_mimg_store.rst
    │   │   │   ├── gfx9_data_mimg_store_d16.rst
    │   │   │   ├── gfx9_data_smem_atomic128.rst
    │   │   │   ├── gfx9_data_smem_atomic32.rst
    │   │   │   ├── gfx9_data_smem_atomic64.rst
    │   │   │   ├── gfx9_dst_buf_128.rst
    │   │   │   ├── gfx9_dst_buf_32.rst
    │   │   │   ├── gfx9_dst_buf_64.rst
    │   │   │   ├── gfx9_dst_buf_96.rst
    │   │   │   ├── gfx9_dst_buf_lds.rst
    │   │   │   ├── gfx9_dst_flat_atomic32.rst
    │   │   │   ├── gfx9_dst_flat_atomic64.rst
    │   │   │   ├── gfx9_dst_mimg_gather4.rst
    │   │   │   ├── gfx9_dst_mimg_regular.rst
    │   │   │   ├── gfx9_dst_mimg_regular_d16.rst
    │   │   │   ├── gfx9_fimm16.rst
    │   │   │   ├── gfx9_fimm32.rst
    │   │   │   ├── gfx9_hwreg.rst
    │   │   │   ├── gfx9_imm4.rst
    │   │   │   ├── gfx9_label.rst
    │   │   │   ├── gfx9_mad_type_dev.rst
    │   │   │   ├── gfx9_mod_dpp_sdwa_abs_neg.rst
    │   │   │   ├── gfx9_mod_sdwa_sext.rst
    │   │   │   ├── gfx9_mod_vop3_abs_neg.rst
    │   │   │   ├── gfx9_msg.rst
    │   │   │   ├── gfx9_offset_buf.rst
    │   │   │   ├── gfx9_offset_smem_buf.rst
    │   │   │   ├── gfx9_offset_smem_plain.rst
    │   │   │   ├── gfx9_opt.rst
    │   │   │   ├── gfx9_param.rst
    │   │   │   ├── gfx9_perm_smem.rst
    │   │   │   ├── gfx9_ret.rst
    │   │   │   ├── gfx9_rsrc_buf.rst
    │   │   │   ├── gfx9_rsrc_mimg.rst
    │   │   │   ├── gfx9_saddr_flat_global.rst
    │   │   │   ├── gfx9_saddr_flat_scratch.rst
    │   │   │   ├── gfx9_samp_mimg.rst
    │   │   │   ├── gfx9_sdata128_0.rst
    │   │   │   ├── gfx9_sdata32_0.rst
    │   │   │   ├── gfx9_sdata64_0.rst
    │   │   │   ├── gfx9_sdst128_0.rst
    │   │   │   ├── gfx9_sdst256_0.rst
    │   │   │   ├── gfx9_sdst32_0.rst
    │   │   │   ├── gfx9_sdst32_1.rst
    │   │   │   ├── gfx9_sdst32_2.rst
    │   │   │   ├── gfx9_sdst512_0.rst
    │   │   │   ├── gfx9_sdst64_0.rst
    │   │   │   ├── gfx9_sdst64_1.rst
    │   │   │   ├── gfx9_simm16.rst
    │   │   │   ├── gfx9_src32_0.rst
    │   │   │   ├── gfx9_src32_1.rst
    │   │   │   ├── gfx9_src64_0.rst
    │   │   │   ├── gfx9_src64_1.rst
    │   │   │   ├── gfx9_src_exp.rst
    │   │   │   ├── gfx9_ssrc32_0.rst
    │   │   │   ├── gfx9_ssrc32_1.rst
    │   │   │   ├── gfx9_ssrc32_2.rst
    │   │   │   ├── gfx9_ssrc32_3.rst
    │   │   │   ├── gfx9_ssrc32_4.rst
    │   │   │   ├── gfx9_ssrc64_0.rst
    │   │   │   ├── gfx9_ssrc64_1.rst
    │   │   │   ├── gfx9_ssrc64_2.rst
    │   │   │   ├── gfx9_ssrc64_3.rst
    │   │   │   ├── gfx9_tgt.rst
    │   │   │   ├── gfx9_type_dev.rst
    │   │   │   ├── gfx9_uimm16.rst
    │   │   │   ├── gfx9_vaddr_flat_global.rst
    │   │   │   ├── gfx9_vaddr_flat_scratch.rst
    │   │   │   ├── gfx9_vcc_64.rst
    │   │   │   ├── gfx9_vdata128_0.rst
    │   │   │   ├── gfx9_vdata32_0.rst
    │   │   │   ├── gfx9_vdata64_0.rst
    │   │   │   ├── gfx9_vdata96_0.rst
    │   │   │   ├── gfx9_vdst128_0.rst
    │   │   │   ├── gfx9_vdst32_0.rst
    │   │   │   ├── gfx9_vdst64_0.rst
    │   │   │   ├── gfx9_vdst96_0.rst
    │   │   │   ├── gfx9_vsrc128_0.rst
    │   │   │   ├── gfx9_vsrc32_0.rst
    │   │   │   ├── gfx9_vsrc64_0.rst
    │   │   │   └── gfx9_waitcnt.rst
    │   │   ├── CommandGuide/
    │   │   │   ├── bugpoint.rst
    │   │   │   ├── dsymutil.rst
    │   │   │   ├── FileCheck.rst
    │   │   │   ├── index.rst
    │   │   │   ├── lit.rst
    │   │   │   ├── llc.rst
    │   │   │   ├── lli.rst
    │   │   │   ├── llvm-ar.rst
    │   │   │   ├── llvm-as.rst
    │   │   │   ├── llvm-bcanalyzer.rst
    │   │   │   ├── llvm-build.rst
    │   │   │   ├── llvm-config.rst
    │   │   │   ├── llvm-cov.rst
    │   │   │   ├── llvm-cxxmap.rst
    │   │   │   ├── llvm-diff.rst
    │   │   │   ├── llvm-dis.rst
    │   │   │   ├── llvm-dwarfdump.rst
    │   │   │   ├── llvm-exegesis.rst
    │   │   │   ├── llvm-extract.rst
    │   │   │   ├── llvm-lib.rst
    │   │   │   ├── llvm-link.rst
    │   │   │   ├── llvm-mca.rst
    │   │   │   ├── llvm-nm.rst
    │   │   │   ├── llvm-objdump.rst
    │   │   │   ├── llvm-pdbutil.rst
    │   │   │   ├── llvm-profdata.rst
    │   │   │   ├── llvm-readobj.rst
    │   │   │   ├── llvm-stress.rst
    │   │   │   ├── llvm-symbolizer.rst
    │   │   │   ├── opt.rst
    │   │   │   └── tblgen.rst
    │   │   ├── Frontend/
    │   │   │   └── PerformanceTips.rst
    │   │   ├── HistoricalNotes/
    │   │   │   ├── 2000-11-18-EarlyDesignIdeas.txt
    │   │   │   ├── 2000-11-18-EarlyDesignIdeasResp.txt
    │   │   │   ├── 2000-12-06-EncodingIdea.txt
    │   │   │   ├── 2000-12-06-MeetingSummary.txt
    │   │   │   ├── 2001-01-31-UniversalIRIdea.txt
    │   │   │   ├── 2001-02-06-TypeNotationDebate.txt
    │   │   │   ├── 2001-02-06-TypeNotationDebateResp1.txt
    │   │   │   ├── 2001-02-06-TypeNotationDebateResp2.txt
    │   │   │   ├── 2001-02-06-TypeNotationDebateResp4.txt
    │   │   │   ├── 2001-02-09-AdveComments.txt
    │   │   │   ├── 2001-02-09-AdveCommentsResponse.txt
    │   │   │   ├── 2001-02-13-Reference-Memory.txt
    │   │   │   ├── 2001-02-13-Reference-MemoryResponse.txt
    │   │   │   ├── 2001-04-16-DynamicCompilation.txt
    │   │   │   ├── 2001-05-18-ExceptionHandling.txt
    │   │   │   ├── 2001-05-19-ExceptionResponse.txt
    │   │   │   ├── 2001-06-01-GCCOptimizations.txt
    │   │   │   ├── 2001-06-01-GCCOptimizations2.txt
    │   │   │   ├── 2001-06-20-.NET-Differences.txt
    │   │   │   ├── 2001-07-06-LoweringIRForCodeGen.txt
    │   │   │   ├── 2001-09-18-OptimizeExceptions.txt
    │   │   │   ├── 2002-05-12-InstListChange.txt
    │   │   │   ├── 2002-06-25-MegaPatchInfo.txt
    │   │   │   ├── 2003-01-23-CygwinNotes.txt
    │   │   │   ├── 2003-06-25-Reoptimizer1.txt
    │   │   │   ├── 2003-06-26-Reoptimizer2.txt
    │   │   │   └── 2007-OriginalClangReadme.txt
    │   │   ├── PDB/
    │   │   │   ├── CodeViewSymbols.rst
    │   │   │   ├── CodeViewTypes.rst
    │   │   │   ├── DbiStream.rst
    │   │   │   ├── GlobalStream.rst
    │   │   │   ├── HashStream.rst
    │   │   │   ├── index.rst
    │   │   │   ├── ModiStream.rst
    │   │   │   ├── MsfFile.rst
    │   │   │   ├── PdbStream.rst
    │   │   │   ├── PublicStream.rst
    │   │   │   └── TpiStream.rst
    │   │   ├── Proposals/
    │   │   │   ├── GitHubMove.rst
    │   │   │   ├── TestSuite.rst
    │   │   │   └── VectorizationPlan.rst
    │   │   ├── TableGen/
    │   │   │   ├── BackEnds.rst
    │   │   │   ├── Deficiencies.rst
    │   │   │   ├── index.rst
    │   │   │   ├── LangIntro.rst
    │   │   │   └── LangRef.rst
    │   │   └── tutorial/
    │   │       ├── BuildingAJIT1.rst
    │   │       ├── BuildingAJIT2.rst
    │   │       ├── BuildingAJIT3.rst
    │   │       ├── BuildingAJIT4.rst
    │   │       ├── BuildingAJIT5.rst
    │   │       ├── index.rst
    │   │       ├── LangImpl01.rst
    │   │       ├── LangImpl02.rst
    │   │       ├── LangImpl03.rst
    │   │       ├── LangImpl04.rst
    │   │       ├── LangImpl05.rst
    │   │       ├── LangImpl06.rst
    │   │       ├── LangImpl07.rst
    │   │       ├── LangImpl08.rst
    │   │       ├── LangImpl09.rst
    │   │       ├── LangImpl10.rst
    │   │       ├── OCamlLangImpl1.rst
    │   │       ├── OCamlLangImpl2.rst
    │   │       ├── OCamlLangImpl3.rst
    │   │       ├── OCamlLangImpl4.rst
    │   │       ├── OCamlLangImpl5.rst
    │   │       ├── OCamlLangImpl6.rst
    │   │       ├── OCamlLangImpl7.rst
    │   │       └── OCamlLangImpl8.rst
    │   ├── resources/
    │   │   └── windows_version_resource.rc
    │   ├── test/
    │   │   ├── lit.cfg.py
    │   │   ├── TestRunner.sh
    │   │   ├── Analysis/
    │   │   │   ├── alias-analysis-uses.ll
    │   │   │   ├── AliasSet/
    │   │   │   │   ├── argmemonly.ll
    │   │   │   │   ├── guards.ll
    │   │   │   │   ├── intrinsics.ll
    │   │   │   │   ├── memset.ll
    │   │   │   │   ├── memtransfer.ll
    │   │   │   │   ├── saturation.ll
    │   │   │   │   └── unknown-inst-tracking.ll
    │   │   │   ├── AssumptionCache/
    │   │   │   │   └── basic.ll
    │   │   │   ├── BasicAA/
    │   │   │   │   ├── 128-bit-ptr.ll
    │   │   │   │   ├── 2003-02-26-AccessSizeTest.ll
    │   │   │   │   ├── 2003-03-04-GEPCrash.ll
    │   │   │   │   ├── 2003-04-22-GEPProblem.ll
    │   │   │   │   ├── 2003-04-25-GEPCrash.ll
    │   │   │   │   ├── 2003-05-21-GEP-Problem.ll
    │   │   │   │   ├── 2003-06-01-AliasCrash.ll
    │   │   │   │   ├── 2003-07-03-BasicAACrash.ll
    │   │   │   │   ├── 2003-09-19-LocalArgument.ll
    │   │   │   │   ├── 2003-11-04-SimpleCases.ll
    │   │   │   │   ├── 2003-12-11-ConstExprGEP.ll
    │   │   │   │   ├── 2004-07-28-MustAliasbug.ll
    │   │   │   │   ├── 2006-03-03-BadArraySubscript.ll
    │   │   │   │   ├── 2006-11-03-BasicAAVectorCrash.ll
    │   │   │   │   ├── 2007-01-13-BasePointerBadNoAlias.ll
    │   │   │   │   ├── 2007-08-01-NoAliasAndCalls.ll
    │   │   │   │   ├── 2007-08-01-NoAliasAndGEP.ll
    │   │   │   │   ├── 2007-08-05-GetOverloadedModRef.ll
    │   │   │   │   ├── 2007-10-24-ArgumentsGlobals.ll
    │   │   │   │   ├── 2007-11-05-SizeCrash.ll
    │   │   │   │   ├── 2007-12-08-OutOfBoundsCrash.ll
    │   │   │   │   ├── 2008-04-15-Byval.ll
    │   │   │   │   ├── 2008-06-02-GEPTailCrash.ll
    │   │   │   │   ├── 2008-11-23-NoaliasRet.ll
    │   │   │   │   ├── 2009-03-04-GEPNoalias.ll
    │   │   │   │   ├── 2009-10-13-AtomicModRef.ll
    │   │   │   │   ├── 2009-10-13-GEP-BaseNoAlias.ll
    │   │   │   │   ├── 2010-09-15-GEP-SignedArithmetic.ll
    │   │   │   │   ├── 2014-03-18-Maxlookup-reached.ll
    │   │   │   │   ├── aligned-overread.ll
    │   │   │   │   ├── args-rets-allocas-loads.ll
    │   │   │   │   ├── assume.ll
    │   │   │   │   ├── bug.23540.ll
    │   │   │   │   ├── bug.23626.ll
    │   │   │   │   ├── byval.ll
    │   │   │   │   ├── call-attrs.ll
    │   │   │   │   ├── cas.ll
    │   │   │   │   ├── constant-over-index.ll
    │   │   │   │   ├── cs-cs-arm.ll
    │   │   │   │   ├── cs-cs.ll
    │   │   │   │   ├── dag.ll
    │   │   │   │   ├── empty.ll
    │   │   │   │   ├── fallback-mayalias.ll
    │   │   │   │   ├── featuretest.ll
    │   │   │   │   ├── full-store-partial-alias.ll
    │   │   │   │   ├── gcsetest.ll
    │   │   │   │   ├── gep-alias.ll
    │   │   │   │   ├── gep-and-alias-64.ll
    │   │   │   │   ├── gep-and-alias.ll
    │   │   │   │   ├── getmodrefinfo-cs-cs.ll
    │   │   │   │   ├── global-size.ll
    │   │   │   │   ├── guards.ll
    │   │   │   │   ├── intrinsics-arm.ll
    │   │   │   │   ├── intrinsics.ll
    │   │   │   │   ├── invalidation.ll
    │   │   │   │   ├── invariant_group.ll
    │   │   │   │   ├── invariant_load.ll
    │   │   │   │   ├── memset_pattern.ll
    │   │   │   │   ├── modref.ll
    │   │   │   │   ├── must-and-partial.ll
    │   │   │   │   ├── negoffset.ll
    │   │   │   │   ├── no-escape-call.ll
    │   │   │   │   ├── noalias-bugs.ll
    │   │   │   │   ├── noalias-geps.ll
    │   │   │   │   ├── noalias-param.ll
    │   │   │   │   ├── noalias-wraparound-bug.ll
    │   │   │   │   ├── nocapture.ll
    │   │   │   │   ├── phi-aa.ll
    │   │   │   │   ├── phi-and-select.ll
    │   │   │   │   ├── phi-loop.ll
    │   │   │   │   ├── phi-spec-order.ll
    │   │   │   │   ├── phi-speculation.ll
    │   │   │   │   ├── phi-values-usage.ll
    │   │   │   │   ├── pr18573.ll
    │   │   │   │   ├── pr31761.ll
    │   │   │   │   ├── pr35821.ll
    │   │   │   │   ├── pr35843.ll
    │   │   │   │   ├── pure-const-dce.ll
    │   │   │   │   ├── q.bad.ll
    │   │   │   │   ├── returned.ll
    │   │   │   │   ├── sequential-gep.ll
    │   │   │   │   ├── store-promote.ll
    │   │   │   │   ├── struct-geps.ll
    │   │   │   │   ├── tail-byval.ll
    │   │   │   │   ├── tailcall-modref.ll
    │   │   │   │   ├── underlying-value.ll
    │   │   │   │   ├── unreachable-block.ll
    │   │   │   │   └── zext.ll
    │   │   │   ├── BlockFrequencyInfo/
    │   │   │   │   ├── bad_input.ll
    │   │   │   │   ├── basic.ll
    │   │   │   │   ├── double_backedge.ll
    │   │   │   │   ├── double_exit.ll
    │   │   │   │   ├── extremely-likely-loop-successor.ll
    │   │   │   │   ├── irreducible.ll
    │   │   │   │   ├── irreducible_loop_crash.ll
    │   │   │   │   ├── irreducible_pgo.ll
    │   │   │   │   ├── loop_with_branch.ll
    │   │   │   │   ├── loop_with_invoke.ll
    │   │   │   │   ├── loops_with_profile_info.ll
    │   │   │   │   ├── nested_loop_with_branches.ll
    │   │   │   │   └── redundant_edges.ll
    │   │   │   ├── BranchProbabilityInfo/
    │   │   │   │   ├── basic.ll
    │   │   │   │   ├── deopt-intrinsic.ll
    │   │   │   │   ├── libfunc_call.ll
    │   │   │   │   ├── loop.ll
    │   │   │   │   ├── noreturn.ll
    │   │   │   │   ├── pr18705.ll
    │   │   │   │   └── pr22718.ll
    │   │   │   ├── CallGraph/
    │   │   │   │   ├── 2008-09-09-DirectCall.ll
    │   │   │   │   ├── 2008-09-09-UsedByGlobal.ll
    │   │   │   │   ├── do-nothing-intrinsic.ll
    │   │   │   │   ├── no-intrinsics.ll
    │   │   │   │   └── non-leaf-intrinsics.ll
    │   │   │   ├── CFLAliasAnalysis/
    │   │   │   │   ├── Andersen/
    │   │   │   │   │   ├── assign.ll
    │   │   │   │   │   ├── assign2.ll
    │   │   │   │   │   ├── attrs-below.ll
    │   │   │   │   │   ├── attrs.ll
    │   │   │   │   │   ├── basic-interproc.ll
    │   │   │   │   │   ├── cycle.ll
    │   │   │   │   │   ├── interproc-arg-deref-escape.ll
    │   │   │   │   │   ├── interproc-arg-escape.ll
    │   │   │   │   │   ├── interproc-ret-arg.ll
    │   │   │   │   │   ├── interproc-ret-deref-arg-multilevel.ll
    │   │   │   │   │   ├── interproc-ret-deref-arg.ll
    │   │   │   │   │   ├── interproc-ret-escape.ll
    │   │   │   │   │   ├── interproc-ret-ref-arg-multilevel.ll
    │   │   │   │   │   ├── interproc-ret-ref-arg.ll
    │   │   │   │   │   ├── interproc-ret-unknown.ll
    │   │   │   │   │   ├── interproc-store-arg-multilevel.ll
    │   │   │   │   │   ├── interproc-store-arg-unknown.ll
    │   │   │   │   │   ├── interproc-store-arg.ll
    │   │   │   │   │   ├── memalias.ll
    │   │   │   │   │   └── struct.ll
    │   │   │   │   └── Steensgaard/
    │   │   │   │       ├── arguments-globals.ll
    │   │   │   │       ├── arguments.ll
    │   │   │   │       ├── asm-global-bugfix.ll
    │   │   │   │       ├── attr-escape.ll
    │   │   │   │       ├── basic-interproc.ll
    │   │   │   │       ├── branch-alias.ll
    │   │   │   │       ├── const-expr-gep.ll
    │   │   │   │       ├── const-exprs.ll
    │   │   │   │       ├── constant-over-index.ll
    │   │   │   │       ├── empty.ll
    │   │   │   │       ├── full-store-partial-alias.ll
    │   │   │   │       ├── gep-index-no-alias.ll
    │   │   │   │       ├── gep-signed-arithmetic.ll
    │   │   │   │       ├── interproc-arg-deref-escape.ll
    │   │   │   │       ├── interproc-arg-escape.ll
    │   │   │   │       ├── interproc-ret-arg.ll
    │   │   │   │       ├── interproc-ret-deref-arg-multilevel.ll
    │   │   │   │       ├── interproc-ret-deref-arg.ll
    │   │   │   │       ├── interproc-ret-escape.ll
    │   │   │   │       ├── interproc-ret-ref-arg-multilevel.ll
    │   │   │   │       ├── interproc-ret-ref-arg.ll
    │   │   │   │       ├── interproc-ret-unknown.ll
    │   │   │   │       ├── interproc-store-arg-multilevel.ll
    │   │   │   │       ├── interproc-store-arg-unknown.ll
    │   │   │   │       ├── interproc-store-arg.ll
    │   │   │   │       ├── malloc-and-free.ll
    │   │   │   │       ├── multilevel-combine.ll
    │   │   │   │       ├── multilevel.ll
    │   │   │   │       ├── must-and-partial.ll
    │   │   │   │       ├── opaque-call-alias.ll
    │   │   │   │       ├── phi-and-select.ll
    │   │   │   │       ├── pr27213.ll
    │   │   │   │       ├── simple.ll
    │   │   │   │       ├── stratified-attrs-indexing.ll
    │   │   │   │       └── va.ll
    │   │   │   ├── ConstantFolding/
    │   │   │   │   ├── bitcount.ll
    │   │   │   │   ├── cast-vector.ll
    │   │   │   │   ├── funnel-shift.ll
    │   │   │   │   ├── gep-constanfolding-error.ll
    │   │   │   │   ├── gep-zeroinit-vector.ll
    │   │   │   │   ├── gep.ll
    │   │   │   │   ├── min-max.ll
    │   │   │   │   ├── saturating-add-sub.ll
    │   │   │   │   ├── timeout.ll
    │   │   │   │   ├── vector-undef-elts.ll
    │   │   │   │   └── vectorgep-crash.ll
    │   │   │   ├── CostModel/
    │   │   │   │   ├── no_info.ll
    │   │   │   │   ├── AArch64/
    │   │   │   │   │   ├── bswap.ll
    │   │   │   │   │   ├── div.ll
    │   │   │   │   │   ├── div_cte.ll
    │   │   │   │   │   ├── free-widening-casts.ll
    │   │   │   │   │   ├── gep.ll
    │   │   │   │   │   ├── kryo.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── select.ll
    │   │   │   │   │   ├── shuffle-broadcast.ll
    │   │   │   │   │   ├── shuffle-select.ll
    │   │   │   │   │   ├── shuffle-transpose.ll
    │   │   │   │   │   ├── store.ll
    │   │   │   │   │   └── vector-reduce.ll
    │   │   │   │   ├── AMDGPU/
    │   │   │   │   │   ├── add-sub.ll
    │   │   │   │   │   ├── addrspacecast.ll
    │   │   │   │   │   ├── bit-ops.ll
    │   │   │   │   │   ├── br.ll
    │   │   │   │   │   ├── extractelement.ll
    │   │   │   │   │   ├── fabs.ll
    │   │   │   │   │   ├── fadd.ll
    │   │   │   │   │   ├── fdiv.ll
    │   │   │   │   │   ├── fmul.ll
    │   │   │   │   │   ├── fsub.ll
    │   │   │   │   │   ├── insertelement.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── mul.ll
    │   │   │   │   │   ├── shifts.ll
    │   │   │   │   │   └── shufflevector.ll
    │   │   │   │   ├── ARM/
    │   │   │   │   │   ├── cast.ll
    │   │   │   │   │   ├── divrem.ll
    │   │   │   │   │   ├── gep.ll
    │   │   │   │   │   ├── insertelement.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── select.ll
    │   │   │   │   │   └── shuffle.ll
    │   │   │   │   ├── PowerPC/
    │   │   │   │   │   ├── cmp-expanded.ll
    │   │   │   │   │   ├── ext.ll
    │   │   │   │   │   ├── insert_extract.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── load_store.ll
    │   │   │   │   │   ├── popcnt.ll
    │   │   │   │   │   ├── unal-vec-ldst.ll
    │   │   │   │   │   ├── unaligned_ld_st.ll
    │   │   │   │   │   └── vsr_load_32_64.ll
    │   │   │   │   ├── SystemZ/
    │   │   │   │   │   ├── cmp-ext-01.ll
    │   │   │   │   │   ├── cmp-ext-02.ll
    │   │   │   │   │   ├── cmp-mem.ll
    │   │   │   │   │   ├── cmp-tofp-scalar.ll
    │   │   │   │   │   ├── cmp-tofp.ll
    │   │   │   │   │   ├── cmpsel.ll
    │   │   │   │   │   ├── divrem-const.ll
    │   │   │   │   │   ├── divrem-pow2.ll
    │   │   │   │   │   ├── divrem-reg.ll
    │   │   │   │   │   ├── ext-load.ll
    │   │   │   │   │   ├── fp-arith.ll
    │   │   │   │   │   ├── fp-cast.ll
    │   │   │   │   │   ├── int-arith.ll
    │   │   │   │   │   ├── int-cast.ll
    │   │   │   │   │   ├── int-operands-extcost.ll
    │   │   │   │   │   ├── intrinsic-cost-crash.ll
    │   │   │   │   │   ├── intrinsics.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── load-and-test.ll
    │   │   │   │   │   ├── load-ptr-cmp-fold.ll
    │   │   │   │   │   ├── load_store.ll
    │   │   │   │   │   ├── logical.ll
    │   │   │   │   │   ├── memop-folding-int-arith.ll
    │   │   │   │   │   ├── numvectorregs.ll
    │   │   │   │   │   ├── scalar-cmp-cmp-log-sel.ll
    │   │   │   │   │   ├── shuffle.ll
    │   │   │   │   │   └── vectorinstrs.ll
    │   │   │   │   └── X86/
    │   │   │   │       ├── alternate-shuffle-cost.ll
    │   │   │   │       ├── arith-fma.ll
    │   │   │   │       ├── arith-fp.ll
    │   │   │   │       ├── arith-ssat.ll
    │   │   │   │       ├── arith-usat.ll
    │   │   │   │       ├── arith.ll
    │   │   │   │       ├── bitreverse.ll
    │   │   │   │       ├── bswap.ll
    │   │   │   │       ├── cast-widen.ll
    │   │   │   │       ├── cast.ll
    │   │   │   │       ├── cmp.ll
    │   │   │   │       ├── costmodel.ll
    │   │   │   │       ├── ctlz.ll
    │   │   │   │       ├── ctpop.ll
    │   │   │   │       ├── cttz.ll
    │   │   │   │       ├── div.ll
    │   │   │   │       ├── extend.ll
    │   │   │   │       ├── fptosi-widen.ll
    │   │   │   │       ├── fptosi.ll
    │   │   │   │       ├── fptoui-widen.ll
    │   │   │   │       ├── fptoui.ll
    │   │   │   │       ├── fround.ll
    │   │   │   │       ├── fshl.ll
    │   │   │   │       ├── fshr.ll
    │   │   │   │       ├── gep.ll
    │   │   │   │       ├── i32.ll
    │   │   │   │       ├── insert-extract-at-zero.ll
    │   │   │   │       ├── interleave-load-i32.ll
    │   │   │   │       ├── interleave-store-i32.ll
    │   │   │   │       ├── interleaved-load-float.ll
    │   │   │   │       ├── interleaved-load-i8.ll
    │   │   │   │       ├── interleaved-load-store-double.ll
    │   │   │   │       ├── interleaved-load-store-i64.ll
    │   │   │   │       ├── interleaved-store-i8.ll
    │   │   │   │       ├── intrinsic-cost.ll
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── load_store.ll
    │   │   │   │       ├── loop_v2.ll
    │   │   │   │       ├── masked-intrinsic-cost-widen.ll
    │   │   │   │       ├── masked-intrinsic-cost.ll
    │   │   │   │       ├── min-legal-vector-width.ll
    │   │   │   │       ├── reduce-add-widen.ll
    │   │   │   │       ├── reduce-add.ll
    │   │   │   │       ├── reduce-and-widen.ll
    │   │   │   │       ├── reduce-and.ll
    │   │   │   │       ├── reduce-mul-widen.ll
    │   │   │   │       ├── reduce-mul.ll
    │   │   │   │       ├── reduce-or-widen.ll
    │   │   │   │       ├── reduce-or.ll
    │   │   │   │       ├── reduce-smax-widen.ll
    │   │   │   │       ├── reduce-smax.ll
    │   │   │   │       ├── reduce-smin-widen.ll
    │   │   │   │       ├── reduce-smin.ll
    │   │   │   │       ├── reduce-umax-widen.ll
    │   │   │   │       ├── reduce-umax.ll
    │   │   │   │       ├── reduce-umin-widen.ll
    │   │   │   │       ├── reduce-umin.ll
    │   │   │   │       ├── reduce-xor-widen.ll
    │   │   │   │       ├── reduce-xor.ll
    │   │   │   │       ├── reduction.ll
    │   │   │   │       ├── rem.ll
    │   │   │   │       ├── scalarize.ll
    │   │   │   │       ├── shuffle-broadcast.ll
    │   │   │   │       ├── shuffle-extract_subvector.ll
    │   │   │   │       ├── shuffle-insert_subvector.ll
    │   │   │   │       ├── shuffle-reverse.ll
    │   │   │   │       ├── shuffle-single-src.ll
    │   │   │   │       ├── shuffle-transpose.ll
    │   │   │   │       ├── shuffle-two-src.ll
    │   │   │   │       ├── sitofp-widen.ll
    │   │   │   │       ├── sitofp.ll
    │   │   │   │       ├── slm-arith-costs.ll
    │   │   │   │       ├── sse-itoi.ll
    │   │   │   │       ├── strided-load-i16.ll
    │   │   │   │       ├── strided-load-i32.ll
    │   │   │   │       ├── strided-load-i64.ll
    │   │   │   │       ├── strided-load-i8.ll
    │   │   │   │       ├── testshiftashr-widen.ll
    │   │   │   │       ├── testshiftashr.ll
    │   │   │   │       ├── testshiftlshr-widen.ll
    │   │   │   │       ├── testshiftlshr.ll
    │   │   │   │       ├── testshiftshl-widen.ll
    │   │   │   │       ├── testshiftshl.ll
    │   │   │   │       ├── tiny.ll
    │   │   │   │       ├── trunc.ll
    │   │   │   │       ├── uitofp-widen.ll
    │   │   │   │       ├── uitofp.ll
    │   │   │   │       ├── uniformshift.ll
    │   │   │   │       ├── vdiv-cost.ll
    │   │   │   │       ├── vector-extract.ll
    │   │   │   │       ├── vector-insert.ll
    │   │   │   │       ├── vector_gep.ll
    │   │   │   │       ├── vectorized-loop.ll
    │   │   │   │       ├── vselect-cost.ll
    │   │   │   │       ├── vshift-ashr-cost.ll
    │   │   │   │       ├── vshift-lshr-cost.ll
    │   │   │   │       └── vshift-shl-cost.ll
    │   │   │   ├── Delinearization/
    │   │   │   │   ├── a.ll
    │   │   │   │   ├── constant_functions_multi_dim.ll
    │   │   │   │   ├── divide_by_one.ll
    │   │   │   │   ├── gcd_multiply_expr.ll
    │   │   │   │   ├── himeno_1.ll
    │   │   │   │   ├── himeno_2.ll
    │   │   │   │   ├── iv_times_constant_in_subscript.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── multidim_ivs_and_integer_offsets_3d.ll
    │   │   │   │   ├── multidim_ivs_and_integer_offsets_nts_3d.ll
    │   │   │   │   ├── multidim_ivs_and_parameteric_offsets_3d.ll
    │   │   │   │   ├── multidim_only_ivs_2d.ll
    │   │   │   │   ├── multidim_only_ivs_2d_nested.ll
    │   │   │   │   ├── multidim_only_ivs_3d.ll
    │   │   │   │   ├── multidim_only_ivs_3d_cast.ll
    │   │   │   │   ├── multidim_two_accesses_different_delinearization.ll
    │   │   │   │   ├── parameter_addrec_product.ll
    │   │   │   │   ├── terms_with_identity_factor.ll
    │   │   │   │   ├── type_mismatch.ll
    │   │   │   │   └── undef.ll
    │   │   │   ├── DemandedBits/
    │   │   │   │   ├── basic.ll
    │   │   │   │   ├── intrinsics.ll
    │   │   │   │   └── vectors.ll
    │   │   │   ├── DependenceAnalysis/
    │   │   │   │   ├── AA.ll
    │   │   │   │   ├── Banerjee.ll
    │   │   │   │   ├── BasePtrBug.ll
    │   │   │   │   ├── Constraints.ll
    │   │   │   │   ├── Coupled.ll
    │   │   │   │   ├── DADelin.ll
    │   │   │   │   ├── ExactRDIV.ll
    │   │   │   │   ├── ExactSIV.ll
    │   │   │   │   ├── GCD.ll
    │   │   │   │   ├── Invariant.ll
    │   │   │   │   ├── MIVCheckConst.ll
    │   │   │   │   ├── NonAffineExpr.ll
    │   │   │   │   ├── NonCanonicalizedSubscript.ll
    │   │   │   │   ├── PR21585.ll
    │   │   │   │   ├── Preliminary.ll
    │   │   │   │   ├── Propagating.ll
    │   │   │   │   ├── Separability.ll
    │   │   │   │   ├── StrongSIV.ll
    │   │   │   │   ├── SymbolicRDIV.ll
    │   │   │   │   ├── SymbolicSIV.ll
    │   │   │   │   ├── UsefulGEP.ll
    │   │   │   │   ├── WeakCrossingSIV.ll
    │   │   │   │   ├── WeakZeroDstSIV.ll
    │   │   │   │   ├── WeakZeroSrcSIV.ll
    │   │   │   │   └── ZIV.ll
    │   │   │   ├── DivergenceAnalysis/
    │   │   │   │   ├── AMDGPU/
    │   │   │   │   │   ├── always_uniform.ll
    │   │   │   │   │   ├── atomics.ll
    │   │   │   │   │   ├── hidden_diverge.ll
    │   │   │   │   │   ├── hidden_loopdiverge.ll
    │   │   │   │   │   ├── intrinsics.ll
    │   │   │   │   │   ├── irreducible.ll
    │   │   │   │   │   ├── kernel-args.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── llvm.amdgcn.buffer.atomic.ll
    │   │   │   │   │   ├── llvm.amdgcn.image.atomic.ll
    │   │   │   │   │   ├── no-return-blocks.ll
    │   │   │   │   │   ├── phi-undef.ll
    │   │   │   │   │   ├── temporal_diverge.ll
    │   │   │   │   │   └── workitem-intrinsics.ll
    │   │   │   │   └── NVPTX/
    │   │   │   │       ├── daorder.ll
    │   │   │   │       ├── diverge.ll
    │   │   │   │       ├── hidden_diverge.ll
    │   │   │   │       ├── irreducible.ll
    │   │   │   │       └── lit.local.cfg
    │   │   │   ├── DominanceFrontier/
    │   │   │   │   └── new_pm_test.ll
    │   │   │   ├── Dominators/
    │   │   │   │   ├── 2006-10-02-BreakCritEdges.ll
    │   │   │   │   ├── 2007-01-14-BreakCritEdges.ll
    │   │   │   │   ├── 2007-07-11-SplitBlock.ll
    │   │   │   │   ├── 2007-07-12-SplitBlock.ll
    │   │   │   │   ├── basic.ll
    │   │   │   │   └── invoke.ll
    │   │   │   ├── GlobalsModRef/
    │   │   │   │   ├── 2008-09-03-ReadGlobals.ll
    │   │   │   │   ├── aliastest.ll
    │   │   │   │   ├── atomic-instrs.ll
    │   │   │   │   ├── chaining-analysis.ll
    │   │   │   │   ├── comdat-ipo.ll
    │   │   │   │   ├── dead-uses.ll
    │   │   │   │   ├── func-memattributes.ll
    │   │   │   │   ├── global-used-by-global.ll
    │   │   │   │   ├── inaccessiblememonly.ll
    │   │   │   │   ├── indirect-global.ll
    │   │   │   │   ├── memset-escape.ll
    │   │   │   │   ├── modreftest.ll
    │   │   │   │   ├── no-escape.ll
    │   │   │   │   ├── nonescaping-noalias.ll
    │   │   │   │   ├── pr12351.ll
    │   │   │   │   ├── pr25309.ll
    │   │   │   │   ├── pr35899-dbg-value.ll
    │   │   │   │   ├── purecse.ll
    │   │   │   │   ├── volatile-instrs.ll
    │   │   │   │   └── weak-interposition.ll
    │   │   │   ├── IVUsers/
    │   │   │   │   ├── deep_recursion_in_scev.ll
    │   │   │   │   └── quadradic-exit-value.ll
    │   │   │   ├── LazyCallGraph/
    │   │   │   │   ├── basic.ll
    │   │   │   │   └── non-leaf-intrinsics.ll
    │   │   │   ├── LazyValueAnalysis/
    │   │   │   │   ├── invalidation.ll
    │   │   │   │   ├── lvi-after-jumpthreading.ll
    │   │   │   │   └── lvi-for-ashr.ll
    │   │   │   ├── LegacyDivergenceAnalysis/
    │   │   │   │   ├── AMDGPU/
    │   │   │   │   │   ├── atomics.ll
    │   │   │   │   │   ├── intrinsics.ll
    │   │   │   │   │   ├── kernel-args.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── llvm.amdgcn.buffer.atomic.ll
    │   │   │   │   │   ├── llvm.amdgcn.image.atomic.ll
    │   │   │   │   │   ├── loads.ll
    │   │   │   │   │   ├── no-return-blocks.ll
    │   │   │   │   │   ├── phi-undef.ll
    │   │   │   │   │   ├── unreachable-loop-block.ll
    │   │   │   │   │   └── workitem-intrinsics.ll
    │   │   │   │   └── NVPTX/
    │   │   │   │       ├── diverge.ll
    │   │   │   │       └── lit.local.cfg
    │   │   │   ├── Lint/
    │   │   │   │   ├── address-spaces.ll
    │   │   │   │   ├── check-zero-divide.ll
    │   │   │   │   ├── cppeh-catch-intrinsics-clean.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── memintrin.ll
    │   │   │   │   ├── noalias-byval.ll
    │   │   │   │   ├── noop-cast-expr-no-pointer.ll
    │   │   │   │   └── tail-call-byval.ll
    │   │   │   ├── LoopAccessAnalysis/
    │   │   │   │   ├── backward-dep-different-types.ll
    │   │   │   │   ├── forward-loop-carried.ll
    │   │   │   │   ├── forward-loop-independent.ll
    │   │   │   │   ├── independent-interleaved.ll
    │   │   │   │   ├── interleave-innermost.ll
    │   │   │   │   ├── memcheck-for-loop-invariant.ll
    │   │   │   │   ├── memcheck-off-by-one-error.ll
    │   │   │   │   ├── memcheck-wrapping-pointers.ll
    │   │   │   │   ├── multiple-strides-rt-memory-checks.ll
    │   │   │   │   ├── non-wrapping-pointer.ll
    │   │   │   │   ├── nullptr.ll
    │   │   │   │   ├── number-of-memchecks.ll
    │   │   │   │   ├── pointer-with-unknown-bounds.ll
    │   │   │   │   ├── pr31098.ll
    │   │   │   │   ├── resort-to-memchecks-only.ll
    │   │   │   │   ├── reverse-memcheck-bounds.ll
    │   │   │   │   ├── safe-no-checks.ll
    │   │   │   │   ├── safe-with-dep-distance.ll
    │   │   │   │   ├── store-to-invariant-check1.ll
    │   │   │   │   ├── store-to-invariant-check2.ll
    │   │   │   │   ├── store-to-invariant-check3.ll
    │   │   │   │   ├── stride-access-dependence.ll
    │   │   │   │   ├── underlying-objects-1.ll
    │   │   │   │   ├── underlying-objects-2.ll
    │   │   │   │   ├── unsafe-and-rt-checks.ll
    │   │   │   │   ├── wrapping-pointer-ni.ll
    │   │   │   │   └── wrapping-pointer-versioning.ll
    │   │   │   ├── LoopInfo/
    │   │   │   │   ├── 2003-05-15-NestingProblem.ll
    │   │   │   │   ├── annotated-parallel-complex.ll
    │   │   │   │   └── annotated-parallel-simple.ll
    │   │   │   ├── MemoryDependenceAnalysis/
    │   │   │   │   ├── invalidation.ll
    │   │   │   │   ├── invariant.group-bug.ll
    │   │   │   │   ├── memdep-block-scan-limit.ll
    │   │   │   │   └── memdep_requires_dominator_tree.ll
    │   │   │   ├── MemorySSA/
    │   │   │   │   ├── assume.ll
    │   │   │   │   ├── atomic-clobber.ll
    │   │   │   │   ├── basicaa-memcpy.ll
    │   │   │   │   ├── constant-memory.ll
    │   │   │   │   ├── cyclicphi.ll
    │   │   │   │   ├── forward-unreachable.ll
    │   │   │   │   ├── function-clobber.ll
    │   │   │   │   ├── function-mem-attrs.ll
    │   │   │   │   ├── invariant-groups.ll
    │   │   │   │   ├── lifetime-simple.ll
    │   │   │   │   ├── load-invariant.ll
    │   │   │   │   ├── many-dom-backedge.ll
    │   │   │   │   ├── many-doms.ll
    │   │   │   │   ├── multi-edges.ll
    │   │   │   │   ├── multiple-backedges-hal.ll
    │   │   │   │   ├── multiple-locations.ll
    │   │   │   │   ├── no-disconnected.ll
    │   │   │   │   ├── optimize-use.ll
    │   │   │   │   ├── phi-translation.ll
    │   │   │   │   ├── pr28880.ll
    │   │   │   │   ├── pr36883.ll
    │   │   │   │   ├── ptr-const-mem.ll
    │   │   │   │   └── volatile-clobber.ll
    │   │   │   ├── MustExecute/
    │   │   │   │   ├── const-cond.ll
    │   │   │   │   ├── infinite_loops.ll
    │   │   │   │   └── loop-header.ll
    │   │   │   ├── PhiValues/
    │   │   │   │   ├── basic.ll
    │   │   │   │   ├── big_phi.ll
    │   │   │   │   └── long_phi_chain.ll
    │   │   │   ├── PostDominators/
    │   │   │   │   ├── infinite-loop.ll
    │   │   │   │   ├── infinite-loop2.ll
    │   │   │   │   ├── infinite-loop3.ll
    │   │   │   │   ├── pr1098.ll
    │   │   │   │   ├── pr24415.ll
    │   │   │   │   ├── pr6047_a.ll
    │   │   │   │   ├── pr6047_b.ll
    │   │   │   │   ├── pr6047_c.ll
    │   │   │   │   └── pr6047_d.ll
    │   │   │   ├── ProfileSummary/
    │   │   │   │   └── basic.ll
    │   │   │   ├── RegionInfo/
    │   │   │   │   ├── 20100809_bb_not_in_domtree.ll
    │   │   │   │   ├── bad_node_traversal.ll
    │   │   │   │   ├── block_sort.ll
    │   │   │   │   ├── cond_loop.ll
    │   │   │   │   ├── condition_complicated.ll
    │   │   │   │   ├── condition_complicated_2.ll
    │   │   │   │   ├── condition_forward_edge.ll
    │   │   │   │   ├── condition_same_exit.ll
    │   │   │   │   ├── condition_simple.ll
    │   │   │   │   ├── exit_in_condition.ll
    │   │   │   │   ├── infinite_loop.ll
    │   │   │   │   ├── infinite_loop_2.ll
    │   │   │   │   ├── infinite_loop_3.ll
    │   │   │   │   ├── infinite_loop_4.ll
    │   │   │   │   ├── infinite_loop_5_a.ll
    │   │   │   │   ├── infinite_loop_5_b.ll
    │   │   │   │   ├── infinite_loop_5_c.ll
    │   │   │   │   ├── loop_with_condition.ll
    │   │   │   │   ├── loops_1.ll
    │   │   │   │   ├── loops_2.ll
    │   │   │   │   ├── mix_1.ll
    │   │   │   │   ├── multiple_exiting_edge.ll
    │   │   │   │   ├── nested_loops.ll
    │   │   │   │   ├── next.ll
    │   │   │   │   ├── outgoing_edge.ll
    │   │   │   │   ├── outgoing_edge_1.ll
    │   │   │   │   ├── paper.ll
    │   │   │   │   ├── two_loops_same_header.ll
    │   │   │   │   └── unreachable_bb.ll
    │   │   │   ├── ScalarEvolution/
    │   │   │   │   ├── 2007-07-15-NegativeStride.ll
    │   │   │   │   ├── 2007-08-06-MisinterpretBranch.ll
    │   │   │   │   ├── 2007-08-06-Unsigned.ll
    │   │   │   │   ├── 2007-09-27-LargeStepping.ll
    │   │   │   │   ├── 2007-11-14-SignedAddRec.ll
    │   │   │   │   ├── 2007-11-18-OrInstruction.ll
    │   │   │   │   ├── 2008-02-11-ReversedCondition.ll
    │   │   │   │   ├── 2008-02-12-SMAXTripCount.ll
    │   │   │   │   ├── 2008-02-15-UMax.ll
    │   │   │   │   ├── 2008-05-25-NegativeStepToZero.ll
    │   │   │   │   ├── 2008-06-12-BinomialInt64.ll
    │   │   │   │   ├── 2008-07-12-UnneededSelect1.ll
    │   │   │   │   ├── 2008-07-12-UnneededSelect2.ll
    │   │   │   │   ├── 2008-07-19-InfiniteLoop.ll
    │   │   │   │   ├── 2008-07-19-WrappingIV.ll
    │   │   │   │   ├── 2008-07-29-SGTTripCount.ll
    │   │   │   │   ├── 2008-07-29-SMinExpr.ll
    │   │   │   │   ├── 2008-08-04-IVOverflow.ll
    │   │   │   │   ├── 2008-08-04-LongAddRec.ll
    │   │   │   │   ├── 2008-11-02-QuadraticCrash.ll
    │   │   │   │   ├── 2008-11-15-CubicOOM.ll
    │   │   │   │   ├── 2008-11-18-LessThanOrEqual.ll
    │   │   │   │   ├── 2008-11-18-Stride1.ll
    │   │   │   │   ├── 2008-11-18-Stride2.ll
    │   │   │   │   ├── 2008-12-08-FiniteSGE.ll
    │   │   │   │   ├── 2008-12-11-SMaxOverflow.ll
    │   │   │   │   ├── 2008-12-14-StrideAndSigned.ll
    │   │   │   │   ├── 2008-12-15-DontUseSDiv.ll
    │   │   │   │   ├── 2009-01-02-SignedNegativeStride.ll
    │   │   │   │   ├── 2009-04-22-TruncCast.ll
    │   │   │   │   ├── 2009-05-09-PointerEdgeCount.ll
    │   │   │   │   ├── 2009-07-04-GroupConstantsWidthMismatch.ll
    │   │   │   │   ├── 2010-09-03-RequiredTransitive.ll
    │   │   │   │   ├── 2011-03-09-ExactNoMaxBECount.ll
    │   │   │   │   ├── 2011-04-26-FoldAddRec.ll
    │   │   │   │   ├── 2011-10-04-ConstEvolve.ll
    │   │   │   │   ├── 2012-03-26-LoadConstant.ll
    │   │   │   │   ├── 2012-05-18-LoopPredRecurse.ll
    │   │   │   │   ├── 2012-05-29-MulAddRec.ll
    │   │   │   │   ├── and-xor.ll
    │   │   │   │   ├── avoid-assume-hang.ll
    │   │   │   │   ├── avoid-infinite-recursion-0.ll
    │   │   │   │   ├── avoid-infinite-recursion-1.ll
    │   │   │   │   ├── avoid-smax-0.ll
    │   │   │   │   ├── avoid-smax-1.ll
    │   │   │   │   ├── binomial-explision.ll
    │   │   │   │   ├── cache_loop_exit_limit.ll
    │   │   │   │   ├── constant_condition.ll
    │   │   │   │   ├── different-loops-recs.ll
    │   │   │   │   ├── div-overflow.ll
    │   │   │   │   ├── do-loop.ll
    │   │   │   │   ├── exact_iter_count.ll
    │   │   │   │   ├── exhaustive-trip-counts.ll
    │   │   │   │   ├── expander-replace-congruent-ivs.ll
    │   │   │   │   ├── exponential-behavior.ll
    │   │   │   │   ├── ext-antecedent.ll
    │   │   │   │   ├── extract-highbits-sameconstmask.ll
    │   │   │   │   ├── extract-highbits-variablemask.ll
    │   │   │   │   ├── extract-lowbits-sameconstmask.ll
    │   │   │   │   ├── extract-lowbits-variablemask.ll
    │   │   │   │   ├── flags-from-poison-dbg.ll
    │   │   │   │   ├── flags-from-poison.ll
    │   │   │   │   ├── flattened-0.ll
    │   │   │   │   ├── fold.ll
    │   │   │   │   ├── guards.ll
    │   │   │   │   ├── how-far-to-zero.ll
    │   │   │   │   ├── implied-via-addition.ll
    │   │   │   │   ├── implied-via-division.ll
    │   │   │   │   ├── incorrect-nsw.ll
    │   │   │   │   ├── increasing-or-decreasing-iv.ll
    │   │   │   │   ├── infer-prestart-no-wrap.ll
    │   │   │   │   ├── infer-via-ranges.ll
    │   │   │   │   ├── inner-loop-by-latch-cond-unknown.ll
    │   │   │   │   ├── invalidation.ll
    │   │   │   │   ├── latch-dominating-conditions.ll
    │   │   │   │   ├── limit-depth.ll
    │   │   │   │   ├── load-with-range-metadata.ll
    │   │   │   │   ├── load.ll
    │   │   │   │   ├── lshr-shl-differentconstmask.ll
    │   │   │   │   ├── max-addops-inline.ll
    │   │   │   │   ├── max-addrec-size.ll
    │   │   │   │   ├── max-be-count-not-constant.ll
    │   │   │   │   ├── max-mulops-inline.ll
    │   │   │   │   ├── max-trip-count-address-space.ll
    │   │   │   │   ├── max-trip-count.ll
    │   │   │   │   ├── merge-add-rec-many-inputs.ll
    │   │   │   │   ├── min-max-exprs.ll
    │   │   │   │   ├── no-wrap-add-exprs.ll
    │   │   │   │   ├── no-wrap-unknown-becount.ll
    │   │   │   │   ├── non-IV-phi.ll
    │   │   │   │   ├── nowrap-preinc-limits.ll
    │   │   │   │   ├── nsw-offset-assume.ll
    │   │   │   │   ├── nsw-offset.ll
    │   │   │   │   ├── nsw.ll
    │   │   │   │   ├── nw-sub-is-not-nw-add.ll
    │   │   │   │   ├── overflow-intrinsics.ll
    │   │   │   │   ├── pointer-sign-bits.ll
    │   │   │   │   ├── pr18606-min-zeros.ll
    │   │   │   │   ├── pr18606.ll
    │   │   │   │   ├── pr22179.ll
    │   │   │   │   ├── pr22641.ll
    │   │   │   │   ├── pr22674.ll
    │   │   │   │   ├── pr22856.ll
    │   │   │   │   ├── pr24757.ll
    │   │   │   │   ├── pr25369.ll
    │   │   │   │   ├── pr27315.ll
    │   │   │   │   ├── pr28705.ll
    │   │   │   │   ├── pr34538.ll
    │   │   │   │   ├── pr35890.ll
    │   │   │   │   ├── pr3909.ll
    │   │   │   │   ├── predicated-trip-count.ll
    │   │   │   │   ├── range-signedness.ll
    │   │   │   │   ├── returned.ll
    │   │   │   │   ├── scev-aa.ll
    │   │   │   │   ├── scev-canonical-mode.ll
    │   │   │   │   ├── scev-dispositions.ll
    │   │   │   │   ├── scev-expander-existing-value-offset.ll
    │   │   │   │   ├── scev-expander-incorrect-nowrap.ll
    │   │   │   │   ├── scev-expander-reuse-gep.ll
    │   │   │   │   ├── scev-expander-reuse-unroll.ll
    │   │   │   │   ├── scev-expander-reuse-vect.ll
    │   │   │   │   ├── scev-invalid.ll
    │   │   │   │   ├── scev-prestart-nowrap.ll
    │   │   │   │   ├── sext-inreg.ll
    │   │   │   │   ├── sext-iv-0.ll
    │   │   │   │   ├── sext-iv-1.ll
    │   │   │   │   ├── sext-iv-2.ll
    │   │   │   │   ├── sext-mul.ll
    │   │   │   │   ├── sext-to-zext.ll
    │   │   │   │   ├── sext-zero.ll
    │   │   │   │   ├── shift-op.ll
    │   │   │   │   ├── shl-lshr-differentconstmask.ll
    │   │   │   │   ├── sle.ll
    │   │   │   │   ├── smax-br-phi-idioms.ll
    │   │   │   │   ├── smax.ll
    │   │   │   │   ├── solve-quadratic-i1.ll
    │   │   │   │   ├── solve-quadratic-overflow.ll
    │   │   │   │   ├── solve-quadratic.ll
    │   │   │   │   ├── SolveQuadraticEquation.ll
    │   │   │   │   ├── strip-injective-zext.ll
    │   │   │   │   ├── trip-count-pow2.ll
    │   │   │   │   ├── trip-count-switch.ll
    │   │   │   │   ├── trip-count-unknown-stride.ll
    │   │   │   │   ├── trip-count.ll
    │   │   │   │   ├── trip-count10.ll
    │   │   │   │   ├── trip-count11.ll
    │   │   │   │   ├── trip-count12.ll
    │   │   │   │   ├── trip-count13.ll
    │   │   │   │   ├── trip-count14.ll
    │   │   │   │   ├── trip-count2.ll
    │   │   │   │   ├── trip-count3.ll
    │   │   │   │   ├── trip-count4.ll
    │   │   │   │   ├── trip-count5.ll
    │   │   │   │   ├── trip-count6.ll
    │   │   │   │   ├── trip-count7.ll
    │   │   │   │   ├── trip-count8.ll
    │   │   │   │   ├── trip-count9.ll
    │   │   │   │   ├── tripmultiple_calculation.ll
    │   │   │   │   ├── trunc-simplify.ll
    │   │   │   │   ├── truncate.ll
    │   │   │   │   ├── undefined.ll
    │   │   │   │   ├── unknown_phis.ll
    │   │   │   │   ├── unreachable-code.ll
    │   │   │   │   ├── unsimplified-loop.ll
    │   │   │   │   ├── urem-0.ll
    │   │   │   │   ├── ZeroStep.ll
    │   │   │   │   ├── zext-divrem.ll
    │   │   │   │   ├── zext-mul.ll
    │   │   │   │   ├── zext-signed-addrec.ll
    │   │   │   │   └── zext-wrap.ll
    │   │   │   ├── ScopedNoAliasAA/
    │   │   │   │   ├── basic-domains.ll
    │   │   │   │   ├── basic.ll
    │   │   │   │   └── basic2.ll
    │   │   │   ├── StackSafetyAnalysis/
    │   │   │   │   ├── ipa-alias.ll
    │   │   │   │   ├── ipa.ll
    │   │   │   │   ├── local.ll
    │   │   │   │   ├── memintrin.ll
    │   │   │   │   ├── scev-udiv.ll
    │   │   │   │   └── Inputs/
    │   │   │   │       ├── ipa-alias.ll
    │   │   │   │       └── ipa.ll
    │   │   │   ├── TypeBasedAliasAnalysis/
    │   │   │   │   ├── aggregates.ll
    │   │   │   │   ├── aliastest.ll
    │   │   │   │   ├── argument-promotion.ll
    │   │   │   │   ├── cyclic.ll
    │   │   │   │   ├── dse.ll
    │   │   │   │   ├── dynamic-indices.ll
    │   │   │   │   ├── functionattrs.ll
    │   │   │   │   ├── gvn-nonlocal-type-mismatch.ll
    │   │   │   │   ├── intrinsics.ll
    │   │   │   │   ├── licm.ll
    │   │   │   │   ├── memcpyopt.ll
    │   │   │   │   ├── placement-tbaa.ll
    │   │   │   │   ├── PR17620.ll
    │   │   │   │   ├── precedence.ll
    │   │   │   │   ├── sink.ll
    │   │   │   │   ├── tbaa-path-new.ll
    │   │   │   │   └── tbaa-path.ll
    │   │   │   └── ValueTracking/
    │   │   │       ├── assume.ll
    │   │   │       ├── deref-bitcast-of-gep.ll
    │   │   │       ├── dereferenceable-and-aligned.ll
    │   │   │       ├── func-ptr-lsb.ll
    │   │   │       ├── gep-negative-issue.ll
    │   │   │       ├── get-pointer-base-with-const-off.ll
    │   │   │       ├── invariant.group.ll
    │   │   │       ├── known-bits-from-range-md.ll
    │   │   │       ├── known-non-equal.ll
    │   │   │       ├── known-nonnull-at.ll
    │   │   │       ├── known-power-of-two.ll
    │   │   │       ├── known-signbit-shift.ll
    │   │   │       ├── knownnonzero-shift.ll
    │   │   │       ├── knownzero-addrspacecast.ll
    │   │   │       ├── knownzero-shift.ll
    │   │   │       ├── memory-dereferenceable.ll
    │   │   │       ├── monotonic-phi.ll
    │   │   │       ├── non-negative-phi-bits.ll
    │   │   │       ├── numsignbits-from-assume.ll
    │   │   │       ├── pr23011.ll
    │   │   │       ├── select-pattern.ll
    │   │   │       └── signbits-extract-elt.ll
    │   │   ├── BugPoint/
    │   │   │   ├── compile-custom.ll
    │   │   │   ├── compile-custom.ll.py
    │   │   │   ├── crash-narrowfunctiontest.ll
    │   │   │   ├── func-attrs-keyval.ll
    │   │   │   ├── func-attrs.ll
    │   │   │   ├── invalid-debuginfo.ll
    │   │   │   ├── metadata.ll
    │   │   │   ├── named-md.ll
    │   │   │   ├── remove_arguments_test.ll
    │   │   │   ├── replace-funcs-with-null.ll
    │   │   │   └── unsymbolized.ll
    │   │   ├── CodeGen/
    │   │   │   ├── ARC/
    │   │   │   │   ├── alu.ll
    │   │   │   │   ├── brcc.ll
    │   │   │   │   ├── call.ll
    │   │   │   │   ├── ldst.ll
    │   │   │   │   └── lit.local.cfg
    │   │   │   ├── ARM/
    │   │   │   │   ├── 2006-11-10-CycleInDAG.ll
    │   │   │   │   ├── 2007-01-19-InfiniteLoop.ll
    │   │   │   │   ├── 2007-03-07-CombinerCrash.ll
    │   │   │   │   ├── 2007-03-13-InstrSched.ll
    │   │   │   │   ├── 2007-03-21-JoinIntervalsCrash.ll
    │   │   │   │   ├── 2007-03-27-RegScavengerAssert.ll
    │   │   │   │   ├── 2007-03-30-RegScavengerAssert.ll
    │   │   │   │   ├── 2007-04-02-RegScavengerAssert.ll
    │   │   │   │   ├── 2007-04-03-PEIBug.ll
    │   │   │   │   ├── 2007-04-03-UndefinedSymbol.ll
    │   │   │   │   ├── 2007-04-30-CombinerCrash.ll
    │   │   │   │   ├── 2007-05-03-BadPostIndexedLd.ll
    │   │   │   │   ├── 2007-05-07-tailmerge-1.ll
    │   │   │   │   ├── 2007-05-09-tailmerge-2.ll
    │   │   │   │   ├── 2007-05-14-InlineAsmCstCrash.ll
    │   │   │   │   ├── 2007-05-14-RegScavengerAssert.ll
    │   │   │   │   ├── 2007-05-22-tailmerge-3.ll
    │   │   │   │   ├── 2007-05-23-BadPreIndexedStore.ll
    │   │   │   │   ├── 2007-08-15-ReuseBug.ll
    │   │   │   │   ├── 2008-02-04-LocalRegAllocBug.ll
    │   │   │   │   ├── 2008-02-29-RegAllocLocal.ll
    │   │   │   │   ├── 2008-03-05-SxtInRegBug.ll
    │   │   │   │   ├── 2008-03-07-RegScavengerAssert.ll
    │   │   │   │   ├── 2008-04-04-ScavengerAssert.ll
    │   │   │   │   ├── 2008-04-10-ScavengerAssert.ll
    │   │   │   │   ├── 2008-04-11-PHIofImpDef.ll
    │   │   │   │   ├── 2008-05-19-LiveIntervalsBug.ll
    │   │   │   │   ├── 2008-05-19-ScavengerAssert.ll
    │   │   │   │   ├── 2008-07-17-Fdiv.ll
    │   │   │   │   ├── 2008-07-24-CodeGenPrepCrash.ll
    │   │   │   │   ├── 2008-08-07-AsmPrintBug.ll
    │   │   │   │   ├── 2008-09-17-CoalescerBug.ll
    │   │   │   │   ├── 2008-11-18-ScavengerAssert.ll
    │   │   │   │   ├── 2009-02-16-SpillerBug.ll
    │   │   │   │   ├── 2009-02-22-SoftenFloatVaArg.ll
    │   │   │   │   ├── 2009-02-27-SpillerBug.ll
    │   │   │   │   ├── 2009-03-07-SpillerBug.ll
    │   │   │   │   ├── 2009-03-09-AddrModeBug.ll
    │   │   │   │   ├── 2009-04-06-AsmModifier.ll
    │   │   │   │   ├── 2009-04-08-AggregateAddr.ll
    │   │   │   │   ├── 2009-04-08-FloatUndef.ll
    │   │   │   │   ├── 2009-04-08-FREM.ll
    │   │   │   │   ├── 2009-04-09-RegScavengerAsm.ll
    │   │   │   │   ├── 2009-05-05-DAGCombineBug.ll
    │   │   │   │   ├── 2009-05-07-RegAllocLocal.ll
    │   │   │   │   ├── 2009-05-11-CodePlacementCrash.ll
    │   │   │   │   ├── 2009-05-18-InlineAsmMem.ll
    │   │   │   │   ├── 2009-06-02-ISelCrash.ll
    │   │   │   │   ├── 2009-06-04-MissingLiveIn.ll
    │   │   │   │   ├── 2009-06-15-RegScavengerAssert.ll
    │   │   │   │   ├── 2009-06-19-RegScavengerAssert.ll
    │   │   │   │   ├── 2009-06-22-CoalescerBug.ll
    │   │   │   │   ├── 2009-06-30-RegScavengerAssert.ll
    │   │   │   │   ├── 2009-06-30-RegScavengerAssert2.ll
    │   │   │   │   ├── 2009-06-30-RegScavengerAssert3.ll
    │   │   │   │   ├── 2009-06-30-RegScavengerAssert4.ll
    │   │   │   │   ├── 2009-06-30-RegScavengerAssert5.ll
    │   │   │   │   ├── 2009-07-01-CommuteBug.ll
    │   │   │   │   ├── 2009-07-09-asm-p-constraint.ll
    │   │   │   │   ├── 2009-07-18-RewriterBug.ll
    │   │   │   │   ├── 2009-07-22-ScavengerAssert.ll
    │   │   │   │   ├── 2009-07-22-SchedulerAssert.ll
    │   │   │   │   ├── 2009-07-29-VFP3Registers.ll
    │   │   │   │   ├── 2009-08-02-RegScavengerAssert-Neon.ll
    │   │   │   │   ├── 2009-08-04-RegScavengerAssert-2.ll
    │   │   │   │   ├── 2009-08-04-RegScavengerAssert.ll
    │   │   │   │   ├── 2009-08-15-RegScavenger-EarlyClobber.ll
    │   │   │   │   ├── 2009-08-15-RegScavengerAssert.ll
    │   │   │   │   ├── 2009-08-21-PostRAKill.ll
    │   │   │   │   ├── 2009-08-21-PostRAKill2.ll
    │   │   │   │   ├── 2009-08-21-PostRAKill3.ll
    │   │   │   │   ├── 2009-08-26-ScalarToVector.ll
    │   │   │   │   ├── 2009-08-27-ScalarToVector.ll
    │   │   │   │   ├── 2009-08-29-ExtractEltf32.ll
    │   │   │   │   ├── 2009-08-29-TooLongSplat.ll
    │   │   │   │   ├── 2009-08-31-LSDA-Name.ll
    │   │   │   │   ├── 2009-08-31-TwoRegShuffle.ll
    │   │   │   │   ├── 2009-09-09-AllOnes.ll
    │   │   │   │   ├── 2009-09-09-fpcmp-ole.ll
    │   │   │   │   ├── 2009-09-10-postdec.ll
    │   │   │   │   ├── 2009-09-13-InvalidSubreg.ll
    │   │   │   │   ├── 2009-09-13-InvalidSuperReg.ll
    │   │   │   │   ├── 2009-09-20-LiveIntervalsBug.ll
    │   │   │   │   ├── 2009-09-21-LiveVariablesBug.ll
    │   │   │   │   ├── 2009-09-22-LiveVariablesBug.ll
    │   │   │   │   ├── 2009-09-23-LiveVariablesBug.ll
    │   │   │   │   ├── 2009-09-24-spill-align.ll
    │   │   │   │   ├── 2009-09-27-CoalescerBug.ll
    │   │   │   │   ├── 2009-09-28-LdStOptiBug.ll
    │   │   │   │   ├── 2009-10-02-NEONSubregsBug.ll
    │   │   │   │   ├── 2009-10-16-Scope.ll
    │   │   │   │   ├── 2009-10-27-double-align.ll
    │   │   │   │   ├── 2009-10-30.ll
    │   │   │   │   ├── 2009-11-01-NeonMoves.ll
    │   │   │   │   ├── 2009-11-02-NegativeLane.ll
    │   │   │   │   ├── 2009-11-07-SubRegAsmPrinting.ll
    │   │   │   │   ├── 2009-11-13-CoalescerCrash.ll
    │   │   │   │   ├── 2009-11-13-ScavengerAssert.ll
    │   │   │   │   ├── 2009-11-13-ScavengerAssert2.ll
    │   │   │   │   ├── 2009-11-13-VRRewriterCrash.ll
    │   │   │   │   ├── 2009-11-30-LiveVariablesBug.ll
    │   │   │   │   ├── 2009-12-02-vtrn-undef.ll
    │   │   │   │   ├── 2010-03-04-eabi-fp-spill.ll
    │   │   │   │   ├── 2010-03-04-stm-undef-addr.ll
    │   │   │   │   ├── 2010-03-18-ldm-rtrn.ll
    │   │   │   │   ├── 2010-04-09-NeonSelect.ll
    │   │   │   │   ├── 2010-04-13-v2f64SplitArg.ll
    │   │   │   │   ├── 2010-04-14-SplitVector.ll
    │   │   │   │   ├── 2010-04-15-ScavengerDebugValue.ll
    │   │   │   │   ├── 2010-05-14-IllegalType.ll
    │   │   │   │   ├── 2010-05-17-FastAllocCrash.ll
    │   │   │   │   ├── 2010-05-18-LocalAllocCrash.ll
    │   │   │   │   ├── 2010-05-18-PostIndexBug.ll
    │   │   │   │   ├── 2010-05-19-Shuffles.ll
    │   │   │   │   ├── 2010-05-20-NEONSpillCrash.ll
    │   │   │   │   ├── 2010-05-21-BuildVector.ll
    │   │   │   │   ├── 2010-06-11-vmovdrr-bitcast.ll
    │   │   │   │   ├── 2010-06-21-LdStMultipleBug.ll
    │   │   │   │   ├── 2010-06-21-nondarwin-tc.ll
    │   │   │   │   ├── 2010-06-25-Thumb2ITInvalidIterator.ll
    │   │   │   │   ├── 2010-06-29-PartialRedefFastAlloc.ll
    │   │   │   │   ├── 2010-06-29-SubregImpDefs.ll
    │   │   │   │   ├── 2010-07-26-GlobalMerge.ll
    │   │   │   │   ├── 2010-08-04-EHCrash.ll
    │   │   │   │   ├── 2010-08-04-StackVariable.ll
    │   │   │   │   ├── 2010-09-21-OptCmpBug.ll
    │   │   │   │   ├── 2010-10-25-ifcvt-ldm.ll
    │   │   │   │   ├── 2010-11-15-SpillEarlyClobber.ll
    │   │   │   │   ├── 2010-11-29-PrologueBug.ll
    │   │   │   │   ├── 2010-12-07-PEIBug.ll
    │   │   │   │   ├── 2010-12-08-tpsoft.ll
    │   │   │   │   ├── 2010-12-15-elf-lcomm.ll
    │   │   │   │   ├── 2010-12-17-LocalStackSlotCrash.ll
    │   │   │   │   ├── 2011-01-19-MergedGlobalDbg.ll
    │   │   │   │   ├── 2011-02-04-AntidepMultidef.ll
    │   │   │   │   ├── 2011-02-07-AntidepClobber.ll
    │   │   │   │   ├── 2011-03-10-DAGCombineCrash.ll
    │   │   │   │   ├── 2011-03-15-LdStMultipleBug.ll
    │   │   │   │   ├── 2011-03-23-PeepholeBug.ll
    │   │   │   │   ├── 2011-04-07-schediv.ll
    │   │   │   │   ├── 2011-04-11-MachineLICMBug.ll
    │   │   │   │   ├── 2011-04-12-AlignBug.ll
    │   │   │   │   ├── 2011-04-12-FastRegAlloc.ll
    │   │   │   │   ├── 2011-04-15-AndVFlagPeepholeBug.ll
    │   │   │   │   ├── 2011-04-15-RegisterCmpPeephole.ll
    │   │   │   │   ├── 2011-04-26-SchedTweak.ll
    │   │   │   │   ├── 2011-04-27-IfCvtBug.ll
    │   │   │   │   ├── 2011-05-04-MultipleLandingPadSuccs.ll
    │   │   │   │   ├── 2011-06-09-TailCallByVal.ll
    │   │   │   │   ├── 2011-06-16-TailCallByVal.ll
    │   │   │   │   ├── 2011-06-29-MergeGlobalsAlign.ll
    │   │   │   │   ├── 2011-07-10-GlobalMergeBug.ll
    │   │   │   │   ├── 2011-08-02-MergedGlobalDbg.ll
    │   │   │   │   ├── 2011-08-12-vmovqqqq-pseudo.ll
    │   │   │   │   ├── 2011-08-25-ldmia_ret.ll
    │   │   │   │   ├── 2011-08-29-ldr_pre_imm.ll
    │   │   │   │   ├── 2011-08-29-SchedCycle.ll
    │   │   │   │   ├── 2011-09-09-OddVectorDivision.ll
    │   │   │   │   ├── 2011-09-19-cpsr.ll
    │   │   │   │   ├── 2011-09-28-CMovCombineBug.ll
    │   │   │   │   ├── 2011-10-26-ExpandUnalignedLoadCrash.ll
    │   │   │   │   ├── 2011-10-26-memset-inline.ll
    │   │   │   │   ├── 2011-10-26-memset-with-neon.ll
    │   │   │   │   ├── 2011-11-07-PromoteVectorLoadStore.ll
    │   │   │   │   ├── 2011-11-09-BitcastVectorDouble.ll
    │   │   │   │   ├── 2011-11-09-IllegalVectorFPIntConvert.ll
    │   │   │   │   ├── 2011-11-14-EarlyClobber.ll
    │   │   │   │   ├── 2011-11-28-DAGCombineBug.ll
    │   │   │   │   ├── 2011-11-29-128bitArithmetics.ll
    │   │   │   │   ├── 2011-11-30-MergeAlignment.ll
    │   │   │   │   ├── 2011-12-14-machine-sink.ll
    │   │   │   │   ├── 2011-12-19-sjlj-clobber.ll
    │   │   │   │   ├── 2012-01-23-PostRA-LICM.ll
    │   │   │   │   ├── 2012-01-24-RegSequenceLiveRange.ll
    │   │   │   │   ├── 2012-01-26-CoalescerBug.ll
    │   │   │   │   ├── 2012-01-26-CopyPropKills.ll
    │   │   │   │   ├── 2012-02-01-CoalescerBug.ll
    │   │   │   │   ├── 2012-03-05-FPSCR-bug.ll
    │   │   │   │   ├── 2012-03-13-DAGCombineBug.ll
    │   │   │   │   ├── 2012-03-26-FoldImmBug.ll
    │   │   │   │   ├── 2012-04-02-TwoAddrInstrCrash.ll
    │   │   │   │   ├── 2012-04-10-DAGCombine.ll
    │   │   │   │   ├── 2012-04-24-SplitEHCriticalEdge.ll
    │   │   │   │   ├── 2012-05-04-vmov.ll
    │   │   │   │   ├── 2012-05-10-PreferVMOVtoVDUP32.ll
    │   │   │   │   ├── 2012-05-29-TailDupBug.ll
    │   │   │   │   ├── 2012-06-12-SchedMemLatency.ll
    │   │   │   │   ├── 2012-08-04-DtripleSpillReload.ll
    │   │   │   │   ├── 2012-08-08-legalize-unaligned.ll
    │   │   │   │   ├── 2012-08-09-neon-extload.ll
    │   │   │   │   ├── 2012-08-13-bfi.ll
    │   │   │   │   ├── 2012-08-23-legalize-vmull.ll
    │   │   │   │   ├── 2012-08-27-CopyPhysRegCrash.ll
    │   │   │   │   ├── 2012-08-30-select.ll
    │   │   │   │   ├── 2012-09-18-ARMv4ISelBug.ll
    │   │   │   │   ├── 2012-09-25-InlineAsmScalarToVectorConv.ll
    │   │   │   │   ├── 2012-09-25-InlineAsmScalarToVectorConv2.ll
    │   │   │   │   ├── 2012-10-04-AAPCS-byval-align8.ll
    │   │   │   │   ├── 2012-10-04-FixedFrame-vs-byval.ll
    │   │   │   │   ├── 2012-10-04-LDRB_POST_IMM-Crash.ll
    │   │   │   │   ├── 2012-10-18-PR14099-ByvalFrameAddress.ll
    │   │   │   │   ├── 2012-11-14-subs_carry.ll
    │   │   │   │   ├── 2013-01-21-PR14992.ll
    │   │   │   │   ├── 2013-02-27-expand-vfma.ll
    │   │   │   │   ├── 2013-04-05-Small-ByVal-Structs-PR15293.ll
    │   │   │   │   ├── 2013-04-16-AAPCS-C4-vs-VFP.ll
    │   │   │   │   ├── 2013-04-16-AAPCS-C5-vs-VFP.ll
    │   │   │   │   ├── 2013-04-18-load-overlap-PR14824.ll
    │   │   │   │   ├── 2013-04-21-AAPCS-VA-C.1.cp.ll
    │   │   │   │   ├── 2013-05-02-AAPCS-ByVal-Structs-C4-C5-VFP.ll
    │   │   │   │   ├── 2013-05-02-AAPCS-ByVal-Structs-C4-C5-VFP2.ll
    │   │   │   │   ├── 2013-05-05-IfConvertBug.ll
    │   │   │   │   ├── 2013-05-07-ByteLoadSameAddress.ll
    │   │   │   │   ├── 2013-05-13-AAPCS-byval-padding.ll
    │   │   │   │   ├── 2013-05-13-AAPCS-byval-padding2.ll
    │   │   │   │   ├── 2013-05-13-DAGCombiner-undef-mask.ll
    │   │   │   │   ├── 2013-05-31-char-shift-crash.ll
    │   │   │   │   ├── 2013-06-03-ByVal-2Kbytes.ll
    │   │   │   │   ├── 2013-07-29-vector-or-combine.ll
    │   │   │   │   ├── 2013-10-11-select-stalls.ll
    │   │   │   │   ├── 2013-11-08-inline-asm-neon-array.ll
    │   │   │   │   ├── 2014-01-09-pseudo_expand_implicit_reg.ll
    │   │   │   │   ├── 2014-02-05-vfp-regs-after-stack.ll
    │   │   │   │   ├── 2014-02-21-byval-reg-split-alignment.ll
    │   │   │   │   ├── 2014-05-14-DwarfEHCrash.ll
    │   │   │   │   ├── 2014-07-18-earlyclobber-str-post.ll
    │   │   │   │   ├── 2014-08-04-muls-it.ll
    │   │   │   │   ├── 2015-01-21-thumbv4t-ldstr-opt.ll
    │   │   │   │   ├── 2016-05-01-RegScavengerAssert.ll
    │   │   │   │   ├── 2016-08-24-ARM-LDST-dbginfo-bug.ll
    │   │   │   │   ├── 2018-02-13-PR36079.ll
    │   │   │   │   ├── a15-mla.ll
    │   │   │   │   ├── a15-partial-update.ll
    │   │   │   │   ├── a15-SD-dep.ll
    │   │   │   │   ├── a15.ll
    │   │   │   │   ├── aapcs-hfa-code.ll
    │   │   │   │   ├── aapcs-hfa.ll
    │   │   │   │   ├── acle-intrinsics-rot.ll
    │   │   │   │   ├── acle-intrinsics-v5.ll
    │   │   │   │   ├── acle-intrinsics.ll
    │   │   │   │   ├── add-like-or.ll
    │   │   │   │   ├── addrmode.ll
    │   │   │   │   ├── addrspacecast.ll
    │   │   │   │   ├── addsubcarry-promotion.ll
    │   │   │   │   ├── adv-copy-opt.ll
    │   │   │   │   ├── aeabi-read-tp.ll
    │   │   │   │   ├── aggregate-padding.ll
    │   │   │   │   ├── alias_align.ll
    │   │   │   │   ├── alias_store.ll
    │   │   │   │   ├── aliases.ll
    │   │   │   │   ├── align-sp-adjustment.ll
    │   │   │   │   ├── align.ll
    │   │   │   │   ├── alloc-no-stack-realign.ll
    │   │   │   │   ├── alloca-align.ll
    │   │   │   │   ├── alloca.ll
    │   │   │   │   ├── analyze-branch-bkpt.ll
    │   │   │   │   ├── and-cmpz.ll
    │   │   │   │   ├── and-load-combine.ll
    │   │   │   │   ├── apcs-vfp.ll
    │   │   │   │   ├── arg-copy-elide.ll
    │   │   │   │   ├── argaddr.ll
    │   │   │   │   ├── arguments-nosplit-double.ll
    │   │   │   │   ├── arguments-nosplit-i64.ll
    │   │   │   │   ├── arguments.ll
    │   │   │   │   ├── arguments2.ll
    │   │   │   │   ├── arguments3.ll
    │   │   │   │   ├── arguments4.ll
    │   │   │   │   ├── arguments5.ll
    │   │   │   │   ├── arguments6.ll
    │   │   │   │   ├── arguments7.ll
    │   │   │   │   ├── arguments8.ll
    │   │   │   │   ├── arguments_f64_backfill.ll
    │   │   │   │   ├── arm-abi-attr.ll
    │   │   │   │   ├── arm-and-tst-peephole.ll
    │   │   │   │   ├── arm-asm.ll
    │   │   │   │   ├── arm-eabi.ll
    │   │   │   │   ├── arm-frame-lowering-no-terminator.ll
    │   │   │   │   ├── arm-frameaddr.ll
    │   │   │   │   ├── arm-insert-subvector.ll
    │   │   │   │   ├── arm-macho-tail.ll
    │   │   │   │   ├── arm-modifier.ll
    │   │   │   │   ├── arm-negative-stride.ll
    │   │   │   │   ├── arm-position-independence-jump-table.ll
    │   │   │   │   ├── arm-position-independence.ll
    │   │   │   │   ├── arm-returnaddr.ll
    │   │   │   │   ├── arm-shrink-wrapping-linux.ll
    │   │   │   │   ├── arm-shrink-wrapping.ll
    │   │   │   │   ├── arm-storebytesmerge.ll
    │   │   │   │   ├── arm-ttype-target2.ll
    │   │   │   │   ├── arm-vld1.ll
    │   │   │   │   ├── arm-vlddup-update.ll
    │   │   │   │   ├── arm-vlddup.ll
    │   │   │   │   ├── arm-vst1.ll
    │   │   │   │   ├── arm32-round-conv.ll
    │   │   │   │   ├── arm32-rounding.ll
    │   │   │   │   ├── ARMLoadStoreDBG.mir
    │   │   │   │   ├── armv4.ll
    │   │   │   │   ├── armv8.2a-fp16-vector-intrinsics.ll
    │   │   │   │   ├── atomic-64bit.ll
    │   │   │   │   ├── atomic-cmp.ll
    │   │   │   │   ├── atomic-cmpxchg.ll
    │   │   │   │   ├── atomic-load-store.ll
    │   │   │   │   ├── atomic-op.ll
    │   │   │   │   ├── atomic-ops-m33.ll
    │   │   │   │   ├── atomic-ops-v8.ll
    │   │   │   │   ├── atomicrmw_minmax.ll
    │   │   │   │   ├── available_externally.ll
    │   │   │   │   ├── avoid-cpsr-rmw.ll
    │   │   │   │   ├── bfc.ll
    │   │   │   │   ├── bfi.ll
    │   │   │   │   ├── bfx.ll
    │   │   │   │   ├── bic.ll
    │   │   │   │   ├── bicZext.ll
    │   │   │   │   ├── big-endian-eh-unwind.ll
    │   │   │   │   ├── big-endian-neon-bitconv.ll
    │   │   │   │   ├── big-endian-neon-extend.ll
    │   │   │   │   ├── big-endian-neon-trunc-store.ll
    │   │   │   │   ├── big-endian-ret-f64.ll
    │   │   │   │   ├── big-endian-vector-callee.ll
    │   │   │   │   ├── big-endian-vector-caller.ll
    │   │   │   │   ├── bit-reverse-to-rbit.ll
    │   │   │   │   ├── bits.ll
    │   │   │   │   ├── bool-ext-inc.ll
    │   │   │   │   ├── bswap-inline-asm.ll
    │   │   │   │   ├── bswap16.ll
    │   │   │   │   ├── build-attributes-encoding.s
    │   │   │   │   ├── build-attributes-fn-attr0.ll
    │   │   │   │   ├── build-attributes-fn-attr1.ll
    │   │   │   │   ├── build-attributes-fn-attr2.ll
    │   │   │   │   ├── build-attributes-fn-attr3.ll
    │   │   │   │   ├── build-attributes-fn-attr4.ll
    │   │   │   │   ├── build-attributes-fn-attr5.ll
    │   │   │   │   ├── build-attributes-fn-attr6.ll
    │   │   │   │   ├── build-attributes-optimization-minsize.ll
    │   │   │   │   ├── build-attributes-optimization-mixed.ll
    │   │   │   │   ├── build-attributes-optimization-optnone.ll
    │   │   │   │   ├── build-attributes-optimization-optsize.ll
    │   │   │   │   ├── build-attributes-optimization.ll
    │   │   │   │   ├── build-attributes.ll
    │   │   │   │   ├── bx_fold.ll
    │   │   │   │   ├── byval-align.ll
    │   │   │   │   ├── byval_load_align.ll
    │   │   │   │   ├── cache-intrinsic.ll
    │   │   │   │   ├── call-noret-minsize.ll
    │   │   │   │   ├── call-noret.ll
    │   │   │   │   ├── call-tc.ll
    │   │   │   │   ├── call.ll
    │   │   │   │   ├── call_nolink.ll
    │   │   │   │   ├── carry.ll
    │   │   │   │   ├── cbz-implicit-it-range.ll
    │   │   │   │   ├── cdp.ll
    │   │   │   │   ├── cdp2.ll
    │   │   │   │   ├── cfi-alignment.ll
    │   │   │   │   ├── clang-section.ll
    │   │   │   │   ├── clz.ll
    │   │   │   │   ├── cmn.ll
    │   │   │   │   ├── cmp.ll
    │   │   │   │   ├── cmp1-peephole-thumb.mir
    │   │   │   │   ├── cmp2-peephole-thumb.mir
    │   │   │   │   ├── cmpxchg-idioms.ll
    │   │   │   │   ├── cmpxchg-O0-be.ll
    │   │   │   │   ├── cmpxchg-O0.ll
    │   │   │   │   ├── cmpxchg-weak.ll
    │   │   │   │   ├── cmpxchg.mir
    │   │   │   │   ├── coalesce-dbgvalue.ll
    │   │   │   │   ├── coalesce-subregs.ll
    │   │   │   │   ├── code-placement.ll
    │   │   │   │   ├── codemodel.ll
    │   │   │   │   ├── coff-no-dead-strip.ll
    │   │   │   │   ├── combine-movc-sub.ll
    │   │   │   │   ├── combine-vmovdrr.ll
    │   │   │   │   ├── commute-movcc.ll
    │   │   │   │   ├── compare-call.ll
    │   │   │   │   ├── constant-island-crash.ll
    │   │   │   │   ├── constant-island-movwt.mir
    │   │   │   │   ├── constant-islands-cfg.mir
    │   │   │   │   ├── constant-islands.ll
    │   │   │   │   ├── constantfp.ll
    │   │   │   │   ├── constantpool-align.ll
    │   │   │   │   ├── constantpool-promote-dbg.ll
    │   │   │   │   ├── constantpool-promote-duplicate.ll
    │   │   │   │   ├── constantpool-promote-ldrh.ll
    │   │   │   │   ├── constantpool-promote.ll
    │   │   │   │   ├── constants.ll
    │   │   │   │   ├── copy-by-struct-i32.ll
    │   │   │   │   ├── copy-cpsr.ll
    │   │   │   │   ├── copy-paired-reg.ll
    │   │   │   │   ├── cortex-a57-misched-alu.ll
    │   │   │   │   ├── cortex-a57-misched-basic.ll
    │   │   │   │   ├── cortex-a57-misched-ldm-wrback.ll
    │   │   │   │   ├── cortex-a57-misched-ldm.ll
    │   │   │   │   ├── cortex-a57-misched-stm-wrback.ll
    │   │   │   │   ├── cortex-a57-misched-stm.ll
    │   │   │   │   ├── cortex-a57-misched-vadd.ll
    │   │   │   │   ├── cortex-a57-misched-vfma.ll
    │   │   │   │   ├── cortex-a57-misched-vldm-wrback.ll
    │   │   │   │   ├── cortex-a57-misched-vldm.ll
    │   │   │   │   ├── cortex-a57-misched-vstm-wrback.ll
    │   │   │   │   ├── cortex-a57-misched-vstm.ll
    │   │   │   │   ├── cortex-a57-misched-vsub.ll
    │   │   │   │   ├── cortexr52-misched-basic.ll
    │   │   │   │   ├── crash-greedy-v6.ll
    │   │   │   │   ├── crash-greedy.ll
    │   │   │   │   ├── crash-O0.ll
    │   │   │   │   ├── crash-on-pow2-shufflevector.ll
    │   │   │   │   ├── crash-shufflevector.ll
    │   │   │   │   ├── crash.ll
    │   │   │   │   ├── crc32.ll
    │   │   │   │   ├── cse-call.ll
    │   │   │   │   ├── cse-flags.ll
    │   │   │   │   ├── cse-ldrlit.ll
    │   │   │   │   ├── cse-libcalls.ll
    │   │   │   │   ├── ctor_order.ll
    │   │   │   │   ├── ctors_dtors.ll
    │   │   │   │   ├── cttz.ll
    │   │   │   │   ├── cttz_vector.ll
    │   │   │   │   ├── cxx-tlscc.ll
    │   │   │   │   ├── dag-combine-ldst.ll
    │   │   │   │   ├── dagcombine-anyexttozeroext.ll
    │   │   │   │   ├── dagcombine-concatvector.ll
    │   │   │   │   ├── darwin-eabi.ll
    │   │   │   │   ├── darwin-tls-preserved.ll
    │   │   │   │   ├── darwin-tls.ll
    │   │   │   │   ├── data-in-code-annotations.ll
    │   │   │   │   ├── dbg-range-extension.mir
    │   │   │   │   ├── dbg.ll
    │   │   │   │   ├── DbgValueOtherTargets.test
    │   │   │   │   ├── debug-frame-large-stack.ll
    │   │   │   │   ├── debug-frame-no-debug.ll
    │   │   │   │   ├── debug-frame-vararg.ll
    │   │   │   │   ├── debug-frame.ll
    │   │   │   │   ├── debug-info-arg.ll
    │   │   │   │   ├── debug-info-blocks.ll
    │   │   │   │   ├── debug-info-branch-folding.ll
    │   │   │   │   ├── debug-info-d16-reg.ll
    │   │   │   │   ├── debug-info-no-frame.ll
    │   │   │   │   ├── debug-info-qreg.ll
    │   │   │   │   ├── debug-info-s16-reg.ll
    │   │   │   │   ├── debug-info-sreg2.ll
    │   │   │   │   ├── debug-segmented-stacks.ll
    │   │   │   │   ├── debugtrap.ll
    │   │   │   │   ├── default-float-abi.ll
    │   │   │   │   ├── default-reloc.ll
    │   │   │   │   ├── demanded-bits-and.ll
    │   │   │   │   ├── deprecated-asm.s
    │   │   │   │   ├── deps-fix.ll
    │   │   │   │   ├── disable-fp-elim.ll
    │   │   │   │   ├── disable-tail-calls.ll
    │   │   │   │   ├── div.ll
    │   │   │   │   ├── divmod-eabi.ll
    │   │   │   │   ├── divmod-hwdiv.ll
    │   │   │   │   ├── divmod.ll
    │   │   │   │   ├── domain-conv-vmovs.ll
    │   │   │   │   ├── dsp-mlal.ll
    │   │   │   │   ├── dwarf-eh.ll
    │   │   │   │   ├── dwarf-unwind.ll
    │   │   │   │   ├── dyn-stackalloc.ll
    │   │   │   │   ├── early-cfi-sections.ll
    │   │   │   │   ├── eh-dispcont.ll
    │   │   │   │   ├── eh-resume-darwin.ll
    │   │   │   │   ├── ehabi-filters.ll
    │   │   │   │   ├── ehabi-handlerdata-nounwind.ll
    │   │   │   │   ├── ehabi-handlerdata.ll
    │   │   │   │   ├── ehabi-no-landingpad.ll
    │   │   │   │   ├── ehabi-unwind.ll
    │   │   │   │   ├── ehabi.ll
    │   │   │   │   ├── elf-lcomm-align.ll
    │   │   │   │   ├── emit-big-cst.ll
    │   │   │   │   ├── emutls.ll
    │   │   │   │   ├── emutls1.ll
    │   │   │   │   ├── emutls_generic.ll
    │   │   │   │   ├── execute-only-big-stack-frame.ll
    │   │   │   │   ├── execute-only-section.ll
    │   │   │   │   ├── execute-only.ll
    │   │   │   │   ├── expand-pseudos.mir
    │   │   │   │   ├── extload-knownzero.ll
    │   │   │   │   ├── extloadi1.ll
    │   │   │   │   ├── fabs-neon.ll
    │   │   │   │   ├── fabs-to-bfc.ll
    │   │   │   │   ├── fabss.ll
    │   │   │   │   ├── fadds.ll
    │   │   │   │   ├── fast-isel-align.ll
    │   │   │   │   ├── fast-isel-binary.ll
    │   │   │   │   ├── fast-isel-br-const.ll
    │   │   │   │   ├── fast-isel-br-phi.ll
    │   │   │   │   ├── fast-isel-call-multi-reg-return.ll
    │   │   │   │   ├── fast-isel-call.ll
    │   │   │   │   ├── fast-isel-cmp-imm.ll
    │   │   │   │   ├── fast-isel-conversion.ll
    │   │   │   │   ├── fast-isel-crash.ll
    │   │   │   │   ├── fast-isel-crash2.ll
    │   │   │   │   ├── fast-isel-deadcode.ll
    │   │   │   │   ├── fast-isel-ext.ll
    │   │   │   │   ├── fast-isel-fold.ll
    │   │   │   │   ├── fast-isel-frameaddr.ll
    │   │   │   │   ├── fast-isel-GEP-coalesce.ll
    │   │   │   │   ├── fast-isel-icmp.ll
    │   │   │   │   ├── fast-isel-indirectbr.ll
    │   │   │   │   ├── fast-isel-inline-asm.ll
    │   │   │   │   ├── fast-isel-intrinsic.ll
    │   │   │   │   ├── fast-isel-ldr-str-arm.ll
    │   │   │   │   ├── fast-isel-ldr-str-thumb-neg-index.ll
    │   │   │   │   ├── fast-isel-ldrh-strh-arm.ll
    │   │   │   │   ├── fast-isel-load-store-verify.ll
    │   │   │   │   ├── fast-isel-mvn.ll
    │   │   │   │   ├── fast-isel-pic.ll
    │   │   │   │   ├── fast-isel-pie.ll
    │   │   │   │   ├── fast-isel-pred.ll
    │   │   │   │   ├── fast-isel-redefinition.ll
    │   │   │   │   ├── fast-isel-remat-same-constant.ll
    │   │   │   │   ├── fast-isel-ret.ll
    │   │   │   │   ├── fast-isel-select.ll
    │   │   │   │   ├── fast-isel-shift-materialize.ll
    │   │   │   │   ├── fast-isel-shifter.ll
    │   │   │   │   ├── fast-isel-static.ll
    │   │   │   │   ├── fast-isel-update-valuemap-for-extract.ll
    │   │   │   │   ├── fast-isel-vaddd.ll
    │   │   │   │   ├── fast-isel-vararg.ll
    │   │   │   │   ├── fast-isel.ll
    │   │   │   │   ├── fast-tail-call.ll
    │   │   │   │   ├── fastcc-vfp.ll
    │   │   │   │   ├── fastisel-gep-promote-before-add.ll
    │   │   │   │   ├── fastisel-thumb-litpool.ll
    │   │   │   │   ├── fcmp-xo.ll
    │   │   │   │   ├── fcopysign.ll
    │   │   │   │   ├── fdivs.ll
    │   │   │   │   ├── fence-singlethread.ll
    │   │   │   │   ├── fixunsdfdi.ll
    │   │   │   │   ├── flag-crash.ll
    │   │   │   │   ├── float-helpers.s
    │   │   │   │   ├── floorf.ll
    │   │   │   │   ├── fmacs.ll
    │   │   │   │   ├── fmdrr-fmrrd.ll
    │   │   │   │   ├── fmscs.ll
    │   │   │   │   ├── fmuls.ll
    │   │   │   │   ├── fnattr-trap.ll
    │   │   │   │   ├── fnegs.ll
    │   │   │   │   ├── fnmacs.ll
    │   │   │   │   ├── fnmscs.ll
    │   │   │   │   ├── fnmul.ll
    │   │   │   │   ├── fnmuls.ll
    │   │   │   │   ├── fold-const.ll
    │   │   │   │   ├── fold-sext-sextload.ll
    │   │   │   │   ├── fold-stack-adjust.ll
    │   │   │   │   ├── fold-zext-zextload.ll
    │   │   │   │   ├── formal.ll
    │   │   │   │   ├── fp-arg-shuffle.ll
    │   │   │   │   ├── fp-fast.ll
    │   │   │   │   ├── fp-only-sp.ll
    │   │   │   │   ├── fp.ll
    │   │   │   │   ├── fp16-args.ll
    │   │   │   │   ├── fp16-instructions.ll
    │   │   │   │   ├── fp16-intrinsic-vector-1op.ll
    │   │   │   │   ├── fp16-intrinsic-vector-2op.ll
    │   │   │   │   ├── fp16-litpool-arm.mir
    │   │   │   │   ├── fp16-litpool-thumb.mir
    │   │   │   │   ├── fp16-litpool2-arm.mir
    │   │   │   │   ├── fp16-litpool3-arm.mir
    │   │   │   │   ├── fp16-promote.ll
    │   │   │   │   ├── fp16-v3.ll
    │   │   │   │   ├── fp16-vld.ll
    │   │   │   │   ├── fp16-vminmaxnm-safe.ll
    │   │   │   │   ├── fp16-vminmaxnm-vector.ll
    │   │   │   │   ├── fp16-vminmaxnm.ll
    │   │   │   │   ├── fp16.ll
    │   │   │   │   ├── fp_convert.ll
    │   │   │   │   ├── fparith.ll
    │   │   │   │   ├── fpcmp-f64-neon-opt.ll
    │   │   │   │   ├── fpcmp-opt.ll
    │   │   │   │   ├── fpcmp.ll
    │   │   │   │   ├── fpcmp_ueq.ll
    │   │   │   │   ├── fpconsts.ll
    │   │   │   │   ├── fpconv.ll
    │   │   │   │   ├── fpmem.ll
    │   │   │   │   ├── fpoffset_overflow.mir
    │   │   │   │   ├── fpow.ll
    │   │   │   │   ├── fpowi.ll
    │   │   │   │   ├── fpscr-intrinsics.ll
    │   │   │   │   ├── fptoint.ll
    │   │   │   │   ├── fpvcvtr.ll
    │   │   │   │   ├── frame-register.ll
    │   │   │   │   ├── fsubs.ll
    │   │   │   │   ├── ftrunc.ll
    │   │   │   │   ├── func-argpassing-endian.ll
    │   │   │   │   ├── fusedMAC.ll
    │   │   │   │   ├── gep-optimization.ll
    │   │   │   │   ├── ghc-tcreturn-lowered.ll
    │   │   │   │   ├── global-merge-1.ll
    │   │   │   │   ├── global-merge-addrspace.ll
    │   │   │   │   ├── global-merge-alignment.ll
    │   │   │   │   ├── global-merge-dllexport.ll
    │   │   │   │   ├── global-merge-external-2.ll
    │   │   │   │   ├── global-merge-external.ll
    │   │   │   │   ├── global-merge.ll
    │   │   │   │   ├── globals.ll
    │   │   │   │   ├── gpr-paired-spill-thumbinst.ll
    │   │   │   │   ├── gpr-paired-spill.ll
    │   │   │   │   ├── gv-stubs-crash.ll
    │   │   │   │   ├── half.ll
    │   │   │   │   ├── hardfloat_neon.ll
    │   │   │   │   ├── hello.ll
    │   │   │   │   ├── hfa-in-contiguous-registers.ll
    │   │   │   │   ├── hidden-vis-2.ll
    │   │   │   │   ├── hidden-vis-3.ll
    │   │   │   │   ├── hidden-vis.ll
    │   │   │   │   ├── hints.ll
    │   │   │   │   ├── i1.ll
    │   │   │   │   ├── iabs.ll
    │   │   │   │   ├── ifconv-kills.ll
    │   │   │   │   ├── ifconv-regmask.ll
    │   │   │   │   ├── ifcvt-branch-weight-bug.ll
    │   │   │   │   ├── ifcvt-branch-weight.ll
    │   │   │   │   ├── ifcvt-callback.ll
    │   │   │   │   ├── ifcvt-dead-def.ll
    │   │   │   │   ├── ifcvt-iter-indbr.ll
    │   │   │   │   ├── ifcvt-regmask-noreturn.ll
    │   │   │   │   ├── ifcvt1.ll
    │   │   │   │   ├── ifcvt10.ll
    │   │   │   │   ├── ifcvt11.ll
    │   │   │   │   ├── ifcvt12.ll
    │   │   │   │   ├── ifcvt2.ll
    │   │   │   │   ├── ifcvt3.ll
    │   │   │   │   ├── ifcvt4.ll
    │   │   │   │   ├── ifcvt5.ll
    │   │   │   │   ├── ifcvt6.ll
    │   │   │   │   ├── ifcvt7.ll
    │   │   │   │   ├── ifcvt8.ll
    │   │   │   │   ├── ifcvt9.ll
    │   │   │   │   ├── ifcvt_canFallThroughTo.mir
    │   │   │   │   ├── ifcvt_diamond_unanalyzable.mir
    │   │   │   │   ├── ifcvt_forked_diamond_unanalyzable.mir
    │   │   │   │   ├── ifcvt_simple_bad_zero_prob_succ.mir
    │   │   │   │   ├── ifcvt_simple_unanalyzable.mir
    │   │   │   │   ├── ifcvt_triangleWoCvtToNextEdge.mir
    │   │   │   │   ├── illegal-bitfield-loadstore.ll
    │   │   │   │   ├── illegal-vector-bitcast.ll
    │   │   │   │   ├── imm-peephole-arm.mir
    │   │   │   │   ├── imm-peephole-thumb.mir
    │   │   │   │   ├── imm.ll
    │   │   │   │   ├── immcost.ll
    │   │   │   │   ├── indirect-hidden.ll
    │   │   │   │   ├── indirect-reg-input.ll
    │   │   │   │   ├── indirectbr-2.ll
    │   │   │   │   ├── indirectbr-3.ll
    │   │   │   │   ├── indirectbr.ll
    │   │   │   │   ├── inline-asm-clobber.ll
    │   │   │   │   ├── inline-diagnostics.ll
    │   │   │   │   ├── inlineasm-64bit.ll
    │   │   │   │   ├── inlineasm-error-t-toofewregs.ll
    │   │   │   │   ├── inlineasm-global.ll
    │   │   │   │   ├── inlineasm-imm-arm.ll
    │   │   │   │   ├── inlineasm-imm-thumb.ll
    │   │   │   │   ├── inlineasm-imm-thumb2.ll
    │   │   │   │   ├── inlineasm-ldr-pseudo.ll
    │   │   │   │   ├── inlineasm-operand-implicit-cast.ll
    │   │   │   │   ├── inlineasm-switch-mode-oneway-from-arm.ll
    │   │   │   │   ├── inlineasm-switch-mode-oneway-from-thumb.ll
    │   │   │   │   ├── inlineasm-switch-mode.ll
    │   │   │   │   ├── inlineasm-X-allocation.ll
    │   │   │   │   ├── inlineasm-X-constraint.ll
    │   │   │   │   ├── inlineasm.ll
    │   │   │   │   ├── inlineasm2.ll
    │   │   │   │   ├── inlineasm3.ll
    │   │   │   │   ├── inlineasm4.ll
    │   │   │   │   ├── insn-sched1.ll
    │   │   │   │   ├── int-to-fp.ll
    │   │   │   │   ├── integer_insertelement.ll
    │   │   │   │   ├── interrupt-attr.ll
    │   │   │   │   ├── interval-update-remat.ll
    │   │   │   │   ├── interwork.ll
    │   │   │   │   ├── intrinsics-coprocessor.ll
    │   │   │   │   ├── intrinsics-crypto.ll
    │   │   │   │   ├── intrinsics-memory-barrier.ll
    │   │   │   │   ├── intrinsics-overflow.ll
    │   │   │   │   ├── intrinsics-v8.ll
    │   │   │   │   ├── invalid-target.ll
    │   │   │   │   ├── invalidated-save-point.ll
    │   │   │   │   ├── invoke-donothing-assert.ll
    │   │   │   │   ├── isel-v8i32-crash.ll
    │   │   │   │   ├── ispositive.ll
    │   │   │   │   ├── jump-table-islands-split.ll
    │   │   │   │   ├── jump-table-islands.ll
    │   │   │   │   ├── jump-table-tbh.ll
    │   │   │   │   ├── jumptable-label.ll
    │   │   │   │   ├── krait-cpu-div-attribute.ll
    │   │   │   │   ├── large-stack.ll
    │   │   │   │   ├── large-vector.ll
    │   │   │   │   ├── ldaex-stlex.ll
    │   │   │   │   ├── ldc2l.ll
    │   │   │   │   ├── ldm-base-writeback.ll
    │   │   │   │   ├── ldm-stm-base-materialization.ll
    │   │   │   │   ├── ldm-stm-i256.ll
    │   │   │   │   ├── ldm.ll
    │   │   │   │   ├── ldr.ll
    │   │   │   │   ├── ldr_ext.ll
    │   │   │   │   ├── ldr_frame.ll
    │   │   │   │   ├── ldr_post.ll
    │   │   │   │   ├── ldr_pre.ll
    │   │   │   │   ├── ldrcppic.ll
    │   │   │   │   ├── ldrd-memoper.ll
    │   │   │   │   ├── ldrd.ll
    │   │   │   │   ├── ldrex-frame-size.ll
    │   │   │   │   ├── ldst-f32-2-i32.ll
    │   │   │   │   ├── ldstrex-m.ll
    │   │   │   │   ├── ldstrex.ll
    │   │   │   │   ├── legalize-unaligned-load.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── litpool-licm.ll
    │   │   │   │   ├── load-address-masked.ll
    │   │   │   │   ├── load-arm.ll
    │   │   │   │   ├── load-combine-big-endian.ll
    │   │   │   │   ├── load-combine.ll
    │   │   │   │   ├── load-global.ll
    │   │   │   │   ├── load-global2.ll
    │   │   │   │   ├── load-store-flags.ll
    │   │   │   │   ├── load.ll
    │   │   │   │   ├── load_i1_select.ll
    │   │   │   │   ├── load_store_multiple.ll
    │   │   │   │   ├── load_store_opt_clobber_cpsr.mir
    │   │   │   │   ├── load_store_opt_kill.mir
    │   │   │   │   ├── load_store_opt_reg_limit.mir
    │   │   │   │   ├── local-call.ll
    │   │   │   │   ├── log2_not_readnone.ll
    │   │   │   │   ├── long-setcc.ll
    │   │   │   │   ├── long.ll
    │   │   │   │   ├── long_shift.ll
    │   │   │   │   ├── longMAC.ll
    │   │   │   │   ├── loop-align-cortex-m.ll
    │   │   │   │   ├── loopvectorize_pr33804.ll
    │   │   │   │   ├── lowerMUL-newload.ll
    │   │   │   │   ├── lsr-code-insertion.ll
    │   │   │   │   ├── lsr-icmp-imm.ll
    │   │   │   │   ├── lsr-scale-addr-mode.ll
    │   │   │   │   ├── lsr-unfolded-offset.ll
    │   │   │   │   ├── machine-copyprop.mir
    │   │   │   │   ├── machine-cse-cmp.ll
    │   │   │   │   ├── machine-licm.ll
    │   │   │   │   ├── macho-embedded-float.ll
    │   │   │   │   ├── macho-extern-hidden.ll
    │   │   │   │   ├── macho-frame-offset.ll
    │   │   │   │   ├── MachO-subtypes.ll
    │   │   │   │   ├── macho-trap.ll
    │   │   │   │   ├── mature-mc-support.ll
    │   │   │   │   ├── mem.ll
    │   │   │   │   ├── memcpy-inline.ll
    │   │   │   │   ├── memcpy-ldm-stm.ll
    │   │   │   │   ├── memcpy-no-inline.ll
    │   │   │   │   ├── memfunc.ll
    │   │   │   │   ├── memset-inline.ll
    │   │   │   │   ├── MergeConsecutiveStores.ll
    │   │   │   │   ├── metadata-default.ll
    │   │   │   │   ├── metadata-short-enums.ll
    │   │   │   │   ├── metadata-short-wchar.ll
    │   │   │   │   ├── minmax.ll
    │   │   │   │   ├── minsize-call-cse.ll
    │   │   │   │   ├── minsize-imms.ll
    │   │   │   │   ├── minsize-litpools.ll
    │   │   │   │   ├── misched-copy-arm.ll
    │   │   │   │   ├── misched-fp-basic.ll
    │   │   │   │   ├── misched-fusion-aes.ll
    │   │   │   │   ├── misched-fusion-lit.ll
    │   │   │   │   ├── misched-int-basic-thumb2.mir
    │   │   │   │   ├── misched-int-basic.mir
    │   │   │   │   ├── mls.ll
    │   │   │   │   ├── movcc-double.ll
    │   │   │   │   ├── movt-movw-global.ll
    │   │   │   │   ├── movt.ll
    │   │   │   │   ├── msr-it-block.ll
    │   │   │   │   ├── mul.ll
    │   │   │   │   ├── mul_const.ll
    │   │   │   │   ├── mulhi.ll
    │   │   │   │   ├── mult-alt-generic-arm.ll
    │   │   │   │   ├── mvn.ll
    │   │   │   │   ├── named-reg-alloc.ll
    │   │   │   │   ├── named-reg-notareg.ll
    │   │   │   │   ├── negate-i1.ll
    │   │   │   │   ├── negative-offset.ll
    │   │   │   │   ├── neon-dot-product.ll
    │   │   │   │   ├── neon-fma.ll
    │   │   │   │   ├── neon-spfp.ll
    │   │   │   │   ├── neon-v8.1a.ll
    │   │   │   │   ├── neon_arith1.ll
    │   │   │   │   ├── neon_cmp.ll
    │   │   │   │   ├── neon_div.ll
    │   │   │   │   ├── neon_fpconv.ll
    │   │   │   │   ├── neon_ld1.ll
    │   │   │   │   ├── neon_ld2.ll
    │   │   │   │   ├── neon_minmax.ll
    │   │   │   │   ├── neon_shift.ll
    │   │   │   │   ├── neon_spill.ll
    │   │   │   │   ├── neon_vabs.ll
    │   │   │   │   ├── neon_vshl_minint.ll
    │   │   │   │   ├── nest-register.ll
    │   │   │   │   ├── no-arm-mode.ll
    │   │   │   │   ├── no-cfi.ll
    │   │   │   │   ├── no-cmov2bfi.ll
    │   │   │   │   ├── no-fpscr-liveness.ll
    │   │   │   │   ├── no-fpu.ll
    │   │   │   │   ├── no-tail-call.ll
    │   │   │   │   ├── no_redundant_trunc_for_cmp.ll
    │   │   │   │   ├── none-macho-v4t.ll
    │   │   │   │   ├── none-macho.ll
    │   │   │   │   ├── nonreserved-callframe-with-basereg.mir
    │   │   │   │   ├── noopt-dmb-v7.ll
    │   │   │   │   ├── nop_concat_vectors.ll
    │   │   │   │   ├── noreturn-csr-skip.mir
    │   │   │   │   ├── noreturn.ll
    │   │   │   │   ├── null-streamer.ll
    │   │   │   │   ├── opt-shuff-tstore.ll
    │   │   │   │   ├── optimize-dmbs-v7.ll
    │   │   │   │   ├── optselect-regclass.ll
    │   │   │   │   ├── out-of-registers.ll
    │   │   │   │   ├── overflow-intrinsic-optimizations.ll
    │   │   │   │   ├── pack.ll
    │   │   │   │   ├── peephole-bitcast.ll
    │   │   │   │   ├── peephole-phi.mir
    │   │   │   │   ├── pei-swiftself.mir
    │   │   │   │   ├── phi.ll
    │   │   │   │   ├── pic.ll
    │   │   │   │   ├── pie.ll
    │   │   │   │   ├── plt-relative-reloc.ll
    │   │   │   │   ├── popcnt.ll
    │   │   │   │   ├── pow.ll
    │   │   │   │   ├── pr13249.ll
    │   │   │   │   ├── PR15053.ll
    │   │   │   │   ├── pr18364-movw.ll
    │   │   │   │   ├── pr25317.ll
    │   │   │   │   ├── pr25838.ll
    │   │   │   │   ├── pr26669.ll
    │   │   │   │   ├── pr32545.ll
    │   │   │   │   ├── pr32578.ll
    │   │   │   │   ├── PR32721_ifcvt_triangle_unanalyzable.mir
    │   │   │   │   ├── pr34045-2.ll
    │   │   │   │   ├── pr34045.ll
    │   │   │   │   ├── pr3502.ll
    │   │   │   │   ├── pr35103.ll
    │   │   │   │   ├── PR35379.ll
    │   │   │   │   ├── pr36577.ll
    │   │   │   │   ├── pr39060.ll
    │   │   │   │   ├── pr39571.ll
    │   │   │   │   ├── preferred-align.ll
    │   │   │   │   ├── prefetch.ll
    │   │   │   │   ├── prera-ldst-aliasing.mir
    │   │   │   │   ├── prera-ldst-insertpt.mir
    │   │   │   │   ├── print-memb-operand.ll
    │   │   │   │   ├── print-registers.ll
    │   │   │   │   ├── private.ll
    │   │   │   │   ├── rbit.ll
    │   │   │   │   ├── readcyclecounter.ll
    │   │   │   │   ├── readonly-aliases.ll
    │   │   │   │   ├── readtp.ll
    │   │   │   │   ├── reg_sequence.ll
    │   │   │   │   ├── regpair_hint_phys.ll
    │   │   │   │   ├── relax-per-target-feature.ll
    │   │   │   │   ├── rem_crash.ll
    │   │   │   │   ├── ret0.ll
    │   │   │   │   ├── ret_arg1.ll
    │   │   │   │   ├── ret_arg2.ll
    │   │   │   │   ├── ret_arg3.ll
    │   │   │   │   ├── ret_arg4.ll
    │   │   │   │   ├── ret_arg5.ll
    │   │   │   │   ├── ret_f32_arg2.ll
    │   │   │   │   ├── ret_f32_arg5.ll
    │   │   │   │   ├── ret_f64_arg2.ll
    │   │   │   │   ├── ret_f64_arg_reg_split.ll
    │   │   │   │   ├── ret_f64_arg_split.ll
    │   │   │   │   ├── ret_f64_arg_stack.ll
    │   │   │   │   ├── ret_i128_arg2.ll
    │   │   │   │   ├── ret_i64_arg2.ll
    │   │   │   │   ├── ret_i64_arg3.ll
    │   │   │   │   ├── ret_i64_arg_split.ll
    │   │   │   │   ├── ret_sret_vector.ll
    │   │   │   │   ├── ret_void.ll
    │   │   │   │   ├── returned-ext.ll
    │   │   │   │   ├── returned-trunc-tail-calls.ll
    │   │   │   │   ├── rev.ll
    │   │   │   │   ├── ror.ll
    │   │   │   │   ├── rotate.ll
    │   │   │   │   ├── sat-to-bitop.ll
    │   │   │   │   ├── saxpy10-a9.ll
    │   │   │   │   ├── sbfx.ll
    │   │   │   │   ├── scavenging.mir
    │   │   │   │   ├── sched-it-debug-nodes.mir
    │   │   │   │   ├── sdiv-pow2-arm-size.ll
    │   │   │   │   ├── sdiv-pow2-thumb-size.ll
    │   │   │   │   ├── section-name.ll
    │   │   │   │   ├── section.ll
    │   │   │   │   ├── segmented-stacks-dynamic.ll
    │   │   │   │   ├── segmented-stacks.ll
    │   │   │   │   ├── select-imm.ll
    │   │   │   │   ├── select-undef.ll
    │   │   │   │   ├── select.ll
    │   │   │   │   ├── select_const.ll
    │   │   │   │   ├── select_xform.ll
    │   │   │   │   ├── setcc-logic.ll
    │   │   │   │   ├── setcc-type-mismatch.ll
    │   │   │   │   ├── setjmp_longjmp.ll
    │   │   │   │   ├── shift-combine.ll
    │   │   │   │   ├── shift-i64.ll
    │   │   │   │   ├── shifter_operand.ll
    │   │   │   │   ├── shuffle.ll
    │   │   │   │   ├── sincos.ll
    │   │   │   │   ├── single-issue-r52.mir
    │   │   │   │   ├── sjlj-prepare-critical-edge.ll
    │   │   │   │   ├── sjljeh-swifterror.ll
    │   │   │   │   ├── sjljehprepare-lower-empty-struct.ll
    │   │   │   │   ├── smlad0.ll
    │   │   │   │   ├── smlad1.ll
    │   │   │   │   ├── smlad10.ll
    │   │   │   │   ├── smlad11.ll
    │   │   │   │   ├── smlad12.ll
    │   │   │   │   ├── smlad2.ll
    │   │   │   │   ├── smlad3.ll
    │   │   │   │   ├── smlad4.ll
    │   │   │   │   ├── smlad5.ll
    │   │   │   │   ├── smlad6.ll
    │   │   │   │   ├── smlad7.ll
    │   │   │   │   ├── smlad8.ll
    │   │   │   │   ├── smlad9.ll
    │   │   │   │   ├── smladx-1.ll
    │   │   │   │   ├── smlald0.ll
    │   │   │   │   ├── smlald1.ll
    │   │   │   │   ├── smlald2.ll
    │   │   │   │   ├── smlaldx-1.ll
    │   │   │   │   ├── smlaldx-2.ll
    │   │   │   │   ├── smml.ll
    │   │   │   │   ├── smul.ll
    │   │   │   │   ├── softfp-fabs-fneg.ll
    │   │   │   │   ├── space-directive.ll
    │   │   │   │   ├── special-reg-acore.ll
    │   │   │   │   ├── special-reg-mcore.ll
    │   │   │   │   ├── special-reg-v8m-base.ll
    │   │   │   │   ├── special-reg-v8m-main.ll
    │   │   │   │   ├── special-reg.ll
    │   │   │   │   ├── spill-q.ll
    │   │   │   │   ├── splitkit.ll
    │   │   │   │   ├── ssat-lower.ll
    │   │   │   │   ├── ssat-upper.ll
    │   │   │   │   ├── ssat-v4t.ll
    │   │   │   │   ├── ssat.ll
    │   │   │   │   ├── ssp-data-layout.ll
    │   │   │   │   ├── stack-alignment.ll
    │   │   │   │   ├── stack-frame.ll
    │   │   │   │   ├── stack-protector-bmovpcb_call.ll
    │   │   │   │   ├── stack-size-section.ll
    │   │   │   │   ├── stack_guard_remat.ll
    │   │   │   │   ├── stackpointer.ll
    │   │   │   │   ├── static-addr-hoisting.ll
    │   │   │   │   ├── stc2.ll
    │   │   │   │   ├── stm.ll
    │   │   │   │   ├── str_post.ll
    │   │   │   │   ├── str_pre-2.ll
    │   │   │   │   ├── str_pre.ll
    │   │   │   │   ├── str_trunc.ll
    │   │   │   │   ├── struct-byval-frame-index.ll
    │   │   │   │   ├── struct_byval.ll
    │   │   │   │   ├── struct_byval_arm_t1_t2.ll
    │   │   │   │   ├── sub-cmp-peephole.ll
    │   │   │   │   ├── sub.ll
    │   │   │   │   ├── subreg-remat.ll
    │   │   │   │   ├── subtarget-features-long-calls.ll
    │   │   │   │   ├── subtarget-no-movt.ll
    │   │   │   │   ├── swift-atomics.ll
    │   │   │   │   ├── swift-ios.ll
    │   │   │   │   ├── swift-return.ll
    │   │   │   │   ├── swift-vldm.ll
    │   │   │   │   ├── swifterror.ll
    │   │   │   │   ├── swiftself.ll
    │   │   │   │   ├── switch-minsize.ll
    │   │   │   │   ├── sxt_rot.ll
    │   │   │   │   ├── t2-imm.ll
    │   │   │   │   ├── t2-shrink-ldrpost.ll
    │   │   │   │   ├── t2abs-killflags.ll
    │   │   │   │   ├── tail-call-builtin.ll
    │   │   │   │   ├── tail-call-float.ll
    │   │   │   │   ├── tail-call-weak.ll
    │   │   │   │   ├── tail-call.ll
    │   │   │   │   ├── tail-dup-bundle.mir
    │   │   │   │   ├── tail-dup-kill-flags.ll
    │   │   │   │   ├── tail-dup.ll
    │   │   │   │   ├── tail-merge-branch-weight.ll
    │   │   │   │   ├── tail-opts.ll
    │   │   │   │   ├── tailcall-mem-intrinsics.ll
    │   │   │   │   ├── taildup-branch-weight.ll
    │   │   │   │   ├── test-sharedidx.ll
    │   │   │   │   ├── this-return.ll
    │   │   │   │   ├── thread_pointer.ll
    │   │   │   │   ├── thumb-alignment.ll
    │   │   │   │   ├── thumb-big-stack.ll
    │   │   │   │   ├── thumb-litpool.ll
    │   │   │   │   ├── thumb-stub.ll
    │   │   │   │   ├── thumb1-div.ll
    │   │   │   │   ├── thumb1-ldst-opt.ll
    │   │   │   │   ├── thumb1-varalloc.ll
    │   │   │   │   ├── thumb1_return_sequence.ll
    │   │   │   │   ├── thumb2-it-block.ll
    │   │   │   │   ├── thumb2-size-opt.ll
    │   │   │   │   ├── thumb2-size-reduction-internal-flags.ll
    │   │   │   │   ├── thumb_indirect_calls.ll
    │   │   │   │   ├── tls-models.ll
    │   │   │   │   ├── tls1.ll
    │   │   │   │   ├── tls2.ll
    │   │   │   │   ├── tls3.ll
    │   │   │   │   ├── trap-unreachable.ll
    │   │   │   │   ├── trap.ll
    │   │   │   │   ├── trunc_ldr.ll
    │   │   │   │   ├── truncstore-dag-combine.ll
    │   │   │   │   ├── tst_teq.ll
    │   │   │   │   ├── twoaddrinstr.ll
    │   │   │   │   ├── uint64tof64.ll
    │   │   │   │   ├── umulo-128-legalisation-lowering.ll
    │   │   │   │   ├── umulo-32.ll
    │   │   │   │   ├── umulo-64-legalisation-lowering.ll
    │   │   │   │   ├── unaligned_load_store.ll
    │   │   │   │   ├── unaligned_load_store_vector.ll
    │   │   │   │   ├── unaligned_load_store_vfp.ll
    │   │   │   │   ├── undef-sext.ll
    │   │   │   │   ├── undefined.ll
    │   │   │   │   ├── unfold-shifts.ll
    │   │   │   │   ├── unord.ll
    │   │   │   │   ├── unsafe-fsub.ll
    │   │   │   │   ├── unschedule-first-call.ll
    │   │   │   │   ├── unwind-fp.ll
    │   │   │   │   ├── unwind-init.ll
    │   │   │   │   ├── urem-opt-size.ll
    │   │   │   │   ├── usat-lower.ll
    │   │   │   │   ├── usat-upper.ll
    │   │   │   │   ├── usat-v4t.ll
    │   │   │   │   ├── usat.ll
    │   │   │   │   ├── useaa.ll
    │   │   │   │   ├── uxt_rot.ll
    │   │   │   │   ├── uxtb.ll
    │   │   │   │   ├── v1-constant-fold.ll
    │   │   │   │   ├── v6-jumptable-clobber.mir
    │   │   │   │   ├── v6m-smul-with-overflow.ll
    │   │   │   │   ├── v6m-umul-with-overflow.ll
    │   │   │   │   ├── v7k-abi-align.ll
    │   │   │   │   ├── v7k-libcalls.ll
    │   │   │   │   ├── v7k-sincos.ll
    │   │   │   │   ├── v8m-tail-call.ll
    │   │   │   │   ├── v8m.base-jumptable_alignment.ll
    │   │   │   │   ├── va_arg.ll
    │   │   │   │   ├── vaba.ll
    │   │   │   │   ├── vabd.ll
    │   │   │   │   ├── vabs.ll
    │   │   │   │   ├── vadd.ll
    │   │   │   │   ├── vararg_no_start.ll
    │   │   │   │   ├── varargs-spill-stack-align-nacl.ll
    │   │   │   │   ├── vargs.ll
    │   │   │   │   ├── vargs_align.ll
    │   │   │   │   ├── vbits.ll
    │   │   │   │   ├── vbsl-constant.ll
    │   │   │   │   ├── vbsl.ll
    │   │   │   │   ├── vceq.ll
    │   │   │   │   ├── vcge.ll
    │   │   │   │   ├── vcgt.ll
    │   │   │   │   ├── vcmp-crash.ll
    │   │   │   │   ├── vcnt.ll
    │   │   │   │   ├── vcombine.ll
    │   │   │   │   ├── vcvt-cost.ll
    │   │   │   │   ├── vcvt-v8.ll
    │   │   │   │   ├── vcvt.ll
    │   │   │   │   ├── vcvt_combine.ll
    │   │   │   │   ├── vdiv_combine.ll
    │   │   │   │   ├── vdup.ll
    │   │   │   │   ├── vector-DAGCombine.ll
    │   │   │   │   ├── vector-extend-narrow.ll
    │   │   │   │   ├── vector-load.ll
    │   │   │   │   ├── vector-promotion.ll
    │   │   │   │   ├── vector-spilling.ll
    │   │   │   │   ├── vector-store.ll
    │   │   │   │   ├── vext.ll
    │   │   │   │   ├── vfcmp.ll
    │   │   │   │   ├── vfloatintrinsics.ll
    │   │   │   │   ├── vfp-libcalls.ll
    │   │   │   │   ├── vfp-reg-stride.ll
    │   │   │   │   ├── vfp-regs-dwarf.ll
    │   │   │   │   ├── vfp.ll
    │   │   │   │   ├── vget_lane.ll
    │   │   │   │   ├── vhadd.ll
    │   │   │   │   ├── vhsub.ll
    │   │   │   │   ├── vicmp-64.ll
    │   │   │   │   ├── vicmp.ll
    │   │   │   │   ├── virtregrewriter-subregliveness.mir
    │   │   │   │   ├── vld-vst-upgrade.ll
    │   │   │   │   ├── vld1.ll
    │   │   │   │   ├── vld2.ll
    │   │   │   │   ├── vld3.ll
    │   │   │   │   ├── vld4.ll
    │   │   │   │   ├── vlddup.ll
    │   │   │   │   ├── vldlane.ll
    │   │   │   │   ├── vldm-liveness.ll
    │   │   │   │   ├── vldm-liveness.mir
    │   │   │   │   ├── vldm-sched-a9.ll
    │   │   │   │   ├── vminmax.ll
    │   │   │   │   ├── vminmaxnm-safe.ll
    │   │   │   │   ├── vminmaxnm.ll
    │   │   │   │   ├── vmla.ll
    │   │   │   │   ├── vmls.ll
    │   │   │   │   ├── vmov.ll
    │   │   │   │   ├── vmul.ll
    │   │   │   │   ├── vneg.ll
    │   │   │   │   ├── vpadal.ll
    │   │   │   │   ├── vpadd.ll
    │   │   │   │   ├── vpminmax.ll
    │   │   │   │   ├── vqadd.ll
    │   │   │   │   ├── vqdmul.ll
    │   │   │   │   ├── vqshl.ll
    │   │   │   │   ├── vqshrn.ll
    │   │   │   │   ├── vqsub.ll
    │   │   │   │   ├── vrec.ll
    │   │   │   │   ├── vrev.ll
    │   │   │   │   ├── vrint.ll
    │   │   │   │   ├── vsel.ll
    │   │   │   │   ├── vselect_imax.ll
    │   │   │   │   ├── vshift.ll
    │   │   │   │   ├── vshiftins.ll
    │   │   │   │   ├── vshl.ll
    │   │   │   │   ├── vshll.ll
    │   │   │   │   ├── vshrn.ll
    │   │   │   │   ├── vsra.ll
    │   │   │   │   ├── vst1.ll
    │   │   │   │   ├── vst2.ll
    │   │   │   │   ├── vst3.ll
    │   │   │   │   ├── vst4.ll
    │   │   │   │   ├── vstlane.ll
    │   │   │   │   ├── vsub.ll
    │   │   │   │   ├── vtbl.ll
    │   │   │   │   ├── vtrn.ll
    │   │   │   │   ├── vuzp.ll
    │   │   │   │   ├── vzip.ll
    │   │   │   │   ├── warn-stack.ll
    │   │   │   │   ├── weak.ll
    │   │   │   │   ├── weak2.ll
    │   │   │   │   ├── wide-compares.ll
    │   │   │   │   ├── widen-vmovs.ll
    │   │   │   │   ├── wrong-t2stmia-size-opt.ll
    │   │   │   │   ├── xray-armv6-attribute-instrumentation.ll
    │   │   │   │   ├── xray-armv7-attribute-instrumentation.ll
    │   │   │   │   ├── xray-tail-call-sled.ll
    │   │   │   │   ├── zero-cycle-zero.ll
    │   │   │   │   ├── zext-logic-shift-load.ll
    │   │   │   │   ├── zextload_demandedbits.ll
    │   │   │   │   ├── CGP/
    │   │   │   │   │   ├── arm-cgp-calls.ll
    │   │   │   │   │   ├── arm-cgp-casts.ll
    │   │   │   │   │   ├── arm-cgp-icmps.ll
    │   │   │   │   │   ├── arm-cgp-overflow.ll
    │   │   │   │   │   ├── arm-cgp-phis-ret.ll
    │   │   │   │   │   ├── arm-cgp-pointers.ll
    │   │   │   │   │   ├── arm-cgp-signed-icmps.ll
    │   │   │   │   │   ├── arm-cgp-signed.ll
    │   │   │   │   │   └── arm-cgp-switch.ll
    │   │   │   │   ├── GlobalISel/
    │   │   │   │   │   ├── arm-call-lowering.ll
    │   │   │   │   │   ├── arm-instruction-select-cmp.mir
    │   │   │   │   │   ├── arm-instruction-select-combos.mir
    │   │   │   │   │   ├── arm-instruction-select.mir
    │   │   │   │   │   ├── arm-irtranslator.ll
    │   │   │   │   │   ├── arm-isel-divmod.ll
    │   │   │   │   │   ├── arm-isel-fp.ll
    │   │   │   │   │   ├── arm-isel-globals-pic.ll
    │   │   │   │   │   ├── arm-isel-globals-ropi-rwpi.ll
    │   │   │   │   │   ├── arm-isel-globals-static.ll
    │   │   │   │   │   ├── arm-isel.ll
    │   │   │   │   │   ├── arm-legalize-binops.mir
    │   │   │   │   │   ├── arm-legalize-bitcounts.mir
    │   │   │   │   │   ├── arm-legalize-casts.mir
    │   │   │   │   │   ├── arm-legalize-consts.mir
    │   │   │   │   │   ├── arm-legalize-divmod.mir
    │   │   │   │   │   ├── arm-legalize-exts.mir
    │   │   │   │   │   ├── arm-legalize-fp.mir
    │   │   │   │   │   ├── arm-legalize-load-store.mir
    │   │   │   │   │   ├── arm-legalize-vfp4.mir
    │   │   │   │   │   ├── arm-legalizer.mir
    │   │   │   │   │   ├── arm-param-lowering.ll
    │   │   │   │   │   ├── arm-regbankselect.mir
    │   │   │   │   │   ├── arm-select-copy_to_regclass-of-fptosi.mir
    │   │   │   │   │   ├── arm-select-globals-pic.mir
    │   │   │   │   │   ├── arm-select-globals-ropi-rwpi.mir
    │   │   │   │   │   ├── arm-select-globals-static.mir
    │   │   │   │   │   ├── arm-unsupported.ll
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── pr35375.ll
    │   │   │   │   │   ├── select-pr35926.mir
    │   │   │   │   │   ├── thumb-select-arithmetic-ops.mir
    │   │   │   │   │   ├── thumb-select-casts.mir
    │   │   │   │   │   ├── thumb-select-exts.mir
    │   │   │   │   │   ├── thumb-select-imm.mir
    │   │   │   │   │   ├── thumb-select-load-store.mir
    │   │   │   │   │   └── thumb-select-logical-ops.mir
    │   │   │   │   └── Windows/
    │   │   │   │       ├── aapcs.ll
    │   │   │   │       ├── alloca-no-stack-arg-probe.ll
    │   │   │   │       ├── alloca.ll
    │   │   │   │       ├── builtin_longjmp.ll
    │   │   │   │       ├── chkstk-movw-movt-isel.ll
    │   │   │   │       ├── chkstk-no-stack-arg-probe.ll
    │   │   │   │       ├── chkstk.ll
    │   │   │   │       ├── dbzchk.ll
    │   │   │   │       ├── division-range.ll
    │   │   │   │       ├── division.ll
    │   │   │   │       ├── dllexport.ll
    │   │   │   │       ├── dllimport.ll
    │   │   │   │       ├── frame-register.ll
    │   │   │   │       ├── global-minsize.ll
    │   │   │   │       ├── hard-float.ll
    │   │   │   │       ├── if-cvt-bundle.ll
    │   │   │   │       ├── libcalls.ll
    │   │   │   │       ├── long-calls.ll
    │   │   │   │       ├── mangling.ll
    │   │   │   │       ├── memset.ll
    │   │   │   │       ├── mingw-refptr.ll
    │   │   │   │       ├── mov32t-bundling.ll
    │   │   │   │       ├── movw-movt-relocations.ll
    │   │   │   │       ├── no-aeabi.ll
    │   │   │   │       ├── no-eabi.ll
    │   │   │   │       ├── no-ehabi.ll
    │   │   │   │       ├── no-frame-register.ll
    │   │   │   │       ├── pic.ll
    │   │   │   │       ├── powi.ll
    │   │   │   │       ├── read-only-data.ll
    │   │   │   │       ├── stack-probe-non-default.ll
    │   │   │   │       ├── structors.ll
    │   │   │   │       ├── tls.ll
    │   │   │   │       ├── trivial-gnu-object.ll
    │   │   │   │       ├── vla-cpsr.ll
    │   │   │   │       ├── vla.ll
    │   │   │   │       └── wineh-basic.ll
    │   │   │   ├── Inputs/
    │   │   │   │   └── DbgValueOtherTargets.ll
    │   │   │   ├── MIR/
    │   │   │   │   ├── README
    │   │   │   │   ├── AArch64/
    │   │   │   │   │   ├── addrspace-memoperands.mir
    │   │   │   │   │   ├── atomic-memoperands.mir
    │   │   │   │   │   ├── cfi.mir
    │   │   │   │   │   ├── expected-target-flag-name.mir
    │   │   │   │   │   ├── generic-virtual-registers-error.mir
    │   │   │   │   │   ├── generic-virtual-registers-with-regbank-error.mir
    │   │   │   │   │   ├── intrinsics.mir
    │   │   │   │   │   ├── invalid-target-flag-name.mir
    │   │   │   │   │   ├── invalid-target-memoperands.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── mirCanonCopyCopyProp.mir
    │   │   │   │   │   ├── mirCanonIdempotent.mir
    │   │   │   │   │   ├── multiple-lhs-operands.mir
    │   │   │   │   │   ├── namedvregs.mir
    │   │   │   │   │   ├── parse-low-level-type-invalid0.mir
    │   │   │   │   │   ├── parse-low-level-type-invalid1.mir
    │   │   │   │   │   ├── parse-low-level-type-invalid2.mir
    │   │   │   │   │   ├── parse-low-level-type-invalid3.mir
    │   │   │   │   │   ├── print-parse-overloaded-intrinsics.mir
    │   │   │   │   │   ├── print-parse-vector-of-pointers-llt.mir
    │   │   │   │   │   ├── print-parse-verify-failedISel-property.mir
    │   │   │   │   │   ├── register-operand-bank.mir
    │   │   │   │   │   ├── return-address-signing.mir
    │   │   │   │   │   ├── stack-object-local-offset.mir
    │   │   │   │   │   ├── swp.mir
    │   │   │   │   │   ├── target-flags.mir
    │   │   │   │   │   └── target-memoperands.mir
    │   │   │   │   ├── AMDGPU/
    │   │   │   │   │   ├── expected-target-index-name.mir
    │   │   │   │   │   ├── intrinsics.mir
    │   │   │   │   │   ├── invalid-target-index-operand.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── mir-canon-multi.mir
    │   │   │   │   │   ├── stack-id.mir
    │   │   │   │   │   ├── syncscopes.mir
    │   │   │   │   │   ├── target-flags.mir
    │   │   │   │   │   └── target-index-operands.mir
    │   │   │   │   ├── ARM/
    │   │   │   │   │   ├── bundled-instructions.mir
    │   │   │   │   │   ├── cfi-same-value.mir
    │   │   │   │   │   ├── expected-closing-brace.mir
    │   │   │   │   │   ├── extraneous-closing-brace-error.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── nested-instruction-bundle-error.mir
    │   │   │   │   │   └── target-constant-pools-error.mir
    │   │   │   │   ├── Generic/
    │   │   │   │   │   ├── basic-blocks.mir
    │   │   │   │   │   ├── expected-colon-after-basic-block.mir
    │   │   │   │   │   ├── expected-mbb-reference-for-successor-mbb.mir
    │   │   │   │   │   ├── frame-info.mir
    │   │   │   │   │   ├── global-isel-properties.mir
    │   │   │   │   │   ├── invalid-jump-table-kind.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── llvm-ir-error-reported.mir
    │   │   │   │   │   ├── llvmIR.mir
    │   │   │   │   │   ├── llvmIRMissing.mir
    │   │   │   │   │   ├── machine-basic-block-ir-block-reference.mir
    │   │   │   │   │   ├── machine-basic-block-redefinition-error.mir
    │   │   │   │   │   ├── machine-basic-block-undefined-ir-block.mir
    │   │   │   │   │   ├── machine-basic-block-unknown-name.mir
    │   │   │   │   │   ├── machine-function-missing-body.mir
    │   │   │   │   │   ├── machine-function-missing-function.mir
    │   │   │   │   │   ├── machine-function-missing-name.mir
    │   │   │   │   │   ├── machine-function-redefinition-error.mir
    │   │   │   │   │   ├── machine-function.mir
    │   │   │   │   │   ├── multiRunPass.mir
    │   │   │   │   │   ├── parse-integer-true-false.mir
    │   │   │   │   │   ├── register-info.mir
    │   │   │   │   │   └── runPass.mir
    │   │   │   │   ├── Hexagon/
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── parse-lane-masks.mir
    │   │   │   │   │   └── target-flags.mir
    │   │   │   │   ├── Mips/
    │   │   │   │   │   ├── expected-global-value-or-symbol-after-call-entry.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   └── memory-operands.mir
    │   │   │   │   ├── NVPTX/
    │   │   │   │   │   ├── expected-floating-point-literal.mir
    │   │   │   │   │   ├── floating-point-immediate-operands.mir
    │   │   │   │   │   ├── floating-point-invalid-type-error.mir
    │   │   │   │   │   └── lit.local.cfg
    │   │   │   │   ├── PowerPC/
    │   │   │   │   │   ├── ifcvt-diamond-ret.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── prolog_vec_spills.mir
    │   │   │   │   │   └── unordered-implicit-registers.mir
    │   │   │   │   ├── WebAssembly/
    │   │   │   │   │   ├── int-type-register-class-name.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── typed-immediate-operand-invalid0.mir
    │   │   │   │   │   └── typed-immediate-operand-invalid1.mir
    │   │   │   │   └── X86/
    │   │   │   │       ├── auto-successor.mir
    │   │   │   │       ├── basic-block-liveins.mir
    │   │   │   │       ├── basic-block-not-at-start-of-line-error.mir
    │   │   │   │       ├── block-address-operands.mir
    │   │   │   │       ├── branch-folder-with-label.mir
    │   │   │   │       ├── branch-probabilities.mir
    │   │   │   │       ├── callee-saved-info.mir
    │   │   │   │       ├── cfi-def-cfa-offset.mir
    │   │   │   │       ├── cfi-def-cfa-register.mir
    │   │   │   │       ├── cfi-offset.mir
    │   │   │   │       ├── constant-pool-item-redefinition-error.mir
    │   │   │   │       ├── constant-pool.mir
    │   │   │   │       ├── constant-value-error.mir
    │   │   │   │       ├── copyIRflags.mir
    │   │   │   │       ├── dead-register-flag.mir
    │   │   │   │       ├── def-register-already-tied-error.mir
    │   │   │   │       ├── diexpr-win32.mir
    │   │   │   │       ├── duplicate-memory-operand-flag.mir
    │   │   │   │       ├── duplicate-register-flag-error.mir
    │   │   │   │       ├── early-clobber-register-flag.mir
    │   │   │   │       ├── empty0.mir
    │   │   │   │       ├── empty1.mir
    │   │   │   │       ├── empty2.mir
    │   │   │   │       ├── escape-function-name.ll
    │   │   │   │       ├── expected-align-in-memory-operand.mir
    │   │   │   │       ├── expected-alignment-after-align-in-memory-operand.mir
    │   │   │   │       ├── expected-basic-block-at-start-of-body.mir
    │   │   │   │       ├── expected-block-reference-in-blockaddress.mir
    │   │   │   │       ├── expected-comma-after-cfi-register.mir
    │   │   │   │       ├── expected-comma-after-memory-operand.mir
    │   │   │   │       ├── expected-different-implicit-operand.mir
    │   │   │   │       ├── expected-different-implicit-register-flag.mir
    │   │   │   │       ├── expected-function-reference-after-blockaddress.mir
    │   │   │   │       ├── expected-global-value-after-blockaddress.mir
    │   │   │   │       ├── expected-integer-after-offset-sign.mir
    │   │   │   │       ├── expected-integer-after-tied-def.mir
    │   │   │   │       ├── expected-integer-in-successor-weight.mir
    │   │   │   │       ├── expected-load-or-store-in-memory-operand.mir
    │   │   │   │       ├── expected-machine-operand.mir
    │   │   │   │       ├── expected-metadata-node-after-debug-location.mir
    │   │   │   │       ├── expected-metadata-node-after-exclaim.mir
    │   │   │   │       ├── expected-metadata-node-in-stack-object.mir
    │   │   │   │       ├── expected-named-register-in-allocation-hint.mir
    │   │   │   │       ├── expected-named-register-in-callee-saved-register.mir
    │   │   │   │       ├── expected-named-register-in-functions-livein.mir
    │   │   │   │       ├── expected-named-register-livein.mir
    │   │   │   │       ├── expected-newline-at-end-of-list.mir
    │   │   │   │       ├── expected-number-after-bb.mir
    │   │   │   │       ├── expected-offset-after-cfi-operand.mir
    │   │   │   │       ├── expected-pointer-value-in-memory-operand.mir
    │   │   │   │       ├── expected-positive-alignment-after-align.mir
    │   │   │   │       ├── expected-register-after-cfi-operand.mir
    │   │   │   │       ├── expected-register-after-flags.mir
    │   │   │   │       ├── expected-size-integer-after-memory-operation.mir
    │   │   │   │       ├── expected-size-integer-after-memory-operation2.mir
    │   │   │   │       ├── expected-stack-object.mir
    │   │   │   │       ├── expected-subregister-after-colon.mir
    │   │   │   │       ├── expected-target-flag-name.mir
    │   │   │   │       ├── expected-tied-def-after-lparen.mir
    │   │   │   │       ├── expected-value-in-memory-operand.mir
    │   │   │   │       ├── expected-virtual-register-in-functions-livein.mir
    │   │   │   │       ├── external-symbol-operands.mir
    │   │   │   │       ├── fastmath.mir
    │   │   │   │       ├── fixed-stack-di.mir
    │   │   │   │       ├── fixed-stack-memory-operands.mir
    │   │   │   │       ├── fixed-stack-object-redefinition-error.mir
    │   │   │   │       ├── fixed-stack-objects.mir
    │   │   │   │       ├── frame-info-save-restore-points.mir
    │   │   │   │       ├── frame-info-stack-references.mir
    │   │   │   │       ├── frame-setup-instruction-flag.mir
    │   │   │   │       ├── function-liveins.mir
    │   │   │   │       ├── generic-instr-type.mir
    │   │   │   │       ├── global-value-operands.mir
    │   │   │   │       ├── immediate-operands.mir
    │   │   │   │       ├── implicit-register-flag.mir
    │   │   │   │       ├── inline-asm-registers.mir
    │   │   │   │       ├── inline-asm.mir
    │   │   │   │       ├── instr-symbols-and-mcsymbol-operands.mir
    │   │   │   │       ├── instructions-debug-location.mir
    │   │   │   │       ├── invalid-constant-pool-item.mir
    │   │   │   │       ├── invalid-debug-location.mir
    │   │   │   │       ├── invalid-metadata-node-type.mir
    │   │   │   │       ├── invalid-target-flag-name.mir
    │   │   │   │       ├── invalid-tied-def-index-error.mir
    │   │   │   │       ├── jump-table-info.mir
    │   │   │   │       ├── jump-table-redefinition-error.mir
    │   │   │   │       ├── killed-register-flag.mir
    │   │   │   │       ├── large-cfi-offset-number-error.mir
    │   │   │   │       ├── large-immediate-operand-error.mir
    │   │   │   │       ├── large-index-number-error.mir
    │   │   │   │       ├── large-offset-number-error.mir
    │   │   │   │       ├── large-size-in-memory-operand-error.mir
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── liveout-register-mask.mir
    │   │   │   │       ├── machine-basic-block-operands.mir
    │   │   │   │       ├── machine-instructions.mir
    │   │   │   │       ├── machine-verifier.mir
    │   │   │   │       ├── memory-operands.mir
    │   │   │   │       ├── metadata-operands.mir
    │   │   │   │       ├── missing-closing-quote.mir
    │   │   │   │       ├── missing-comma.mir
    │   │   │   │       ├── missing-implicit-operand.mir
    │   │   │   │       ├── named-registers.mir
    │   │   │   │       ├── newline-handling.mir
    │   │   │   │       ├── null-register-operands.mir
    │   │   │   │       ├── pr38773.mir
    │   │   │   │       ├── register-mask-operands.mir
    │   │   │   │       ├── register-operand-class-invalid0.mir
    │   │   │   │       ├── register-operand-class-invalid1.mir
    │   │   │   │       ├── register-operand-class.mir
    │   │   │   │       ├── register-operands-target-flag-error.mir
    │   │   │   │       ├── renamable-register-flag.mir
    │   │   │   │       ├── roundtrip.mir
    │   │   │   │       ├── simple-register-allocation-hints.mir
    │   │   │   │       ├── spill-slot-fixed-stack-object-aliased.mir
    │   │   │   │       ├── spill-slot-fixed-stack-object-immutable.mir
    │   │   │   │       ├── spill-slot-fixed-stack-objects.mir
    │   │   │   │       ├── stack-object-debug-info.mir
    │   │   │   │       ├── stack-object-invalid-name.mir
    │   │   │   │       ├── stack-object-operand-name-mismatch-error.mir
    │   │   │   │       ├── stack-object-operands.mir
    │   │   │   │       ├── stack-object-redefinition-error.mir
    │   │   │   │       ├── stack-objects.mir
    │   │   │   │       ├── standalone-register-error.mir
    │   │   │   │       ├── subreg-on-physreg.mir
    │   │   │   │       ├── subregister-index-operands.mir
    │   │   │   │       ├── subregister-operands.mir
    │   │   │   │       ├── successor-basic-blocks-weights.mir
    │   │   │   │       ├── successor-basic-blocks.mir
    │   │   │   │       ├── tied-def-operand-invalid.mir
    │   │   │   │       ├── tied-physical-regs-match.mir
    │   │   │   │       ├── undef-register-flag.mir
    │   │   │   │       ├── undefined-fixed-stack-object.mir
    │   │   │   │       ├── undefined-global-value.mir
    │   │   │   │       ├── undefined-ir-block-in-blockaddress.mir
    │   │   │   │       ├── undefined-ir-block-slot-in-blockaddress.mir
    │   │   │   │       ├── undefined-jump-table-id.mir
    │   │   │   │       ├── undefined-named-global-value.mir
    │   │   │   │       ├── undefined-register-class.mir
    │   │   │   │       ├── undefined-stack-object.mir
    │   │   │   │       ├── undefined-value-in-memory-operand.mir
    │   │   │   │       ├── undefined-virtual-register.mir
    │   │   │   │       ├── unexpected-type-phys.mir
    │   │   │   │       ├── unknown-instruction.mir
    │   │   │   │       ├── unknown-machine-basic-block.mir
    │   │   │   │       ├── unknown-metadata-keyword.mir
    │   │   │   │       ├── unknown-metadata-node.mir
    │   │   │   │       ├── unknown-named-machine-basic-block.mir
    │   │   │   │       ├── unknown-register.mir
    │   │   │   │       ├── unknown-subregister-index-op.mir
    │   │   │   │       ├── unknown-subregister-index.mir
    │   │   │   │       ├── unreachable_block.ll
    │   │   │   │       ├── unrecognized-character.mir
    │   │   │   │       ├── variable-sized-stack-object-size-error.mir
    │   │   │   │       ├── variable-sized-stack-objects.mir
    │   │   │   │       ├── virtual-register-redefinition-error.mir
    │   │   │   │       ├── virtual-registers.mir
    │   │   │   │       └── zero-probability.mir
    │   │   │   ├── PowerPC/
    │   │   │   │   ├── 2004-11-30-shr-var-crash.ll
    │   │   │   │   ├── 2004-12-12-ZeroSizeCommon.ll
    │   │   │   │   ├── 2005-01-14-SetSelectCrash.ll
    │   │   │   │   ├── 2005-01-14-UndefLong.ll
    │   │   │   │   ├── 2005-08-12-rlwimi-crash.ll
    │   │   │   │   ├── 2005-10-08-ArithmeticRotate.ll
    │   │   │   │   ├── 2005-11-30-vastart-crash.ll
    │   │   │   │   ├── 2006-01-11-darwin-fp-argument.ll
    │   │   │   │   ├── 2006-04-01-FloatDoubleExtend.ll
    │   │   │   │   ├── 2006-04-19-vmaddfp-crash.ll
    │   │   │   │   ├── 2006-05-12-rlwimi-crash.ll
    │   │   │   │   ├── 2006-07-07-ComputeMaskedBits.ll
    │   │   │   │   ├── 2006-07-19-stwbrx-crash.ll
    │   │   │   │   ├── 2006-08-11-RetVector.ll
    │   │   │   │   ├── 2006-08-15-SelectionCrash.ll
    │   │   │   │   ├── 2006-09-28-shift_64.ll
    │   │   │   │   ├── 2006-11-10-DAGCombineMiscompile.ll
    │   │   │   │   ├── 2006-12-07-SelectCrash.ll
    │   │   │   │   ├── 2007-01-15-AsmDialect.ll
    │   │   │   │   ├── 2007-01-29-lbrx-asm.ll
    │   │   │   │   ├── 2007-02-16-AlignPacked.ll
    │   │   │   │   ├── 2007-02-16-InlineAsmNConstraint.ll
    │   │   │   │   ├── 2007-02-23-lr-saved-twice.ll
    │   │   │   │   ├── 2007-03-24-cntlzd.ll
    │   │   │   │   ├── 2007-03-30-SpillerCrash.ll
    │   │   │   │   ├── 2007-04-24-InlineAsm-I-Modifier.ll
    │   │   │   │   ├── 2007-04-30-InlineAsmEarlyClobber.ll
    │   │   │   │   ├── 2007-05-14-InlineAsmSelectCrash.ll
    │   │   │   │   ├── 2007-05-22-tailmerge-3.ll
    │   │   │   │   ├── 2007-05-30-dagcombine-miscomp.ll
    │   │   │   │   ├── 2007-06-28-BCCISelBug.ll
    │   │   │   │   ├── 2007-08-04-CoalescerAssert.ll
    │   │   │   │   ├── 2007-09-04-AltivecDST.ll
    │   │   │   │   ├── 2007-09-08-unaligned.ll
    │   │   │   │   ├── 2007-09-11-RegCoalescerAssert.ll
    │   │   │   │   ├── 2007-09-12-LiveIntervalsAssert.ll
    │   │   │   │   ├── 2007-10-16-InlineAsmFrameOffset.ll
    │   │   │   │   ├── 2007-10-18-PtrArithmetic.ll
    │   │   │   │   ├── 2007-10-21-LocalRegAllocAssert.ll
    │   │   │   │   ├── 2007-10-21-LocalRegAllocAssert2.ll
    │   │   │   │   ├── 2007-11-04-CoalescerCrash.ll
    │   │   │   │   ├── 2007-11-16-landingpad-split.ll
    │   │   │   │   ├── 2007-11-19-VectorSplitting.ll
    │   │   │   │   ├── 2008-02-05-LiveIntervalsAssert.ll
    │   │   │   │   ├── 2008-02-09-LocalRegAllocAssert.ll
    │   │   │   │   ├── 2008-03-05-RegScavengerAssert.ll
    │   │   │   │   ├── 2008-03-17-RegScavengerCrash.ll
    │   │   │   │   ├── 2008-03-18-RegScavengerAssert.ll
    │   │   │   │   ├── 2008-03-24-AddressRegImm.ll
    │   │   │   │   ├── 2008-03-26-CoalescerBug.ll
    │   │   │   │   ├── 2008-04-16-CoalescerBug.ll
    │   │   │   │   ├── 2008-04-23-CoalescerCrash.ll
    │   │   │   │   ├── 2008-05-01-ppc_fp128.ll
    │   │   │   │   ├── 2008-06-21-F128LoadStore.ll
    │   │   │   │   ├── 2008-06-23-LiveVariablesCrash.ll
    │   │   │   │   ├── 2008-07-10-SplatMiscompile.ll
    │   │   │   │   ├── 2008-07-15-Bswap.ll
    │   │   │   │   ├── 2008-07-15-Fabs.ll
    │   │   │   │   ├── 2008-07-15-SignExtendInreg.ll
    │   │   │   │   ├── 2008-07-17-Fneg.ll
    │   │   │   │   ├── 2008-07-24-PPC64-CCBug.ll
    │   │   │   │   ├── 2008-09-12-CoalescerBug.ll
    │   │   │   │   ├── 2008-10-17-AsmMatchingOperands.ll
    │   │   │   │   ├── 2008-10-28-f128-i32.ll
    │   │   │   │   ├── 2008-10-28-UnprocessedNode.ll
    │   │   │   │   ├── 2008-10-31-PPCF128Libcalls.ll
    │   │   │   │   ├── 2008-12-02-LegalizeTypeAssert.ll
    │   │   │   │   ├── 2009-01-16-DeclareISelBug.ll
    │   │   │   │   ├── 2009-03-17-LSRBug.ll
    │   │   │   │   ├── 2009-05-28-LegalizeBRCC.ll
    │   │   │   │   ├── 2009-08-17-inline-asm-addr-mode-breakage.ll
    │   │   │   │   ├── 2009-09-18-carrybit.ll
    │   │   │   │   ├── 2009-11-15-ProcImpDefsBug.ll
    │   │   │   │   ├── 2009-11-25-ImpDefBug.ll
    │   │   │   │   ├── 2010-02-04-EmptyGlobal.ll
    │   │   │   │   ├── 2010-02-12-saveCR.ll
    │   │   │   │   ├── 2010-03-09-indirect-call.ll
    │   │   │   │   ├── 2010-04-01-MachineCSEBug.ll
    │   │   │   │   ├── 2010-05-03-retaddr1.ll
    │   │   │   │   ├── 2010-10-11-Fast-Varargs.ll
    │   │   │   │   ├── 2010-12-18-PPCStackRefs.ll
    │   │   │   │   ├── 2011-12-05-NoSpillDupCR.ll
    │   │   │   │   ├── 2011-12-06-SpillAndRestoreCR.ll
    │   │   │   │   ├── 2011-12-08-DemandedBitsMiscompile.ll
    │   │   │   │   ├── 2012-10-11-dynalloc.ll
    │   │   │   │   ├── 2012-10-12-bitcast.ll
    │   │   │   │   ├── 2012-11-16-mischedcall.ll
    │   │   │   │   ├── 2013-05-15-preinc-fold.ll
    │   │   │   │   ├── 2013-07-01-PHIElimBug.mir
    │   │   │   │   ├── 2016-01-07-BranchWeightCrash.ll
    │   │   │   │   ├── 2016-04-16-ADD8TLS.ll
    │   │   │   │   ├── a2q-stackalign.ll
    │   │   │   │   ├── a2q.ll
    │   │   │   │   ├── aa-tbaa.ll
    │   │   │   │   ├── aantidep-inline-asm-use.ll
    │   │   │   │   ├── add-fi.ll
    │   │   │   │   ├── addc.ll
    │   │   │   │   ├── adde_return_type.ll
    │   │   │   │   ├── addegluecrash.ll
    │   │   │   │   ├── addi-licm.ll
    │   │   │   │   ├── addi-offset-fold.ll
    │   │   │   │   ├── addi-reassoc.ll
    │   │   │   │   ├── addisdtprelha-nonr3.mir
    │   │   │   │   ├── addrfuncstr.ll
    │   │   │   │   ├── addrspacecast.ll
    │   │   │   │   ├── addze.ll
    │   │   │   │   ├── aggressive-anti-dep-breaker-subreg.ll
    │   │   │   │   ├── align.ll
    │   │   │   │   ├── allocate-r0.ll
    │   │   │   │   ├── and-branch.ll
    │   │   │   │   ├── and-elim.ll
    │   │   │   │   ├── and-imm.ll
    │   │   │   │   ├── andc.ll
    │   │   │   │   ├── anyext_srl.ll
    │   │   │   │   ├── arr-fp-arg-no-copy.ll
    │   │   │   │   ├── ashr-neg1.ll
    │   │   │   │   ├── asm-constraints.ll
    │   │   │   │   ├── asm-dialect.ll
    │   │   │   │   ├── asm-printer-topological-order.ll
    │   │   │   │   ├── asm-Zy.ll
    │   │   │   │   ├── asym-regclass-copy.ll
    │   │   │   │   ├── atomic-1.ll
    │   │   │   │   ├── atomic-2.ll
    │   │   │   │   ├── atomic-minmax.ll
    │   │   │   │   ├── atomics-constant.ll
    │   │   │   │   ├── atomics-fences.ll
    │   │   │   │   ├── atomics-indexed.ll
    │   │   │   │   ├── atomics-regression.ll
    │   │   │   │   ├── atomics.ll
    │   │   │   │   ├── available-externally.ll
    │   │   │   │   ├── bdzlr.ll
    │   │   │   │   ├── big-endian-actual-args.ll
    │   │   │   │   ├── big-endian-call-result.ll
    │   │   │   │   ├── big-endian-store-forward.ll
    │   │   │   │   ├── bitcasts-direct-move.ll
    │   │   │   │   ├── bitfieldinsert.ll
    │   │   │   │   ├── blockaddress.ll
    │   │   │   │   ├── bool-math.ll
    │   │   │   │   ├── BoolRetToIntTest.ll
    │   │   │   │   ├── bperm.ll
    │   │   │   │   ├── branch_coalesce.ll
    │   │   │   │   ├── BreakableToken-reduced.ll
    │   │   │   │   ├── bswap-load-store.ll
    │   │   │   │   ├── build-vector-tests.ll
    │   │   │   │   ├── builtins-ppc-elf2-abi.ll
    │   │   │   │   ├── builtins-ppc-p8vector.ll
    │   │   │   │   ├── builtins-ppc-p9-f128.ll
    │   │   │   │   ├── bv-pres-v8i1.ll
    │   │   │   │   ├── bv-widen-undef.ll
    │   │   │   │   ├── byval-agg-info.ll
    │   │   │   │   ├── can-lower-ret.ll
    │   │   │   │   ├── cannonicalize-vector-shifts.ll
    │   │   │   │   ├── cc.ll
    │   │   │   │   ├── change-no-infs.ll
    │   │   │   │   ├── cmp-cmp.ll
    │   │   │   │   ├── cmpb-ppc32.ll
    │   │   │   │   ├── cmpb.ll
    │   │   │   │   ├── coalesce-ext.ll
    │   │   │   │   ├── codemodel.ll
    │   │   │   │   ├── coldcc2.ll
    │   │   │   │   ├── combine-setcc.ll
    │   │   │   │   ├── combine-to-pre-index-store-crash.ll
    │   │   │   │   ├── compare-duplicate.ll
    │   │   │   │   ├── compare-simm.ll
    │   │   │   │   ├── CompareEliminationSpillIssue.ll
    │   │   │   │   ├── constants-i64.ll
    │   │   │   │   ├── convert-rr-to-ri-instrs-out-of-range.mir
    │   │   │   │   ├── convert-rr-to-ri-instrs-R0-special-handling.mir
    │   │   │   │   ├── convert-rr-to-ri-p9-vector.mir
    │   │   │   │   ├── cr-spills.ll
    │   │   │   │   ├── cr1eq-no-extra-moves.ll
    │   │   │   │   ├── cr_spilling.ll
    │   │   │   │   ├── crash.ll
    │   │   │   │   ├── crbit-asm-disabled.ll
    │   │   │   │   ├── crbit-asm.ll
    │   │   │   │   ├── crbits.ll
    │   │   │   │   ├── crsave.ll
    │   │   │   │   ├── ctr-cleanup.ll
    │   │   │   │   ├── ctr-minmaxnum.ll
    │   │   │   │   ├── ctrloop-asm.ll
    │   │   │   │   ├── ctrloop-fp64.ll
    │   │   │   │   ├── ctrloop-i128.ll
    │   │   │   │   ├── ctrloop-i64.ll
    │   │   │   │   ├── ctrloop-intrin.ll
    │   │   │   │   ├── ctrloop-large-ec.ll
    │   │   │   │   ├── ctrloop-le.ll
    │   │   │   │   ├── ctrloop-lt.ll
    │   │   │   │   ├── ctrloop-ne.ll
    │   │   │   │   ├── ctrloop-reg.ll
    │   │   │   │   ├── ctrloop-s000.ll
    │   │   │   │   ├── ctrloop-sh.ll
    │   │   │   │   ├── ctrloop-shortLoops.ll
    │   │   │   │   ├── ctrloop-udivti3.ll
    │   │   │   │   ├── ctrloops-hot-exit.ll
    │   │   │   │   ├── ctrloops-softfloat.ll
    │   │   │   │   ├── ctrloops.ll
    │   │   │   │   ├── cttz.ll
    │   │   │   │   ├── darwin-labels.ll
    │   │   │   │   ├── dbg.ll
    │   │   │   │   ├── DbgValueOtherTargets.test
    │   │   │   │   ├── debuginfo-split-int.ll
    │   │   │   │   ├── delete-node.ll
    │   │   │   │   ├── direct-move-profit.ll
    │   │   │   │   ├── div-2.ll
    │   │   │   │   ├── div-e-32.ll
    │   │   │   │   ├── div-e-all.ll
    │   │   │   │   ├── duplicate-returns-for-tailcall.ll
    │   │   │   │   ├── e500-1.ll
    │   │   │   │   ├── early-ret2.ll
    │   │   │   │   ├── ec-input.ll
    │   │   │   │   ├── eh-dwarf-cfa.ll
    │   │   │   │   ├── empty-functions.ll
    │   │   │   │   ├── emptystruct.ll
    │   │   │   │   ├── emutls_generic.ll
    │   │   │   │   ├── eqv-andc-orc-nor.ll
    │   │   │   │   ├── expand-contiguous-isel.ll
    │   │   │   │   ├── expand-foldable-isel.ll
    │   │   │   │   ├── expand-isel-1.mir
    │   │   │   │   ├── expand-isel-10.mir
    │   │   │   │   ├── expand-isel-2.mir
    │   │   │   │   ├── expand-isel-3.mir
    │   │   │   │   ├── expand-isel-4.mir
    │   │   │   │   ├── expand-isel-5.mir
    │   │   │   │   ├── expand-isel-7.mir
    │   │   │   │   ├── expand-isel-8.mir
    │   │   │   │   ├── expand-isel-9.mir
    │   │   │   │   ├── expand-isel.ll
    │   │   │   │   ├── extra-toc-reg-deps.ll
    │   │   │   │   ├── extract-and-store.ll
    │   │   │   │   ├── extsh.ll
    │   │   │   │   ├── extswsli.ll
    │   │   │   │   ├── f128-aggregates.ll
    │   │   │   │   ├── f128-arith.ll
    │   │   │   │   ├── f128-bitcast.ll
    │   │   │   │   ├── f128-compare.ll
    │   │   │   │   ├── f128-conv.ll
    │   │   │   │   ├── f128-truncateNconv.ll
    │   │   │   │   ├── f128-vecExtractNconv.ll
    │   │   │   │   ├── f32-to-i64.ll
    │   │   │   │   ├── fabs.ll
    │   │   │   │   ├── fast-isel-binary.ll
    │   │   │   │   ├── fast-isel-br-const.ll
    │   │   │   │   ├── fast-isel-call.ll
    │   │   │   │   ├── fast-isel-cmp-imm.ll
    │   │   │   │   ├── fast-isel-const.ll
    │   │   │   │   ├── fast-isel-conversion-p5.ll
    │   │   │   │   ├── fast-isel-conversion.ll
    │   │   │   │   ├── fast-isel-crash.ll
    │   │   │   │   ├── fast-isel-fcmp-nan.ll
    │   │   │   │   ├── fast-isel-fold.ll
    │   │   │   │   ├── fast-isel-fpconv.ll
    │   │   │   │   ├── fast-isel-GEP-coalesce.ll
    │   │   │   │   ├── fast-isel-i64offset.ll
    │   │   │   │   ├── fast-isel-icmp-split.ll
    │   │   │   │   ├── fast-isel-indirectbr.ll
    │   │   │   │   ├── fast-isel-load-store-vsx.ll
    │   │   │   │   ├── fast-isel-load-store.ll
    │   │   │   │   ├── fast-isel-redefinition.ll
    │   │   │   │   ├── fast-isel-shifter.ll
    │   │   │   │   ├── fastcc_stacksize.ll
    │   │   │   │   ├── fastisel-gep-promote-before-add.ll
    │   │   │   │   ├── fcpsgn.ll
    │   │   │   │   ├── fdiv-combine.ll
    │   │   │   │   ├── float-asmprint.ll
    │   │   │   │   ├── floatPSA.ll
    │   │   │   │   ├── flt-preinc.ll
    │   │   │   │   ├── fma-aggr-FMF.ll
    │   │   │   │   ├── fma-assoc.ll
    │   │   │   │   ├── fma-mutate-duplicate-vreg.ll
    │   │   │   │   ├── fma-mutate-register-constraint.ll
    │   │   │   │   ├── fma.ll
    │   │   │   │   ├── fmaxnum.ll
    │   │   │   │   ├── fmf-propagation.ll
    │   │   │   │   ├── fminnum.ll
    │   │   │   │   ├── fnabs.ll
    │   │   │   │   ├── fneg.ll
    │   │   │   │   ├── fold-li.ll
    │   │   │   │   ├── fold-zero.ll
    │   │   │   │   ├── fp-branch.ll
    │   │   │   │   ├── fp-int-conversions-direct-moves.ll
    │   │   │   │   ├── fp-int-fp.ll
    │   │   │   │   ├── fp-int128-fp-combine.ll
    │   │   │   │   ├── fp-splat.ll
    │   │   │   │   ├── fp-to-int-ext.ll
    │   │   │   │   ├── fp128-bitcast-after-operation.ll
    │   │   │   │   ├── fp2int2fp-ppcfp128.ll
    │   │   │   │   ├── fp64-to-int16.ll
    │   │   │   │   ├── frame-size.ll
    │   │   │   │   ├── frameaddr.ll
    │   │   │   │   ├── Frames-alloca.ll
    │   │   │   │   ├── Frames-large.ll
    │   │   │   │   ├── Frames-small.ll
    │   │   │   │   ├── fsel.ll
    │   │   │   │   ├── fsl-e500mc.ll
    │   │   │   │   ├── fsl-e5500.ll
    │   │   │   │   ├── fsqrt.ll
    │   │   │   │   ├── func-addr-consts.ll
    │   │   │   │   ├── func-addr.ll
    │   │   │   │   ├── funnel-shift-rot.ll
    │   │   │   │   ├── funnel-shift.ll
    │   │   │   │   ├── glob-comp-aa-crash.ll
    │   │   │   │   ├── gpr-vsr-spill.ll
    │   │   │   │   ├── hello-reloc.s
    │   │   │   │   ├── hello.ll
    │   │   │   │   ├── hidden-vis-2.ll
    │   │   │   │   ├── hidden-vis.ll
    │   │   │   │   ├── hoist-logic.ll
    │   │   │   │   ├── htm.ll
    │   │   │   │   ├── i1-ext-fold.ll
    │   │   │   │   ├── i1-to-double.ll
    │   │   │   │   ├── i128-and-beyond.ll
    │   │   │   │   ├── i32-to-float.ll
    │   │   │   │   ├── i64-to-float.ll
    │   │   │   │   ├── i64_fp_round.ll
    │   │   │   │   ├── ia-mem-r0.ll
    │   │   │   │   ├── ia-neg-const.ll
    │   │   │   │   ├── iabs.ll
    │   │   │   │   ├── ifcvt-forked-bug-2016-08-08.ll
    │   │   │   │   ├── ifcvt.ll
    │   │   │   │   ├── illegal-element-type.ll
    │   │   │   │   ├── in-asm-f64-reg.ll
    │   │   │   │   ├── indexed-load.ll
    │   │   │   │   ├── indirect-hidden.ll
    │   │   │   │   ├── indirectbr.ll
    │   │   │   │   ├── inline-asm-s-modifier.ll
    │   │   │   │   ├── inlineasm-copy.ll
    │   │   │   │   ├── inlineasm-i64-reg.ll
    │   │   │   │   ├── inlineasm-vsx-reg.ll
    │   │   │   │   ├── int-fp-conv-0.ll
    │   │   │   │   ├── isel-rc-nox0.ll
    │   │   │   │   ├── isel.ll
    │   │   │   │   ├── ispositive.ll
    │   │   │   │   ├── jaggedstructs.ll
    │   │   │   │   ├── lbz-from-ld-shift.ll
    │   │   │   │   ├── lbzux.ll
    │   │   │   │   ├── ld-st-upd.ll
    │   │   │   │   ├── ldtoc-inv.ll
    │   │   │   │   ├── licm-remat.ll
    │   │   │   │   ├── licm-tocReg.ll
    │   │   │   │   ├── livephysregs.mir
    │   │   │   │   ├── load-constant-addr.ll
    │   │   │   │   ├── load-shift-combine.ll
    │   │   │   │   ├── load-two-flts.ll
    │   │   │   │   ├── load-v4i8-improved.ll
    │   │   │   │   ├── logic-ops-on-compares.ll
    │   │   │   │   ├── longcall.ll
    │   │   │   │   ├── longdbl-truncate.ll
    │   │   │   │   ├── loop-data-prefetch-inner.ll
    │   │   │   │   ├── loop-data-prefetch.ll
    │   │   │   │   ├── loop-hoist-toc-save.ll
    │   │   │   │   ├── lsa.ll
    │   │   │   │   ├── lsr-postinc-pos.ll
    │   │   │   │   ├── lxv-aligned-stack-slots.ll
    │   │   │   │   ├── lxvw4x-bug.ll
    │   │   │   │   ├── machine-combiner.ll
    │   │   │   │   ├── mask64.ll
    │   │   │   │   ├── mature-mc-support.ll
    │   │   │   │   ├── mcm-1.ll
    │   │   │   │   ├── mcm-10.ll
    │   │   │   │   ├── mcm-11.ll
    │   │   │   │   ├── mcm-12.ll
    │   │   │   │   ├── mcm-13.ll
    │   │   │   │   ├── mcm-2.ll
    │   │   │   │   ├── mcm-3.ll
    │   │   │   │   ├── mcm-4.ll
    │   │   │   │   ├── mcm-5.ll
    │   │   │   │   ├── mcm-6.ll
    │   │   │   │   ├── mcm-7.ll
    │   │   │   │   ├── mcm-9.ll
    │   │   │   │   ├── mcm-obj-2.ll
    │   │   │   │   ├── mcm-obj.ll
    │   │   │   │   ├── mcount-insertion.ll
    │   │   │   │   ├── MCSE-caller-preserved-reg.ll
    │   │   │   │   ├── mem-rr-addr-mode.ll
    │   │   │   │   ├── mem_update.ll
    │   │   │   │   ├── memcmp-mergeexpand.ll
    │   │   │   │   ├── memcmpIR.ll
    │   │   │   │   ├── memCmpUsedInZeroEqualityComparison.ll
    │   │   │   │   ├── memcpy_dereferenceable.ll
    │   │   │   │   ├── memset-nc-le.ll
    │   │   │   │   ├── memset-nc.ll
    │   │   │   │   ├── merge-st-chain-op.ll
    │   │   │   │   ├── merge_stores_dereferenceable.ll
    │   │   │   │   ├── MergeConsecutiveStores.ll
    │   │   │   │   ├── mi-scheduling-lhs.ll
    │   │   │   │   ├── misched-inorder-latency.ll
    │   │   │   │   ├── misched.ll
    │   │   │   │   ├── MMO-flags-assertion.ll
    │   │   │   │   ├── mul-neg-power-2.ll
    │   │   │   │   ├── mul-with-overflow.ll
    │   │   │   │   ├── mulhs.ll
    │   │   │   │   ├── mulld.ll
    │   │   │   │   ├── mulli64.ll
    │   │   │   │   ├── mult-alt-generic-powerpc.ll
    │   │   │   │   ├── mult-alt-generic-powerpc64.ll
    │   │   │   │   ├── multi-return.ll
    │   │   │   │   ├── named-reg-alloc-r1-64.ll
    │   │   │   │   ├── named-reg-alloc-r1.ll
    │   │   │   │   ├── named-reg-alloc-r13-64.ll
    │   │   │   │   ├── named-reg-alloc-r2-64.ll
    │   │   │   │   ├── neg.ll
    │   │   │   │   ├── negate-i1.ll
    │   │   │   │   ├── negctr.ll
    │   │   │   │   ├── no-ctr-loop-if-exit-in-nested-loop.ll
    │   │   │   │   ├── no-dead-strip.ll
    │   │   │   │   ├── no-dup-of-bdnz.ll
    │   │   │   │   ├── no-ext-with-count-zeros.ll
    │   │   │   │   ├── no-extra-fp-conv-ldst.ll
    │   │   │   │   ├── no-pref-jumps.ll
    │   │   │   │   ├── no-rlwimi-trivial-commute.mir
    │   │   │   │   ├── NoCRFieldRedefWhenSpillingCRBIT.mir
    │   │   │   │   ├── noPermuteFormasking.ll
    │   │   │   │   ├── novrsave.ll
    │   │   │   │   ├── opt-cmp-inst-cr0-live.ll
    │   │   │   │   ├── opt-li-add-to-addi.ll
    │   │   │   │   ├── optimize-andiso.ll
    │   │   │   │   ├── optnone-crbits-i1-ret.ll
    │   │   │   │   ├── or-addressing-mode.ll
    │   │   │   │   ├── ori_imm32.ll
    │   │   │   │   ├── p8-isel-sched.ll
    │   │   │   │   ├── p8altivec-shuffles-pred.ll
    │   │   │   │   ├── p9-dform-load-alignment.ll
    │   │   │   │   ├── p9-vector-compares-and-counts.ll
    │   │   │   │   ├── p9-xxinsertw-xxextractuw.ll
    │   │   │   │   ├── p9_copy_fp.ll
    │   │   │   │   ├── peephole-align.ll
    │   │   │   │   ├── pip-inner.ll
    │   │   │   │   ├── popcnt.ll
    │   │   │   │   ├── post-ra-ec.ll
    │   │   │   │   ├── power9-moves-and-splats.ll
    │   │   │   │   ├── ppc-crbits-onoff.ll
    │   │   │   │   ├── ppc-ctr-dead-code.ll
    │   │   │   │   ├── ppc-empty-fs.ll
    │   │   │   │   ├── ppc-label2.ll
    │   │   │   │   ├── ppc-prologue.ll
    │   │   │   │   ├── ppc-redzone-alignment-bug.ll
    │   │   │   │   ├── ppc-shrink-wrapping.ll
    │   │   │   │   ├── ppc-vaarg-agg.ll
    │   │   │   │   ├── ppc32-align-long-double-sf.ll
    │   │   │   │   ├── ppc32-i1-stack-arguments-abi-bug.ll
    │   │   │   │   ├── ppc32-lshrti3.ll
    │   │   │   │   ├── ppc32-nest.ll
    │   │   │   │   ├── ppc32-pic-large.ll
    │   │   │   │   ├── ppc32-pic.ll
    │   │   │   │   ├── ppc32-skip-regs.ll
    │   │   │   │   ├── ppc440-fp-basic.ll
    │   │   │   │   ├── ppc440-msync.ll
    │   │   │   │   ├── ppc64-32bit-addic.ll
    │   │   │   │   ├── ppc64-abi-extend.ll
    │   │   │   │   ├── ppc64-align-long-double.ll
    │   │   │   │   ├── ppc64-altivec-abi.ll
    │   │   │   │   ├── ppc64-anyregcc-crash.ll
    │   │   │   │   ├── ppc64-anyregcc.ll
    │   │   │   │   ├── ppc64-blnop.ll
    │   │   │   │   ├── ppc64-byval-align.ll
    │   │   │   │   ├── ppc64-calls.ll
    │   │   │   │   ├── ppc64-cyclecounter.ll
    │   │   │   │   ├── ppc64-fastcc-fast-isel.ll
    │   │   │   │   ├── ppc64-func-desc-hoist.ll
    │   │   │   │   ├── ppc64-gep-opt.ll
    │   │   │   │   ├── ppc64-get-cache-line-size.ll
    │   │   │   │   ├── ppc64-i128-abi.ll
    │   │   │   │   ├── ppc64-icbt-pwr7.ll
    │   │   │   │   ├── ppc64-icbt-pwr8.ll
    │   │   │   │   ├── ppc64-linux-func-size.ll
    │   │   │   │   ├── ppc64-nest.ll
    │   │   │   │   ├── ppc64-nonfunc-calls.ll
    │   │   │   │   ├── ppc64-P9-mod.ll
    │   │   │   │   ├── ppc64-P9-setb.ll
    │   │   │   │   ├── ppc64-patchpoint.ll
    │   │   │   │   ├── ppc64-pre-inc-no-extra-phi.ll
    │   │   │   │   ├── ppc64-prefetch.ll
    │   │   │   │   ├── ppc64-sibcall-shrinkwrap.ll
    │   │   │   │   ├── ppc64-smallarg.ll
    │   │   │   │   ├── ppc64-stackmap-nops.ll
    │   │   │   │   ├── ppc64-vaarg-int.ll
    │   │   │   │   ├── ppc64-zext.ll
    │   │   │   │   ├── ppc64le-calls.ll
    │   │   │   │   ├── ppc64le-crsave.ll
    │   │   │   │   ├── ppc64le-localentry-large.ll
    │   │   │   │   ├── ppc64le-localentry.ll
    │   │   │   │   ├── ppcf128-1-opt.ll
    │   │   │   │   ├── ppcf128-1.ll
    │   │   │   │   ├── ppcf128-2.ll
    │   │   │   │   ├── ppcf128-3.ll
    │   │   │   │   ├── ppcf128-4.ll
    │   │   │   │   ├── ppcf128-endian.ll
    │   │   │   │   ├── ppcf128sf.ll
    │   │   │   │   ├── ppcsoftops.ll
    │   │   │   │   ├── pr12757.ll
    │   │   │   │   ├── pr13641.ll
    │   │   │   │   ├── pr13891.ll
    │   │   │   │   ├── pr15359.ll
    │   │   │   │   ├── pr15632.ll
    │   │   │   │   ├── pr16556-2.ll
    │   │   │   │   ├── pr16573.ll
    │   │   │   │   ├── pr17168.ll
    │   │   │   │   ├── pr17354.ll
    │   │   │   │   ├── pr18663-2.ll
    │   │   │   │   ├── pr20442.ll
    │   │   │   │   ├── pr24546.ll
    │   │   │   │   ├── pr24636.ll
    │   │   │   │   ├── pr26180.ll
    │   │   │   │   ├── pr26193.ll
    │   │   │   │   ├── pr26356.ll
    │   │   │   │   ├── pr26378.ll
    │   │   │   │   ├── pr26381.ll
    │   │   │   │   ├── pr26617.ll
    │   │   │   │   ├── pr26690.ll
    │   │   │   │   ├── pr27350.ll
    │   │   │   │   ├── pr28130.ll
    │   │   │   │   ├── pr28630.ll
    │   │   │   │   ├── pr30451.ll
    │   │   │   │   ├── pr30715.ll
    │   │   │   │   ├── pr31144.ll
    │   │   │   │   ├── pr32063.ll
    │   │   │   │   ├── pr33093.ll
    │   │   │   │   ├── pr33547.ll
    │   │   │   │   ├── PR33636.ll
    │   │   │   │   ├── PR3488.ll
    │   │   │   │   ├── pr35402.ll
    │   │   │   │   ├── PR35812-neg-cmpxchg.ll
    │   │   │   │   ├── pr36068.ll
    │   │   │   │   ├── pr36292.ll
    │   │   │   │   ├── pr3711_widen_bit.ll
    │   │   │   │   ├── pr38087.ll
    │   │   │   │   ├── pr39478.ll
    │   │   │   │   ├── pr39815.ll
    │   │   │   │   ├── pre-inc-disable.ll
    │   │   │   │   ├── preemption.ll
    │   │   │   │   ├── preinc-ld-sel-crash.ll
    │   │   │   │   ├── preincprep-invoke.ll
    │   │   │   │   ├── preincprep-nontrans-crash.ll
    │   │   │   │   ├── private.ll
    │   │   │   │   ├── pwr3-6x.ll
    │   │   │   │   ├── pwr7-gt-nop.ll
    │   │   │   │   ├── qpx-bv-sint.ll
    │   │   │   │   ├── qpx-bv.ll
    │   │   │   │   ├── qpx-func-clobber.ll
    │   │   │   │   ├── qpx-load-splat.ll
    │   │   │   │   ├── qpx-load.ll
    │   │   │   │   ├── qpx-recipest.ll
    │   │   │   │   ├── qpx-rounding-ops.ll
    │   │   │   │   ├── qpx-s-load.ll
    │   │   │   │   ├── qpx-s-sel.ll
    │   │   │   │   ├── qpx-s-store.ll
    │   │   │   │   ├── qpx-sel.ll
    │   │   │   │   ├── qpx-store.ll
    │   │   │   │   ├── qpx-unal-cons-lds.ll
    │   │   │   │   ├── qpx-unalperm.ll
    │   │   │   │   ├── quadint-return.ll
    │   │   │   │   ├── r31.ll
    │   │   │   │   ├── recipest.ll
    │   │   │   │   ├── reloc-align.ll
    │   │   │   │   ├── remap-crash.ll
    │   │   │   │   ├── remat-imm.ll
    │   │   │   │   ├── remove-implicit-use.mir
    │   │   │   │   ├── remove-redundant-moves.ll
    │   │   │   │   ├── remove-redundant-toc-saves.ll
    │   │   │   │   ├── remove-self-copies.mir
    │   │   │   │   ├── resolvefi-basereg.ll
    │   │   │   │   ├── resolvefi-disp.ll
    │   │   │   │   ├── retaddr.ll
    │   │   │   │   ├── return-val-i128.ll
    │   │   │   │   ├── rlwimi-and-or-bits.ll
    │   │   │   │   ├── rlwimi-commute.ll
    │   │   │   │   ├── rlwimi-dyn-and.ll
    │   │   │   │   ├── rlwimi-keep-rsh.ll
    │   │   │   │   ├── rlwimi2.ll
    │   │   │   │   ├── rlwinm-zero-ext.ll
    │   │   │   │   ├── rlwinm.ll
    │   │   │   │   ├── rlwinm2.ll
    │   │   │   │   ├── rm-zext.ll
    │   │   │   │   ├── rotl-2.ll
    │   │   │   │   ├── rotl-64.ll
    │   │   │   │   ├── rotl-rotr-crash.ll
    │   │   │   │   ├── rotl.ll
    │   │   │   │   ├── rounding-ops.ll
    │   │   │   │   ├── s000-alias-misched.ll
    │   │   │   │   ├── save-bp.ll
    │   │   │   │   ├── save-cr-ppc32svr4.ll
    │   │   │   │   ├── save-crbp-ppc32svr4.ll
    │   │   │   │   ├── scalar_vector_test_1.ll
    │   │   │   │   ├── scalar_vector_test_2.ll
    │   │   │   │   ├── scalar_vector_test_3.ll
    │   │   │   │   ├── scalar_vector_test_4.ll
    │   │   │   │   ├── sdag-ppcf128.ll
    │   │   │   │   ├── sdiv-pow2.ll
    │   │   │   │   ├── sections.ll
    │   │   │   │   ├── select-addrRegRegOnly.ll
    │   │   │   │   ├── select-cc.ll
    │   │   │   │   ├── select-i1-vs-i1.ll
    │   │   │   │   ├── select_const.ll
    │   │   │   │   ├── select_lt0.ll
    │   │   │   │   ├── selectiondag-extload-computeknownbits.ll
    │   │   │   │   ├── selectiondag-sextload.ll
    │   │   │   │   ├── set0-v8i16.ll
    │   │   │   │   ├── setcc-logic.ll
    │   │   │   │   ├── setcc-to-sub.ll
    │   │   │   │   ├── setcc_no_zext.ll
    │   │   │   │   ├── setcclike-or-comb.ll
    │   │   │   │   ├── setcr_bc.mir
    │   │   │   │   ├── setcr_bc2.mir
    │   │   │   │   ├── setcr_bc3.mir
    │   │   │   │   ├── seteq-0.ll
    │   │   │   │   ├── shift-cmp.ll
    │   │   │   │   ├── shift128.ll
    │   │   │   │   ├── shift_mask.ll
    │   │   │   │   ├── shl_elim.ll
    │   │   │   │   ├── shl_sext.ll
    │   │   │   │   ├── sign_ext_inreg1.ll
    │   │   │   │   ├── simplifyConstCmpToISEL.ll
    │   │   │   │   ├── sj-ctr-loop.ll
    │   │   │   │   ├── sjlj.ll
    │   │   │   │   ├── sjlj_no0x.ll
    │   │   │   │   ├── small-arguments.ll
    │   │   │   │   ├── spe.ll
    │   │   │   │   ├── spill-nor0.ll
    │   │   │   │   ├── splat-larger-types-as-v16i8.ll
    │   │   │   │   ├── stack-no-redzone.ll
    │   │   │   │   ├── stack-protector.ll
    │   │   │   │   ├── stack-realign.ll
    │   │   │   │   ├── stackmap-frame-setup.ll
    │   │   │   │   ├── stacksize.ll
    │   │   │   │   ├── stfiwx-2.ll
    │   │   │   │   ├── store-constant.ll
    │   │   │   │   ├── store-load-fwd.ll
    │   │   │   │   ├── store-update.ll
    │   │   │   │   ├── store_fptoi.ll
    │   │   │   │   ├── structsinmem.ll
    │   │   │   │   ├── structsinregs.ll
    │   │   │   │   ├── stubs.ll
    │   │   │   │   ├── stwu-gta.ll
    │   │   │   │   ├── stwu-sched.ll
    │   │   │   │   ├── stwu8.ll
    │   │   │   │   ├── stwux.ll
    │   │   │   │   ├── sub-bv-types.ll
    │   │   │   │   ├── subc.ll
    │   │   │   │   ├── subreg-postra-2.ll
    │   │   │   │   ├── subreg-postra.ll
    │   │   │   │   ├── svr4-redzone.ll
    │   │   │   │   ├── swaps-le-1.ll
    │   │   │   │   ├── swaps-le-4.ll
    │   │   │   │   ├── swaps-le-6.ll
    │   │   │   │   ├── swaps-le-7.ll
    │   │   │   │   ├── tail-dup-analyzable-fallthrough.ll
    │   │   │   │   ├── tail-dup-branch-to-fallthrough.ll
    │   │   │   │   ├── tail-dup-break-cfg.ll
    │   │   │   │   ├── tail-dup-layout.ll
    │   │   │   │   ├── tailcall-string-rvo.ll
    │   │   │   │   ├── tailcall1-64.ll
    │   │   │   │   ├── tailcall1.ll
    │   │   │   │   ├── tailcallpic1.ll
    │   │   │   │   ├── test-and-cmp-folding.ll
    │   │   │   │   ├── testComparesi32gtu.ll
    │   │   │   │   ├── testComparesi32leu.ll
    │   │   │   │   ├── testComparesi32ltu.ll
    │   │   │   │   ├── testComparesieqsc.ll
    │   │   │   │   ├── testComparesieqsi.ll
    │   │   │   │   ├── testComparesieqsll.ll
    │   │   │   │   ├── testComparesieqss.ll
    │   │   │   │   ├── testComparesiequc.ll
    │   │   │   │   ├── testComparesiequi.ll
    │   │   │   │   ├── testComparesiequll.ll
    │   │   │   │   ├── testComparesigesi.ll
    │   │   │   │   ├── testComparesigeuc.ll
    │   │   │   │   ├── testComparesigeui.ll
    │   │   │   │   ├── testComparesigeull.ll
    │   │   │   │   ├── testComparesigeus.ll
    │   │   │   │   ├── testComparesigtsc.ll
    │   │   │   │   ├── testComparesigtsi.ll
    │   │   │   │   ├── testComparesigtsll.ll
    │   │   │   │   ├── testComparesigtuc.ll
    │   │   │   │   ├── testComparesigtui.ll
    │   │   │   │   ├── testComparesigtus.ll
    │   │   │   │   ├── testComparesilesi.ll
    │   │   │   │   ├── testComparesilesll.ll
    │   │   │   │   ├── testComparesiless.ll
    │   │   │   │   ├── testComparesileuc.ll
    │   │   │   │   ├── testComparesileui.ll
    │   │   │   │   ├── testComparesileus.ll
    │   │   │   │   ├── testComparesiltsi.ll
    │   │   │   │   ├── testComparesiltsll.ll
    │   │   │   │   ├── testComparesiltss.ll
    │   │   │   │   ├── testComparesiltui.ll
    │   │   │   │   ├── testComparesinesc.ll
    │   │   │   │   ├── testComparesinesi.ll
    │   │   │   │   ├── testComparesinesll.ll
    │   │   │   │   ├── testComparesiness.ll
    │   │   │   │   ├── testComparesineuc.ll
    │   │   │   │   ├── testComparesineui.ll
    │   │   │   │   ├── testComparesineull.ll
    │   │   │   │   ├── testCompareslleqsc.ll
    │   │   │   │   ├── testCompareslleqsll.ll
    │   │   │   │   ├── testCompareslleqss.ll
    │   │   │   │   ├── testComparesllequc.ll
    │   │   │   │   ├── testComparesllequi.ll
    │   │   │   │   ├── testComparesllequll.ll
    │   │   │   │   ├── testComparesllequs.ll
    │   │   │   │   ├── testComparesllgesc.ll
    │   │   │   │   ├── testComparesllgesi.ll
    │   │   │   │   ├── testComparesllgeuc.ll
    │   │   │   │   ├── testComparesllgeui.ll
    │   │   │   │   ├── testComparesllgeus.ll
    │   │   │   │   ├── testComparesllgtsll.ll
    │   │   │   │   ├── testComparesllgtuc.ll
    │   │   │   │   ├── testComparesllgtui.ll
    │   │   │   │   ├── testCompareslllesc.ll
    │   │   │   │   ├── testCompareslllesi.ll
    │   │   │   │   ├── testCompareslllesll.ll
    │   │   │   │   ├── testComparesllless.ll
    │   │   │   │   ├── testComparesllleuc.ll
    │   │   │   │   ├── testComparesllleui.ll
    │   │   │   │   ├── testComparesllleull.ll
    │   │   │   │   ├── testComparesllleus.ll
    │   │   │   │   ├── testComparesllltsll.ll
    │   │   │   │   ├── testComparesllltuc.ll
    │   │   │   │   ├── testComparesllltui.ll
    │   │   │   │   ├── testComparesllltus.ll
    │   │   │   │   ├── testComparesllnesll.ll
    │   │   │   │   ├── testComparesllneull.ll
    │   │   │   │   ├── thread-pointer.ll
    │   │   │   │   ├── tls-cse.ll
    │   │   │   │   ├── tls-pie-xform.ll
    │   │   │   │   ├── tls-store2.ll
    │   │   │   │   ├── tls.ll
    │   │   │   │   ├── tls_get_addr_clobbers.ll
    │   │   │   │   ├── tls_get_addr_fence1.mir
    │   │   │   │   ├── tls_get_addr_fence2.mir
    │   │   │   │   ├── tls_get_addr_stackframe.ll
    │   │   │   │   ├── toc-float.ll
    │   │   │   │   ├── toc-load-sched-bug.ll
    │   │   │   │   ├── trampoline.ll
    │   │   │   │   ├── uint-to-ppcfp128-crash.ll
    │   │   │   │   ├── unal-altivec-wint.ll
    │   │   │   │   ├── unal-altivec2.ll
    │   │   │   │   ├── unal-vec-ldst.ll
    │   │   │   │   ├── unal4-std.ll
    │   │   │   │   ├── unsafe-math.ll
    │   │   │   │   ├── unwind-dw2-g.ll
    │   │   │   │   ├── unwind-dw2.ll
    │   │   │   │   ├── vaddsplat.ll
    │   │   │   │   ├── varargs-struct-float.ll
    │   │   │   │   ├── varargs.ll
    │   │   │   │   ├── variable_elem_vec_extracts.ll
    │   │   │   │   ├── vcmp-fold.ll
    │   │   │   │   ├── vec-abi-align.ll
    │   │   │   │   ├── vec-asm-disabled.ll
    │   │   │   │   ├── vec-itofp.ll
    │   │   │   │   ├── vec_abs.ll
    │   │   │   │   ├── vec_absd.ll
    │   │   │   │   ├── vec_add_sub_doubleword.ll
    │   │   │   │   ├── vec_add_sub_quadword.ll
    │   │   │   │   ├── vec_auto_constant.ll
    │   │   │   │   ├── vec_buildvector_loadstore.ll
    │   │   │   │   ├── vec_clz.ll
    │   │   │   │   ├── vec_cmp.ll
    │   │   │   │   ├── vec_cmpd.ll
    │   │   │   │   ├── vec_constants.ll
    │   │   │   │   ├── vec_conv.ll
    │   │   │   │   ├── vec_conv_fp32_to_i64_elts.ll
    │   │   │   │   ├── vec_conv_fp64_to_i16_elts.ll
    │   │   │   │   ├── vec_conv_fp64_to_i32_elts.ll
    │   │   │   │   ├── vec_conv_fp64_to_i8_elts.ll
    │   │   │   │   ├── vec_conv_fp_to_i_4byte_elts.ll
    │   │   │   │   ├── vec_conv_fp_to_i_8byte_elts.ll
    │   │   │   │   ├── vec_conv_i16_to_fp32_elts.ll
    │   │   │   │   ├── vec_conv_i16_to_fp64_elts.ll
    │   │   │   │   ├── vec_conv_i8_to_fp32_elts.ll
    │   │   │   │   ├── vec_conv_i_to_fp_4byte_elts.ll
    │   │   │   │   ├── vec_conv_i_to_fp_8byte_elts.ll
    │   │   │   │   ├── vec_extract_p9.ll
    │   │   │   │   ├── vec_extract_p9_2.ll
    │   │   │   │   ├── vec_fmuladd.ll
    │   │   │   │   ├── vec_fneg.ll
    │   │   │   │   ├── vec_insert.ll
    │   │   │   │   ├── vec_int_ext.ll
    │   │   │   │   ├── vec_mergeow.ll
    │   │   │   │   ├── vec_misaligned.ll
    │   │   │   │   ├── vec_mul.ll
    │   │   │   │   ├── vec_mul_even_odd.ll
    │   │   │   │   ├── vec_perf_shuffle.ll
    │   │   │   │   ├── vec_popcnt.ll
    │   │   │   │   ├── vec_rotate_shift.ll
    │   │   │   │   ├── vec_rounding.ll
    │   │   │   │   ├── vec_select.ll
    │   │   │   │   ├── vec_shift.ll
    │   │   │   │   ├── vec_shuffle_le.ll
    │   │   │   │   ├── vec_shuffle_p8vector.ll
    │   │   │   │   ├── vec_shuffle_p8vector_le.ll
    │   │   │   │   ├── vec_splat_constant.ll
    │   │   │   │   ├── vec_veqv_vnand_vorc.ll
    │   │   │   │   ├── vec_vrsave.ll
    │   │   │   │   ├── vec_xxpermdi.ll
    │   │   │   │   ├── vec_zero.ll
    │   │   │   │   ├── vector-identity-shuffle.ll
    │   │   │   │   ├── vector-merge-store-fp-constants.ll
    │   │   │   │   ├── vector.ll
    │   │   │   │   ├── vperm-instcombine.ll
    │   │   │   │   ├── vperm-lowering.ll
    │   │   │   │   ├── vrspill.ll
    │   │   │   │   ├── vsel-prom.ll
    │   │   │   │   ├── vselect-constants.ll
    │   │   │   │   ├── vsx-args.ll
    │   │   │   │   ├── VSX-DForm-Scalars.ll
    │   │   │   │   ├── vsx-elementary-arith.ll
    │   │   │   │   ├── vsx-fma-m.ll
    │   │   │   │   ├── vsx-fma-mutate-trivial-copy.ll
    │   │   │   │   ├── vsx-fma-sp.ll
    │   │   │   │   ├── vsx-infl-copy1.ll
    │   │   │   │   ├── vsx-ldst-builtin-le.ll
    │   │   │   │   ├── vsx-minmax.ll
    │   │   │   │   ├── vsx-p8.ll
    │   │   │   │   ├── vsx-p9.ll
    │   │   │   │   ├── vsx-partword-int-loads-and-stores.ll
    │   │   │   │   ├── vsx-recip-est.ll
    │   │   │   │   ├── vsx-spill-norwstore.ll
    │   │   │   │   ├── vsx-spill.ll
    │   │   │   │   ├── vsx-vec-spill.ll
    │   │   │   │   ├── vsx-word-splats.ll
    │   │   │   │   ├── vsx.ll
    │   │   │   │   ├── vsx_builtins.ll
    │   │   │   │   ├── vsx_insert_extract_le.ll
    │   │   │   │   ├── vsx_scalar_ld_st.ll
    │   │   │   │   ├── vsx_shuffle_le.ll
    │   │   │   │   ├── vsxD-Form-spills.ll
    │   │   │   │   ├── vtable-reloc.ll
    │   │   │   │   ├── weak_def_can_be_hidden.ll
    │   │   │   │   ├── xray-ret-is-terminator.ll
    │   │   │   │   ├── xray-tail-call-hidden.ll
    │   │   │   │   ├── xvcmpeqdp-v2f64.ll
    │   │   │   │   ├── xxleqv_xxlnand_xxlorc.ll
    │   │   │   │   ├── zero-not-run.ll
    │   │   │   │   └── zext-and-cmp.ll
    │   │   │   └── X86/
    │   │   │       ├── 2003-08-03-CallArgLiveRanges.ll
    │   │   │       ├── 2003-08-23-DeadBlockTest.ll
    │   │   │       ├── 2003-11-03-GlobalBool.ll
    │   │   │       ├── 2004-02-13-FrameReturnAddress.ll
    │   │   │       ├── 2004-02-14-InefficientStackPointer.ll
    │   │   │       ├── 2004-02-22-Casts.ll
    │   │   │       ├── 2004-03-30-Select-Max.ll
    │   │   │       ├── 2004-04-13-FPCMOV-Crash.ll
    │   │   │       ├── 2004-06-10-StackifierCrash.ll
    │   │   │       ├── 2004-10-08-SelectSetCCFold.ll
    │   │   │       ├── 2005-01-17-CycleInDAG.ll
    │   │   │       ├── 2005-02-14-IllegalAssembler.ll
    │   │   │       ├── 2005-05-08-FPStackifierPHI.ll
    │   │   │       ├── 2006-01-19-ISelFoldingBug.ll
    │   │   │       ├── 2006-03-01-InstrSchedBug.ll
    │   │   │       ├── 2006-03-02-InstrSchedBug.ll
    │   │   │       ├── 2006-04-04-CrossBlockCrash.ll
    │   │   │       ├── 2006-04-27-ISelFoldingBug.ll
    │   │   │       ├── 2006-05-01-SchedCausingSpills.ll
    │   │   │       ├── 2006-05-02-InstrSched1.ll
    │   │   │       ├── 2006-05-02-InstrSched2.ll
    │   │   │       ├── 2006-05-08-CoalesceSubRegClass.ll
    │   │   │       ├── 2006-05-08-InstrSched.ll
    │   │   │       ├── 2006-05-11-InstrSched.ll
    │   │   │       ├── 2006-05-17-VectorArg.ll
    │   │   │       ├── 2006-05-22-FPSetEQ.ll
    │   │   │       ├── 2006-05-25-CycleInDAG.ll
    │   │   │       ├── 2006-07-10-InlineAsmAConstraint.ll
    │   │   │       ├── 2006-07-12-InlineAsmQConstraint.ll
    │   │   │       ├── 2006-07-20-InlineAsm.ll
    │   │   │       ├── 2006-07-28-AsmPrint-Long-As-Pointer.ll
    │   │   │       ├── 2006-07-31-SingleRegClass.ll
    │   │   │       ├── 2006-08-07-CycleInDAG.ll
    │   │   │       ├── 2006-08-16-CycleInDAG.ll
    │   │   │       ├── 2006-08-21-ExtraMovInst.ll
    │   │   │       ├── 2006-09-01-CycleInDAG.ll
    │   │   │       ├── 2006-10-02-BoolRetCrash.ll
    │   │   │       ├── 2006-10-09-CycleInDAG.ll
    │   │   │       ├── 2006-10-10-FindModifiedNodeSlotBug.ll
    │   │   │       ├── 2006-10-12-CycleInDAG.ll
    │   │   │       ├── 2006-10-13-CycleInDAG.ll
    │   │   │       ├── 2006-10-19-SwitchUnnecessaryBranching.ll
    │   │   │       ├── 2006-11-12-CSRetCC.ll
    │   │   │       ├── 2006-11-17-IllegalMove.ll
    │   │   │       ├── 2006-11-27-SelectLegalize.ll
    │   │   │       ├── 2006-12-16-InlineAsmCrash.ll
    │   │   │       ├── 2006-12-19-IntelSyntax.ll
    │   │   │       ├── 2007-01-08-InstrSched.ll
    │   │   │       ├── 2007-01-08-X86-64-Pointer.ll
    │   │   │       ├── 2007-01-13-StackPtrIndex.ll
    │   │   │       ├── 2007-01-29-InlineAsm-ir.ll
    │   │   │       ├── 2007-02-04-OrAddrMode.ll
    │   │   │       ├── 2007-02-16-BranchFold.ll
    │   │   │       ├── 2007-02-19-LiveIntervalAssert.ll
    │   │   │       ├── 2007-02-23-DAGCombine-Miscompile.ll
    │   │   │       ├── 2007-02-25-FastCCStack.ll
    │   │   │       ├── 2007-03-01-SpillerCrash.ll
    │   │   │       ├── 2007-03-15-GEP-Idx-Sink.ll
    │   │   │       ├── 2007-03-16-InlineAsm.ll
    │   │   │       ├── 2007-03-18-LiveIntervalAssert.ll
    │   │   │       ├── 2007-03-24-InlineAsmMultiRegConstraint.ll
    │   │   │       ├── 2007-03-24-InlineAsmPModifier.ll
    │   │   │       ├── 2007-03-24-InlineAsmVectorOp.ll
    │   │   │       ├── 2007-03-24-InlineAsmXConstraint.ll
    │   │   │       ├── 2007-03-26-CoalescerBug.ll
    │   │   │       ├── 2007-04-08-InlineAsmCrash.ll
    │   │   │       ├── 2007-04-11-InlineAsmVectorResult.ll
    │   │   │       ├── 2007-04-17-LiveIntervalAssert.ll
    │   │   │       ├── 2007-04-24-Huge-Stack.ll
    │   │   │       ├── 2007-04-24-VectorCrash.ll
    │   │   │       ├── 2007-04-27-InlineAsm-IntMemInput.ll
    │   │   │       ├── 2007-05-05-Personality.ll
    │   │   │       ├── 2007-05-05-VecCastExpand.ll
    │   │   │       ├── 2007-05-14-LiveIntervalAssert.ll
    │   │   │       ├── 2007-05-15-maskmovq.ll
    │   │   │       ├── 2007-05-17-ShuffleISelBug.ll
    │   │   │       ├── 2007-06-04-X86-64-CtorAsmBugs.ll
    │   │   │       ├── 2007-06-28-X86-64-isel.ll
    │   │   │       ├── 2007-06-29-DAGCombinerBug.ll
    │   │   │       ├── 2007-06-29-VecFPConstantCSEBug.ll
    │   │   │       ├── 2007-07-03-GR64ToVR64.ll
    │   │   │       ├── 2007-07-10-StackerAssert.ll
    │   │   │       ├── 2007-07-18-Vector-Extract.ll
    │   │   │       ├── 2007-08-01-LiveVariablesBug.ll
    │   │   │       ├── 2007-08-09-IllegalX86-64Asm.ll
    │   │   │       ├── 2007-08-10-SignExtSubreg.ll
    │   │   │       ├── 2007-09-05-InvalidAsm.ll
    │   │   │       ├── 2007-09-06-ExtWeakAliasee.ll
    │   │   │       ├── 2007-09-27-LDIntrinsics.ll
    │   │   │       ├── 2007-10-04-AvoidEFLAGSCopy.ll
    │   │   │       ├── 2007-10-12-CoalesceExtSubReg.ll
    │   │   │       ├── 2007-10-12-SpillerUnfold1.ll
    │   │   │       ├── 2007-10-12-SpillerUnfold2.ll
    │   │   │       ├── 2007-10-14-CoalescerCrash.ll
    │   │   │       ├── 2007-10-15-CoalescerCrash.ll
    │   │   │       ├── 2007-10-16-CoalescerCrash.ll
    │   │   │       ├── 2007-10-19-SpillerUnfold.ll
    │   │   │       ├── 2007-10-28-inlineasm-q-modifier.ll
    │   │   │       ├── 2007-10-29-ExtendSetCC.ll
    │   │   │       ├── 2007-10-30-LSRCrash.ll
    │   │   │       ├── 2007-10-31-extractelement-i64.ll
    │   │   │       ├── 2007-11-01-ISelCrash.ll
    │   │   │       ├── 2007-11-03-x86-64-q-constraint.ll
    │   │   │       ├── 2007-11-04-LiveIntervalCrash.ll
    │   │   │       ├── 2007-11-04-LiveVariablesBug.ll
    │   │   │       ├── 2007-11-04-rip-immediate-constant.ll
    │   │   │       ├── 2007-11-06-InstrSched.ll
    │   │   │       ├── 2007-11-07-MulBy4.ll
    │   │   │       ├── 2007-11-30-LoadFolding-Bug.ll
    │   │   │       ├── 2007-12-16-BURRSchedCrash.ll
    │   │   │       ├── 2007-12-18-LoadCSEBug.ll
    │   │   │       ├── 2008-01-08-IllegalCMP.ll
    │   │   │       ├── 2008-01-08-SchedulerCrash.ll
    │   │   │       ├── 2008-01-09-LongDoubleSin.ll
    │   │   │       ├── 2008-01-16-FPStackifierAssert.ll
    │   │   │       ├── 2008-01-16-InvalidDAGCombineXform.ll
    │   │   │       ├── 2008-02-05-ISelCrash.ll
    │   │   │       ├── 2008-02-06-LoadFoldingBug.ll
    │   │   │       ├── 2008-02-14-BitMiscompile.ll
    │   │   │       ├── 2008-02-18-TailMergingBug.ll
    │   │   │       ├── 2008-02-20-InlineAsmClobber.ll
    │   │   │       ├── 2008-02-22-LocalRegAllocBug.ll
    │   │   │       ├── 2008-02-25-InlineAsmBug.ll
    │   │   │       ├── 2008-02-25-X86-64-CoalescerBug.ll
    │   │   │       ├── 2008-02-26-AsmDirectMemOp.ll
    │   │   │       ├── 2008-02-27-DeadSlotElimBug.ll
    │   │   │       ├── 2008-02-27-PEICrash.ll
    │   │   │       ├── 2008-03-06-frem-fpstack.ll
    │   │   │       ├── 2008-03-07-APIntBug.ll
    │   │   │       ├── 2008-03-10-RegAllocInfLoop.ll
    │   │   │       ├── 2008-03-12-ThreadLocalAlias.ll
    │   │   │       ├── 2008-03-13-TwoAddrPassCrash.ll
    │   │   │       ├── 2008-03-14-SpillerCrash.ll
    │   │   │       ├── 2008-03-19-DAGCombinerBug.ll
    │   │   │       ├── 2008-03-23-DarwinAsmComments.ll
    │   │   │       ├── 2008-03-25-TwoAddrPassBug.ll
    │   │   │       ├── 2008-03-31-SpillerFoldingBug.ll
    │   │   │       ├── 2008-04-02-unnamedEH.ll
    │   │   │       ├── 2008-04-08-CoalescerCrash.ll
    │   │   │       ├── 2008-04-09-BranchFolding.ll
    │   │   │       ├── 2008-04-15-LiveVariableBug.ll
    │   │   │       ├── 2008-04-16-CoalescerBug.ll
    │   │   │       ├── 2008-04-16-ReMatBug.ll
    │   │   │       ├── 2008-04-17-CoalescerBug.ll
    │   │   │       ├── 2008-04-24-MemCpyBug.ll
    │   │   │       ├── 2008-04-24-pblendw-fold-crash.ll
    │   │   │       ├── 2008-04-26-Asm-Optimize-Imm.ll
    │   │   │       ├── 2008-04-28-CoalescerBug.ll
    │   │   │       ├── 2008-04-28-CyclicSchedUnit.ll
    │   │   │       ├── 2008-05-01-InvalidOrdCompare.ll
    │   │   │       ├── 2008-05-09-PHIElimBug.ll
    │   │   │       ├── 2008-05-09-ShuffleLoweringBug.ll
    │   │   │       ├── 2008-05-12-tailmerge-5.ll
    │   │   │       ├── 2008-05-21-CoalescerBug.ll
    │   │   │       ├── 2008-05-22-FoldUnalignedLoad.ll
    │   │   │       ├── 2008-05-28-CoalescerBug.ll
    │   │   │       ├── 2008-05-28-LocalRegAllocBug.ll
    │   │   │       ├── 2008-06-13-NotVolatileLoadStore.ll
    │   │   │       ├── 2008-06-13-VolatileLoadStore.ll
    │   │   │       ├── 2008-06-16-SubregsBug.ll
    │   │   │       ├── 2008-06-25-VecISelBug.ll
    │   │   │       ├── 2008-07-07-DanglingDeadInsts.ll
    │   │   │       ├── 2008-07-09-ELFSectionAttributes.ll
    │   │   │       ├── 2008-07-11-SHLBy1.ll
    │   │   │       ├── 2008-07-16-CoalescerCrash.ll
    │   │   │       ├── 2008-07-19-movups-spills.ll
    │   │   │       ├── 2008-07-22-CombinerCrash.ll
    │   │   │       ├── 2008-07-23-VSetCC.ll
    │   │   │       ├── 2008-08-06-CmpStride.ll
    │   │   │       ├── 2008-08-06-RewriterBug.ll
    │   │   │       ├── 2008-08-17-UComiCodeGenBug.ll
    │   │   │       ├── 2008-08-23-64Bit-maskmovq.ll
    │   │   │       ├── 2008-08-31-EH_RETURN32.ll
    │   │   │       ├── 2008-08-31-EH_RETURN64.ll
    │   │   │       ├── 2008-09-05-sinttofp-2xi32.ll
    │   │   │       ├── 2008-09-09-LinearScanBug.ll
    │   │   │       ├── 2008-09-11-CoalescerBug.ll
    │   │   │       ├── 2008-09-11-CoalescerBug2.ll
    │   │   │       ├── 2008-09-17-inline-asm-1.ll
    │   │   │       ├── 2008-09-18-inline-asm-2.ll
    │   │   │       ├── 2008-09-19-RegAllocBug.ll
    │   │   │       ├── 2008-09-25-sseregparm-1.ll
    │   │   │       ├── 2008-09-26-FrameAddrBug.ll
    │   │   │       ├── 2008-09-29-ReMatBug.ll
    │   │   │       ├── 2008-09-29-VolatileBug.ll
    │   │   │       ├── 2008-10-06-x87ld-nan-1.ll
    │   │   │       ├── 2008-10-06-x87ld-nan-2.ll
    │   │   │       ├── 2008-10-07-SSEISelBug.ll
    │   │   │       ├── 2008-10-11-CallCrash.ll
    │   │   │       ├── 2008-10-13-CoalescerBug.ll
    │   │   │       ├── 2008-10-16-VecUnaryOp.ll
    │   │   │       ├── 2008-10-17-Asm64bitRConstraint.ll
    │   │   │       ├── 2008-10-20-AsmDoubleInI32.ll
    │   │   │       ├── 2008-10-24-FlippedCompare.ll
    │   │   │       ├── 2008-10-27-CoalescerBug.ll
    │   │   │       ├── 2008-10-29-ExpandVAARG.ll
    │   │   │       ├── 2008-11-03-F80VAARG.ll
    │   │   │       ├── 2008-11-06-testb.ll
    │   │   │       ├── 2008-11-13-inlineasm-3.ll
    │   │   │       ├── 2008-11-29-ULT-Sign.ll
    │   │   │       ├── 2008-12-01-loop-iv-used-outside-loop.ll
    │   │   │       ├── 2008-12-01-SpillerAssert.ll
    │   │   │       ├── 2008-12-02-dagcombine-1.ll
    │   │   │       ├── 2008-12-02-dagcombine-2.ll
    │   │   │       ├── 2008-12-02-dagcombine-3.ll
    │   │   │       ├── 2008-12-02-IllegalResultType.ll
    │   │   │       ├── 2008-12-16-dagcombine-4.ll
    │   │   │       ├── 2008-12-19-EarlyClobberBug.ll
    │   │   │       ├── 2008-12-22-dagcombine-5.ll
    │   │   │       ├── 2008-12-23-crazy-address.ll
    │   │   │       ├── 2008-12-23-dagcombine-6.ll
    │   │   │       ├── 2009-01-13-DoubleUpdate.ll
    │   │   │       ├── 2009-01-16-SchedulerBug.ll
    │   │   │       ├── 2009-01-16-UIntToFP.ll
    │   │   │       ├── 2009-01-18-ConstantExprCrash.ll
    │   │   │       ├── 2009-01-25-NoSSE.ll
    │   │   │       ├── 2009-01-26-WrongCheck.ll
    │   │   │       ├── 2009-01-27-NullStrings.ll
    │   │   │       ├── 2009-01-31-BigShift.ll
    │   │   │       ├── 2009-01-31-BigShift2.ll
    │   │   │       ├── 2009-01-31-BigShift3.ll
    │   │   │       ├── 2009-02-01-LargeMask.ll
    │   │   │       ├── 2009-02-03-AnalyzedTwice.ll
    │   │   │       ├── 2009-02-04-sext-i64-gep.ll
    │   │   │       ├── 2009-02-08-CoalescerBug.ll
    │   │   │       ├── 2009-02-09-ivs-different-sizes.ll
    │   │   │       ├── 2009-02-11-codegenprepare-reuse.ll
    │   │   │       ├── 2009-02-12-DebugInfoVLA.ll
    │   │   │       ├── 2009-02-12-InlineAsm-nieZ-constraints.ll
    │   │   │       ├── 2009-02-12-SpillerBug.ll
    │   │   │       ├── 2009-02-21-ExtWeakInitializer.ll
    │   │   │       ├── 2009-02-25-CommuteBug.ll
    │   │   │       ├── 2009-02-26-MachineLICMBug.ll
    │   │   │       ├── 2009-03-03-BitcastLongDouble.ll
    │   │   │       ├── 2009-03-03-BTHang.ll
    │   │   │       ├── 2009-03-05-burr-list-crash.ll
    │   │   │       ├── 2009-03-09-APIntCrash.ll
    │   │   │       ├── 2009-03-09-SpillerBug.ll
    │   │   │       ├── 2009-03-10-CoalescerBug.ll
    │   │   │       ├── 2009-03-12-CPAlignBug.ll
    │   │   │       ├── 2009-03-13-PHIElimBug.ll
    │   │   │       ├── 2009-03-16-PHIElimInLPad.ll
    │   │   │       ├── 2009-03-23-i80-fp80.ll
    │   │   │       ├── 2009-03-23-LinearScanBug.ll
    │   │   │       ├── 2009-03-23-MultiUseSched.ll
    │   │   │       ├── 2009-03-25-TestBug.ll
    │   │   │       ├── 2009-03-26-NoImplicitFPBug.ll
    │   │   │       ├── 2009-04-12-FastIselOverflowCrash.ll
    │   │   │       ├── 2009-04-12-picrel.ll
    │   │   │       ├── 2009-04-13-2AddrAssert-2.ll
    │   │   │       ├── 2009-04-13-2AddrAssert.ll
    │   │   │       ├── 2009-04-14-IllegalRegs.ll
    │   │   │       ├── 2009-04-16-SpillerUnfold.ll
    │   │   │       ├── 2009-04-24.ll
    │   │   │       ├── 2009-04-25-CoalescerBug.ll
    │   │   │       ├── 2009-04-27-CoalescerAssert.ll
    │   │   │       ├── 2009-04-27-LiveIntervalsAssert.ll
    │   │   │       ├── 2009-04-27-LiveIntervalsAssert2.ll
    │   │   │       ├── 2009-04-29-IndirectDestOperands.ll
    │   │   │       ├── 2009-04-29-LinearScanBug.ll
    │   │   │       ├── 2009-04-29-RegAllocAssert.ll
    │   │   │       ├── 2009-04-scale.ll
    │   │   │       ├── 2009-05-08-InlineAsmIOffset.ll
    │   │   │       ├── 2009-05-11-tailmerge-crash.ll
    │   │   │       ├── 2009-05-19-SingleElementExtractElement.ll
    │   │   │       ├── 2009-05-23-available_externally.ll
    │   │   │       ├── 2009-05-23-dagcombine-shifts.ll
    │   │   │       ├── 2009-05-28-DAGCombineCrash.ll
    │   │   │       ├── 2009-05-30-ISelBug.ll
    │   │   │       ├── 2009-06-02-RewriterBug.ll
    │   │   │       ├── 2009-06-03-Win64DisableRedZone.ll
    │   │   │       ├── 2009-06-03-Win64SpillXMM.ll
    │   │   │       ├── 2009-06-04-VirtualLiveIn.ll
    │   │   │       ├── 2009-06-05-sitofpCrash.ll
    │   │   │       ├── 2009-06-05-VariableIndexInsert.ll
    │   │   │       ├── 2009-06-05-VZextByteShort.ll
    │   │   │       ├── 2009-06-06-ConcatVectors.ll
    │   │   │       ├── 2009-06-12-x86_64-tail-call-conv-out-of-sync-bug.ll
    │   │   │       ├── 2009-06-15-not-a-tail-call.ll
    │   │   │       ├── 2009-06-18-movlp-shuffle-register.ll
    │   │   │       ├── 2009-07-06-TwoAddrAssert.ll
    │   │   │       ├── 2009-07-07-SplitICmp.ll
    │   │   │       ├── 2009-07-09-ExtractBoolFromVector.ll
    │   │   │       ├── 2009-07-15-CoalescerBug.ll
    │   │   │       ├── 2009-07-16-CoalescerBug.ll
    │   │   │       ├── 2009-07-19-AsmExtraOperands.ll
    │   │   │       ├── 2009-07-20-CoalescerBug.ll
    │   │   │       ├── 2009-07-20-DAGCombineBug.ll
    │   │   │       ├── 2009-08-06-branchfolder-crash.ll
    │   │   │       ├── 2009-08-06-inlineasm.ll
    │   │   │       ├── 2009-08-08-CastError.ll
    │   │   │       ├── 2009-08-12-badswitch.ll
    │   │   │       ├── 2009-08-14-Win64MemoryIndirectArg.ll
    │   │   │       ├── 2009-08-19-LoadNarrowingMiscompile.ll
    │   │   │       ├── 2009-08-23-SubRegReuseUndo.ll
    │   │   │       ├── 2009-09-10-LoadFoldingBug.ll
    │   │   │       ├── 2009-09-10-SpillComments.ll
    │   │   │       ├── 2009-09-16-CoalescerBug.ll
    │   │   │       ├── 2009-09-19-earlyclobber.ll
    │   │   │       ├── 2009-09-21-NoSpillLoopCount.ll
    │   │   │       ├── 2009-09-22-CoalescerBug.ll
    │   │   │       ├── 2009-09-23-LiveVariablesBug.ll
    │   │   │       ├── 2009-10-14-LiveVariablesBug.ll
    │   │   │       ├── 2009-10-16-Scope.ll
    │   │   │       ├── 2009-10-19-atomic-cmp-eflags.ll
    │   │   │       ├── 2009-10-19-EmergencySpill.ll
    │   │   │       ├── 2009-10-25-RewriterBug.ll
    │   │   │       ├── 2009-11-04-SubregCoalescingBug.ll
    │   │   │       ├── 2009-11-13-VirtRegRewriterBug.ll
    │   │   │       ├── 2009-11-16-MachineLICM.ll
    │   │   │       ├── 2009-11-16-UnfoldMemOpBug.ll
    │   │   │       ├── 2009-11-17-UpdateTerminator.ll
    │   │   │       ├── 2009-11-18-TwoAddrKill.ll
    │   │   │       ├── 2009-11-25-ImpDefBug.ll
    │   │   │       ├── 2009-12-01-EarlyClobberBug.ll
    │   │   │       ├── 2009-12-11-TLSNoRedZone.ll
    │   │   │       ├── 20090313-signext.ll
    │   │   │       ├── 2010-01-05-ZExt-Shl.ll
    │   │   │       ├── 2010-01-07-ISelBug.ll
    │   │   │       ├── 2010-01-08-Atomic64Bug.ll
    │   │   │       ├── 2010-01-11-ExtraPHIArg.ll
    │   │   │       ├── 2010-01-13-OptExtBug.ll
    │   │   │       ├── 2010-01-15-SelectionDAGCycle.ll
    │   │   │       ├── 2010-01-18-DbgValue.ll
    │   │   │       ├── 2010-01-19-OptExtBug.ll
    │   │   │       ├── 2010-02-01-DbgValueCrash.ll
    │   │   │       ├── 2010-02-01-TaillCallCrash.ll
    │   │   │       ├── 2010-02-03-DualUndef.ll
    │   │   │       ├── 2010-02-04-SchedulerBug.ll
    │   │   │       ├── 2010-02-11-NonTemporal.ll
    │   │   │       ├── 2010-02-12-CoalescerBug-Impdef.ll
    │   │   │       ├── 2010-02-15-ImplicitDefBug.ll
    │   │   │       ├── 2010-02-19-TailCallRetAddrBug.ll
    │   │   │       ├── 2010-02-23-DAGCombineBug.ll
    │   │   │       ├── 2010-02-23-DIV8rDefinesAX.ll
    │   │   │       ├── 2010-02-23-RematImplicitSubreg.ll
    │   │   │       ├── 2010-02-23-SingleDefPhiJoin.ll
    │   │   │       ├── 2010-03-04-Mul8Bug.ll
    │   │   │       ├── 2010-03-05-ConstantFoldCFG.ll
    │   │   │       ├── 2010-03-05-EFLAGS-Redef.ll
    │   │   │       ├── 2010-03-17-ISelBug.ll
    │   │   │       ├── 2010-04-06-SSEDomainFixCrash.ll
    │   │   │       ├── 2010-04-08-CoalescerBug.ll
    │   │   │       ├── 2010-04-13-AnalyzeBranchCrash.ll
    │   │   │       ├── 2010-04-21-CoalescerBug.ll
    │   │   │       ├── 2010-04-29-CoalescerCrash.ll
    │   │   │       ├── 2010-04-30-LocalAlloc-LandingPad.ll
    │   │   │       ├── 2010-05-03-CoalescerSubRegClobber.ll
    │   │   │       ├── 2010-05-05-LocalAllocEarlyClobber.ll
    │   │   │       ├── 2010-05-06-LocalInlineAsmClobber.ll
    │   │   │       ├── 2010-05-07-ldconvert.ll
    │   │   │       ├── 2010-05-10-DAGCombinerBug.ll
    │   │   │       ├── 2010-05-12-FastAllocKills.ll
    │   │   │       ├── 2010-05-16-nosseconversion.ll
    │   │   │       ├── 2010-05-25-DotDebugLoc.ll
    │   │   │       ├── 2010-05-26-DotDebugLoc.ll
    │   │   │       ├── 2010-05-26-FP_TO_INT-crash.ll
    │   │   │       ├── 2010-05-28-Crash.ll
    │   │   │       ├── 2010-06-01-DeadArg-DbgInfo.ll
    │   │   │       ├── 2010-06-09-FastAllocRegisters.ll
    │   │   │       ├── 2010-06-14-fast-isel-fs-load.ll
    │   │   │       ├── 2010-06-15-FastAllocEarlyCLobber.ll
    │   │   │       ├── 2010-06-24-g-constraint-crash.ll
    │   │   │       ├── 2010-06-25-asm-RA-crash.ll
    │   │   │       ├── 2010-06-25-CoalescerSubRegDefDead.ll
    │   │   │       ├── 2010-06-28-FastAllocTiedOperand.ll
    │   │   │       ├── 2010-06-28-matched-g-constraint.ll
    │   │   │       ├── 2010-07-02-asm-alignstack.ll
    │   │   │       ├── 2010-07-02-UnfoldBug.ll
    │   │   │       ├── 2010-07-06-asm-RIP.ll
    │   │   │       ├── 2010-07-06-DbgCrash.ll
    │   │   │       ├── 2010-07-11-FPStackLoneUse.ll
    │   │   │       ├── 2010-07-13-indirectXconstraint.ll
    │   │   │       ├── 2010-07-15-Crash.ll
    │   │   │       ├── 2010-07-29-SetccSimplify.ll
    │   │   │       ├── 2010-08-04-MaskedSignedCompare.ll
    │   │   │       ├── 2010-08-04-MingWCrash.ll
    │   │   │       ├── 2010-08-04-StackVariable.ll
    │   │   │       ├── 2010-09-01-RemoveCopyByCommutingDef.ll
    │   │   │       ├── 2010-09-16-asmcrash.ll
    │   │   │       ├── 2010-09-16-EmptyFilename.ll
    │   │   │       ├── 2010-09-17-SideEffectsInChain.ll
    │   │   │       ├── 2010-09-30-CMOV-JumpTable-PHI.ll
    │   │   │       ├── 2010-10-08-cmpxchg8b.ll
    │   │   │       ├── 2010-11-02-DbgParameter.ll
    │   │   │       ├── 2010-11-09-MOVLPS.ll
    │   │   │       ├── 2010-11-18-SelectOfExtload.ll
    │   │   │       ├── 2011-01-07-LegalizeTypesCrash.ll
    │   │   │       ├── 2011-01-10-DagCombineHang.ll
    │   │   │       ├── 2011-01-24-DbgValue-Before-Use.ll
    │   │   │       ├── 2011-02-04-FastRegallocNoFP.ll
    │   │   │       ├── 2011-02-12-shuffle.ll
    │   │   │       ├── 2011-02-21-VirtRegRewriter-KillSubReg.ll
    │   │   │       ├── 2011-02-23-UnfoldBug.ll
    │   │   │       ├── 2011-02-27-Fpextend.ll
    │   │   │       ├── 2011-03-02-DAGCombiner.ll
    │   │   │       ├── 2011-03-08-Sched-crash.ll
    │   │   │       ├── 2011-03-09-Physreg-Coalescing.ll
    │   │   │       ├── 2011-03-30-CreateFixedObjCrash.ll
    │   │   │       ├── 2011-04-13-SchedCmpJmp.ll
    │   │   │       ├── 2011-04-19-sclr-bb.ll
    │   │   │       ├── 2011-05-09-loaduse.ll
    │   │   │       ├── 2011-05-26-UnreachableBlockElim.ll
    │   │   │       ├── 2011-05-27-CrossClassCoalescing.ll
    │   │   │       ├── 2011-06-01-fildll.ll
    │   │   │       ├── 2011-06-03-x87chain.ll
    │   │   │       ├── 2011-06-06-fgetsign80bit.ll
    │   │   │       ├── 2011-06-12-FastAllocSpill.ll
    │   │   │       ├── 2011-06-14-mmx-inlineasm.ll
    │   │   │       ├── 2011-06-14-PreschedRegalias.ll
    │   │   │       ├── 2011-06-19-QuicksortCoalescerBug.ll
    │   │   │       ├── 2011-07-13-BadFrameIndexDisplacement.ll
    │   │   │       ├── 2011-08-23-PerformSubCombine128.ll
    │   │   │       ├── 2011-08-23-Trampoline.ll
    │   │   │       ├── 2011-08-29-BlockConstant.ll
    │   │   │       ├── 2011-08-29-InitOrder.ll
    │   │   │       ├── 2011-09-14-valcoalesce.ll
    │   │   │       ├── 2011-09-18-sse2cmp.ll
    │   │   │       ├── 2011-09-21-setcc-bug.ll
    │   │   │       ├── 2011-10-11-SpillDead.ll
    │   │   │       ├── 2011-10-11-srl.ll
    │   │   │       ├── 2011-10-12-MachineCSE.ll
    │   │   │       ├── 2011-10-18-FastISel-VectorParams.ll
    │   │   │       ├── 2011-10-19-LegelizeLoad.ll
    │   │   │       ├── 2011-10-19-widen_vselect.ll
    │   │   │       ├── 2011-10-21-widen-cmp.ll
    │   │   │       ├── 2011-10-27-tstore.ll
    │   │   │       ├── 2011-10-30-padd.ll
    │   │   │       ├── 2011-11-07-LegalizeBuildVector.ll
    │   │   │       ├── 2011-11-22-AVX2-Domains.ll
    │   │   │       ├── 2011-11-30-or.ll
    │   │   │       ├── 2011-12-06-AVXVectorExtractCombine.ll
    │   │   │       ├── 2011-12-06-BitcastVectorGlobal.ll
    │   │   │       ├── 2011-12-08-AVXISelBugs.ll
    │   │   │       ├── 2011-12-15-vec_shift.ll
    │   │   │       ├── 2011-12-26-extractelement-duplicate-load.ll
    │   │   │       ├── 2011-12-28-vselecti8.ll
    │   │   │       ├── 2011-12-8-bitcastintprom.ll
    │   │   │       ├── 2011-20-21-zext-ui2fp.ll
    │   │   │       ├── 2012-01-10-UndefExceptionEdge.ll
    │   │   │       ├── 2012-01-11-split-cv.ll
    │   │   │       ├── 2012-01-12-extract-sv.ll
    │   │   │       ├── 2012-01-16-mfence-nosse-flags.ll
    │   │   │       ├── 2012-01-18-vbitcast.ll
    │   │   │       ├── 2012-02-12-dagco.ll
    │   │   │       ├── 2012-02-14-scalar.ll
    │   │   │       ├── 2012-02-23-mmx-inlineasm.ll
    │   │   │       ├── 2012-02-29-CoalescerBug.ll
    │   │   │       ├── 2012-03-15-build_vector_wl.ll
    │   │   │       ├── 2012-03-20-LargeConstantExpr.ll
    │   │   │       ├── 2012-03-26-PostRALICMBug.ll
    │   │   │       ├── 2012-04-09-TwoAddrPassBug.ll
    │   │   │       ├── 2012-04-26-sdglue.ll
    │   │   │       ├── 2012-05-17-TwoAddressBug.ll
    │   │   │       ├── 2012-05-19-CoalescerCrash.ll
    │   │   │       ├── 2012-07-10-extload64.ll
    │   │   │       ├── 2012-07-10-shufnorm.ll
    │   │   │       ├── 2012-07-15-broadcastfold.ll
    │   │   │       ├── 2012-07-15-BuildVectorPromote.ll
    │   │   │       ├── 2012-07-15-tconst_shl.ll
    │   │   │       ├── 2012-07-15-vshl.ll
    │   │   │       ├── 2012-07-16-fp2ui-i1.ll
    │   │   │       ├── 2012-07-16-LeaUndef.ll
    │   │   │       ├── 2012-07-17-vtrunc.ll
    │   │   │       ├── 2012-07-23-select_cc.ll
    │   │   │       ├── 2012-08-07-CmpISelBug.ll
    │   │   │       ├── 2012-08-16-setcc.ll
    │   │   │       ├── 2012-08-17-legalizer-crash.ll
    │   │   │       ├── 2012-08-28-UnsafeMathCrash.ll
    │   │   │       ├── 2012-09-13-dagco-fneg.ll
    │   │   │       ├── 2012-09-28-CGPBug.ll
    │   │   │       ├── 2012-1-10-buildvector.ll
    │   │   │       ├── 2012-10-02-DAGCycle.ll
    │   │   │       ├── 2012-10-03-DAGCycle.ll
    │   │   │       ├── 2012-10-18-crash-dagco.ll
    │   │   │       ├── 2012-11-28-merge-store-alias.ll
    │   │   │       ├── 2012-12-1-merge-multiple.ll
    │   │   │       ├── 2012-12-12-DAGCombineCrash.ll
    │   │   │       ├── 2012-12-14-v8fp80-crash.ll
    │   │   │       ├── 2012-12-19-NoImplicitFloat.ll
    │   │   │       ├── 2013-01-09-DAGCombineBug.ll
    │   │   │       ├── 2013-03-13-VEX-DestReg.ll
    │   │   │       ├── 2013-05-06-ConactVectorCrash.ll
    │   │   │       ├── 2013-10-14-FastISel-incorrect-vreg.ll
    │   │   │       ├── 2014-05-29-factorial.ll
    │   │   │       ├── 2014-08-29-CompactUnwind.ll
    │   │   │       ├── 3addr-16bit.ll
    │   │   │       ├── 3addr-or.ll
    │   │   │       ├── 3dnow-intrinsics.ll
    │   │   │       ├── 3dnow-schedule.ll
    │   │   │       ├── 4char-promote.ll
    │   │   │       ├── 9601.ll
    │   │   │       ├── abi-isel.ll
    │   │   │       ├── absolute-bit-mask-fastisel.ll
    │   │   │       ├── absolute-bit-mask.ll
    │   │   │       ├── absolute-bt.ll
    │   │   │       ├── absolute-cmp.ll
    │   │   │       ├── absolute-constant.ll
    │   │   │       ├── absolute-rotate.ll
    │   │   │       ├── add-ext.ll
    │   │   │       ├── add-i64.ll
    │   │   │       ├── add-of-carry.ll
    │   │   │       ├── add-sub-nsw-nuw.ll
    │   │   │       ├── add.ll
    │   │   │       ├── add32ri8.ll
    │   │   │       ├── add_shl_constant.ll
    │   │   │       ├── addcarry.ll
    │   │   │       ├── addcarry2.ll
    │   │   │       ├── addr-label-difference.ll
    │   │   │       ├── addr-mode-matcher.ll
    │   │   │       ├── addr-of-ret-addr.ll
    │   │   │       ├── address-type-promotion-constantexpr.ll
    │   │   │       ├── addrsig.ll
    │   │   │       ├── adx-commute.mir
    │   │   │       ├── adx-intrinsics-upgrade.ll
    │   │   │       ├── adx-intrinsics.ll
    │   │   │       ├── adx-schedule.ll
    │   │   │       ├── aes-schedule.ll
    │   │   │       ├── aes_intrinsics.ll
    │   │   │       ├── alias-gep.ll
    │   │   │       ├── alias-static-alloca.ll
    │   │   │       ├── aliases.ll
    │   │   │       ├── aligned-comm.ll
    │   │   │       ├── aligned-variadic.ll
    │   │   │       ├── alignment-2.ll
    │   │   │       ├── alignment.ll
    │   │   │       ├── all-ones-vector.ll
    │   │   │       ├── alldiv-divdi3.ll
    │   │   │       ├── alloca-align-rounding-32.ll
    │   │   │       ├── alloca-align-rounding.ll
    │   │   │       ├── allrem-moddi3.ll
    │   │   │       ├── and-encoding.ll
    │   │   │       ├── and-load-fold.ll
    │   │   │       ├── and-or-fold.ll
    │   │   │       ├── and-sink.ll
    │   │   │       ├── and-su.ll
    │   │   │       ├── andimm8.ll
    │   │   │       ├── anyext.ll
    │   │   │       ├── anyregcc-crash.ll
    │   │   │       ├── anyregcc.ll
    │   │   │       ├── apm.ll
    │   │   │       ├── AppendingLinkage.ll
    │   │   │       ├── arg-cast.ll
    │   │   │       ├── arg-copy-elide.ll
    │   │   │       ├── asm-block-labels.ll
    │   │   │       ├── asm-global-imm.ll
    │   │   │       ├── asm-indirect-mem.ll
    │   │   │       ├── asm-invalid-register-class-crasher.ll
    │   │   │       ├── asm-label.ll
    │   │   │       ├── asm-label2.ll
    │   │   │       ├── asm-mismatched-types.ll
    │   │   │       ├── asm-modifier-P.ll
    │   │   │       ├── asm-modifier.ll
    │   │   │       ├── asm-reg-type-mismatch.ll
    │   │   │       ├── asm-reject-reg-type-mismatch.ll
    │   │   │       ├── asm-reject-rex.ll
    │   │   │       ├── asm-reject-xmm16.ll
    │   │   │       ├── atom-call-reg-indirect-foldedreload32.ll
    │   │   │       ├── atom-call-reg-indirect-foldedreload64.ll
    │   │   │       ├── atom-call-reg-indirect.ll
    │   │   │       ├── atom-cmpb.ll
    │   │   │       ├── atom-fixup-lea1.ll
    │   │   │       ├── atom-fixup-lea2.ll
    │   │   │       ├── atom-fixup-lea3.ll
    │   │   │       ├── atom-fixup-lea4.ll
    │   │   │       ├── atom-lea-addw-bug.ll
    │   │   │       ├── atom-lea-sp.ll
    │   │   │       ├── atom-pad-short-functions.ll
    │   │   │       ├── atom-sched.ll
    │   │   │       ├── atom-shuf.ll
    │   │   │       ├── atomic-dagsched.ll
    │   │   │       ├── atomic-eflags-reuse.ll
    │   │   │       ├── atomic-flags.ll
    │   │   │       ├── atomic-load-store-wide.ll
    │   │   │       ├── atomic-load-store.ll
    │   │   │       ├── atomic-minmax-i6432.ll
    │   │   │       ├── atomic-non-integer.ll
    │   │   │       ├── atomic-ops-ancient-64.ll
    │   │   │       ├── atomic-or.ll
    │   │   │       ├── atomic-pointer.ll
    │   │   │       ├── atomic128.ll
    │   │   │       ├── atomic16.ll
    │   │   │       ├── atomic32.ll
    │   │   │       ├── atomic64.ll
    │   │   │       ├── atomic6432.ll
    │   │   │       ├── atomic8.ll
    │   │   │       ├── atomic_add.ll
    │   │   │       ├── atomic_idempotent.ll
    │   │   │       ├── atomic_mi.ll
    │   │   │       ├── atomic_op.ll
    │   │   │       ├── Atomics-64.ll
    │   │   │       ├── attribute-sections.ll
    │   │   │       ├── avg-mask.ll
    │   │   │       ├── avg.ll
    │   │   │       ├── avoid-lea-scale2.ll
    │   │   │       ├── avoid-loop-align-2.ll
    │   │   │       ├── avoid-loop-align.ll
    │   │   │       ├── avoid-sfb-kill-flags.mir
    │   │   │       ├── avoid-sfb-offset.mir
    │   │   │       ├── avoid-sfb-overlaps.ll
    │   │   │       ├── avoid-sfb.ll
    │   │   │       ├── avoid_complex_am.ll
    │   │   │       ├── avx-arith.ll
    │   │   │       ├── avx-basic.ll
    │   │   │       ├── avx-bitcast.ll
    │   │   │       ├── avx-brcond.ll
    │   │   │       ├── avx-cast.ll
    │   │   │       ├── avx-cmp.ll
    │   │   │       ├── avx-cvt-2.ll
    │   │   │       ├── avx-cvt-3.ll
    │   │   │       ├── avx-cvt.ll
    │   │   │       ├── avx-cvttp2si.ll
    │   │   │       ├── avx-fp2int.ll
    │   │   │       ├── avx-gfni-intrinsics.ll
    │   │   │       ├── avx-insertelt.ll
    │   │   │       ├── avx-intel-ocl.ll
    │   │   │       ├── avx-intrinsics-fast-isel.ll
    │   │   │       ├── avx-intrinsics-x86-upgrade.ll
    │   │   │       ├── avx-intrinsics-x86.ll
    │   │   │       ├── avx-intrinsics-x86_64.ll
    │   │   │       ├── avx-isa-check.ll
    │   │   │       ├── avx-load-store.ll
    │   │   │       ├── avx-logic.ll
    │   │   │       ├── avx-minmax.ll
    │   │   │       ├── avx-schedule.ll
    │   │   │       ├── avx-select.ll
    │   │   │       ├── avx-shift.ll
    │   │   │       ├── avx-shuffle-x86_32.ll
    │   │   │       ├── avx-splat.ll
    │   │   │       ├── avx-trunc.ll
    │   │   │       ├── avx-unpack.ll
    │   │   │       ├── avx-varargs-x86_64.ll
    │   │   │       ├── avx-vbroadcast.ll
    │   │   │       ├── avx-vbroadcastf128.ll
    │   │   │       ├── avx-vextractf128.ll
    │   │   │       ├── avx-vinsertf128.ll
    │   │   │       ├── avx-vpclmulqdq.ll
    │   │   │       ├── avx-vperm2x128.ll
    │   │   │       ├── avx-vzeroupper.ll
    │   │   │       ├── avx-win64-args.ll
    │   │   │       ├── avx-win64.ll
    │   │   │       ├── avx.ll
    │   │   │       ├── avx1-logical-load-folding.ll
    │   │   │       ├── avx2-arith.ll
    │   │   │       ├── avx2-cmp.ll
    │   │   │       ├── avx2-conversions.ll
    │   │   │       ├── avx2-fma-fneg-combine.ll
    │   │   │       ├── avx2-gather.ll
    │   │   │       ├── avx2-intrinsics-canonical.ll
    │   │   │       ├── avx2-intrinsics-fast-isel.ll
    │   │   │       ├── avx2-intrinsics-x86-upgrade.ll
    │   │   │       ├── avx2-intrinsics-x86.ll
    │   │   │       ├── avx2-logic.ll
    │   │   │       ├── avx2-masked-gather.ll
    │   │   │       ├── avx2-nontemporal.ll
    │   │   │       ├── avx2-phaddsub.ll
    │   │   │       ├── avx2-pmovxrm.ll
    │   │   │       ├── avx2-schedule.ll
    │   │   │       ├── avx2-shift.ll
    │   │   │       ├── avx2-vbroadcast.ll
    │   │   │       ├── avx2-vbroadcasti128.ll
    │   │   │       ├── avx2-vector-shifts.ll
    │   │   │       ├── avx2-vperm.ll
    │   │   │       ├── avx512-adc-sbb.ll
    │   │   │       ├── avx512-any_extend_load.ll
    │   │   │       ├── avx512-arith.ll
    │   │   │       ├── avx512-bugfix-23634.ll
    │   │   │       ├── avx512-bugfix-25270.ll
    │   │   │       ├── avx512-bugfix-26264.ll
    │   │   │       ├── avx512-build-vector.ll
    │   │   │       ├── avx512-calling-conv.ll
    │   │   │       ├── avx512-cmp-kor-sequence.ll
    │   │   │       ├── avx512-cmp.ll
    │   │   │       ├── avx512-cvt-widen.ll
    │   │   │       ├── avx512-cvt.ll
    │   │   │       ├── avx512-cvttp2i.ll
    │   │   │       ├── avx512-ext.ll
    │   │   │       ├── avx512-extract-subvector-load-store.ll
    │   │   │       ├── avx512-extract-subvector.ll
    │   │   │       ├── avx512-fma-commute.ll
    │   │   │       ├── avx512-fma-intrinsics-upgrade.ll
    │   │   │       ├── avx512-fma-intrinsics.ll
    │   │   │       ├── avx512-fma.ll
    │   │   │       ├── avx512-fsel.ll
    │   │   │       ├── avx512-gather-scatter-intrin-deprecated.ll
    │   │   │       ├── avx512-gather-scatter-intrin.ll
    │   │   │       ├── avx512-gfni-intrinsics.ll
    │   │   │       ├── avx512-hadd-hsub.ll
    │   │   │       ├── avx512-i1test.ll
    │   │   │       ├── avx512-inc-dec.ll
    │   │   │       ├── avx512-insert-extract.ll
    │   │   │       ├── avx512-insert-extract_i1.ll
    │   │   │       ├── avx512-intel-ocl.ll
    │   │   │       ├── avx512-intrinsics-canonical.ll
    │   │   │       ├── avx512-intrinsics-fast-isel.ll
    │   │   │       ├── avx512-intrinsics-upgrade.ll
    │   │   │       ├── avx512-intrinsics.ll
    │   │   │       ├── avx512-load-store.ll
    │   │   │       ├── avx512-load-trunc-store-i1.ll
    │   │   │       ├── avx512-logic.ll
    │   │   │       ├── avx512-mask-op.ll
    │   │   │       ├── avx512-mask-spills.ll
    │   │   │       ├── avx512-mask-zext-bugfix.ll
    │   │   │       ├── avx512-masked-memop-64-32.ll
    │   │   │       ├── avx512-masked_memop-16-8.ll
    │   │   │       ├── avx512-memfold.ll
    │   │   │       ├── avx512-mov.ll
    │   │   │       ├── avx512-nontemporal.ll
    │   │   │       ├── avx512-pmovxrm.ll
    │   │   │       ├── avx512-regcall-Mask.ll
    │   │   │       ├── avx512-regcall-NoMask.ll
    │   │   │       ├── avx512-rndscale.ll
    │   │   │       ├── avx512-rotate.ll
    │   │   │       ├── avx512-scalar.ll
    │   │   │       ├── avx512-scalar_mask.ll
    │   │   │       ├── avx512-scalarIntrinsics.ll
    │   │   │       ├── avx512-schedule.ll
    │   │   │       ├── avx512-select.ll
    │   │   │       ├── avx512-shift.ll
    │   │   │       ├── avx512-shuffle-schedule.ll
    │   │   │       ├── avx512-skx-insert-subvec.ll
    │   │   │       ├── avx512-trunc-widen.ll
    │   │   │       ├── avx512-trunc.ll
    │   │   │       ├── avx512-unsafe-fp-math.ll
    │   │   │       ├── avx512-vbroadcast.ll
    │   │   │       ├── avx512-vbroadcasti128.ll
    │   │   │       ├── avx512-vbroadcasti256.ll
    │   │   │       ├── avx512-vec-cmp.ll
    │   │   │       ├── avx512-vec3-crash.ll
    │   │   │       ├── avx512-vpclmulqdq.ll
    │   │   │       ├── avx512-vpermv3-commute.ll
    │   │   │       ├── avx512-vpternlog-commute.ll
    │   │   │       ├── avx512-vselect-crash.ll
    │   │   │       ├── avx512-vselect.ll
    │   │   │       ├── avx512bw-arith.ll
    │   │   │       ├── avx512bw-intrinsics-canonical.ll
    │   │   │       ├── avx512bw-intrinsics-fast-isel.ll
    │   │   │       ├── avx512bw-intrinsics-upgrade.ll
    │   │   │       ├── avx512bw-intrinsics.ll
    │   │   │       ├── avx512bw-mask-op.ll
    │   │   │       ├── avx512bw-mov.ll
    │   │   │       ├── avx512bw-vec-cmp.ll
    │   │   │       ├── avx512bw-vec-test-testn.ll
    │   │   │       ├── avx512bwvl-arith.ll
    │   │   │       ├── avx512bwvl-intrinsics-canonical.ll
    │   │   │       ├── avx512bwvl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512bwvl-intrinsics-upgrade.ll
    │   │   │       ├── avx512bwvl-intrinsics.ll
    │   │   │       ├── avx512bwvl-mov.ll
    │   │   │       ├── avx512bwvl-vec-cmp.ll
    │   │   │       ├── avx512bwvl-vec-test-testn.ll
    │   │   │       ├── avx512cd-intrinsics-fast-isel.ll
    │   │   │       ├── avx512cd-intrinsics-upgrade.ll
    │   │   │       ├── avx512cd-intrinsics.ll
    │   │   │       ├── avx512cdvl-intrinsics-upgrade.ll
    │   │   │       ├── avx512cdvl-intrinsics.ll
    │   │   │       ├── avx512dq-intrinsics-fast-isel.ll
    │   │   │       ├── avx512dq-intrinsics-upgrade.ll
    │   │   │       ├── avx512dq-intrinsics.ll
    │   │   │       ├── avx512dq-mask-op.ll
    │   │   │       ├── avx512dqvl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512dqvl-intrinsics-upgrade.ll
    │   │   │       ├── avx512dqvl-intrinsics.ll
    │   │   │       ├── avx512er-intrinsics.ll
    │   │   │       ├── avx512f-vec-test-testn.ll
    │   │   │       ├── avx512ifma-intrinsics-fast-isel.ll
    │   │   │       ├── avx512ifma-intrinsics-upgrade.ll
    │   │   │       ├── avx512ifma-intrinsics.ll
    │   │   │       ├── avx512ifmavl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512ifmavl-intrinsics-upgrade.ll
    │   │   │       ├── avx512ifmavl-intrinsics.ll
    │   │   │       ├── avx512vbmi-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vbmi-intrinsics-upgrade.ll
    │   │   │       ├── avx512vbmi-intrinsics.ll
    │   │   │       ├── avx512vbmi2-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vbmi2-intrinsics-upgrade.ll
    │   │   │       ├── avx512vbmi2-intrinsics.ll
    │   │   │       ├── avx512vbmi2vl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vbmi2vl-intrinsics-upgrade.ll
    │   │   │       ├── avx512vbmi2vl-intrinsics.ll
    │   │   │       ├── avx512vbmivl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vbmivl-intrinsics-upgrade.ll
    │   │   │       ├── avx512vbmivl-intrinsics.ll
    │   │   │       ├── avx512vl-arith.ll
    │   │   │       ├── avx512vl-intrinsics-canonical.ll
    │   │   │       ├── avx512vl-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vl-intrinsics-upgrade.ll
    │   │   │       ├── avx512vl-intrinsics.ll
    │   │   │       ├── avx512vl-logic.ll
    │   │   │       ├── avx512vl-mov.ll
    │   │   │       ├── avx512vl-nontemporal.ll
    │   │   │       ├── avx512vl-vbroadcast.ll
    │   │   │       ├── avx512vl-vec-cmp.ll
    │   │   │       ├── avx512vl-vec-masked-cmp.ll
    │   │   │       ├── avx512vl-vec-test-testn.ll
    │   │   │       ├── avx512vl-vpclmulqdq.ll
    │   │   │       ├── avx512vl_vnni-intrinsics-upgrade.ll
    │   │   │       ├── avx512vl_vnni-intrinsics.ll
    │   │   │       ├── avx512vlcd-intrinsics-fast-isel.ll
    │   │   │       ├── avx512vnni-intrinsics-upgrade.ll
    │   │   │       ├── avx512vnni-intrinsics.ll
    │   │   │       ├── avx512vpopcntdq-intrinsics.ll
    │   │   │       ├── avx512vpopcntdq-schedule.ll
    │   │   │       ├── backpropmask.ll
    │   │   │       ├── bad-tls-fold.mir
    │   │   │       ├── barrier-sse.ll
    │   │   │       ├── barrier.ll
    │   │   │       ├── base-pointer-and-cmpxchg.ll
    │   │   │       ├── basic-promote-integers.ll
    │   │   │       ├── bc-extract.ll
    │   │   │       ├── bigstructret.ll
    │   │   │       ├── bigstructret2.ll
    │   │   │       ├── bit-piece-comment.ll
    │   │   │       ├── bit-test-shift.ll
    │   │   │       ├── bitcast-and-setcc-128.ll
    │   │   │       ├── bitcast-and-setcc-256.ll
    │   │   │       ├── bitcast-and-setcc-512.ll
    │   │   │       ├── bitcast-i256.ll
    │   │   │       ├── bitcast-int-to-vector-bool-sext.ll
    │   │   │       ├── bitcast-int-to-vector-bool-zext.ll
    │   │   │       ├── bitcast-int-to-vector-bool.ll
    │   │   │       ├── bitcast-int-to-vector.ll
    │   │   │       ├── bitcast-mmx.ll
    │   │   │       ├── bitcast-setcc-128.ll
    │   │   │       ├── bitcast-setcc-256.ll
    │   │   │       ├── bitcast-setcc-512.ll
    │   │   │       ├── bitcast.ll
    │   │   │       ├── bitcast2.ll
    │   │   │       ├── bitcnt-false-dep.ll
    │   │   │       ├── bitreverse.ll
    │   │   │       ├── block-placement.ll
    │   │   │       ├── block-placement.mir
    │   │   │       ├── bmi-intrinsics-fast-isel-x86_64.ll
    │   │   │       ├── bmi-intrinsics-fast-isel.ll
    │   │   │       ├── bmi-schedule.ll
    │   │   │       ├── bmi-x86_64.ll
    │   │   │       ├── bmi.ll
    │   │   │       ├── bmi2-schedule.ll
    │   │   │       ├── bmi2-x86_64.ll
    │   │   │       ├── bmi2.ll
    │   │   │       ├── bool-ext-inc.ll
    │   │   │       ├── bool-math.ll
    │   │   │       ├── bool-simplify.ll
    │   │   │       ├── bool-vector.ll
    │   │   │       ├── bool-zext.ll
    │   │   │       ├── br-fold.ll
    │   │   │       ├── branchfolding-catchpads.ll
    │   │   │       ├── branchfolding-debugloc.ll
    │   │   │       ├── branchfolding-landingpads.ll
    │   │   │       ├── branchfolding-undef.mir
    │   │   │       ├── brcond.ll
    │   │   │       ├── break-anti-dependencies.ll
    │   │   │       ├── break-false-dep.ll
    │   │   │       ├── broadcast-elm-cross-splat-vec.ll
    │   │   │       ├── broadcastm-lowering.ll
    │   │   │       ├── bss_pagealigned.ll
    │   │   │       ├── bswap-inline-asm.ll
    │   │   │       ├── bswap-rotate.ll
    │   │   │       ├── bswap-vector.ll
    │   │   │       ├── bswap-wide-int.ll
    │   │   │       ├── bswap.ll
    │   │   │       ├── bswap_tree.ll
    │   │   │       ├── bswap_tree2.ll
    │   │   │       ├── bt.ll
    │   │   │       ├── btc_bts_btr.ll
    │   │   │       ├── btq.ll
    │   │   │       ├── bug26810.ll
    │   │   │       ├── bug37521.ll
    │   │   │       ├── build-vector-128.ll
    │   │   │       ├── build-vector-256.ll
    │   │   │       ├── build-vector-512.ll
    │   │   │       ├── buildvec-extract.ll
    │   │   │       ├── buildvec-insertvec.ll
    │   │   │       ├── bypass-slow-division-32.ll
    │   │   │       ├── bypass-slow-division-64.ll
    │   │   │       ├── bypass-slow-division-tune.ll
    │   │   │       ├── byval-align.ll
    │   │   │       ├── byval-callee-cleanup.ll
    │   │   │       ├── byval.ll
    │   │   │       ├── byval2.ll
    │   │   │       ├── byval3.ll
    │   │   │       ├── byval4.ll
    │   │   │       ├── byval5.ll
    │   │   │       ├── byval6.ll
    │   │   │       ├── byval7.ll
    │   │   │       ├── cache-intrinsic.ll
    │   │   │       ├── call-imm.ll
    │   │   │       ├── call-push.ll
    │   │   │       ├── cas.ll
    │   │   │       ├── cast-vsel.ll
    │   │   │       ├── catch.ll
    │   │   │       ├── catchpad-dynamic-alloca.ll
    │   │   │       ├── catchpad-lifetime.ll
    │   │   │       ├── catchpad-realign-savexmm.ll
    │   │   │       ├── catchpad-regmask.ll
    │   │   │       ├── catchpad-reuse.ll
    │   │   │       ├── catchpad-weight.ll
    │   │   │       ├── catchret-empty-fallthrough.ll
    │   │   │       ├── catchret-fallthrough.ll
    │   │   │       ├── catchret-regmask.ll
    │   │   │       ├── cfi-inserter-cfg-with-merge.mir
    │   │   │       ├── cfi-inserter-check-order.ll
    │   │   │       ├── cfi-inserter-noreturnblock.mir
    │   │   │       ├── cfi-inserter-verify-inconsistent-offset.mir
    │   │   │       ├── cfi-inserter-verify-inconsistent-register.mir
    │   │   │       ├── cfi-xmm.ll
    │   │   │       ├── cfi.ll
    │   │   │       ├── cfstring.ll
    │   │   │       ├── chain_order.ll
    │   │   │       ├── change-compare-stride-1.ll
    │   │   │       ├── change-compare-stride-trickiness-0.ll
    │   │   │       ├── change-compare-stride-trickiness-1.ll
    │   │   │       ├── change-compare-stride-trickiness-2.ll
    │   │   │       ├── change-unsafe-fp-math.ll
    │   │   │       ├── cldemote-intrinsic.ll
    │   │   │       ├── cleanuppad-inalloca.ll
    │   │   │       ├── cleanuppad-large-codemodel.ll
    │   │   │       ├── cleanuppad-realign.ll
    │   │   │       ├── clear-highbits.ll
    │   │   │       ├── clear-lowbits.ll
    │   │   │       ├── clear_upper_vector_element_bits.ll
    │   │   │       ├── clflushopt-schedule.ll
    │   │   │       ├── clflushopt.ll
    │   │   │       ├── clwb-schedule.ll
    │   │   │       ├── clwb.ll
    │   │   │       ├── clz.ll
    │   │   │       ├── clzero-schedule.ll
    │   │   │       ├── clzero.ll
    │   │   │       ├── cmov-double.ll
    │   │   │       ├── cmov-fp.ll
    │   │   │       ├── cmov-into-branch.ll
    │   │   │       ├── cmov-promotion.ll
    │   │   │       ├── cmov-schedule.ll
    │   │   │       ├── cmov.ll
    │   │   │       ├── cmovcmov.ll
    │   │   │       ├── cmp-fast-isel.ll
    │   │   │       ├── cmp.ll
    │   │   │       ├── cmpxchg-clobber-flags.ll
    │   │   │       ├── cmpxchg-i1.ll
    │   │   │       ├── cmpxchg-i128-i1.ll
    │   │   │       ├── cmpxchg16b.ll
    │   │   │       ├── cmpxchg8b.ll
    │   │   │       ├── cmpxchg8b_alloca_regalloc_handling.ll
    │   │   │       ├── coal-sections.ll
    │   │   │       ├── coalesce-dbg-value-subreg-rewrite.mir
    │   │   │       ├── coalesce-dead-lanes.mir
    │   │   │       ├── coalesce-esp.ll
    │   │   │       ├── coalesce-implicitdef.ll
    │   │   │       ├── coalesce_commute_movsd.ll
    │   │   │       ├── coalesce_commute_subreg.ll
    │   │   │       ├── coalescer-commute1.ll
    │   │   │       ├── coalescer-commute2.ll
    │   │   │       ├── coalescer-commute3.ll
    │   │   │       ├── coalescer-commute4.ll
    │   │   │       ├── coalescer-commute5.ll
    │   │   │       ├── coalescer-cross.ll
    │   │   │       ├── coalescer-dce.ll
    │   │   │       ├── coalescer-dce2.ll
    │   │   │       ├── coalescer-identity.ll
    │   │   │       ├── coalescer-remat.ll
    │   │   │       ├── coalescer-subreg.ll
    │   │   │       ├── coalescer-win64.ll
    │   │   │       ├── code-model-elf-memset.ll
    │   │   │       ├── code-model-elf.ll
    │   │   │       ├── code-model-kernel.ll
    │   │   │       ├── code_placement.ll
    │   │   │       ├── code_placement_align_all.ll
    │   │   │       ├── code_placement_cold_loop_blocks.ll
    │   │   │       ├── code_placement_eh.ll
    │   │   │       ├── code_placement_ignore_succ_in_inner_loop.ll
    │   │   │       ├── code_placement_loop_rotation.ll
    │   │   │       ├── code_placement_loop_rotation2.ll
    │   │   │       ├── code_placement_loop_rotation3.ll
    │   │   │       ├── codegen-prepare-addrmode-sext.ll
    │   │   │       ├── codegen-prepare-cast.ll
    │   │   │       ├── codegen-prepare-crash.ll
    │   │   │       ├── codegen-prepare-extload.ll
    │   │   │       ├── codegen-prepare.ll
    │   │   │       ├── codemodel.ll
    │   │   │       ├── coff-comdat.ll
    │   │   │       ├── coff-comdat2.ll
    │   │   │       ├── coff-comdat3.ll
    │   │   │       ├── coff-feat00.ll
    │   │   │       ├── coff-no-dead-strip.ll
    │   │   │       ├── coff-weak.ll
    │   │   │       ├── coldcc64.ll
    │   │   │       ├── combine-64bit-vec-binop.ll
    │   │   │       ├── combine-abs.ll
    │   │   │       ├── combine-add-ssat.ll
    │   │   │       ├── combine-add-usat.ll
    │   │   │       ├── combine-add.ll
    │   │   │       ├── combine-and.ll
    │   │   │       ├── combine-avx-intrinsics.ll
    │   │   │       ├── combine-avx2-intrinsics.ll
    │   │   │       ├── combine-bitselect.ll
    │   │   │       ├── combine-concatvectors.ll
    │   │   │       ├── combine-fabs.ll
    │   │   │       ├── combine-fcopysign.ll
    │   │   │       ├── combine-lds.ll
    │   │   │       ├── combine-mul.ll
    │   │   │       ├── combine-multiplies.ll
    │   │   │       ├── combine-or.ll
    │   │   │       ├── combine-pmuldq.ll
    │   │   │       ├── combine-rotates.ll
    │   │   │       ├── combine-sdiv.ll
    │   │   │       ├── combine-select.ll
    │   │   │       ├── combine-sext-in-reg.ll
    │   │   │       ├── combine-shl.ll
    │   │   │       ├── combine-smax.ll
    │   │   │       ├── combine-smin.ll
    │   │   │       ├── combine-sra.ll
    │   │   │       ├── combine-srem.ll
    │   │   │       ├── combine-srl.ll
    │   │   │       ├── combine-sse41-intrinsics.ll
    │   │   │       ├── combine-sub-ssat.ll
    │   │   │       ├── combine-sub-usat.ll
    │   │   │       ├── combine-sub.ll
    │   │   │       ├── combine-testm-and.ll
    │   │   │       ├── combine-udiv.ll
    │   │   │       ├── combine-umax.ll
    │   │   │       ├── combine-umin.ll
    │   │   │       ├── combine-urem.ll
    │   │   │       ├── commandline-metadata.ll
    │   │   │       ├── commute-3dnow.ll
    │   │   │       ├── commute-blend-avx2.ll
    │   │   │       ├── commute-blend-sse41.ll
    │   │   │       ├── commute-clmul.ll
    │   │   │       ├── commute-fcmp.ll
    │   │   │       ├── commute-intrinsic.ll
    │   │   │       ├── commute-two-addr.ll
    │   │   │       ├── commute-vpclmulqdq-avx.ll
    │   │   │       ├── commute-vpclmulqdq-avx512.ll
    │   │   │       ├── commute-xop.ll
    │   │   │       ├── commuted-blend-mask.ll
    │   │   │       ├── compact-unwind.ll
    │   │   │       ├── compare-add.ll
    │   │   │       ├── compare-global.ll
    │   │   │       ├── compare-inf.ll
    │   │   │       ├── compare_folding.ll
    │   │   │       ├── compiler_used.ll
    │   │   │       ├── complex-asm.ll
    │   │   │       ├── complex-fastmath.ll
    │   │   │       ├── complex-fca.ll
    │   │   │       ├── compress_expand.ll
    │   │   │       ├── computeKnownBits_urem.ll
    │   │   │       ├── condbr_if.ll
    │   │   │       ├── condbr_switch.ll
    │   │   │       ├── conditional-indecrement.ll
    │   │   │       ├── conditional-tailcall-samedest.mir
    │   │   │       ├── conditional-tailcall.ll
    │   │   │       ├── consecutive-load-shuffle.ll
    │   │   │       ├── const-base-addr.ll
    │   │   │       ├── constant-combines.ll
    │   │   │       ├── constant-hoisting-and.ll
    │   │   │       ├── constant-hoisting-bfi.ll
    │   │   │       ├── constant-hoisting-cmp.ll
    │   │   │       ├── constant-hoisting-optnone.ll
    │   │   │       ├── constant-hoisting-shift-immediate.ll
    │   │   │       ├── constant-pool-remat-0.ll
    │   │   │       ├── constant-pool-sharing.ll
    │   │   │       ├── constpool.ll
    │   │   │       ├── constructor.ll
    │   │   │       ├── convert-2-addr-3-addr-inc64.ll
    │   │   │       ├── copy-eflags.ll
    │   │   │       ├── copy-propagation.ll
    │   │   │       ├── copysign-constant-magnitude.ll
    │   │   │       ├── cpus-amd-no-x86_64.ll
    │   │   │       ├── cpus-amd.ll
    │   │   │       ├── cpus-intel-no-x86_64.ll
    │   │   │       ├── cpus-intel.ll
    │   │   │       ├── cpus-no-x86_64.ll
    │   │   │       ├── cpus-other.ll
    │   │   │       ├── crash-lre-eliminate-dead-def.ll
    │   │   │       ├── crash-nosse.ll
    │   │   │       ├── crash-O0.ll
    │   │   │       ├── crash.ll
    │   │   │       ├── critical-anti-dep-breaker.ll
    │   │   │       ├── critical-edge-split-2.ll
    │   │   │       ├── cse-add-with-overflow.ll
    │   │   │       ├── cstring.ll
    │   │   │       ├── ctor-priority-coff.ll
    │   │   │       ├── ctpop-combine.ll
    │   │   │       ├── cvt16.ll
    │   │   │       ├── cvtv2f32.ll
    │   │   │       ├── cxx_tlscc64.ll
    │   │   │       ├── dag-fmf-cse.ll
    │   │   │       ├── dag-merge-fast-accesses.ll
    │   │   │       ├── dag-optnone.ll
    │   │   │       ├── dag-rauw-cse.ll
    │   │   │       ├── dag-update-nodetomatch.ll
    │   │   │       ├── dagcombine-and-setcc.ll
    │   │   │       ├── dagcombine-buildvector.ll
    │   │   │       ├── dagcombine-cse.ll
    │   │   │       ├── dagcombine-select.ll
    │   │   │       ├── dagcombine-shifts.ll
    │   │   │       ├── dagcombine-unsafe-math.ll
    │   │   │       ├── darwin-bzero.ll
    │   │   │       ├── darwin-no-dead-strip.ll
    │   │   │       ├── darwin-preemption.ll
    │   │   │       ├── darwin-quote.ll
    │   │   │       ├── darwin-tls.ll
    │   │   │       ├── dbg-baseptr.ll
    │   │   │       ├── dbg-changes-codegen-branch-folding.ll
    │   │   │       ├── dbg-changes-codegen-branch-folding2.mir
    │   │   │       ├── dbg-changes-codegen.ll
    │   │   │       ├── dbg-combine.ll
    │   │   │       ├── dbg-line-0-no-discriminator.ll
    │   │   │       ├── dbg-value-superreg-copy.mir
    │   │   │       ├── DbgValueOtherTargets.test
    │   │   │       ├── debug-loclists.ll
    │   │   │       ├── debug-nodebug-crash.ll
    │   │   │       ├── debuginfo-locations-dce.ll
    │   │   │       ├── debugloc-argsize.ll
    │   │   │       ├── debugloc-no-line-0.ll
    │   │   │       ├── deopt-bundles.ll
    │   │   │       ├── deopt-intrinsic-cconv.ll
    │   │   │       ├── deopt-intrinsic.ll
    │   │   │       ├── disable-tail-calls.ll
    │   │   │       ├── discontiguous-loops.ll
    │   │   │       ├── discriminate-mem-ops.ll
    │   │   │       ├── div-rem-simplify.ll
    │   │   │       ├── div8.ll
    │   │   │       ├── divide-by-constant.ll
    │   │   │       ├── divide-windows-itanium.ll
    │   │   │       ├── divrem.ll
    │   │   │       ├── divrem8_ext.ll
    │   │   │       ├── dllexport-x86_64.ll
    │   │   │       ├── dllexport.ll
    │   │   │       ├── dllimport-x86_64.ll
    │   │   │       ├── dllimport.ll
    │   │   │       ├── dollar-name.ll
    │   │   │       ├── domain-reassignment-implicit-def.ll
    │   │   │       ├── domain-reassignment-test.ll
    │   │   │       ├── domain-reassignment.mir
    │   │   │       ├── dont-trunc-store-double-to-float.ll
    │   │   │       ├── dropped_constructor.ll
    │   │   │       ├── dwarf-comp-dir.ll
    │   │   │       ├── dwarf-eh-prepare.ll
    │   │   │       ├── dwarf-headers.ll
    │   │   │       ├── dwarf-split-line-1.ll
    │   │   │       ├── dwarf-split-line-2.ll
    │   │   │       ├── dyn-stackalloc.ll
    │   │   │       ├── dyn_alloca_aligned.ll
    │   │   │       ├── dynamic-alloca-in-entry.ll
    │   │   │       ├── dynamic-alloca-lifetime.ll
    │   │   │       ├── dynamic-allocas-VLAs.ll
    │   │   │       ├── dynamic-regmask.ll
    │   │   │       ├── DynamicCalleeSavedRegisters.ll
    │   │   │       ├── early-cfi-sections.ll
    │   │   │       ├── early-ifcvt-crash.ll
    │   │   │       ├── early-ifcvt.ll
    │   │   │       ├── eh-frame-unreachable.ll
    │   │   │       ├── eh-label.ll
    │   │   │       ├── eh-nolandingpads.ll
    │   │   │       ├── eh-null-personality.ll
    │   │   │       ├── eh-unknown.ll
    │   │   │       ├── eh_frame.ll
    │   │   │       ├── eip-addressing-i386.ll
    │   │   │       ├── element-wise-atomic-memory-intrinsics.ll
    │   │   │       ├── elf-associated.ll
    │   │   │       ├── elf-comdat.ll
    │   │   │       ├── elf-comdat2.ll
    │   │   │       ├── emit-big-cst.ll
    │   │   │       ├── empty-function.ll
    │   │   │       ├── empty-functions.ll
    │   │   │       ├── empty-struct-return-type.ll
    │   │   │       ├── emutls-pic.ll
    │   │   │       ├── emutls-pie.ll
    │   │   │       ├── emutls.ll
    │   │   │       ├── emutls_generic.ll
    │   │   │       ├── epilogue-cfi-fp.ll
    │   │   │       ├── epilogue-cfi-no-fp.ll
    │   │   │       ├── epilogue.ll
    │   │   │       ├── equiv_with_fndef.ll
    │   │   │       ├── equiv_with_vardef.ll
    │   │   │       ├── evex-to-vex-compress.mir
    │   │   │       ├── exception-label.ll
    │   │   │       ├── exedeps-movq.ll
    │   │   │       ├── exedepsfix-broadcast.ll
    │   │   │       ├── expand-opaque-const.ll
    │   │   │       ├── expand-post-ra-pseudo.mir
    │   │   │       ├── expand-vr64-gr64-copy.mir
    │   │   │       ├── extend-set-cc-uses-dbg.ll
    │   │   │       ├── extend.ll
    │   │   │       ├── extended-fma-contraction.ll
    │   │   │       ├── extern_weak.ll
    │   │   │       ├── extmul128.ll
    │   │   │       ├── extmul64.ll
    │   │   │       ├── extract-bits.ll
    │   │   │       ├── extract-combine.ll
    │   │   │       ├── extract-concat.ll
    │   │   │       ├── extract-extract.ll
    │   │   │       ├── extract-fp.ll
    │   │   │       ├── extract-insert.ll
    │   │   │       ├── extract-lowbits.ll
    │   │   │       ├── extract-store.ll
    │   │   │       ├── extractelement-from-arg.ll
    │   │   │       ├── extractelement-index.ll
    │   │   │       ├── extractelement-legalization-cycle.ll
    │   │   │       ├── extractelement-legalization-store-ordering.ll
    │   │   │       ├── extractelement-load.ll
    │   │   │       ├── extractelement-shuffle.ll
    │   │   │       ├── extractps.ll
    │   │   │       ├── f16c-intrinsics-fast-isel.ll
    │   │   │       ├── f16c-intrinsics.ll
    │   │   │       ├── f16c-schedule.ll
    │   │   │       ├── fabs.ll
    │   │   │       ├── fadd-combines.ll
    │   │   │       ├── fast-cc-callee-pops.ll
    │   │   │       ├── fast-cc-merge-stack-adj.ll
    │   │   │       ├── fast-cc-pass-in-regs.ll
    │   │   │       ├── fast-isel-abort-warm.ll
    │   │   │       ├── fast-isel-agg-constant.ll
    │   │   │       ├── fast-isel-args-fail.ll
    │   │   │       ├── fast-isel-args-fail2.ll
    │   │   │       ├── fast-isel-args.ll
    │   │   │       ├── fast-isel-atomic.ll
    │   │   │       ├── fast-isel-avoid-unnecessary-pic-base.ll
    │   │   │       ├── fast-isel-bail.ll
    │   │   │       ├── fast-isel-bc.ll
    │   │   │       ├── fast-isel-bitcasts-avx.ll
    │   │   │       ├── fast-isel-bitcasts-avx512.ll
    │   │   │       ├── fast-isel-bitcasts.ll
    │   │   │       ├── fast-isel-branch_weights.ll
    │   │   │       ├── fast-isel-call-bool.ll
    │   │   │       ├── fast-isel-call-cleanup.ll
    │   │   │       ├── fast-isel-call.ll
    │   │   │       ├── fast-isel-cmp-branch.ll
    │   │   │       ├── fast-isel-cmp-branch2.ll
    │   │   │       ├── fast-isel-cmp-branch3.ll
    │   │   │       ├── fast-isel-cmp.ll
    │   │   │       ├── fast-isel-constant.ll
    │   │   │       ├── fast-isel-constpool.ll
    │   │   │       ├── fast-isel-constrain-store-indexreg.ll
    │   │   │       ├── fast-isel-deadcode.ll
    │   │   │       ├── fast-isel-divrem-x86-64.ll
    │   │   │       ├── fast-isel-divrem.ll
    │   │   │       ├── fast-isel-double-half-convertion.ll
    │   │   │       ├── fast-isel-emutls.ll
    │   │   │       ├── fast-isel-expect.ll
    │   │   │       ├── fast-isel-extract.ll
    │   │   │       ├── fast-isel-float-half-convertion.ll
    │   │   │       ├── fast-isel-fneg.ll
    │   │   │       ├── fast-isel-fold-mem.ll
    │   │   │       ├── fast-isel-fptrunc-fpext.ll
    │   │   │       ├── fast-isel-gc-intrinsics.ll
    │   │   │       ├── fast-isel-gep.ll
    │   │   │       ├── fast-isel-gv.ll
    │   │   │       ├── fast-isel-i1.ll
    │   │   │       ├── fast-isel-int-float-conversion-x86-64.ll
    │   │   │       ├── fast-isel-int-float-conversion.ll
    │   │   │       ├── fast-isel-load-i1.ll
    │   │   │       ├── fast-isel-mem.ll
    │   │   │       ├── fast-isel-movsbl-indexreg.ll
    │   │   │       ├── fast-isel-nontemporal.ll
    │   │   │       ├── fast-isel-noplt-pic.ll
    │   │   │       ├── fast-isel-ret-ext.ll
    │   │   │       ├── fast-isel-select-cmov.ll
    │   │   │       ├── fast-isel-select-cmov2.ll
    │   │   │       ├── fast-isel-select-cmp.ll
    │   │   │       ├── fast-isel-select-pseudo-cmov.ll
    │   │   │       ├── fast-isel-select-sse.ll
    │   │   │       ├── fast-isel-select.ll
    │   │   │       ├── fast-isel-sext-zext.ll
    │   │   │       ├── fast-isel-sext.ll
    │   │   │       ├── fast-isel-shift.ll
    │   │   │       ├── fast-isel-sse12-fptoint.ll
    │   │   │       ├── fast-isel-stackcheck.ll
    │   │   │       ├── fast-isel-store.ll
    │   │   │       ├── fast-isel-tailcall.ll
    │   │   │       ├── fast-isel-tls.ll
    │   │   │       ├── fast-isel-trunc-kill-subreg.ll
    │   │   │       ├── fast-isel-uint-float-conversion-x86-64.ll
    │   │   │       ├── fast-isel-uint-float-conversion.ll
    │   │   │       ├── fast-isel-vecload.ll
    │   │   │       ├── fast-isel-x32.ll
    │   │   │       ├── fast-isel-x86-64.ll
    │   │   │       ├── fast-isel-x86.ll
    │   │   │       ├── fast-isel.ll
    │   │   │       ├── fastcall-correct-mangling.ll
    │   │   │       ├── fastcc-2.ll
    │   │   │       ├── fastcc-byval.ll
    │   │   │       ├── fastcc-sret.ll
    │   │   │       ├── fastcc.ll
    │   │   │       ├── fastcc3struct.ll
    │   │   │       ├── fastisel-gep-promote-before-add.ll
    │   │   │       ├── fastisel-softfloat.ll
    │   │   │       ├── fastmath-float-half-conversion.ll
    │   │   │       ├── fcmove.ll
    │   │   │       ├── fdiv-combine.ll
    │   │   │       ├── fdiv.ll
    │   │   │       ├── fentry-insertion.ll
    │   │   │       ├── field-extract-use-trunc.ll
    │   │   │       ├── fildll.ll
    │   │   │       ├── file-directive.ll
    │   │   │       ├── file-source-filename.ll
    │   │   │       ├── finite-libcalls.ll
    │   │   │       ├── fixed-stack-di-mir.ll
    │   │   │       ├── fixup-bw-copy.ll
    │   │   │       ├── fixup-bw-copy.mir
    │   │   │       ├── fixup-bw-inst.ll
    │   │   │       ├── fixup-bw-inst.mir
    │   │   │       ├── fixup-lea.ll
    │   │   │       ├── flags-copy-lowering.mir
    │   │   │       ├── float-asmprint.ll
    │   │   │       ├── float-conv-elim.ll
    │   │   │       ├── floor-soft-float.ll
    │   │   │       ├── fltused.ll
    │   │   │       ├── fltused_function_pointer.ll
    │   │   │       ├── fma-commute-x86.ll
    │   │   │       ├── fma-do-not-commute.ll
    │   │   │       ├── fma-fneg-combine.ll
    │   │   │       ├── fma-intrinsics-canonical.ll
    │   │   │       ├── fma-intrinsics-fast-isel.ll
    │   │   │       ├── fma-intrinsics-phi-213-to-231.ll
    │   │   │       ├── fma-intrinsics-x86-upgrade.ll
    │   │   │       ├── fma-intrinsics-x86.ll
    │   │   │       ├── fma-phi-213-to-231.ll
    │   │   │       ├── fma-scalar-combine.ll
    │   │   │       ├── fma-scalar-memfold.ll
    │   │   │       ├── fma-schedule.ll
    │   │   │       ├── fma.ll
    │   │   │       ├── fma4-commute-x86.ll
    │   │   │       ├── fma4-fneg-combine.ll
    │   │   │       ├── fma4-intrinsics-x86-upgrade.ll
    │   │   │       ├── fma4-intrinsics-x86.ll
    │   │   │       ├── fma4-intrinsics-x86_64-folded-load.ll
    │   │   │       ├── fma4-scalar-memfold.ll
    │   │   │       ├── fma4-schedule.ll
    │   │   │       ├── fma_patterns.ll
    │   │   │       ├── fma_patterns_wide.ll
    │   │   │       ├── fmaddsub-combine.ll
    │   │   │       ├── fmaxnum.ll
    │   │   │       ├── fmf-flags.ll
    │   │   │       ├── fmf-propagation.ll
    │   │   │       ├── fminnum.ll
    │   │   │       ├── fmsubadd-combine.ll
    │   │   │       ├── fmul-combines.ll
    │   │   │       ├── fnabs.ll
    │   │   │       ├── fold-add.ll
    │   │   │       ├── fold-and-shift.ll
    │   │   │       ├── fold-call-2.ll
    │   │   │       ├── fold-call-3.ll
    │   │   │       ├── fold-call-oper.ll
    │   │   │       ├── fold-call.ll
    │   │   │       ├── fold-imm.ll
    │   │   │       ├── fold-load-binops.ll
    │   │   │       ├── fold-load-unops.ll
    │   │   │       ├── fold-load-vec.ll
    │   │   │       ├── fold-load.ll
    │   │   │       ├── fold-mul-lohi.ll
    │   │   │       ├── fold-pcmpeqd-1.ll
    │   │   │       ├── fold-pcmpeqd-2.ll
    │   │   │       ├── fold-push.ll
    │   │   │       ├── fold-rmw-ops.ll
    │   │   │       ├── fold-sext-trunc.ll
    │   │   │       ├── fold-tied-op.ll
    │   │   │       ├── fold-vector-bv-crash.ll
    │   │   │       ├── fold-vector-sext-crash.ll
    │   │   │       ├── fold-vector-sext-crash2.ll
    │   │   │       ├── fold-vector-sext-zext.ll
    │   │   │       ├── fold-vector-shl-crash.ll
    │   │   │       ├── fold-vector-shuffle-crash.ll
    │   │   │       ├── fold-vector-trunc-sitofp.ll
    │   │   │       ├── fold-vex.ll
    │   │   │       ├── fold-xmm-zero.ll
    │   │   │       ├── fold-zext-trunc.ll
    │   │   │       ├── fops-windows-itanium.ll
    │   │   │       ├── force-align-stack-alloca.ll
    │   │   │       ├── force-align-stack.ll
    │   │   │       ├── fp-arith.ll
    │   │   │       ├── fp-cvt.ll
    │   │   │       ├── fp-double-rounding.ll
    │   │   │       ├── fp-elim-and-no-fp-elim.ll
    │   │   │       ├── fp-elim.ll
    │   │   │       ├── fp-fast.ll
    │   │   │       ├── fp-fold.ll
    │   │   │       ├── fp-immediate-shorten.ll
    │   │   │       ├── fp-in-intregs.ll
    │   │   │       ├── fp-intrinsics.ll
    │   │   │       ├── fp-load-trunc.ll
    │   │   │       ├── fp-logic-replace.ll
    │   │   │       ├── fp-logic.ll
    │   │   │       ├── fp-select-cmp-and.ll
    │   │   │       ├── fp-stack-2results.ll
    │   │   │       ├── fp-stack-compare-cmov.ll
    │   │   │       ├── fp-stack-compare.ll
    │   │   │       ├── fp-stack-direct-ret.ll
    │   │   │       ├── fp-stack-O0-crash.ll
    │   │   │       ├── fp-stack-O0.ll
    │   │   │       ├── fp-stack-ret-conv.ll
    │   │   │       ├── fp-stack-ret-store.ll
    │   │   │       ├── fp-stack-ret.ll
    │   │   │       ├── fp-stack-retcopy.ll
    │   │   │       ├── fp-stack-set-st1.ll
    │   │   │       ├── fp-stack.ll
    │   │   │       ├── fp-trunc.ll
    │   │   │       ├── fp-undef.ll
    │   │   │       ├── fp-une-cmp.ll
    │   │   │       ├── fp128-calling-conv.ll
    │   │   │       ├── fp128-cast.ll
    │   │   │       ├── fp128-compare.ll
    │   │   │       ├── fp128-extract.ll
    │   │   │       ├── fp128-g.ll
    │   │   │       ├── fp128-i128.ll
    │   │   │       ├── fp128-libcalls.ll
    │   │   │       ├── fp128-load.ll
    │   │   │       ├── fp128-select.ll
    │   │   │       ├── fp128-store.ll
    │   │   │       ├── fp2sint.ll
    │   │   │       ├── fp_constant_op.ll
    │   │   │       ├── fp_load_cast_fold.ll
    │   │   │       ├── fp_load_fold.ll
    │   │   │       ├── fpcmp-soft-fp.ll
    │   │   │       ├── fpstack-debuginstr-kill.ll
    │   │   │       ├── fptosi-constant.ll
    │   │   │       ├── frame-base.ll
    │   │   │       ├── frame-lowering-debug-intrinsic-2.ll
    │   │   │       ├── frame-lowering-debug-intrinsic.ll
    │   │   │       ├── frame-order.ll
    │   │   │       ├── frameaddr.ll
    │   │   │       ├── frameregister.ll
    │   │   │       ├── frem-msvc32.ll
    │   │   │       ├── fsgsbase-schedule.ll
    │   │   │       ├── fsgsbase.ll
    │   │   │       ├── fshl.ll
    │   │   │       ├── fshr.ll
    │   │   │       ├── fsxor-alignment.ll
    │   │   │       ├── ftrunc.ll
    │   │   │       ├── full-lsr.ll
    │   │   │       ├── funclet-layout.ll
    │   │   │       ├── function-alias.ll
    │   │   │       ├── function-subtarget-features-2.ll
    │   │   │       ├── function-subtarget-features.ll
    │   │   │       ├── funnel-shift-rot.ll
    │   │   │       ├── funnel-shift.ll
    │   │   │       ├── ga-offset.ll
    │   │   │       ├── ga-offset2.ll
    │   │   │       ├── gather-addresses.ll
    │   │   │       ├── gcc_except_table.ll
    │   │   │       ├── gcc_except_table_functions.ll
    │   │   │       ├── gep-expanded-vector.ll
    │   │   │       ├── getelementptr.ll
    │   │   │       ├── gfni-intrinsics.ll
    │   │   │       ├── ghc-cc.ll
    │   │   │       ├── ghc-cc64.ll
    │   │   │       ├── global-access-pie-copyrelocs.ll
    │   │   │       ├── global-access-pie.ll
    │   │   │       ├── global-fill.ll
    │   │   │       ├── global-sections-comdat.ll
    │   │   │       ├── global-sections-tls.ll
    │   │   │       ├── global-sections.ll
    │   │   │       ├── gnu-seh-nolpads.ll
    │   │   │       ├── gpr-to-mask.ll
    │   │   │       ├── greedy_regalloc_bad_eviction_sequence.ll
    │   │   │       ├── gs-fold.ll
    │   │   │       ├── h-register-addressing-32.ll
    │   │   │       ├── h-register-addressing-64.ll
    │   │   │       ├── h-register-store.ll
    │   │   │       ├── h-registers-0.ll
    │   │   │       ├── h-registers-1.ll
    │   │   │       ├── h-registers-2.ll
    │   │   │       ├── h-registers-3.ll
    │   │   │       ├── haddsub-2.ll
    │   │   │       ├── haddsub-3.ll
    │   │   │       ├── haddsub-shuf.ll
    │   │   │       ├── haddsub-undef.ll
    │   │   │       ├── haddsub.ll
    │   │   │       ├── half.ll
    │   │   │       ├── handle-move.ll
    │   │   │       ├── hhvm-cc.ll
    │   │   │       ├── hidden-vis-2.ll
    │   │   │       ├── hidden-vis-3.ll
    │   │   │       ├── hidden-vis-4.ll
    │   │   │       ├── hidden-vis-pic.ll
    │   │   │       ├── hidden-vis.ll
    │   │   │       ├── hipe-cc.ll
    │   │   │       ├── hipe-cc64.ll
    │   │   │       ├── hipe-prologue.ll
    │   │   │       ├── hoist-common.ll
    │   │   │       ├── hoist-invariant-load.ll
    │   │   │       ├── hoist-spill-lpad.ll
    │   │   │       ├── hoist-spill.ll
    │   │   │       ├── horizontal-reduce-smax.ll
    │   │   │       ├── horizontal-reduce-smin.ll
    │   │   │       ├── horizontal-reduce-umax.ll
    │   │   │       ├── horizontal-reduce-umin.ll
    │   │   │       ├── horizontal-shuffle.ll
    │   │   │       ├── huge-stack-offset.ll
    │   │   │       ├── huge-stack-offset2.ll
    │   │   │       ├── i128-and-beyond.ll
    │   │   │       ├── i128-immediate.ll
    │   │   │       ├── i128-mul.ll
    │   │   │       ├── i128-ret.ll
    │   │   │       ├── i128-sdiv.ll
    │   │   │       ├── i16lshr8pat.ll
    │   │   │       ├── i1narrowfail.ll
    │   │   │       ├── i256-add.ll
    │   │   │       ├── i2k.ll
    │   │   │       ├── i386-setjmp-pic.ll
    │   │   │       ├── i386-shrink-wrapping.ll
    │   │   │       ├── i386-tlscall-fastregalloc.ll
    │   │   │       ├── i486-fence-loop.ll
    │   │   │       ├── i64-mem-copy.ll
    │   │   │       ├── i64-to-float.ll
    │   │   │       ├── i686-win-shrink-wrapping.ll
    │   │   │       ├── iabs.ll
    │   │   │       ├── icall-branch-funnel.ll
    │   │   │       ├── icmp-opt.ll
    │   │   │       ├── ident-metadata.ll
    │   │   │       ├── ifunc-asm.ll
    │   │   │       ├── illegal-bitfield-loadstore.ll
    │   │   │       ├── illegal-insert.ll
    │   │   │       ├── illegal-vector-args-return.ll
    │   │   │       ├── immediate_merging.ll
    │   │   │       ├── immediate_merging64.ll
    │   │   │       ├── implicit-null-check-negative.ll
    │   │   │       ├── implicit-null-check.ll
    │   │   │       ├── implicit-null-checks.mir
    │   │   │       ├── implicit-null-chk-reg-rewrite.mir
    │   │   │       ├── implicit-use-spill.mir
    │   │   │       ├── imul-lea-2.ll
    │   │   │       ├── imul-lea.ll
    │   │   │       ├── imul.ll
    │   │   │       ├── inalloca-ctor.ll
    │   │   │       ├── inalloca-invoke.ll
    │   │   │       ├── inalloca-regparm.ll
    │   │   │       ├── inalloca-stdcall.ll
    │   │   │       ├── inalloca.ll
    │   │   │       ├── inconsistent_landingpad.ll
    │   │   │       ├── indirect-branch-tracking.ll
    │   │   │       ├── indirect-hidden.ll
    │   │   │       ├── init-priority.ll
    │   │   │       ├── inline-0bh.ll
    │   │   │       ├── inline-asm-2addr.ll
    │   │   │       ├── inline-asm-A-constraint.ll
    │   │   │       ├── inline-asm-avx-v-constraint-32bit.ll
    │   │   │       ├── inline-asm-avx-v-constraint.ll
    │   │   │       ├── inline-asm-avx512f-v-constraint.ll
    │   │   │       ├── inline-asm-avx512vl-v-constraint-32bit.ll
    │   │   │       ├── inline-asm-avx512vl-v-constraint.ll
    │   │   │       ├── inline-asm-bad-constraint-n.ll
    │   │   │       ├── inline-asm-bad-modifier.ll
    │   │   │       ├── inline-asm-default-clobbers.ll
    │   │   │       ├── inline-asm-duplicated-constraint.ll
    │   │   │       ├── inline-asm-error.ll
    │   │   │       ├── inline-asm-flag-clobber.ll
    │   │   │       ├── inline-asm-fpstack.ll
    │   │   │       ├── inline-asm-h.ll
    │   │   │       ├── inline-asm-modifier-n.ll
    │   │   │       ├── inline-asm-modifier-q.ll
    │   │   │       ├── inline-asm-modifier-V.ll
    │   │   │       ├── inline-asm-mrv.ll
    │   │   │       ├── inline-asm-out-regs.ll
    │   │   │       ├── inline-asm-pic.ll
    │   │   │       ├── inline-asm-ptr-cast.ll
    │   │   │       ├── inline-asm-q-regs.ll
    │   │   │       ├── inline-asm-R-constraint.ll
    │   │   │       ├── inline-asm-sp-clobber-memcpy.ll
    │   │   │       ├── inline-asm-stack-realign.ll
    │   │   │       ├── inline-asm-stack-realign2.ll
    │   │   │       ├── inline-asm-stack-realign3.ll
    │   │   │       ├── inline-asm-tied.ll
    │   │   │       ├── inline-asm-x-scalar.ll
    │   │   │       ├── inline-asm.ll
    │   │   │       ├── inline-sse.ll
    │   │   │       ├── inlineasm-sched-bug.ll
    │   │   │       ├── inreg.ll
    │   │   │       ├── ins_split_regalloc.ll
    │   │   │       ├── ins_subreg_coalesce-1.ll
    │   │   │       ├── ins_subreg_coalesce-2.ll
    │   │   │       ├── ins_subreg_coalesce-3.ll
    │   │   │       ├── insert-into-constant-vector.ll
    │   │   │       ├── insert-loaded-scalar.ll
    │   │   │       ├── insert-positions.ll
    │   │   │       ├── insert-prefetch-inline.afdo
    │   │   │       ├── insert-prefetch-inline.ll
    │   │   │       ├── insert-prefetch-invalid-instr.afdo
    │   │   │       ├── insert-prefetch-invalid-instr.ll
    │   │   │       ├── insert-prefetch-other.afdo
    │   │   │       ├── insert-prefetch.afdo
    │   │   │       ├── insert-prefetch.ll
    │   │   │       ├── insertelement-copytoregs.ll
    │   │   │       ├── insertelement-duplicates.ll
    │   │   │       ├── insertelement-legalize.ll
    │   │   │       ├── insertelement-ones.ll
    │   │   │       ├── insertelement-shuffle.ll
    │   │   │       ├── insertelement-var-index.ll
    │   │   │       ├── insertelement-zero.ll
    │   │   │       ├── insertps-combine.ll
    │   │   │       ├── insertps-from-constantpool.ll
    │   │   │       ├── insertps-O0-bug.ll
    │   │   │       ├── insertps-unfold-load-bug.ll
    │   │   │       ├── instr-symbols.mir
    │   │   │       ├── int-intrinsic.ll
    │   │   │       ├── intersect-fma-fmf.ll
    │   │   │       ├── interval-update-remat.ll
    │   │   │       ├── invalid-liveness.mir
    │   │   │       ├── invalid-shift-immediate.ll
    │   │   │       ├── invpcid-intrinsic.ll
    │   │   │       ├── ipra-inline-asm.ll
    │   │   │       ├── ipra-local-linkage.ll
    │   │   │       ├── ipra-reg-alias.ll
    │   │   │       ├── ipra-reg-usage.ll
    │   │   │       ├── ipra-transform.ll
    │   │   │       ├── is-constant.ll
    │   │   │       ├── isel-optnone.ll
    │   │   │       ├── isel-sink.ll
    │   │   │       ├── isel-sink2.ll
    │   │   │       ├── isel-sink3.ll
    │   │   │       ├── isint.ll
    │   │   │       ├── isnan.ll
    │   │   │       ├── isnan2.ll
    │   │   │       ├── ispositive.ll
    │   │   │       ├── jump_sign.ll
    │   │   │       ├── known-bits-vector.ll
    │   │   │       ├── known-bits.ll
    │   │   │       ├── known-signbits-vector.ll
    │   │   │       ├── kshift.ll
    │   │   │       ├── label-annotation.ll
    │   │   │       ├── label-redefinition.ll
    │   │   │       ├── lack-of-signed-truncation-check.ll
    │   │   │       ├── lakemont.ll
    │   │   │       ├── large-code-model-isel.ll
    │   │   │       ├── large-constants.ll
    │   │   │       ├── large-gep-chain.ll
    │   │   │       ├── large-gep-scale.ll
    │   │   │       ├── large-global.ll
    │   │   │       ├── large-pic-string.ll
    │   │   │       ├── late-address-taken.ll
    │   │   │       ├── late-remat-update-2.mir
    │   │   │       ├── late-remat-update.mir
    │   │   │       ├── ldzero.ll
    │   │   │       ├── lea-2.ll
    │   │   │       ├── lea-3.ll
    │   │   │       ├── lea-4.ll
    │   │   │       ├── lea-5.ll
    │   │   │       ├── lea-opt-cse1.ll
    │   │   │       ├── lea-opt-cse2.ll
    │   │   │       ├── lea-opt-cse3.ll
    │   │   │       ├── lea-opt-cse4.ll
    │   │   │       ├── lea-opt-memop-check-1.ll
    │   │   │       ├── lea-opt-memop-check-2.ll
    │   │   │       ├── lea-opt-with-debug.mir
    │   │   │       ├── lea-opt.ll
    │   │   │       ├── lea-recursion.ll
    │   │   │       ├── lea.ll
    │   │   │       ├── lea32-schedule.ll
    │   │   │       ├── lea64-schedule.ll
    │   │   │       ├── leaf-fp-elim.ll
    │   │   │       ├── leaFixup32.mir
    │   │   │       ├── leaFixup64.mir
    │   │   │       ├── legalize-fmp-oeq-vector-select.ll
    │   │   │       ├── legalize-libcalls.ll
    │   │   │       ├── legalize-shift-64.ll
    │   │   │       ├── legalize-shift.ll
    │   │   │       ├── legalize-shl-vec.ll
    │   │   │       ├── legalize-sub-zero-2.ll
    │   │   │       ├── legalize-sub-zero.ll
    │   │   │       ├── legalize-types-remapid.ll
    │   │   │       ├── legalizedag_vec.ll
    │   │   │       ├── libcall-sret.ll
    │   │   │       ├── licm-dominance.ll
    │   │   │       ├── licm-nested.ll
    │   │   │       ├── licm-regpressure.ll
    │   │   │       ├── licm-symbol.ll
    │   │   │       ├── limit-split-cost.mir
    │   │   │       ├── limited-prec.ll
    │   │   │       ├── linux-preemption.ll
    │   │   │       ├── lit.local.cfg
    │   │   │       ├── live-out-reg-info.ll
    │   │   │       ├── live-range-nosubreg.ll
    │   │   │       ├── liveness-local-regalloc.ll
    │   │   │       ├── llc-override-mcpu-mattr.ll
    │   │   │       ├── llc-print-machineinstrs.mir
    │   │   │       ├── llc-start-stop-instance.ll
    │   │   │       ├── load-combine-dbg.ll
    │   │   │       ├── load-combine.ll
    │   │   │       ├── load-scalar-as-vector.ll
    │   │   │       ├── load-slice.ll
    │   │   │       ├── loadStore_vectorizer.ll
    │   │   │       ├── loc-remat.ll
    │   │   │       ├── local_stack_symbol_ordering.ll
    │   │   │       ├── localescape.ll
    │   │   │       ├── log2_not_readnone.ll
    │   │   │       ├── logical-load-fold.ll
    │   │   │       ├── long-setcc.ll
    │   │   │       ├── longlong-deadload.ll
    │   │   │       ├── loop-blocks.ll
    │   │   │       ├── loop-hoist.ll
    │   │   │       ├── loop-search.ll
    │   │   │       ├── loop-strength-reduce-2.ll
    │   │   │       ├── loop-strength-reduce-3.ll
    │   │   │       ├── loop-strength-reduce-crash.ll
    │   │   │       ├── loop-strength-reduce.ll
    │   │   │       ├── loop-strength-reduce2.ll
    │   │   │       ├── loop-strength-reduce4.ll
    │   │   │       ├── loop-strength-reduce5.ll
    │   │   │       ├── loop-strength-reduce6.ll
    │   │   │       ├── loop-strength-reduce7.ll
    │   │   │       ├── loop-strength-reduce8.ll
    │   │   │       ├── lower-bitcast.ll
    │   │   │       ├── lower-vec-shift-2.ll
    │   │   │       ├── lower-vec-shift.ll
    │   │   │       ├── lower-vec-shuffle-bug.ll
    │   │   │       ├── lrshrink.ll
    │   │   │       ├── lsr-crash-empty-uses.ll
    │   │   │       ├── lsr-delayed-fold.ll
    │   │   │       ├── lsr-i386.ll
    │   │   │       ├── lsr-interesting-step.ll
    │   │   │       ├── lsr-loop-exit-cond.ll
    │   │   │       ├── lsr-negative-stride.ll
    │   │   │       ├── lsr-nonaffine.ll
    │   │   │       ├── lsr-normalization.ll
    │   │   │       ├── lsr-overflow.ll
    │   │   │       ├── lsr-quadratic-expand.ll
    │   │   │       ├── lsr-redundant-addressing.ll
    │   │   │       ├── lsr-reuse-trunc.ll
    │   │   │       ├── lsr-reuse.ll
    │   │   │       ├── lsr-sort.ll
    │   │   │       ├── lsr-static-addr.ll
    │   │   │       ├── lsr-wrap.ll
    │   │   │       ├── lwp-intrinsics-x86_64.ll
    │   │   │       ├── lwp-intrinsics.ll
    │   │   │       ├── lwp-schedule.ll
    │   │   │       ├── lzcnt-schedule.ll
    │   │   │       ├── lzcnt-tzcnt.ll
    │   │   │       ├── lzcnt-zext-cmp.ll
    │   │   │       ├── lzcnt.ll
    │   │   │       ├── machine-combiner-int-vec.ll
    │   │   │       ├── machine-combiner-int.ll
    │   │   │       ├── machine-combiner.ll
    │   │   │       ├── machine-copy-prop.mir
    │   │   │       ├── machine-cp-debug.mir
    │   │   │       ├── machine-cp.ll
    │   │   │       ├── machine-cse.ll
    │   │   │       ├── machine-outliner-debuginfo.ll
    │   │   │       ├── machine-outliner-disubprogram.ll
    │   │   │       ├── machine-outliner-noredzone.ll
    │   │   │       ├── machine-outliner-tailcalls.ll
    │   │   │       ├── machine-outliner.ll
    │   │   │       ├── machine-region-info.mir
    │   │   │       ├── machine-sink-and-implicit-null-checks.ll
    │   │   │       ├── machine-sink.ll
    │   │   │       ├── machine-trace-metrics-crash.ll
    │   │   │       ├── MachineBranchProb.ll
    │   │   │       ├── MachineSink-CritEdge.ll
    │   │   │       ├── MachineSink-DbgValue.ll
    │   │   │       ├── MachineSink-eflags.ll
    │   │   │       ├── machinesink-merge-debuginfo.ll
    │   │   │       ├── machinesink-null-debuginfo.ll
    │   │   │       ├── MachineSink-PHIUse.ll
    │   │   │       ├── MachineSink-SubReg.ll
    │   │   │       ├── macho-comdat.ll
    │   │   │       ├── macho-trap.ll
    │   │   │       ├── madd.ll
    │   │   │       ├── mangle-question-mark.ll
    │   │   │       ├── mask-negated-bool.ll
    │   │   │       ├── masked-iv-safe.ll
    │   │   │       ├── masked-iv-unsafe.ll
    │   │   │       ├── masked_gather.ll
    │   │   │       ├── masked_gather_scatter.ll
    │   │   │       ├── masked_gather_scatter_widen.ll
    │   │   │       ├── masked_load.ll
    │   │   │       ├── masked_store.ll
    │   │   │       ├── maskmovdqu.ll
    │   │   │       ├── materialize.ll
    │   │   │       ├── mature-mc-support.ll
    │   │   │       ├── mbp-false-cfg-break.ll
    │   │   │       ├── mcinst-avx-lowering.ll
    │   │   │       ├── mcinst-lowering.ll
    │   │   │       ├── mcu-abi.ll
    │   │   │       ├── mem-intrin-base-reg.ll
    │   │   │       ├── mem-promote-integers.ll
    │   │   │       ├── membarrier.ll
    │   │   │       ├── memcmp-mergeexpand.ll
    │   │   │       ├── memcmp-minsize.ll
    │   │   │       ├── memcmp-optsize.ll
    │   │   │       ├── memcmp.ll
    │   │   │       ├── memcpy-2.ll
    │   │   │       ├── memcpy-from-string.ll
    │   │   │       ├── memcpy-struct-by-value.ll
    │   │   │       ├── memcpy.ll
    │   │   │       ├── mempcpy-32.ll
    │   │   │       ├── mempcpy.ll
    │   │   │       ├── memset-2.ll
    │   │   │       ├── memset-3.ll
    │   │   │       ├── memset-nonzero.ll
    │   │   │       ├── memset-sse-stack-realignment.ll
    │   │   │       ├── memset-zero.ll
    │   │   │       ├── memset.ll
    │   │   │       ├── memset64-on-x86-32.ll
    │   │   │       ├── merge-consecutive-loads-128.ll
    │   │   │       ├── merge-consecutive-loads-256.ll
    │   │   │       ├── merge-consecutive-loads-512.ll
    │   │   │       ├── merge-consecutive-stores-i1.ll
    │   │   │       ├── merge-consecutive-stores.ll
    │   │   │       ├── merge-sp-update-lea.ll
    │   │   │       ├── merge-sp-updates-cfi.ll
    │   │   │       ├── merge-store-constants.ll
    │   │   │       ├── merge-store-partially-alias-loads.ll
    │   │   │       ├── merge-vector-stores-scale-idx-crash.ll
    │   │   │       ├── merge_store.ll
    │   │   │       ├── merge_store_duplicated_loads.ll
    │   │   │       ├── MergeConsecutiveStores.ll
    │   │   │       ├── mfence.ll
    │   │   │       ├── min-legal-vector-width.ll
    │   │   │       ├── mingw-alloca.ll
    │   │   │       ├── mingw-comdats-xdata.ll
    │   │   │       ├── mingw-comdats.ll
    │   │   │       ├── mingw-refptr.ll
    │   │   │       ├── misaligned-memset.ll
    │   │   │       ├── misched-aa-colored.ll
    │   │   │       ├── misched-aa-mmos.ll
    │   │   │       ├── misched-balance.ll
    │   │   │       ├── misched-code-difference-with-debug.ll
    │   │   │       ├── misched-copy.ll
    │   │   │       ├── misched-crash.ll
    │   │   │       ├── misched-fusion.ll
    │   │   │       ├── misched-ilp.ll
    │   │   │       ├── misched-matmul.ll
    │   │   │       ├── misched-matrix.ll
    │   │   │       ├── misched-new.ll
    │   │   │       ├── misched_phys_reg_assign_order.ll
    │   │   │       ├── mmx-arg-passing-x86-64.ll
    │   │   │       ├── mmx-arg-passing.ll
    │   │   │       ├── mmx-arith.ll
    │   │   │       ├── mmx-bitcast-fold.ll
    │   │   │       ├── mmx-bitcast.ll
    │   │   │       ├── mmx-build-vector.ll
    │   │   │       ├── mmx-coalescing.ll
    │   │   │       ├── mmx-copy-gprs.ll
    │   │   │       ├── mmx-cvt.ll
    │   │   │       ├── mmx-fold-load.ll
    │   │   │       ├── mmx-fold-zero.ll
    │   │   │       ├── mmx-intrinsics.ll
    │   │   │       ├── mmx-only.ll
    │   │   │       ├── mmx-schedule.ll
    │   │   │       ├── mod128.ll
    │   │   │       ├── movbe-schedule.ll
    │   │   │       ├── movbe.ll
    │   │   │       ├── movddup-load-fold.ll
    │   │   │       ├── movdir-intrinsic-x86.ll
    │   │   │       ├── movdir-intrinsic-x86_64.ll
    │   │   │       ├── movfs.ll
    │   │   │       ├── movgs.ll
    │   │   │       ├── movmsk-cmp.ll
    │   │   │       ├── movmsk.ll
    │   │   │       ├── movntdq-no-avx.ll
    │   │   │       ├── movpc32-check.ll
    │   │   │       ├── movtopush.ll
    │   │   │       ├── movtopush.mir
    │   │   │       ├── movtopush64.ll
    │   │   │       ├── ms-inline-asm-avx512.ll
    │   │   │       ├── ms-inline-asm-redundant-clobber.ll
    │   │   │       ├── ms-inline-asm.ll
    │   │   │       ├── mul-constant-i16.ll
    │   │   │       ├── mul-constant-i32.ll
    │   │   │       ├── mul-constant-i64.ll
    │   │   │       ├── mul-constant-i8.ll
    │   │   │       ├── mul-constant-result.ll
    │   │   │       ├── mul-i1024.ll
    │   │   │       ├── mul-i256.ll
    │   │   │       ├── mul-i512.ll
    │   │   │       ├── mul-legalize.ll
    │   │   │       ├── mul-remat.ll
    │   │   │       ├── mul-shift-reassoc.ll
    │   │   │       ├── mul128.ll
    │   │   │       ├── mul128_sext_loop.ll
    │   │   │       ├── mul64.ll
    │   │   │       ├── muloti.ll
    │   │   │       ├── mult-alt-generic-i686.ll
    │   │   │       ├── mult-alt-generic-x86_64.ll
    │   │   │       ├── mult-alt-x86.ll
    │   │   │       ├── multiple-loop-post-inc.ll
    │   │   │       ├── multiple-return-values-cross-block.ll
    │   │   │       ├── mulvi32.ll
    │   │   │       ├── mulx32.ll
    │   │   │       ├── mulx64.ll
    │   │   │       ├── musttail-fastcall.ll
    │   │   │       ├── musttail-indirect.ll
    │   │   │       ├── musttail-thiscall.ll
    │   │   │       ├── musttail-varargs.ll
    │   │   │       ├── musttail.ll
    │   │   │       ├── mwaitx-schedule.ll
    │   │   │       ├── mwaitx.ll
    │   │   │       ├── named-reg-alloc.ll
    │   │   │       ├── named-reg-notareg.ll
    │   │   │       ├── nancvt.ll
    │   │   │       ├── narrow-shl-cst.ll
    │   │   │       ├── narrow-shl-load.ll
    │   │   │       ├── narrow_op-1.ll
    │   │   │       ├── neg-shl-add.ll
    │   │   │       ├── neg_cmp.ll
    │   │   │       ├── neg_fp.ll
    │   │   │       ├── negate-add-zero.ll
    │   │   │       ├── negate-i1.ll
    │   │   │       ├── negate-shift.ll
    │   │   │       ├── negate.ll
    │   │   │       ├── negative-offset.ll
    │   │   │       ├── negative-sin.ll
    │   │   │       ├── negative-stride-fptosi-user.ll
    │   │   │       ├── negative-subscript.ll
    │   │   │       ├── negative_zero.ll
    │   │   │       ├── new-remat.ll
    │   │   │       ├── newline-and-quote.ll
    │   │   │       ├── no-and8ri8.ll
    │   │   │       ├── no-cmov.ll
    │   │   │       ├── no-plt-libcalls.ll
    │   │   │       ├── no-plt.ll
    │   │   │       ├── no-prolog-kill.ll
    │   │   │       ├── no-sse2-avg.ll
    │   │   │       ├── no-stack-arg-probe.ll
    │   │   │       ├── nobt.ll
    │   │   │       ├── nocf_check.ll
    │   │   │       ├── nocx16.ll
    │   │   │       ├── non-lazy-bind.ll
    │   │   │       ├── non-unique-sections.ll
    │   │   │       ├── non-value-mem-operand.mir
    │   │   │       ├── nonconst-static-ev.ll
    │   │   │       ├── nonconst-static-iv.ll
    │   │   │       ├── nontemporal-2.ll
    │   │   │       ├── nontemporal-loads.ll
    │   │   │       ├── nontemporal.ll
    │   │   │       ├── noreturn-call.ll
    │   │   │       ├── norex-subreg.ll
    │   │   │       ├── nosse-error1.ll
    │   │   │       ├── nosse-error2.ll
    │   │   │       ├── nosse-varargs.ll
    │   │   │       ├── nosse-vector.ll
    │   │   │       ├── not-and-simplify.ll
    │   │   │       ├── note-cet-property.ll
    │   │   │       ├── note-sections.ll
    │   │   │       ├── null-streamer.ll
    │   │   │       ├── O0-pipeline.ll
    │   │   │       ├── O3-pipeline.ll
    │   │   │       ├── objc-gc-module-flags.ll
    │   │   │       ├── object-size.ll
    │   │   │       ├── oddshuffles.ll
    │   │   │       ├── opaque-constant-asm.ll
    │   │   │       ├── opt-ext-uses.ll
    │   │   │       ├── opt-shuff-tstore.ll
    │   │   │       ├── opt_phis.mir
    │   │   │       ├── opt_phis2.mir
    │   │   │       ├── optimize-max-0.ll
    │   │   │       ├── optimize-max-1.ll
    │   │   │       ├── optimize-max-2.ll
    │   │   │       ├── optimize-max-3.ll
    │   │   │       ├── or-address.ll
    │   │   │       ├── or-branch.ll
    │   │   │       ├── or-lea.ll
    │   │   │       ├── osx-private-labels.ll
    │   │   │       ├── overflow-intrinsic-setcc-fold.ll
    │   │   │       ├── overflow.ll
    │   │   │       ├── overlap-shift.ll
    │   │   │       ├── packed_struct.ll
    │   │   │       ├── packss.ll
    │   │   │       ├── paddus.ll
    │   │   │       ├── palignr.ll
    │   │   │       ├── parity.ll
    │   │   │       ├── partial-fold32.ll
    │   │   │       ├── partial-fold64.ll
    │   │   │       ├── pass-three.ll
    │   │   │       ├── patchable-prologue.ll
    │   │   │       ├── patchpoint-invoke.ll
    │   │   │       ├── patchpoint-verifiable.mir
    │   │   │       ├── patchpoint-webkit_jscc.ll
    │   │   │       ├── patchpoint.ll
    │   │   │       ├── pause.ll
    │   │   │       ├── peep-setb.ll
    │   │   │       ├── peep-test-0.ll
    │   │   │       ├── peep-test-1.ll
    │   │   │       ├── peep-test-2.ll
    │   │   │       ├── peep-test-3.ll
    │   │   │       ├── peep-test-4.ll
    │   │   │       ├── peephole-cvt-sse.ll
    │   │   │       ├── peephole-fold-movsd.ll
    │   │   │       ├── peephole-multiple-folds.ll
    │   │   │       ├── peephole-na-phys-copy-folding.ll
    │   │   │       ├── peephole-recurrence.mir
    │   │   │       ├── peephole.mir
    │   │   │       ├── personality.ll
    │   │   │       ├── personality_size.ll
    │   │   │       ├── phaddsub-extract.ll
    │   │   │       ├── phaddsub-undef.ll
    │   │   │       ├── phaddsub.ll
    │   │   │       ├── phi-bit-propagation.ll
    │   │   │       ├── phi-immediate-factoring.ll
    │   │   │       ├── phielim-split.ll
    │   │   │       ├── phys-reg-local-regalloc.ll
    │   │   │       ├── phys_subreg_coalesce-2.ll
    │   │   │       ├── phys_subreg_coalesce-3.ll
    │   │   │       ├── phys_subreg_coalesce.ll
    │   │   │       ├── physreg-pairs-error.ll
    │   │   │       ├── physreg-pairs.ll
    │   │   │       ├── pic-load-remat.ll
    │   │   │       ├── pic.ll
    │   │   │       ├── pic_jumptable.ll
    │   │   │       ├── pie.ll
    │   │   │       ├── pku.ll
    │   │   │       ├── pmaddubsw.ll
    │   │   │       ├── pmovext.ll
    │   │   │       ├── pmovsx-inreg.ll
    │   │   │       ├── pmul.ll
    │   │   │       ├── pmulh.ll
    │   │   │       ├── pmulld.ll
    │   │   │       ├── pointer-vector.ll
    │   │   │       ├── pop-stack-cleanup-msvc.ll
    │   │   │       ├── pop-stack-cleanup.ll
    │   │   │       ├── popcnt-schedule.ll
    │   │   │       ├── popcnt.ll
    │   │   │       ├── post-ra-sched-with-debug.mir
    │   │   │       ├── post-ra-sched.ll
    │   │   │       ├── postalloc-coalescing.ll
    │   │   │       ├── postra-ignore-dbg-instrs.mir
    │   │   │       ├── postra-licm.ll
    │   │   │       ├── pow.ll
    │   │   │       ├── powi.ll
    │   │   │       ├── pr10068.ll
    │   │   │       ├── pr10475.ll
    │   │   │       ├── pr10499.ll
    │   │   │       ├── pr10523.ll
    │   │   │       ├── pr10524.ll
    │   │   │       ├── pr10525.ll
    │   │   │       ├── pr10526.ll
    │   │   │       ├── pr11202.ll
    │   │   │       ├── pr11334.ll
    │   │   │       ├── pr11415.ll
    │   │   │       ├── pr11468.ll
    │   │   │       ├── pr11985.ll
    │   │   │       ├── pr11998.ll
    │   │   │       ├── pr12360.ll
    │   │   │       ├── pr12889.ll
    │   │   │       ├── pr13209.ll
    │   │   │       ├── pr13220.ll
    │   │   │       ├── pr13458.ll
    │   │   │       ├── pr13577.ll
    │   │   │       ├── pr13859.ll
    │   │   │       ├── pr13899.ll
    │   │   │       ├── pr14088.ll
    │   │   │       ├── pr14098.ll
    │   │   │       ├── pr14161.ll
    │   │   │       ├── pr14204.ll
    │   │   │       ├── pr14314.ll
    │   │   │       ├── pr14333.ll
    │   │   │       ├── pr14562.ll
    │   │   │       ├── pr1462.ll
    │   │   │       ├── pr1489.ll
    │   │   │       ├── pr1505.ll
    │   │   │       ├── pr1505b.ll
    │   │   │       ├── pr15267.ll
    │   │   │       ├── pr15296.ll
    │   │   │       ├── pr15309.ll
    │   │   │       ├── pr15705.ll
    │   │   │       ├── pr15981.ll
    │   │   │       ├── pr16031.ll
    │   │   │       ├── pr16360.ll
    │   │   │       ├── pr16807.ll
    │   │   │       ├── pr17546.ll
    │   │   │       ├── pr17631.ll
    │   │   │       ├── pr17764.ll
    │   │   │       ├── pr18014.ll
    │   │   │       ├── pr18054.ll
    │   │   │       ├── pr18162.ll
    │   │   │       ├── pr18344.ll
    │   │   │       ├── pr18846.ll
    │   │   │       ├── pr19049.ll
    │   │   │       ├── pr20011.ll
    │   │   │       ├── pr20012.ll
    │   │   │       ├── pr20020.ll
    │   │   │       ├── pr20088.ll
    │   │   │       ├── pr21099.ll
    │   │   │       ├── pr2177.ll
    │   │   │       ├── pr21792.ll
    │   │   │       ├── pr2182.ll
    │   │   │       ├── pr22019.ll
    │   │   │       ├── pr22103.ll
    │   │   │       ├── pr22338.ll
    │   │   │       ├── pr22774.ll
    │   │   │       ├── pr22970.ll
    │   │   │       ├── pr23103.ll
    │   │   │       ├── pr23246.ll
    │   │   │       ├── pr2326.ll
    │   │   │       ├── pr23273.ll
    │   │   │       ├── pr23603.ll
    │   │   │       ├── pr23664.ll
    │   │   │       ├── pr24139.ll
    │   │   │       ├── pr24374.ll
    │   │   │       ├── pr24602.ll
    │   │   │       ├── pr25828.ll
    │   │   │       ├── pr2585.ll
    │   │   │       ├── pr26350.ll
    │   │   │       ├── pr2656.ll
    │   │   │       ├── pr2659.ll
    │   │   │       ├── pr26625.ll
    │   │   │       ├── pr26652.ll
    │   │   │       ├── pr26757.ll
    │   │   │       ├── pr26835.ll
    │   │   │       ├── pr26870.ll
    │   │   │       ├── pr27071.ll
    │   │   │       ├── pr27501.ll
    │   │   │       ├── pr27591.ll
    │   │   │       ├── pr27681.mir
    │   │   │       ├── pr28129.ll
    │   │   │       ├── pr28173.ll
    │   │   │       ├── pr28444.ll
    │   │   │       ├── pr28472.ll
    │   │   │       ├── pr28489.ll
    │   │   │       ├── pr2849.ll
    │   │   │       ├── pr28504.ll
    │   │   │       ├── pr28515.ll
    │   │   │       ├── pr28560.ll
    │   │   │       ├── pr28824.ll
    │   │   │       ├── pr29010.ll
    │   │   │       ├── pr29022.ll
    │   │   │       ├── pr29061.ll
    │   │   │       ├── pr29112.ll
    │   │   │       ├── pr29170.ll
    │   │   │       ├── pr29222.ll
    │   │   │       ├── pr2924.ll
    │   │   │       ├── pr2982.ll
    │   │   │       ├── pr30284.ll
    │   │   │       ├── pr30290.ll
    │   │   │       ├── pr30430.ll
    │   │   │       ├── pr30511.ll
    │   │   │       ├── pr30562.ll
    │   │   │       ├── pr30813.ll
    │   │   │       ├── pr30821.mir
    │   │   │       ├── pr31045.ll
    │   │   │       ├── pr31088.ll
    │   │   │       ├── pr31143.ll
    │   │   │       ├── pr31242.ll
    │   │   │       ├── pr31271.ll
    │   │   │       ├── pr31323.ll
    │   │   │       ├── pr3154.ll
    │   │   │       ├── pr31593.ll
    │   │   │       ├── pr31773.ll
    │   │   │       ├── pr31956.ll
    │   │   │       ├── pr32108.ll
    │   │   │       ├── pr3216.ll
    │   │   │       ├── pr32241.ll
    │   │   │       ├── pr32256.ll
    │   │   │       ├── pr32278.ll
    │   │   │       ├── pr32282.ll
    │   │   │       ├── pr32284.ll
    │   │   │       ├── pr32329.ll
    │   │   │       ├── pr32340.ll
    │   │   │       ├── pr32345.ll
    │   │   │       ├── pr32368.ll
    │   │   │       ├── pr3241.ll
    │   │   │       ├── pr32420.ll
    │   │   │       ├── pr3243.ll
    │   │   │       ├── pr3244.ll
    │   │   │       ├── pr32451.ll
    │   │   │       ├── pr32484.ll
    │   │   │       ├── pr3250.ll
    │   │   │       ├── pr32515.ll
    │   │   │       ├── pr32588.ll
    │   │   │       ├── pr32610.ll
    │   │   │       ├── pr32659.ll
    │   │   │       ├── pr32907.ll
    │   │   │       ├── pr3317.ll
    │   │   │       ├── pr33290.ll
    │   │   │       ├── pr33349.ll
    │   │   │       ├── pr33396.ll
    │   │   │       ├── pr3366.ll
    │   │   │       ├── pr33715.ll
    │   │   │       ├── pr33747.ll
    │   │   │       ├── pr33772.ll
    │   │   │       ├── pr33828.ll
    │   │   │       ├── pr33844.ll
    │   │   │       ├── pr33954.ll
    │   │   │       ├── pr33960.ll
    │   │   │       ├── pr34080-2.ll
    │   │   │       ├── pr34080.ll
    │   │   │       ├── pr34088.ll
    │   │   │       ├── pr34137.ll
    │   │   │       ├── pr34139.ll
    │   │   │       ├── pr34149.ll
    │   │   │       ├── pr34177.ll
    │   │   │       ├── pr34271-1.ll
    │   │   │       ├── pr34271.ll
    │   │   │       ├── pr34381.ll
    │   │   │       ├── pr34397.ll
    │   │   │       ├── pr34421.ll
    │   │   │       ├── PR34565.ll
    │   │   │       ├── pr3457.ll
    │   │   │       ├── pr34592.ll
    │   │   │       ├── pr34605.ll
    │   │   │       ├── pr34629.ll
    │   │   │       ├── pr34634.ll
    │   │   │       ├── pr34653.ll
    │   │   │       ├── pr34657.ll
    │   │   │       ├── pr34855.ll
    │   │   │       ├── pr3522.ll
    │   │   │       ├── pr35272.ll
    │   │   │       ├── pr35316.ll
    │   │   │       ├── pr35399.ll
    │   │   │       ├── pr35443.ll
    │   │   │       ├── pr35636.ll
    │   │   │       ├── pr35761.ll
    │   │   │       ├── pr35763.ll
    │   │   │       ├── pr35765.ll
    │   │   │       ├── pr35918.ll
    │   │   │       ├── pr35972.ll
    │   │   │       ├── pr35982.ll
    │   │   │       ├── pr36199.ll
    │   │   │       ├── pr36274.ll
    │   │   │       ├── pr36312.ll
    │   │   │       ├── pr36553.ll
    │   │   │       ├── pr36602.ll
    │   │   │       ├── pr36865.ll
    │   │   │       ├── pr37063.ll
    │   │   │       ├── pr37264.ll
    │   │   │       ├── PR37310.mir
    │   │   │       ├── pr37359.ll
    │   │   │       ├── pr37499.ll
    │   │   │       ├── pr37820.ll
    │   │   │       ├── pr37826.ll
    │   │   │       ├── pr37879.ll
    │   │   │       ├── pr37916.ll
    │   │   │       ├── pr38038.ll
    │   │   │       ├── pr38185.ll
    │   │   │       ├── pr38217.ll
    │   │   │       ├── pr38533.ll
    │   │   │       ├── pr38539.ll
    │   │   │       ├── pr38639.ll
    │   │   │       ├── pr38738.ll
    │   │   │       ├── pr38743.ll
    │   │   │       ├── pr38762.ll
    │   │   │       ├── pr38763.ll
    │   │   │       ├── pr38795.ll
    │   │   │       ├── pr38803.ll
    │   │   │       ├── pr38819.ll
    │   │   │       ├── pr38865-2.ll
    │   │   │       ├── pr38865-3.ll
    │   │   │       ├── pr38865.ll
    │   │   │       ├── pr38952.mir
    │   │   │       ├── pr39187-g.ll
    │   │   │       ├── pr39243.ll
    │   │   │       ├── pr39733.ll
    │   │   │       ├── pr39896.ll
    │   │   │       ├── pr39926.ll
    │   │   │       ├── pr40090.ll
    │   │   │       ├── pr40289-64bit.ll
    │   │   │       ├── pr40289.ll
    │   │   │       ├── pr40529.ll
    │   │   │       ├── pr5145.ll
    │   │   │       ├── pr7882.ll
    │   │   │       ├── pr9127.ll
    │   │   │       ├── pr9517.ll
    │   │   │       ├── pr9743.ll
    │   │   │       ├── pre-coalesce-2.ll
    │   │   │       ├── pre-coalesce.ll
    │   │   │       ├── pre-coalesce.mir
    │   │   │       ├── pre-ra-sched.ll
    │   │   │       ├── prefer-avx256-lzcnt.ll
    │   │   │       ├── prefer-avx256-mask-extend.ll
    │   │   │       ├── prefer-avx256-mask-shuffle.ll
    │   │   │       ├── prefer-avx256-popcnt.ll
    │   │   │       ├── prefer-avx256-shift.ll
    │   │   │       ├── prefer-avx256-trunc.ll
    │   │   │       ├── prefer-avx256-wide-mul.ll
    │   │   │       ├── prefetch.ll
    │   │   │       ├── prefixdata.ll
    │   │   │       ├── preserve_allcc64.ll
    │   │   │       ├── preserve_mostcc64.ll
    │   │   │       ├── private-2.ll
    │   │   │       ├── private.ll
    │   │   │       ├── prolog-push-seq.ll
    │   │   │       ├── prologue-epilogue-remarks.mir
    │   │   │       ├── prologuedata.ll
    │   │   │       ├── promote-assert-zext.ll
    │   │   │       ├── promote-i16.ll
    │   │   │       ├── promote-trunc.ll
    │   │   │       ├── promote-vec3.ll
    │   │   │       ├── promote.ll
    │   │   │       ├── ps4-noreturn.ll
    │   │   │       ├── pseudo_cmov_lower.ll
    │   │   │       ├── pseudo_cmov_lower1.ll
    │   │   │       ├── pseudo_cmov_lower2.ll
    │   │   │       ├── pshufb-mask-comments.ll
    │   │   │       ├── pshufd-combine-crash.ll
    │   │   │       ├── psubus.ll
    │   │   │       ├── ptest.ll
    │   │   │       ├── ptr-rotate.ll
    │   │   │       ├── ptrtoint-constexpr.ll
    │   │   │       ├── ptwrite32-intrinsic.ll
    │   │   │       ├── ptwrite64-intrinsic.ll
    │   │   │       ├── push-cfi-debug.ll
    │   │   │       ├── push-cfi-obj.ll
    │   │   │       ├── push-cfi.ll
    │   │   │       ├── ragreedy-bug.ll
    │   │   │       ├── ragreedy-hoist-spill.ll
    │   │   │       ├── ragreedy-last-chance-recoloring.ll
    │   │   │       ├── rd-mod-wr-eflags.ll
    │   │   │       ├── rdpid-schedule.ll
    │   │   │       ├── rdpid.ll
    │   │   │       ├── rdpmc.ll
    │   │   │       ├── rdrand-schedule.ll
    │   │   │       ├── rdrand-x86_64.ll
    │   │   │       ├── rdrand.ll
    │   │   │       ├── rdseed-schedule.ll
    │   │   │       ├── rdseed-x86_64.ll
    │   │   │       ├── rdseed.ll
    │   │   │       ├── rdtsc-upgrade.ll
    │   │   │       ├── rdtsc.ll
    │   │   │       ├── read-fp-no-frame-pointer.ll
    │   │   │       ├── recip-fastmath.ll
    │   │   │       ├── recip-fastmath2.ll
    │   │   │       ├── recip-pic.ll
    │   │   │       ├── red-zone.ll
    │   │   │       ├── red-zone2.ll
    │   │   │       ├── reduce-trunc-shl.ll
    │   │   │       ├── regalloc-advanced-split-cost.ll
    │   │   │       ├── regalloc-reconcile-broken-hints.ll
    │   │   │       ├── regalloc-spill-at-ehpad.ll
    │   │   │       ├── regcall-no-plt.ll
    │   │   │       ├── reghinting.ll
    │   │   │       ├── regparm.ll
    │   │   │       ├── regpressure.ll
    │   │   │       ├── rem.ll
    │   │   │       ├── rem_crash.ll
    │   │   │       ├── remat-constant.ll
    │   │   │       ├── remat-fold-load.ll
    │   │   │       ├── remat-mov-0.ll
    │   │   │       ├── remat-phys-dead.ll
    │   │   │       ├── remat-scalar-zero.ll
    │   │   │       ├── replace-load-and-with-bzhi.ll
    │   │   │       ├── replace_unsupported_masked_mem_intrin.ll
    │   │   │       ├── ret-addr.ll
    │   │   │       ├── ret-i64-0.ll
    │   │   │       ├── ret-mmx.ll
    │   │   │       ├── retpoline-external.ll
    │   │   │       ├── retpoline-regparm.ll
    │   │   │       ├── retpoline.ll
    │   │   │       ├── return-ext.ll
    │   │   │       ├── return_zeroext_i2.ll
    │   │   │       ├── returned-trunc-tail-calls.ll
    │   │   │       ├── reverse_branches.ll
    │   │   │       ├── rip-rel-address.ll
    │   │   │       ├── rip-rel-lea.ll
    │   │   │       ├── rodata-relocs.ll
    │   │   │       ├── rot16.ll
    │   │   │       ├── rot32.ll
    │   │   │       ├── rot64.ll
    │   │   │       ├── rotate-extract-vector.ll
    │   │   │       ├── rotate-extract.ll
    │   │   │       ├── rotate.ll
    │   │   │       ├── rotate2.ll
    │   │   │       ├── rotate4.ll
    │   │   │       ├── rotate_vec.ll
    │   │   │       ├── rounding-ops.ll
    │   │   │       ├── rrlist-livereg-corrutpion.ll
    │   │   │       ├── rtm-schedule.ll
    │   │   │       ├── rtm.ll
    │   │   │       ├── sad.ll
    │   │   │       ├── sad_variations.ll
    │   │   │       ├── sadd_sat.ll
    │   │   │       ├── sadd_sat_vec.ll
    │   │   │       ├── saddo-redundant-add.ll
    │   │   │       ├── safestack.ll
    │   │   │       ├── safestack_inline.ll
    │   │   │       ├── safestack_ssp.ll
    │   │   │       ├── sandybridge-loads.ll
    │   │   │       ├── sar_fold.ll
    │   │   │       ├── sar_fold64.ll
    │   │   │       ├── sat-add.ll
    │   │   │       ├── sbb.ll
    │   │   │       ├── scalar-extract.ll
    │   │   │       ├── scalar-fp-to-i64.ll
    │   │   │       ├── scalar-int-to-fp.ll
    │   │   │       ├── scalar-min-max-fill-operand.ll
    │   │   │       ├── scalar_sse_minmax.ll
    │   │   │       ├── scalar_widen_div.ll
    │   │   │       ├── scalarize-bitcast.ll
    │   │   │       ├── scalarize-fp.ll
    │   │   │       ├── scatter-schedule.ll
    │   │   │       ├── scavenger.mir
    │   │   │       ├── scev-interchange.ll
    │   │   │       ├── schedule-x86-64-shld.ll
    │   │   │       ├── schedule-x86_32.ll
    │   │   │       ├── schedule-x86_64.ll
    │   │   │       ├── scheduler-backtracking.ll
    │   │   │       ├── sdiv-exact.ll
    │   │   │       ├── sdiv-pow2.ll
    │   │   │       ├── section_mergeable_size.ll
    │   │   │       ├── segmented-stacks-dynamic.ll
    │   │   │       ├── segmented-stacks-standalone.ll
    │   │   │       ├── segmented-stacks.ll
    │   │   │       ├── seh-catch-all-win32.ll
    │   │   │       ├── seh-catch-all.ll
    │   │   │       ├── seh-catchpad.ll
    │   │   │       ├── seh-except-finally.ll
    │   │   │       ├── seh-exception-code.ll
    │   │   │       ├── seh-filter-no-personality.ll
    │   │   │       ├── seh-finally.ll
    │   │   │       ├── seh-no-invokes.ll
    │   │   │       ├── seh-safe-div-win32.ll
    │   │   │       ├── seh-safe-div.ll
    │   │   │       ├── seh-stack-realign.ll
    │   │   │       ├── select-1-or-neg1.ll
    │   │   │       ├── select-mmx.ll
    │   │   │       ├── select-of-fp-constants.ll
    │   │   │       ├── select-with-and-or.ll
    │   │   │       ├── select.ll
    │   │   │       ├── select_const.ll
    │   │   │       ├── select_meta.ll
    │   │   │       ├── selectcc-to-shiftand.ll
    │   │   │       ├── selectiondag-crash.ll
    │   │   │       ├── selectiondag-cse.ll
    │   │   │       ├── selectiondag-debug-loc.ll
    │   │   │       ├── selectiondag-dominator.ll
    │   │   │       ├── selectiondag-order.ll
    │   │   │       ├── setcc-combine.ll
    │   │   │       ├── setcc-logic.ll
    │   │   │       ├── setcc-lowering.ll
    │   │   │       ├── setcc-narrowing.ll
    │   │   │       ├── setcc-wide-types.ll
    │   │   │       ├── setcc.ll
    │   │   │       ├── setjmp-spills.ll
    │   │   │       ├── setoeq.ll
    │   │   │       ├── setuge.ll
    │   │   │       ├── sext-i1.ll
    │   │   │       ├── sext-load.ll
    │   │   │       ├── sext-ret-val.ll
    │   │   │       ├── sext-setcc-self.ll
    │   │   │       ├── sext-subreg.ll
    │   │   │       ├── sext-trunc.ll
    │   │   │       ├── sha-schedule.ll
    │   │   │       ├── sha.ll
    │   │   │       ├── shadow-call-stack.mir
    │   │   │       ├── shadow-stack.ll
    │   │   │       ├── shift-and.ll
    │   │   │       ├── shift-avx2-crash.ll
    │   │   │       ├── shift-bmi2.ll
    │   │   │       ├── shift-coalesce.ll
    │   │   │       ├── shift-codegen.ll
    │   │   │       ├── shift-combine-crash.ll
    │   │   │       ├── shift-combine.ll
    │   │   │       ├── shift-double-x86_64.ll
    │   │   │       ├── shift-double.ll
    │   │   │       ├── shift-folding.ll
    │   │   │       ├── shift-i128.ll
    │   │   │       ├── shift-i256.ll
    │   │   │       ├── shift-one.ll
    │   │   │       ├── shift-pair.ll
    │   │   │       ├── shift-parts.ll
    │   │   │       ├── shift-pcmp.ll
    │   │   │       ├── shl-anyext.ll
    │   │   │       ├── shl-crash-on-legalize.ll
    │   │   │       ├── shl-i64.ll
    │   │   │       ├── shl_elim.ll
    │   │   │       ├── shl_undef.ll
    │   │   │       ├── shrink-compare.ll
    │   │   │       ├── shrink-fp-const1.ll
    │   │   │       ├── shrink-fp-const2.ll
    │   │   │       ├── shrink-wrap-chkstk-x86_64.ll
    │   │   │       ├── shrink-wrap-chkstk.ll
    │   │   │       ├── shrink-wrapping-vla.ll
    │   │   │       ├── shrink_vmul-widen.ll
    │   │   │       ├── shrink_vmul.ll
    │   │   │       ├── shrink_vmul_sse.ll
    │   │   │       ├── shrink_wrap_dbg_value.mir
    │   │   │       ├── shrinkwrap-hang.ll
    │   │   │       ├── shuffle-combine-crash-2.ll
    │   │   │       ├── shuffle-combine-crash.ll
    │   │   │       ├── shuffle-of-insert.ll
    │   │   │       ├── shuffle-of-splat-multiuses.ll
    │   │   │       ├── shuffle-strided-with-offset-128.ll
    │   │   │       ├── shuffle-strided-with-offset-256.ll
    │   │   │       ├── shuffle-strided-with-offset-512.ll
    │   │   │       ├── shuffle-vs-trunc-128-widen.ll
    │   │   │       ├── shuffle-vs-trunc-128.ll
    │   │   │       ├── shuffle-vs-trunc-256-widen.ll
    │   │   │       ├── shuffle-vs-trunc-256.ll
    │   │   │       ├── shuffle-vs-trunc-512-widen.ll
    │   │   │       ├── shuffle-vs-trunc-512.ll
    │   │   │       ├── sibcall-2.ll
    │   │   │       ├── sibcall-3.ll
    │   │   │       ├── sibcall-4.ll
    │   │   │       ├── sibcall-5.ll
    │   │   │       ├── sibcall-6.ll
    │   │   │       ├── sibcall-byval.ll
    │   │   │       ├── sibcall-win64.ll
    │   │   │       ├── sibcall.ll
    │   │   │       ├── signbit-shift.ll
    │   │   │       ├── signed-truncation-check.ll
    │   │   │       ├── simple-register-allocation-read-undef.mir
    │   │   │       ├── simple-zext.ll
    │   │   │       ├── sincos-opt.ll
    │   │   │       ├── sincos.ll
    │   │   │       ├── sink-blockfreq.ll
    │   │   │       ├── sink-cheap-instructions.ll
    │   │   │       ├── sink-gep-before-mem-inst.ll
    │   │   │       ├── sink-hoist.ll
    │   │   │       ├── sink-local-value.ll
    │   │   │       ├── sink-out-of-loop.ll
    │   │   │       ├── sitofp.ll
    │   │   │       ├── sjlj-baseptr.ll
    │   │   │       ├── sjlj-eh.ll
    │   │   │       ├── sjlj-shadow-stack-liveness.mir
    │   │   │       ├── sjlj.ll
    │   │   │       ├── slow-incdec.ll
    │   │   │       ├── slow-pmulld.ll
    │   │   │       ├── slow-unaligned-mem.ll
    │   │   │       ├── small-byval-memcpy.ll
    │   │   │       ├── smul-with-overflow.ll
    │   │   │       ├── smul_fix.ll
    │   │   │       ├── soft-fp-legal-in-HW-reg.ll
    │   │   │       ├── soft-fp.ll
    │   │   │       ├── soft-sitofp.ll
    │   │   │       ├── speculative-load-hardening-call-and-ret.ll
    │   │   │       ├── speculative-load-hardening-gather.ll
    │   │   │       ├── speculative-load-hardening-indirect.ll
    │   │   │       ├── speculative-load-hardening.ll
    │   │   │       ├── splat-const.ll
    │   │   │       ├── splat-for-size.ll
    │   │   │       ├── split-eh-lpad-edges.ll
    │   │   │       ├── split-extend-vector-inreg.ll
    │   │   │       ├── split-store.ll
    │   │   │       ├── split-vector-bitcast.ll
    │   │   │       ├── split-vector-rem.ll
    │   │   │       ├── sqrt-fastmath-mir.ll
    │   │   │       ├── sqrt-fastmath-tune.ll
    │   │   │       ├── sqrt-fastmath.ll
    │   │   │       ├── sqrt-partial.ll
    │   │   │       ├── sqrt.ll
    │   │   │       ├── sret-implicit.ll
    │   │   │       ├── sse-align-0.ll
    │   │   │       ├── sse-align-1.ll
    │   │   │       ├── sse-align-10.ll
    │   │   │       ├── sse-align-11.ll
    │   │   │       ├── sse-align-12.ll
    │   │   │       ├── sse-align-2.ll
    │   │   │       ├── sse-align-3.ll
    │   │   │       ├── sse-align-4.ll
    │   │   │       ├── sse-align-5.ll
    │   │   │       ├── sse-align-6.ll
    │   │   │       ├── sse-align-7.ll
    │   │   │       ├── sse-align-8.ll
    │   │   │       ├── sse-align-9.ll
    │   │   │       ├── sse-commute.ll
    │   │   │       ├── sse-cvttp2si.ll
    │   │   │       ├── sse-domains.ll
    │   │   │       ├── sse-fcopysign.ll
    │   │   │       ├── sse-fsignum.ll
    │   │   │       ├── sse-intel-ocl.ll
    │   │   │       ├── sse-intrinsics-fast-isel-x86_64.ll
    │   │   │       ├── sse-intrinsics-fast-isel.ll
    │   │   │       ├── sse-intrinsics-x86-upgrade.ll
    │   │   │       ├── sse-intrinsics-x86.ll
    │   │   │       ├── sse-intrinsics-x86_64-upgrade.ll
    │   │   │       ├── sse-intrinsics-x86_64.ll
    │   │   │       ├── sse-load-ret.ll
    │   │   │       ├── sse-minmax.ll
    │   │   │       ├── sse-only.ll
    │   │   │       ├── sse-regcall.ll
    │   │   │       ├── sse-scalar-fp-arith-unary.ll
    │   │   │       ├── sse-scalar-fp-arith.ll
    │   │   │       ├── sse-schedule.ll
    │   │   │       ├── sse-unaligned-mem-feature.ll
    │   │   │       ├── sse-varargs.ll
    │   │   │       ├── sse1-fcopysign.ll
    │   │   │       ├── sse1.ll
    │   │   │       ├── sse2-intrinsics-canonical.ll
    │   │   │       ├── sse2-intrinsics-fast-isel-x86_64.ll
    │   │   │       ├── sse2-intrinsics-fast-isel.ll
    │   │   │       ├── sse2-intrinsics-x86-upgrade.ll
    │   │   │       ├── sse2-intrinsics-x86.ll
    │   │   │       ├── sse2-intrinsics-x86_64-upgrade.ll
    │   │   │       ├── sse2-intrinsics-x86_64.ll
    │   │   │       ├── sse2-schedule.ll
    │   │   │       ├── sse2-vector-shifts.ll
    │   │   │       ├── sse2.ll
    │   │   │       ├── sse3-avx-addsub-2.ll
    │   │   │       ├── sse3-avx-addsub.ll
    │   │   │       ├── sse3-intrinsics-fast-isel.ll
    │   │   │       ├── sse3-intrinsics-x86.ll
    │   │   │       ├── sse3-schedule.ll
    │   │   │       ├── sse3.ll
    │   │   │       ├── sse41-intrinsics-fast-isel.ll
    │   │   │       ├── sse41-intrinsics-x86-upgrade.ll
    │   │   │       ├── sse41-intrinsics-x86.ll
    │   │   │       ├── sse41-pmovxrm.ll
    │   │   │       ├── sse41-schedule.ll
    │   │   │       ├── sse41.ll
    │   │   │       ├── sse42-intrinsics-fast-isel-x86_64.ll
    │   │   │       ├── sse42-intrinsics-fast-isel.ll
    │   │   │       ├── sse42-intrinsics-x86.ll
    │   │   │       ├── sse42-intrinsics-x86_64.ll
    │   │   │       ├── sse42-schedule.ll
    │   │   │       ├── sse4a-intrinsics-fast-isel.ll
    │   │   │       ├── sse4a-schedule.ll
    │   │   │       ├── sse4a-upgrade.ll
    │   │   │       ├── sse4a.ll
    │   │   │       ├── sse_partial_update.ll
    │   │   │       ├── sse_reload_fold.ll
    │   │   │       ├── ssp-data-layout.ll
    │   │   │       ├── ssp-guard-spill.ll
    │   │   │       ├── ssse3-intrinsics-fast-isel.ll
    │   │   │       ├── ssse3-intrinsics-x86.ll
    │   │   │       ├── ssse3-schedule.ll
    │   │   │       ├── ssub_sat.ll
    │   │   │       ├── ssub_sat_vec.ll
    │   │   │       ├── stack-align-memcpy.ll
    │   │   │       ├── stack-align.ll
    │   │   │       ├── stack-align2.ll
    │   │   │       ├── stack-folding-3dnow.ll
    │   │   │       ├── stack-folding-adx-x86_64.ll
    │   │   │       ├── stack-folding-adx.mir
    │   │   │       ├── stack-folding-bmi.ll
    │   │   │       ├── stack-folding-bmi2.ll
    │   │   │       ├── stack-folding-bmi2.mir
    │   │   │       ├── stack-folding-fp-avx1.ll
    │   │   │       ├── stack-folding-fp-avx512.ll
    │   │   │       ├── stack-folding-fp-avx512vl.ll
    │   │   │       ├── stack-folding-fp-sse42.ll
    │   │   │       ├── stack-folding-int-avx1.ll
    │   │   │       ├── stack-folding-int-avx2.ll
    │   │   │       ├── stack-folding-int-avx512.ll
    │   │   │       ├── stack-folding-int-avx512vl.ll
    │   │   │       ├── stack-folding-int-sse42.ll
    │   │   │       ├── stack-folding-lwp.ll
    │   │   │       ├── stack-folding-mmx.ll
    │   │   │       ├── stack-folding-sha.ll
    │   │   │       ├── stack-folding-tbm.ll
    │   │   │       ├── stack-folding-x86_64.ll
    │   │   │       ├── stack-folding-xop.ll
    │   │   │       ├── stack-probe-red-zone.ll
    │   │   │       ├── stack-probe-size.ll
    │   │   │       ├── stack-probes.ll
    │   │   │       ├── stack-protector-dbginfo.ll
    │   │   │       ├── stack-protector-msvc.ll
    │   │   │       ├── stack-protector-remarks.ll
    │   │   │       ├── stack-protector-target.ll
    │   │   │       ├── stack-protector-vreg-to-vreg-copy.ll
    │   │   │       ├── stack-protector-weight.ll
    │   │   │       ├── stack-protector.ll
    │   │   │       ├── stack-size-section-function-sections.ll
    │   │   │       ├── stack-size-section.ll
    │   │   │       ├── stack-update-frame-opcode.ll
    │   │   │       ├── stack_guard_remat.ll
    │   │   │       ├── StackColoring-dbg.ll
    │   │   │       ├── StackColoring.ll
    │   │   │       ├── stackguard-internal.ll
    │   │   │       ├── stackmap-fast-isel.ll
    │   │   │       ├── stackmap-frame-setup.ll
    │   │   │       ├── stackmap-large-constants.ll
    │   │   │       ├── stackmap-large-location-size.ll
    │   │   │       ├── stackmap-liveness.ll
    │   │   │       ├── stackmap-nops.ll
    │   │   │       ├── stackmap-shadow-optimization.ll
    │   │   │       ├── stackmap.ll
    │   │   │       ├── stackpointer.ll
    │   │   │       ├── statepoint-allocas.ll
    │   │   │       ├── statepoint-call-lowering.ll
    │   │   │       ├── statepoint-far-call.ll
    │   │   │       ├── statepoint-forward.ll
    │   │   │       ├── statepoint-gctransition-call-lowering.ll
    │   │   │       ├── statepoint-invoke.ll
    │   │   │       ├── statepoint-live-in.ll
    │   │   │       ├── statepoint-stack-usage.ll
    │   │   │       ├── statepoint-stackmap-format.ll
    │   │   │       ├── statepoint-uniqueing.ll
    │   │   │       ├── statepoint-vector-bad-spill.ll
    │   │   │       ├── statepoint-vector.ll
    │   │   │       ├── stdarg.ll
    │   │   │       ├── stdcall-notailcall.ll
    │   │   │       ├── stdcall.ll
    │   │   │       ├── store-empty-member.ll
    │   │   │       ├── store-fp-constant.ll
    │   │   │       ├── store-global-address.ll
    │   │   │       ├── store-narrow.ll
    │   │   │       ├── store-zero-and-minus-one.ll
    │   │   │       ├── store_op_load_fold.ll
    │   │   │       ├── store_op_load_fold2.ll
    │   │   │       ├── stores-merging.ll
    │   │   │       ├── storetrunc-fp.ll
    │   │   │       ├── stride-nine-with-base-reg.ll
    │   │   │       ├── stride-reuse.ll
    │   │   │       ├── sttni.ll
    │   │   │       ├── sub-with-overflow.ll
    │   │   │       ├── sub.ll
    │   │   │       ├── subcarry.ll
    │   │   │       ├── subreg-to-reg-0.ll
    │   │   │       ├── subreg-to-reg-1.ll
    │   │   │       ├── subreg-to-reg-2.ll
    │   │   │       ├── subreg-to-reg-3.ll
    │   │   │       ├── subreg-to-reg-4.ll
    │   │   │       ├── subreg-to-reg-6.ll
    │   │   │       ├── subvector-broadcast.ll
    │   │   │       ├── sunkaddr-ext.ll
    │   │   │       ├── swift-error.ll
    │   │   │       ├── swift-return.ll
    │   │   │       ├── swiftcc.ll
    │   │   │       ├── swifterror.ll
    │   │   │       ├── swiftself.ll
    │   │   │       ├── switch-bt.ll
    │   │   │       ├── switch-crit-edge-constant.ll
    │   │   │       ├── switch-default-only.ll
    │   │   │       ├── switch-density.ll
    │   │   │       ├── switch-edge-weight.ll
    │   │   │       ├── switch-jump-table.ll
    │   │   │       ├── switch-lower-peel-top-case.ll
    │   │   │       ├── switch-or.ll
    │   │   │       ├── switch-order-weight.ll
    │   │   │       ├── switch-zextload.ll
    │   │   │       ├── switch.ll
    │   │   │       ├── SwitchLowering.ll
    │   │   │       ├── swizzle-2.ll
    │   │   │       ├── swizzle-avx2.ll
    │   │   │       ├── SwizzleShuff.ll
    │   │   │       ├── system-intrinsics-64-xsave.ll
    │   │   │       ├── system-intrinsics-64-xsavec.ll
    │   │   │       ├── system-intrinsics-64-xsaveopt.ll
    │   │   │       ├── system-intrinsics-64-xsaves.ll
    │   │   │       ├── system-intrinsics-64.ll
    │   │   │       ├── system-intrinsics-xgetbv.ll
    │   │   │       ├── system-intrinsics-xsave.ll
    │   │   │       ├── system-intrinsics-xsavec.ll
    │   │   │       ├── system-intrinsics-xsaveopt.ll
    │   │   │       ├── system-intrinsics-xsaves.ll
    │   │   │       ├── system-intrinsics-xsetbv.ll
    │   │   │       ├── system-intrinsics.ll
    │   │   │       ├── tail-call-attrs.ll
    │   │   │       ├── tail-call-casts.ll
    │   │   │       ├── tail-call-conditional.mir
    │   │   │       ├── tail-call-got.ll
    │   │   │       ├── tail-call-legality.ll
    │   │   │       ├── tail-call-mutable-memarg.ll
    │   │   │       ├── tail-call-parameter-attrs-mismatch.ll
    │   │   │       ├── tail-call-win64.ll
    │   │   │       ├── tail-dup-addr.ll
    │   │   │       ├── tail-dup-catchret.ll
    │   │   │       ├── tail-dup-debugloc.ll
    │   │   │       ├── tail-dup-merge-loop-headers.ll
    │   │   │       ├── tail-dup-no-other-successor.ll
    │   │   │       ├── tail-dup-repeat.ll
    │   │   │       ├── tail-merge-after-mbp.mir
    │   │   │       ├── tail-merge-debugloc.ll
    │   │   │       ├── tail-merge-identical.ll
    │   │   │       ├── tail-merge-unreachable.ll
    │   │   │       ├── tail-merge-wineh.ll
    │   │   │       ├── tail-opts.ll
    │   │   │       ├── tail-threshold.ll
    │   │   │       ├── tailcall-64.ll
    │   │   │       ├── tailcall-calleesave.ll
    │   │   │       ├── tailcall-cgp-dup.ll
    │   │   │       ├── tailcall-disable.ll
    │   │   │       ├── tailcall-fastisel.ll
    │   │   │       ├── tailcall-largecode.ll
    │   │   │       ├── tailcall-lifetime-end.ll
    │   │   │       ├── tailcall-mem-intrinsics.ll
    │   │   │       ├── tailcall-msvc-conventions.ll
    │   │   │       ├── tailcall-multiret.ll
    │   │   │       ├── tailcall-readnone.ll
    │   │   │       ├── tailcall-returndup-void.ll
    │   │   │       ├── tailcall-ri64.ll
    │   │   │       ├── tailcall-stackalign.ll
    │   │   │       ├── tailcall-structret.ll
    │   │   │       ├── tailcall.ll
    │   │   │       ├── tailcallbyval.ll
    │   │   │       ├── tailcallbyval64.ll
    │   │   │       ├── tailcallfp.ll
    │   │   │       ├── tailcallfp2.ll
    │   │   │       ├── tailcallpic1.ll
    │   │   │       ├── tailcallpic2.ll
    │   │   │       ├── tailcallpic3.ll
    │   │   │       ├── tailcallstack64.ll
    │   │   │       ├── taildup-crash.ll
    │   │   │       ├── tailjmp_gotpcrel_relax_relocation.ll
    │   │   │       ├── targetLoweringGeneric.ll
    │   │   │       ├── tbm-intrinsics-fast-isel-x86_64.ll
    │   │   │       ├── tbm-intrinsics-fast-isel.ll
    │   │   │       ├── tbm-intrinsics-x86_64.ll
    │   │   │       ├── tbm-intrinsics.ll
    │   │   │       ├── tbm-schedule.ll
    │   │   │       ├── tbm_patterns.ll
    │   │   │       ├── test-nofold.ll
    │   │   │       ├── test-shrink-bug.ll
    │   │   │       ├── test-shrink.ll
    │   │   │       ├── test-vs-bittest.ll
    │   │   │       ├── test_x86condbr_globaladdr.mir
    │   │   │       ├── testb-je-fusion.ll
    │   │   │       ├── testl-commute.ll
    │   │   │       ├── this-return-64.ll
    │   │   │       ├── throws-cfi-fp.ll
    │   │   │       ├── throws-cfi-no-fp.ll
    │   │   │       ├── tls-addr-non-leaf-function.ll
    │   │   │       ├── tls-android-negative.ll
    │   │   │       ├── tls-android.ll
    │   │   │       ├── tls-local-dynamic.ll
    │   │   │       ├── tls-models.ll
    │   │   │       ├── tls-pic.ll
    │   │   │       ├── tls-pie.ll
    │   │   │       ├── tls-shrink-wrapping.ll
    │   │   │       ├── tls-windows-itanium.ll
    │   │   │       ├── tls.ll
    │   │   │       ├── tlv-1.ll
    │   │   │       ├── tlv-2.ll
    │   │   │       ├── tlv-3.ll
    │   │   │       ├── token_landingpad.ll
    │   │   │       ├── trap.ll
    │   │   │       ├── trunc-ext-ld-st.ll
    │   │   │       ├── trunc-store.ll
    │   │   │       ├── trunc-subvector.ll
    │   │   │       ├── trunc-to-bool.ll
    │   │   │       ├── TruncAssertSext.ll
    │   │   │       ├── TruncAssertZext.ll
    │   │   │       ├── twoaddr-coalesce-2.ll
    │   │   │       ├── twoaddr-coalesce-3.ll
    │   │   │       ├── twoaddr-coalesce.ll
    │   │   │       ├── twoaddr-dbg-value.mir
    │   │   │       ├── twoaddr-lea.ll
    │   │   │       ├── twoaddr-pass-sink.ll
    │   │   │       ├── twoaddr-sink-terminator.ll
    │   │   │       ├── uadd_sat.ll
    │   │   │       ├── uadd_sat_vec.ll
    │   │   │       ├── uint64-to-float.ll
    │   │   │       ├── uint_to_fp-2.ll
    │   │   │       ├── uint_to_fp-3.ll
    │   │   │       ├── uint_to_fp.ll
    │   │   │       ├── umul-with-carry.ll
    │   │   │       ├── umul-with-overflow.ll
    │   │   │       ├── umulo-128-legalisation-lowering.ll
    │   │   │       ├── umulo-64-legalisation-lowering.ll
    │   │   │       ├── unaligned-32-byte-memops.ll
    │   │   │       ├── unaligned-load.ll
    │   │   │       ├── unaligned-spill-folding.ll
    │   │   │       ├── undef-eflags.mir
    │   │   │       ├── undef-globals-bss.ll
    │   │   │       ├── undef-label.ll
    │   │   │       ├── undef-ops.ll
    │   │   │       ├── unfold-masked-merge-scalar-constmask-innerouter.ll
    │   │   │       ├── unfold-masked-merge-scalar-constmask-interleavedbits.ll
    │   │   │       ├── unfold-masked-merge-scalar-constmask-interleavedbytehalves.ll
    │   │   │       ├── unfold-masked-merge-scalar-constmask-lowhigh.ll
    │   │   │       ├── unfold-masked-merge-scalar-variablemask.ll
    │   │   │       ├── unfold-masked-merge-vector-variablemask-const.ll
    │   │   │       ├── unfold-masked-merge-vector-variablemask.ll
    │   │   │       ├── unknown-location.ll
    │   │   │       ├── unreachable-loop-sinking.ll
    │   │   │       ├── unreachable-mbb-undef-phi.mir
    │   │   │       ├── unreachable-trap.ll
    │   │   │       ├── unreachableblockelim.ll
    │   │   │       ├── unused_stackslots.ll
    │   │   │       ├── unwind-init.ll
    │   │   │       ├── unwindraise.ll
    │   │   │       ├── update-terminator-debugloc.ll
    │   │   │       ├── update-terminator.mir
    │   │   │       ├── urem-i8-constant.ll
    │   │   │       ├── urem-power-of-two.ll
    │   │   │       ├── urem-seteq-optsize.ll
    │   │   │       ├── urem-seteq-vec-nonsplat.ll
    │   │   │       ├── urem-seteq-vec-splat.ll
    │   │   │       ├── urem-seteq.ll
    │   │   │       ├── use-add-flags.ll
    │   │   │       ├── usub_sat.ll
    │   │   │       ├── usub_sat_vec.ll
    │   │   │       ├── utf16-cfstrings.ll
    │   │   │       ├── utf8.ll
    │   │   │       ├── uwtables.ll
    │   │   │       ├── v2f32.ll
    │   │   │       ├── v4f32-immediate.ll
    │   │   │       ├── v4i32load-crash.ll
    │   │   │       ├── v8i1-masks.ll
    │   │   │       ├── vaargs.ll
    │   │   │       ├── vaes-intrinsics-avx-x86.ll
    │   │   │       ├── vaes-intrinsics-avx512-x86.ll
    │   │   │       ├── vaes-intrinsics-avx512vl-x86.ll
    │   │   │       ├── var-permute-128.ll
    │   │   │       ├── var-permute-256.ll
    │   │   │       ├── var-permute-512.ll
    │   │   │       ├── vararg-callee-cleanup.ll
    │   │   │       ├── vararg_no_start.ll
    │   │   │       ├── vararg_tailcall.ll
    │   │   │       ├── variable-sized-darwin-bzero.ll
    │   │   │       ├── variadic-node-pic.ll
    │   │   │       ├── vastart-defs-eflags.ll
    │   │   │       ├── vbinop-simplify-bug.ll
    │   │   │       ├── vec-copysign-avx512.ll
    │   │   │       ├── vec-copysign.ll
    │   │   │       ├── vec-libcalls.ll
    │   │   │       ├── vec-loadsingles-alignment.ll
    │   │   │       ├── vec-trunc-store.ll
    │   │   │       ├── vec3.ll
    │   │   │       ├── vec_add.ll
    │   │   │       ├── vec_align.ll
    │   │   │       ├── vec_align_i256.ll
    │   │   │       ├── vec_anyext.ll
    │   │   │       ├── vec_call.ll
    │   │   │       ├── vec_cast.ll
    │   │   │       ├── vec_cast2.ll
    │   │   │       ├── vec_cast3.ll
    │   │   │       ├── vec_cmp_sint-128.ll
    │   │   │       ├── vec_cmp_uint-128.ll
    │   │   │       ├── vec_compare-sse4.ll
    │   │   │       ├── vec_compare.ll
    │   │   │       ├── vec_ctbits.ll
    │   │   │       ├── vec_ext_inreg.ll
    │   │   │       ├── vec_extract-avx.ll
    │   │   │       ├── vec_extract-mmx.ll
    │   │   │       ├── vec_extract-sse4.ll
    │   │   │       ├── vec_extract.ll
    │   │   │       ├── vec_fabs.ll
    │   │   │       ├── vec_floor.ll
    │   │   │       ├── vec_fneg.ll
    │   │   │       ├── vec_fp_to_int-widen.ll
    │   │   │       ├── vec_fp_to_int.ll
    │   │   │       ├── vec_fpext.ll
    │   │   │       ├── vec_fptrunc.ll
    │   │   │       ├── vec_i64.ll
    │   │   │       ├── vec_ins_extract-1.ll
    │   │   │       ├── vec_ins_extract.ll
    │   │   │       ├── vec_insert-2.ll
    │   │   │       ├── vec_insert-3.ll
    │   │   │       ├── vec_insert-4.ll
    │   │   │       ├── vec_insert-5.ll
    │   │   │       ├── vec_insert-7.ll
    │   │   │       ├── vec_insert-8.ll
    │   │   │       ├── vec_insert-9.ll
    │   │   │       ├── vec_insert-mmx.ll
    │   │   │       ├── vec_int_to_fp-widen.ll
    │   │   │       ├── vec_int_to_fp.ll
    │   │   │       ├── vec_loadsingles.ll
    │   │   │       ├── vec_logical.ll
    │   │   │       ├── vec_minmax_match.ll
    │   │   │       ├── vec_minmax_sint.ll
    │   │   │       ├── vec_minmax_uint.ll
    │   │   │       ├── vec_partial.ll
    │   │   │       ├── vec_reassociate.ll
    │   │   │       ├── vec_return.ll
    │   │   │       ├── vec_round.ll
    │   │   │       ├── vec_sdiv_to_shift.ll
    │   │   │       ├── vec_set-2.ll
    │   │   │       ├── vec_set-3.ll
    │   │   │       ├── vec_set-4.ll
    │   │   │       ├── vec_set-6.ll
    │   │   │       ├── vec_set-7.ll
    │   │   │       ├── vec_set-8.ll
    │   │   │       ├── vec_set-A.ll
    │   │   │       ├── vec_set-B.ll
    │   │   │       ├── vec_set-C.ll
    │   │   │       ├── vec_set-D.ll
    │   │   │       ├── vec_set-F.ll
    │   │   │       ├── vec_set-H.ll
    │   │   │       ├── vec_set.ll
    │   │   │       ├── vec_setcc-2.ll
    │   │   │       ├── vec_setcc.ll
    │   │   │       ├── vec_shift.ll
    │   │   │       ├── vec_shift2.ll
    │   │   │       ├── vec_shift3.ll
    │   │   │       ├── vec_shift4.ll
    │   │   │       ├── vec_shift5.ll
    │   │   │       ├── vec_shift6.ll
    │   │   │       ├── vec_shift7.ll
    │   │   │       ├── vec_shuf-insert.ll
    │   │   │       ├── vec_split.ll
    │   │   │       ├── vec_ss_load_fold.ll
    │   │   │       ├── vec_trunc_sext.ll
    │   │   │       ├── vec_udiv_to_shift.ll
    │   │   │       ├── vec_uint_to_fp-fastmath.ll
    │   │   │       ├── vec_uint_to_fp.ll
    │   │   │       ├── vec_unsafe-fp-math.ll
    │   │   │       ├── vec_zero-2.ll
    │   │   │       ├── vec_zero.ll
    │   │   │       ├── vec_zero_cse.ll
    │   │   │       ├── vector-bitreverse.ll
    │   │   │       ├── vector-blend.ll
    │   │   │       ├── vector-compare-all_of.ll
    │   │   │       ├── vector-compare-any_of.ll
    │   │   │       ├── vector-compare-combines.ll
    │   │   │       ├── vector-compare-results.ll
    │   │   │       ├── vector-compare-simplify.ll
    │   │   │       ├── vector-constrained-fp-intrinsics-fma.ll
    │   │   │       ├── vector-constrained-fp-intrinsics.ll
    │   │   │       ├── vector-ext-logic.ll
    │   │   │       ├── vector-extend-inreg.ll
    │   │   │       ├── vector-fshl-128.ll
    │   │   │       ├── vector-fshl-256.ll
    │   │   │       ├── vector-fshl-512.ll
    │   │   │       ├── vector-fshl-rot-128.ll
    │   │   │       ├── vector-fshl-rot-256.ll
    │   │   │       ├── vector-fshl-rot-512.ll
    │   │   │       ├── vector-fshr-128.ll
    │   │   │       ├── vector-fshr-256.ll
    │   │   │       ├── vector-fshr-512.ll
    │   │   │       ├── vector-fshr-rot-128.ll
    │   │   │       ├── vector-fshr-rot-256.ll
    │   │   │       ├── vector-fshr-rot-512.ll
    │   │   │       ├── vector-gep.ll
    │   │   │       ├── vector-half-conversions.ll
    │   │   │       ├── vector-idiv-sdiv-128.ll
    │   │   │       ├── vector-idiv-sdiv-256.ll
    │   │   │       ├── vector-idiv-sdiv-512.ll
    │   │   │       ├── vector-idiv-udiv-128.ll
    │   │   │       ├── vector-idiv-udiv-256.ll
    │   │   │       ├── vector-idiv-udiv-512.ll
    │   │   │       ├── vector-idiv-v2i32.ll
    │   │   │       ├── vector-idiv.ll
    │   │   │       ├── vector-interleave.ll
    │   │   │       ├── vector-intrinsics.ll
    │   │   │       ├── vector-lzcnt-128.ll
    │   │   │       ├── vector-lzcnt-256.ll
    │   │   │       ├── vector-lzcnt-512.ll
    │   │   │       ├── vector-merge-store-fp-constants.ll
    │   │   │       ├── vector-mul.ll
    │   │   │       ├── vector-narrow-binop.ll
    │   │   │       ├── vector-pcmp.ll
    │   │   │       ├── vector-popcnt-128.ll
    │   │   │       ├── vector-popcnt-256.ll
    │   │   │       ├── vector-popcnt-512.ll
    │   │   │       ├── vector-reduce-add-widen.ll
    │   │   │       ├── vector-reduce-add.ll
    │   │   │       ├── vector-reduce-and-widen.ll
    │   │   │       ├── vector-reduce-and.ll
    │   │   │       ├── vector-reduce-fadd-fast.ll
    │   │   │       ├── vector-reduce-fadd.ll
    │   │   │       ├── vector-reduce-fmax-nnan.ll
    │   │   │       ├── vector-reduce-fmax.ll
    │   │   │       ├── vector-reduce-fmin-nnan.ll
    │   │   │       ├── vector-reduce-fmin.ll
    │   │   │       ├── vector-reduce-fmul-fast.ll
    │   │   │       ├── vector-reduce-fmul.ll
    │   │   │       ├── vector-reduce-mul-widen.ll
    │   │   │       ├── vector-reduce-mul.ll
    │   │   │       ├── vector-reduce-or-widen.ll
    │   │   │       ├── vector-reduce-or.ll
    │   │   │       ├── vector-reduce-smax-widen.ll
    │   │   │       ├── vector-reduce-smax.ll
    │   │   │       ├── vector-reduce-smin-widen.ll
    │   │   │       ├── vector-reduce-smin.ll
    │   │   │       ├── vector-reduce-umax-widen.ll
    │   │   │       ├── vector-reduce-umax.ll
    │   │   │       ├── vector-reduce-umin-widen.ll
    │   │   │       ├── vector-reduce-umin.ll
    │   │   │       ├── vector-reduce-xor-widen.ll
    │   │   │       ├── vector-reduce-xor.ll
    │   │   │       ├── vector-rem.ll
    │   │   │       ├── vector-rotate-128.ll
    │   │   │       ├── vector-rotate-256.ll
    │   │   │       ├── vector-rotate-512.ll
    │   │   │       ├── vector-sext-widen.ll
    │   │   │       ├── vector-sext.ll
    │   │   │       ├── vector-shift-ashr-128.ll
    │   │   │       ├── vector-shift-ashr-256.ll
    │   │   │       ├── vector-shift-ashr-512.ll
    │   │   │       ├── vector-shift-ashr-sub128-widen.ll
    │   │   │       ├── vector-shift-ashr-sub128.ll
    │   │   │       ├── vector-shift-lshr-128.ll
    │   │   │       ├── vector-shift-lshr-256.ll
    │   │   │       ├── vector-shift-lshr-512.ll
    │   │   │       ├── vector-shift-lshr-sub128-widen.ll
    │   │   │       ├── vector-shift-lshr-sub128.ll
    │   │   │       ├── vector-shift-shl-128.ll
    │   │   │       ├── vector-shift-shl-256.ll
    │   │   │       ├── vector-shift-shl-512.ll
    │   │   │       ├── vector-shift-shl-sub128-widen.ll
    │   │   │       ├── vector-shift-shl-sub128.ll
    │   │   │       ├── vector-shuffle-128-v16.ll
    │   │   │       ├── vector-shuffle-128-v2.ll
    │   │   │       ├── vector-shuffle-128-v4.ll
    │   │   │       ├── vector-shuffle-128-v8.ll
    │   │   │       ├── vector-shuffle-256-v16.ll
    │   │   │       ├── vector-shuffle-256-v32.ll
    │   │   │       ├── vector-shuffle-256-v4.ll
    │   │   │       ├── vector-shuffle-256-v8.ll
    │   │   │       ├── vector-shuffle-512-v16.ll
    │   │   │       ├── vector-shuffle-512-v32.ll
    │   │   │       ├── vector-shuffle-512-v64.ll
    │   │   │       ├── vector-shuffle-512-v8.ll
    │   │   │       ├── vector-shuffle-avx512.ll
    │   │   │       ├── vector-shuffle-combining-avx.ll
    │   │   │       ├── vector-shuffle-combining-avx2.ll
    │   │   │       ├── vector-shuffle-combining-avx512bw.ll
    │   │   │       ├── vector-shuffle-combining-avx512bwvl.ll
    │   │   │       ├── vector-shuffle-combining-avx512vbmi.ll
    │   │   │       ├── vector-shuffle-combining-sse41.ll
    │   │   │       ├── vector-shuffle-combining-sse4a.ll
    │   │   │       ├── vector-shuffle-combining-ssse3.ll
    │   │   │       ├── vector-shuffle-combining-xop.ll
    │   │   │       ├── vector-shuffle-combining.ll
    │   │   │       ├── vector-shuffle-masked.ll
    │   │   │       ├── vector-shuffle-mmx.ll
    │   │   │       ├── vector-shuffle-sse1.ll
    │   │   │       ├── vector-shuffle-sse41.ll
    │   │   │       ├── vector-shuffle-sse4a.ll
    │   │   │       ├── vector-shuffle-v1.ll
    │   │   │       ├── vector-shuffle-v48.ll
    │   │   │       ├── vector-shuffle-variable-128.ll
    │   │   │       ├── vector-shuffle-variable-256.ll
    │   │   │       ├── vector-sqrt.ll
    │   │   │       ├── vector-trunc-math-widen.ll
    │   │   │       ├── vector-trunc-math.ll
    │   │   │       ├── vector-trunc-packus-widen.ll
    │   │   │       ├── vector-trunc-packus.ll
    │   │   │       ├── vector-trunc-ssat-widen.ll
    │   │   │       ├── vector-trunc-ssat.ll
    │   │   │       ├── vector-trunc-usat-widen.ll
    │   │   │       ├── vector-trunc-usat.ll
    │   │   │       ├── vector-trunc-widen.ll
    │   │   │       ├── vector-trunc.ll
    │   │   │       ├── vector-truncate-combine.ll
    │   │   │       ├── vector-tzcnt-128.ll
    │   │   │       ├── vector-tzcnt-256.ll
    │   │   │       ├── vector-tzcnt-512.ll
    │   │   │       ├── vector-unsigned-cmp.ll
    │   │   │       ├── vector-variable-idx.ll
    │   │   │       ├── vector-variable-idx2.ll
    │   │   │       ├── vector-zext-widen.ll
    │   │   │       ├── vector-zext.ll
    │   │   │       ├── vector-zmov.ll
    │   │   │       ├── vector.ll
    │   │   │       ├── vectorcall.ll
    │   │   │       ├── verifier-generic-extend-truncate.mir
    │   │   │       ├── verifier-generic-types-1.mir
    │   │   │       ├── verifier-generic-types-2.mir
    │   │   │       ├── verifier-phi-fail0.mir
    │   │   │       ├── verifier-phi.mir
    │   │   │       ├── version_directive.ll
    │   │   │       ├── vfcmp.ll
    │   │   │       ├── viabs.ll
    │   │   │       ├── virtual-registers-cleared-in-machine-functions-liveins.ll
    │   │   │       ├── visibility.ll
    │   │   │       ├── visibility2.ll
    │   │   │       ├── vmaskmov-offset.ll
    │   │   │       ├── vmovq.ll
    │   │   │       ├── volatile.ll
    │   │   │       ├── vortex-bug.ll
    │   │   │       ├── vpshufbitqbm-intrinsics-upgrade.ll
    │   │   │       ├── vpshufbitqbm-intrinsics.ll
    │   │   │       ├── vsel-cmp-load.ll
    │   │   │       ├── vselect-2.ll
    │   │   │       ├── vselect-avx.ll
    │   │   │       ├── vselect-constants.ll
    │   │   │       ├── vselect-minmax.ll
    │   │   │       ├── vselect-packss.ll
    │   │   │       ├── vselect-pcmp.ll
    │   │   │       ├── vselect-zero.ll
    │   │   │       ├── vselect.ll
    │   │   │       ├── vshift-1.ll
    │   │   │       ├── vshift-2.ll
    │   │   │       ├── vshift-3.ll
    │   │   │       ├── vshift-4.ll
    │   │   │       ├── vshift-5.ll
    │   │   │       ├── vshift-6.ll
    │   │   │       ├── vshift_scalar.ll
    │   │   │       ├── vshift_split.ll
    │   │   │       ├── vshift_split2.ll
    │   │   │       ├── vsplit-and.ll
    │   │   │       ├── vzero-excess.ll
    │   │   │       ├── waitpkg-intrinsics.ll
    │   │   │       ├── warn-stack.ll
    │   │   │       ├── wbinvd-intrinsic.ll
    │   │   │       ├── wbnoinvd-intrinsic.ll
    │   │   │       ├── weak-undef.ll
    │   │   │       ├── weak.ll
    │   │   │       ├── weak_def_can_be_hidden.ll
    │   │   │       ├── webkit-jscc.ll
    │   │   │       ├── wide-fma-contraction.ll
    │   │   │       ├── wide-integer-cmp.ll
    │   │   │       ├── wide-integer-fold.ll
    │   │   │       ├── widen_arith-1.ll
    │   │   │       ├── widen_arith-2.ll
    │   │   │       ├── widen_arith-3.ll
    │   │   │       ├── widen_arith-4.ll
    │   │   │       ├── widen_arith-5.ll
    │   │   │       ├── widen_arith-6.ll
    │   │   │       ├── widen_bitops-0.ll
    │   │   │       ├── widen_bitops-1.ll
    │   │   │       ├── widen_cast-1.ll
    │   │   │       ├── widen_cast-2.ll
    │   │   │       ├── widen_cast-3.ll
    │   │   │       ├── widen_cast-4.ll
    │   │   │       ├── widen_cast-5.ll
    │   │   │       ├── widen_cast-6.ll
    │   │   │       ├── widen_compare-1.ll
    │   │   │       ├── widen_conv-1.ll
    │   │   │       ├── widen_conv-2.ll
    │   │   │       ├── widen_conv-3.ll
    │   │   │       ├── widen_conv-4.ll
    │   │   │       ├── widen_conversions.ll
    │   │   │       ├── widen_extract-1.ll
    │   │   │       ├── widen_load-0.ll
    │   │   │       ├── widen_load-1.ll
    │   │   │       ├── widen_load-2.ll
    │   │   │       ├── widen_load-3.ll
    │   │   │       ├── widen_mul.ll
    │   │   │       ├── widen_shuffle-1.ll
    │   │   │       ├── WidenArith.ll
    │   │   │       ├── widened-broadcast.ll
    │   │   │       ├── win-alloca-expander.ll
    │   │   │       ├── win-catchpad-csrs.ll
    │   │   │       ├── win-catchpad-nested-cxx.ll
    │   │   │       ├── win-catchpad-nested.ll
    │   │   │       ├── win-catchpad-varargs.ll
    │   │   │       ├── win-catchpad.ll
    │   │   │       ├── win-cleanuppad.ll
    │   │   │       ├── win-funclet-cfi.ll
    │   │   │       ├── win-mixed-ehpersonality.ll
    │   │   │       ├── win-smallparams.ll
    │   │   │       ├── win32-bool.ll
    │   │   │       ├── win32-eh-available-externally.ll
    │   │   │       ├── win32-eh-states.ll
    │   │   │       ├── win32-eh.ll
    │   │   │       ├── win32-pic-jumptable.ll
    │   │   │       ├── win32-preemption.ll
    │   │   │       ├── win32-seh-catchpad-realign.ll
    │   │   │       ├── win32-seh-catchpad.ll
    │   │   │       ├── win32-seh-nested-finally.ll
    │   │   │       ├── win32-spill-xmm.ll
    │   │   │       ├── win32-ssp.ll
    │   │   │       ├── win32_sret.ll
    │   │   │       ├── win64-bool.ll
    │   │   │       ├── win64-byval.ll
    │   │   │       ├── win64-jumptable.ll
    │   │   │       ├── win64-long-double.ll
    │   │   │       ├── win64-nosse-csrs.ll
    │   │   │       ├── win64_alloca_dynalloca.ll
    │   │   │       ├── win64_call_epi.ll
    │   │   │       ├── win64_eh.ll
    │   │   │       ├── win64_eh_leaf.ll
    │   │   │       ├── win64_eh_leaf2.ll
    │   │   │       ├── win64_frame.ll
    │   │   │       ├── win64_nonvol.ll
    │   │   │       ├── win64_params.ll
    │   │   │       ├── win64_sibcall.ll
    │   │   │       ├── win64_vararg.ll
    │   │   │       ├── win_chkstk.ll
    │   │   │       ├── win_coreclr_chkstk.ll
    │   │   │       ├── win_coreclr_chkstk_liveins.mir
    │   │   │       ├── win_cst_pool.ll
    │   │   │       ├── windows-itanium-alloca.ll
    │   │   │       ├── wineh-coreclr.ll
    │   │   │       ├── wineh-exceptionpointer.ll
    │   │   │       ├── wineh-no-ehpads.ll
    │   │   │       ├── x32-cet-intrinsics.ll
    │   │   │       ├── x32-function_pointer-1.ll
    │   │   │       ├── x32-function_pointer-2.ll
    │   │   │       ├── x32-function_pointer-3.ll
    │   │   │       ├── x32-indirectbr.ll
    │   │   │       ├── x32-landingpad.ll
    │   │   │       ├── x32-lea-1.ll
    │   │   │       ├── x32-movtopush64.ll
    │   │   │       ├── x32-va_start.ll
    │   │   │       ├── x64-cet-intrinsics.ll
    │   │   │       ├── x86-16.ll
    │   │   │       ├── x86-32-intrcc.ll
    │   │   │       ├── x86-32-vector-calling-conv.ll
    │   │   │       ├── x86-64-and-mask.ll
    │   │   │       ├── x86-64-arg.ll
    │   │   │       ├── x86-64-asm.ll
    │   │   │       ├── x86-64-baseptr.ll
    │   │   │       ├── x86-64-bittest-logic.ll
    │   │   │       ├── x86-64-call.ll
    │   │   │       ├── x86-64-disp.ll
    │   │   │       ├── x86-64-double-precision-shift-left.ll
    │   │   │       ├── x86-64-double-precision-shift-right.ll
    │   │   │       ├── x86-64-double-shifts-Oz-Os-O2.ll
    │   │   │       ├── x86-64-double-shifts-var.ll
    │   │   │       ├── x86-64-extend-shift.ll
    │   │   │       ├── x86-64-flags-intrinsics.ll
    │   │   │       ├── x86-64-gv-offset.ll
    │   │   │       ├── x86-64-intrcc-nosse.ll
    │   │   │       ├── x86-64-intrcc.ll
    │   │   │       ├── x86-64-jumps.ll
    │   │   │       ├── x86-64-mem.ll
    │   │   │       ├── x86-64-ms_abi-vararg.ll
    │   │   │       ├── x86-64-pic-1.ll
    │   │   │       ├── x86-64-pic-10.ll
    │   │   │       ├── x86-64-pic-11.ll
    │   │   │       ├── x86-64-pic-12.ll
    │   │   │       ├── x86-64-pic-2.ll
    │   │   │       ├── x86-64-pic-3.ll
    │   │   │       ├── x86-64-pic-4.ll
    │   │   │       ├── x86-64-pic-5.ll
    │   │   │       ├── x86-64-pic-6.ll
    │   │   │       ├── x86-64-pic-7.ll
    │   │   │       ├── x86-64-pic-8.ll
    │   │   │       ├── x86-64-pic-9.ll
    │   │   │       ├── x86-64-pic.ll
    │   │   │       ├── x86-64-plt-relative-reloc.ll
    │   │   │       ├── x86-64-psub.ll
    │   │   │       ├── x86-64-ptr-arg-simple.ll
    │   │   │       ├── x86-64-ret0.ll
    │   │   │       ├── x86-64-shortint.ll
    │   │   │       ├── x86-64-sret-return-2.ll
    │   │   │       ├── x86-64-sret-return.ll
    │   │   │       ├── x86-64-stack-and-frame-ptr.ll
    │   │   │       ├── x86-64-static-relo-movl.ll
    │   │   │       ├── x86-64-tls-1.ll
    │   │   │       ├── x86-64-varargs.ll
    │   │   │       ├── x86-big-ret.ll
    │   │   │       ├── x86-cmov-converter.ll
    │   │   │       ├── x86-flags-intrinsics.ll
    │   │   │       ├── x86-fold-pshufb.ll
    │   │   │       ├── x86-framelowering-trap.ll
    │   │   │       ├── x86-inline-asm-validation.ll
    │   │   │       ├── x86-interleaved-access.ll
    │   │   │       ├── x86-interleaved-check.ll
    │   │   │       ├── x86-interrupt_cc.ll
    │   │   │       ├── x86-interrupt_cld.ll
    │   │   │       ├── x86-interrupt_vzeroupper.ll
    │   │   │       ├── x86-mixed-alignment-dagcombine.ll
    │   │   │       ├── x86-no_caller_saved_registers-preserve.ll
    │   │   │       ├── x86-no_caller_saved_registers.ll
    │   │   │       ├── x86-plt-relative-reloc.ll
    │   │   │       ├── x86-repmov-copy-eflags.ll
    │   │   │       ├── x86-sanitizer-shrink-wrapping.ll
    │   │   │       ├── x86-setcc-int-to-fp-combine.ll
    │   │   │       ├── x86-shifts.ll
    │   │   │       ├── x86-shrink-wrap-unwind.ll
    │   │   │       ├── x86-shrink-wrapping.ll
    │   │   │       ├── x86-store-gv-addr.ll
    │   │   │       ├── x86-upgrade-avx-vbroadcast.ll
    │   │   │       ├── x86-upgrade-avx2-vbroadcast.ll
    │   │   │       ├── x86-win64-shrink-wrapping.ll
    │   │   │       ├── x86_64-mul-by-const.ll
    │   │   │       ├── x87-schedule.ll
    │   │   │       ├── x87.ll
    │   │   │       ├── xaluo.ll
    │   │   │       ├── xchg-nofold.ll
    │   │   │       ├── xmm-r64.ll
    │   │   │       ├── xmulo.ll
    │   │   │       ├── xop-ifma.ll
    │   │   │       ├── xop-intrinsics-fast-isel.ll
    │   │   │       ├── xop-intrinsics-x86_64-upgrade.ll
    │   │   │       ├── xop-intrinsics-x86_64.ll
    │   │   │       ├── xop-mask-comments.ll
    │   │   │       ├── xop-pcmov.ll
    │   │   │       ├── xop-schedule.ll
    │   │   │       ├── xor-combine-debugloc.ll
    │   │   │       ├── xor-icmp.ll
    │   │   │       ├── xor-select-i1-combine.ll
    │   │   │       ├── xor.ll
    │   │   │       ├── xray-attribute-instrumentation.ll
    │   │   │       ├── xray-custom-log.ll
    │   │   │       ├── xray-empty-firstmbb.mir
    │   │   │       ├── xray-empty-function.mir
    │   │   │       ├── xray-log-args.ll
    │   │   │       ├── xray-loop-detection.ll
    │   │   │       ├── xray-multiplerets-in-blocks.mir
    │   │   │       ├── xray-section-group.ll
    │   │   │       ├── xray-selective-instrumentation-miss.ll
    │   │   │       ├── xray-selective-instrumentation.ll
    │   │   │       ├── xray-tail-call-sled.ll
    │   │   │       ├── xray-typed-event-log.ll
    │   │   │       ├── xtest.ll
    │   │   │       ├── zero-remat.ll
    │   │   │       ├── zext-demanded.ll
    │   │   │       ├── zext-extract_subreg.ll
    │   │   │       ├── zext-fold.ll
    │   │   │       ├── zext-inreg-0.ll
    │   │   │       ├── zext-inreg-1.ll
    │   │   │       ├── zext-logicop-shift-load.ll
    │   │   │       ├── zext-sext.ll
    │   │   │       ├── zext-shl.ll
    │   │   │       ├── zext-trunc.ll
    │   │   │       ├── zlib-longest-match.ll
    │   │   │       ├── avx512-shuffles/
    │   │   │       │   ├── broadcast-scalar-fp.ll
    │   │   │       │   ├── broadcast-scalar-int.ll
    │   │   │       │   ├── broadcast-vector-fp.ll
    │   │   │       │   ├── broadcast-vector-int.ll
    │   │   │       │   ├── duplicate-high.ll
    │   │   │       │   ├── duplicate-low.ll
    │   │   │       │   ├── in_lane_permute.ll
    │   │   │       │   ├── partial_permute.ll
    │   │   │       │   ├── permute.ll
    │   │   │       │   ├── shuffle-interleave.ll
    │   │   │       │   ├── shuffle-vec.ll
    │   │   │       │   ├── shuffle.ll
    │   │   │       │   └── unpack.ll
    │   │   │       ├── GC/
    │   │   │       │   ├── alloc_loop.ll
    │   │   │       │   ├── argpromotion.ll
    │   │   │       │   ├── badreadproto.ll
    │   │   │       │   ├── badrootproto.ll
    │   │   │       │   ├── badwriteproto.ll
    │   │   │       │   ├── cg-O0.ll
    │   │   │       │   ├── deadargelim.ll
    │   │   │       │   ├── dynamic-frame-size.ll
    │   │   │       │   ├── erlang-gc.ll
    │   │   │       │   ├── fat.ll
    │   │   │       │   ├── inline.ll
    │   │   │       │   ├── inline2.ll
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   ├── lower_gcroot.ll
    │   │   │       │   ├── ocaml-gc-assert.ll
    │   │   │       │   ├── ocaml-gc.ll
    │   │   │       │   └── outside.ll
    │   │   │       └── GlobalISel/
    │   │   │           ├── add-ext.ll
    │   │   │           ├── add-scalar.ll
    │   │   │           ├── add-vec.ll
    │   │   │           ├── and-scalar.ll
    │   │   │           ├── ashr-scalar.ll
    │   │   │           ├── avoid-matchtable-crash.mir
    │   │   │           ├── binop.ll
    │   │   │           ├── br.ll
    │   │   │           ├── brcond.ll
    │   │   │           ├── callingconv.ll
    │   │   │           ├── calllowering-nocrashret.ll
    │   │   │           ├── cmp.ll
    │   │   │           ├── constant.ll
    │   │   │           ├── ext-x86-64.ll
    │   │   │           ├── ext.ll
    │   │   │           ├── fadd-scalar.ll
    │   │   │           ├── fconstant.ll
    │   │   │           ├── fdiv-scalar.ll
    │   │   │           ├── fmul-scalar.ll
    │   │   │           ├── fpext-scalar.ll
    │   │   │           ├── frameIndex.ll
    │   │   │           ├── fsub-scalar.ll
    │   │   │           ├── gep.ll
    │   │   │           ├── GV.ll
    │   │   │           ├── inttoptr.ll
    │   │   │           ├── irtranslator-callingconv.ll
    │   │   │           ├── legalize-add-v128.mir
    │   │   │           ├── legalize-add-v256.mir
    │   │   │           ├── legalize-add-v512.mir
    │   │   │           ├── legalize-add.mir
    │   │   │           ├── legalize-and-scalar.mir
    │   │   │           ├── legalize-ashr-scalar.mir
    │   │   │           ├── legalize-brcond.mir
    │   │   │           ├── legalize-cmp.mir
    │   │   │           ├── legalize-constant.mir
    │   │   │           ├── legalize-ext-x86-64.mir
    │   │   │           ├── legalize-ext.mir
    │   │   │           ├── legalize-fadd-scalar.mir
    │   │   │           ├── legalize-fdiv-scalar.mir
    │   │   │           ├── legalize-fmul-scalar.mir
    │   │   │           ├── legalize-fpext-scalar.mir
    │   │   │           ├── legalize-fptrunc-scalar.mir
    │   │   │           ├── legalize-fsub-scalar.mir
    │   │   │           ├── legalize-gep.mir
    │   │   │           ├── legalize-insert-vec256.mir
    │   │   │           ├── legalize-insert-vec512.mir
    │   │   │           ├── legalize-lshr-scalar.mir
    │   │   │           ├── legalize-memop-scalar.mir
    │   │   │           ├── legalize-mul-scalar.mir
    │   │   │           ├── legalize-mul-v128.mir
    │   │   │           ├── legalize-mul-v256.mir
    │   │   │           ├── legalize-mul-v512.mir
    │   │   │           ├── legalize-or-scalar.mir
    │   │   │           ├── legalize-phi.mir
    │   │   │           ├── legalize-shl-scalar.mir
    │   │   │           ├── legalize-sub-v128.mir
    │   │   │           ├── legalize-sub-v256.mir
    │   │   │           ├── legalize-sub-v512.mir
    │   │   │           ├── legalize-sub.mir
    │   │   │           ├── legalize-trunc.mir
    │   │   │           ├── legalize-undef.mir
    │   │   │           ├── legalize-xor-scalar.mir
    │   │   │           ├── lit.local.cfg
    │   │   │           ├── lshr-scalar.ll
    │   │   │           ├── memop-scalar-x32.ll
    │   │   │           ├── memop-scalar.ll
    │   │   │           ├── memop-vec.ll
    │   │   │           ├── mul-scalar.ll
    │   │   │           ├── mul-vec.ll
    │   │   │           ├── or-scalar.ll
    │   │   │           ├── phi.ll
    │   │   │           ├── ptrtoint.ll
    │   │   │           ├── regbankselect-AVX2.mir
    │   │   │           ├── regbankselect-AVX512.mir
    │   │   │           ├── regbankselect-X32.mir
    │   │   │           ├── regbankselect-X86_64.mir
    │   │   │           ├── select-add-v128.mir
    │   │   │           ├── select-add-v256.mir
    │   │   │           ├── select-add-v512.mir
    │   │   │           ├── select-add-x32.mir
    │   │   │           ├── select-add.mir
    │   │   │           ├── select-and-scalar.mir
    │   │   │           ├── select-ashr-scalar.mir
    │   │   │           ├── select-blsi.mir
    │   │   │           ├── select-blsr.mir
    │   │   │           ├── select-br.mir
    │   │   │           ├── select-brcond.mir
    │   │   │           ├── select-cmp.mir
    │   │   │           ├── select-constant.mir
    │   │   │           ├── select-copy.mir
    │   │   │           ├── select-ext-x86-64.mir
    │   │   │           ├── select-ext.mir
    │   │   │           ├── select-extract-vec256.mir
    │   │   │           ├── select-extract-vec512.mir
    │   │   │           ├── select-fadd-scalar.mir
    │   │   │           ├── select-fconstant.mir
    │   │   │           ├── select-fdiv-scalar.mir
    │   │   │           ├── select-fmul-scalar.mir
    │   │   │           ├── select-fpext-scalar.mir
    │   │   │           ├── select-fptrunc-scalar.mir
    │   │   │           ├── select-fsub-scalar.mir
    │   │   │           ├── select-gep.mir
    │   │   │           ├── select-GV.mir
    │   │   │           ├── select-inc.mir
    │   │   │           ├── select-insert-vec256.mir
    │   │   │           ├── select-insert-vec512.mir
    │   │   │           ├── select-intrinsic-x86-flags-read-u32.mir
    │   │   │           ├── select-leaf-constant.mir
    │   │   │           ├── select-lshr-scalar.mir
    │   │   │           ├── select-memop-scalar-x32.mir
    │   │   │           ├── select-memop-scalar.mir
    │   │   │           ├── select-memop-v128.mir
    │   │   │           ├── select-memop-v256.mir
    │   │   │           ├── select-memop-v512.mir
    │   │   │           ├── select-merge-vec256.mir
    │   │   │           ├── select-merge-vec512.mir
    │   │   │           ├── select-mul-scalar.mir
    │   │   │           ├── select-mul-vec.mir
    │   │   │           ├── select-or-scalar.mir
    │   │   │           ├── select-phi.mir
    │   │   │           ├── select-shl-scalar.mir
    │   │   │           ├── select-sub-v128.mir
    │   │   │           ├── select-sub-v256.mir
    │   │   │           ├── select-sub-v512.mir
    │   │   │           ├── select-sub.mir
    │   │   │           ├── select-trunc.mir
    │   │   │           ├── select-undef.mir
    │   │   │           ├── select-unmerge-vec256.mir
    │   │   │           ├── select-unmerge-vec512.mir
    │   │   │           ├── select-xor-scalar.mir
    │   │   │           ├── shl-scalar-widening.ll
    │   │   │           ├── shl-scalar.ll
    │   │   │           ├── sub-scalar.ll
    │   │   │           ├── sub-vec.ll
    │   │   │           ├── trunc.ll
    │   │   │           ├── undef.ll
    │   │   │           ├── x32-select-frameIndex.mir
    │   │   │           ├── x86-legalize-GV.mir
    │   │   │           ├── x86-legalize-inttoptr.mir
    │   │   │           ├── x86-legalize-ptrtoint.mir
    │   │   │           ├── x86-legalize-sdiv.mir
    │   │   │           ├── x86-legalize-srem.mir
    │   │   │           ├── x86-legalize-udiv.mir
    │   │   │           ├── x86-legalize-urem.mir
    │   │   │           ├── x86-select-frameIndex.mir
    │   │   │           ├── x86-select-inttoptr.mir
    │   │   │           ├── x86-select-ptrtoint.mir
    │   │   │           ├── x86-select-sdiv.mir
    │   │   │           ├── x86-select-srem.mir
    │   │   │           ├── x86-select-trap.mir
    │   │   │           ├── x86-select-udiv.mir
    │   │   │           ├── x86-select-urem.mir
    │   │   │           ├── x86_64-fallback.ll
    │   │   │           ├── x86_64-irtranslator-struct-return.ll
    │   │   │           ├── x86_64-irtranslator.ll
    │   │   │           ├── x86_64-legalize-fcmp.mir
    │   │   │           ├── x86_64-legalize-fptosi.mir
    │   │   │           ├── x86_64-legalize-GV.mir
    │   │   │           ├── x86_64-legalize-inttoptr.mir
    │   │   │           ├── x86_64-legalize-ptrtoint.mir
    │   │   │           ├── x86_64-legalize-sdiv.mir
    │   │   │           ├── x86_64-legalize-sitofp.mir
    │   │   │           ├── x86_64-legalize-srem.mir
    │   │   │           ├── x86_64-legalize-udiv.mir
    │   │   │           ├── x86_64-legalize-urem.mir
    │   │   │           ├── x86_64-legalize-zext.mir
    │   │   │           ├── x86_64-select-fcmp.mir
    │   │   │           ├── x86_64-select-fptosi.mir
    │   │   │           ├── x86_64-select-frameIndex.mir
    │   │   │           ├── x86_64-select-inttoptr.mir
    │   │   │           ├── x86_64-select-ptrtoint.mir
    │   │   │           ├── x86_64-select-sdiv.mir
    │   │   │           ├── x86_64-select-sitofp.mir
    │   │   │           ├── x86_64-select-srem.mir
    │   │   │           ├── x86_64-select-udiv.mir
    │   │   │           ├── x86_64-select-urem.mir
    │   │   │           ├── x86_64-select-zext.mir
    │   │   │           └── xor-scalar.ll
    │   │   ├── DebugInfo/
    │   │   │   ├── arm-relocs.test
    │   │   │   ├── check-debugify-preserves-analyses.ll
    │   │   │   ├── cross-cu-scope.ll
    │   │   │   ├── debugify-bogus-dbg-value.ll
    │   │   │   ├── debugify-each.ll
    │   │   │   ├── debugify-export.ll
    │   │   │   ├── debugify-report-missing-locs-only.ll
    │   │   │   ├── debugify.ll
    │   │   │   ├── debuglineinfo-macho.test
    │   │   │   ├── debuglineinfo-path.ll
    │   │   │   ├── debuglineinfo.test
    │   │   │   ├── debugmacinfo.test
    │   │   │   ├── dwarfdump-64-bit-dwarf.test
    │   │   │   ├── dwarfdump-accel.test
    │   │   │   ├── dwarfdump-debug-frame-simple.test
    │   │   │   ├── dwarfdump-decompression-corrupt.test
    │   │   │   ├── dwarfdump-decompression-error.test
    │   │   │   ├── dwarfdump-dump-flags.test
    │   │   │   ├── dwarfdump-dump-gdbindex.test
    │   │   │   ├── dwarfdump-dwp.test
    │   │   │   ├── dwarfdump-implicit-const.test
    │   │   │   ├── dwarfdump-invalid-line-table.test
    │   │   │   ├── dwarfdump-invalid.test
    │   │   │   ├── dwarfdump-macho-relocs.test
    │   │   │   ├── dwarfdump-macho-universal.test
    │   │   │   ├── dwarfdump-objc.test
    │   │   │   ├── dwarfdump-pubnames.test
    │   │   │   ├── dwarfdump-ranges.test
    │   │   │   ├── dwarfdump-type-units.test
    │   │   │   ├── dwarfdump-zlib.test
    │   │   │   ├── dwo.ll
    │   │   │   ├── invalid-relocations.test
    │   │   │   ├── llvm-symbolizer-split-dwarf-empty.test
    │   │   │   ├── llvm-symbolizer-split-dwarf-no-skel-address.test
    │   │   │   ├── llvm-symbolizer-tu.test
    │   │   │   ├── llvm-symbolizer-zlib.test
    │   │   │   ├── llvm-symbolizer.test
    │   │   │   ├── macro_link.ll
    │   │   │   ├── omit-empty.ll
    │   │   │   ├── pr34186.ll
    │   │   │   ├── pr34672.ll
    │   │   │   ├── precomp.test
    │   │   │   ├── skeletoncu.ll
    │   │   │   ├── strip-DIGlobalVariable.ll
    │   │   │   ├── strip-loop-metadata.ll
    │   │   │   ├── strip-module-flags.ll
    │   │   │   ├── typeunit-header.test
    │   │   │   ├── unrolled-loop-remainder.ll
    │   │   │   ├── AArch64/
    │   │   │   │   ├── asan-stack-vars.mir
    │   │   │   │   ├── big-endian-dump.ll
    │   │   │   │   ├── big-endian.ll
    │   │   │   │   ├── bitfields.ll
    │   │   │   │   ├── cfi-eof-prologue.ll
    │   │   │   │   ├── coalescing.ll
    │   │   │   │   ├── compiler-gen-bbs-livedebugvalues.mir
    │   │   │   │   ├── constant-dbgloc.ll
    │   │   │   │   ├── dagcombine-zext.ll
    │   │   │   │   ├── dbg-value-i16.ll
    │   │   │   │   ├── dbg-value-i8.ll
    │   │   │   │   ├── dwarfdump.ll
    │   │   │   │   ├── eh_frame.s
    │   │   │   │   ├── eh_frame_personality.ll
    │   │   │   │   ├── frameindices.ll
    │   │   │   │   ├── inlined-argument.ll
    │   │   │   │   ├── line-header.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── little-endian-dump.ll
    │   │   │   │   ├── machine-outliner.ll
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── prologue_end.ll
    │   │   │   │   ├── return-address-signing.ll
    │   │   │   │   ├── struct_by_value.ll
    │   │   │   │   └── tls-at-location.ll
    │   │   │   ├── AMDGPU/
    │   │   │   │   ├── code-pointer-size.ll
    │   │   │   │   ├── dbg-value-sched-crash.ll
    │   │   │   │   ├── dwarfdump-relocs.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── pointer-address-space.ll
    │   │   │   │   └── variable-locations.ll
    │   │   │   ├── ARM/
    │   │   │   │   ├── big-endian-bitfield.ll
    │   │   │   │   ├── big-endian-dump.ll
    │   │   │   │   ├── bitfield.ll
    │   │   │   │   ├── cfi-eof-prologue.mir
    │   │   │   │   ├── constant-dbgloc.ll
    │   │   │   │   ├── float-args.ll
    │   │   │   │   ├── header.ll
    │   │   │   │   ├── illegal-fragment.ll
    │   │   │   │   ├── line.test
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── little-endian-dump.ll
    │   │   │   │   ├── lowerbdgdeclare_vla.ll
    │   │   │   │   ├── multiple-constant-uses-drops-dbgloc.ll
    │   │   │   │   ├── partial-subreg.ll
    │   │   │   │   ├── PR16736.ll
    │   │   │   │   ├── PR26163.ll
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── prologue_end.ll
    │   │   │   │   ├── s-super-register.ll
    │   │   │   │   ├── salvage-debug-info.ll
    │   │   │   │   ├── sdag-split-arg.ll
    │   │   │   │   ├── sdag-split-arg1.ll
    │   │   │   │   ├── selectiondag-deadcode.ll
    │   │   │   │   ├── single-constant-use-preserves-dbgloc.ll
    │   │   │   │   ├── split-complex.ll
    │   │   │   │   ├── sroa-complex.ll
    │   │   │   │   └── tls.ll
    │   │   │   ├── COFF/
    │   │   │   │   ├── anonymous-struct.ll
    │   │   │   │   ├── array-odr-violation.ll
    │   │   │   │   ├── asan-module-ctor.ll
    │   │   │   │   ├── asan-module-without-functions.ll
    │   │   │   │   ├── asm.ll
    │   │   │   │   ├── big-type.ll
    │   │   │   │   ├── bitfields.ll
    │   │   │   │   ├── build-info.ll
    │   │   │   │   ├── comdat.ll
    │   │   │   │   ├── const-unnamed-member.ll
    │   │   │   │   ├── cpp-mangling.ll
    │   │   │   │   ├── defer-complete-type.ll
    │   │   │   │   ├── dlang.ll
    │   │   │   │   ├── enum-co.ll
    │   │   │   │   ├── enum.ll
    │   │   │   │   ├── fp-stack.ll
    │   │   │   │   ├── fpo-argsize.ll
    │   │   │   │   ├── fpo-csrs.ll
    │   │   │   │   ├── fpo-funclet.ll
    │   │   │   │   ├── fpo-realign-alloca.ll
    │   │   │   │   ├── fpo-realign-vframe.ll
    │   │   │   │   ├── fpo-shrink-wrap.ll
    │   │   │   │   ├── fpo-stack-protect.ll
    │   │   │   │   ├── frameproc-flags.ll
    │   │   │   │   ├── function-options.ll
    │   │   │   │   ├── global-dllimport.ll
    │   │   │   │   ├── global-type-hashes.ll
    │   │   │   │   ├── global_visibility.ll
    │   │   │   │   ├── globals-discarded.ll
    │   │   │   │   ├── globals.ll
    │   │   │   │   ├── inheritance.ll
    │   │   │   │   ├── inlining-files.ll
    │   │   │   │   ├── inlining-header.ll
    │   │   │   │   ├── inlining-levels.ll
    │   │   │   │   ├── inlining-padding.ll
    │   │   │   │   ├── inlining-same-name.ll
    │   │   │   │   ├── inlining.ll
    │   │   │   │   ├── int8-char-type.ll
    │   │   │   │   ├── lambda.ll
    │   │   │   │   ├── lexicalblock.ll
    │   │   │   │   ├── lines-bb-start.ll
    │   │   │   │   ├── lines-difile.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── local-constant.ll
    │   │   │   │   ├── local-variable-gap.ll
    │   │   │   │   ├── local-variables.ll
    │   │   │   │   ├── long-name.ll
    │   │   │   │   ├── long-type-name.ll
    │   │   │   │   ├── multifile.ll
    │   │   │   │   ├── multifunction.ll
    │   │   │   │   ├── nested-types.ll
    │   │   │   │   ├── no-cus.ll
    │   │   │   │   ├── parameter-order.ll
    │   │   │   │   ├── pieces.ll
    │   │   │   │   ├── pr28747.ll
    │   │   │   │   ├── pr37492.ll
    │   │   │   │   ├── purge-typedef-udts.ll
    │   │   │   │   ├── register-variables.ll
    │   │   │   │   ├── retained-types.ll
    │   │   │   │   ├── scopes.ll
    │   │   │   │   ├── simple.ll
    │   │   │   │   ├── static-methods.ll
    │   │   │   │   ├── synthetic.ll
    │   │   │   │   ├── tail-call-without-lexical-scopes.ll
    │   │   │   │   ├── thunk.ll
    │   │   │   │   ├── type-quals.ll
    │   │   │   │   ├── typedef.ll
    │   │   │   │   ├── types-array-advanced.ll
    │   │   │   │   ├── types-array-unsized.ll
    │   │   │   │   ├── types-array.ll
    │   │   │   │   ├── types-basic.ll
    │   │   │   │   ├── types-calling-conv.ll
    │   │   │   │   ├── types-cvarargs.ll
    │   │   │   │   ├── types-data-members.ll
    │   │   │   │   ├── types-empty-member-fn.ll
    │   │   │   │   ├── types-method-ref-qualifiers.ll
    │   │   │   │   ├── types-nested-class.ll
    │   │   │   │   ├── types-non-virtual-methods.ll
    │   │   │   │   ├── types-ptr-to-member.ll
    │   │   │   │   ├── types-recursive-struct.ll
    │   │   │   │   ├── types-recursive-unnamed.ll
    │   │   │   │   ├── types-std-nullptr-t.ll
    │   │   │   │   ├── types-this-not-ptr.ll
    │   │   │   │   ├── udts-complete.ll
    │   │   │   │   ├── udts.ll
    │   │   │   │   ├── unnamed.ll
    │   │   │   │   ├── vframe-csr.ll
    │   │   │   │   ├── vframe-fpo.ll
    │   │   │   │   ├── vftables.ll
    │   │   │   │   ├── virtual-method-kinds.ll
    │   │   │   │   ├── virtual-methods.ll
    │   │   │   │   └── vtable-optzn-array.ll
    │   │   │   ├── Generic/
    │   │   │   │   ├── 2009-10-16-Phi.ll
    │   │   │   │   ├── 2009-11-03-InsertExtractValue.ll
    │   │   │   │   ├── 2009-11-05-DeadGlobalVariable.ll
    │   │   │   │   ├── 2009-11-06-NamelessGlobalVariable.ll
    │   │   │   │   ├── 2009-11-10-CurrentFn.ll
    │   │   │   │   ├── 2010-01-05-DbgScope.ll
    │   │   │   │   ├── 2010-03-12-llc-crash.ll
    │   │   │   │   ├── 2010-03-19-DbgDeclare.ll
    │   │   │   │   ├── 2010-03-24-MemberFn.ll
    │   │   │   │   ├── 2010-04-06-NestedFnDbgInfo.ll
    │   │   │   │   ├── 2010-04-19-FramePtr.ll
    │   │   │   │   ├── 2010-05-03-DisableFramePtr.ll
    │   │   │   │   ├── 2010-05-03-OriginDIE.ll
    │   │   │   │   ├── 2010-05-10-MultipleCU.ll
    │   │   │   │   ├── 2010-06-29-InlinedFnLocalVar.ll
    │   │   │   │   ├── 2010-10-01-crash.ll
    │   │   │   │   ├── accel-table-hash-collisions.ll
    │   │   │   │   ├── array.ll
    │   │   │   │   ├── block-asan.ll
    │   │   │   │   ├── bug_null_debuginfo.ll
    │   │   │   │   ├── callsite-attr-invalid.ll
    │   │   │   │   ├── codegenprep-value.ll
    │   │   │   │   ├── constant-pointers.ll
    │   │   │   │   ├── containing-type-extension.ll
    │   │   │   │   ├── cross-cu-inlining.ll
    │   │   │   │   ├── cross-cu-linkonce-distinct.ll
    │   │   │   │   ├── cross-cu-linkonce.ll
    │   │   │   │   ├── cu-range-hole.ll
    │   │   │   │   ├── cu-ranges.ll
    │   │   │   │   ├── dbg-at-specficiation.ll
    │   │   │   │   ├── dead-argument-order.ll
    │   │   │   │   ├── debug-info-always-inline.ll
    │   │   │   │   ├── debug-info-enum.ll
    │   │   │   │   ├── debug-info-qualifiers.ll
    │   │   │   │   ├── debug-label-inline.ll
    │   │   │   │   ├── debug-label-mi.ll
    │   │   │   │   ├── debug-label-opt.ll
    │   │   │   │   ├── debug-label.ll
    │   │   │   │   ├── debug-names-empty-cu.ll
    │   │   │   │   ├── debug-names-empty-name.ll
    │   │   │   │   ├── debug-names-hash-collisions.ll
    │   │   │   │   ├── debug-names-index-type.ll
    │   │   │   │   ├── debug-names-linkage-name.ll
    │   │   │   │   ├── debug-names-many-cu.ll
    │   │   │   │   ├── debug-names-name-collisions.ll
    │   │   │   │   ├── debug-names-one-cu.ll
    │   │   │   │   ├── debug-names-two-cu.ll
    │   │   │   │   ├── debuginfofinder-forward-declaration.ll
    │   │   │   │   ├── debuginfofinder-imported-global-variable.ll
    │   │   │   │   ├── debuginfofinder-inlined-cu.ll
    │   │   │   │   ├── debuginfofinder-multiple-cu.ll
    │   │   │   │   ├── def-line.ll
    │   │   │   │   ├── directives-only.ll
    │   │   │   │   ├── discriminated-union.ll
    │   │   │   │   ├── discriminator.ll
    │   │   │   │   ├── disubrange_vla.ll
    │   │   │   │   ├── disubrange_vla_no_dbgvalue.ll
    │   │   │   │   ├── dwarf-public-names.ll
    │   │   │   │   ├── empty.ll
    │   │   │   │   ├── enum-types.ll
    │   │   │   │   ├── enum.ll
    │   │   │   │   ├── extended-loc-directive.ll
    │   │   │   │   ├── global-sra-array.ll
    │   │   │   │   ├── global-sra-single-member.ll
    │   │   │   │   ├── global-sra-struct.ll
    │   │   │   │   ├── global.ll
    │   │   │   │   ├── gmlt.test
    │   │   │   │   ├── gmlt_profiling.ll
    │   │   │   │   ├── gvn.ll
    │   │   │   │   ├── imported-name-inlined.ll
    │   │   │   │   ├── incorrect-variable-debugloc.ll
    │   │   │   │   ├── incorrect-variable-debugloc1.ll
    │   │   │   │   ├── indvar-discriminator.ll
    │   │   │   │   ├── inheritance.ll
    │   │   │   │   ├── inline-debug-info-multiret.ll
    │   │   │   │   ├── inline-debug-info.ll
    │   │   │   │   ├── inline-debug-loc.ll
    │   │   │   │   ├── inline-no-debug-info.ll
    │   │   │   │   ├── inline-scopes.ll
    │   │   │   │   ├── inlined-arguments.ll
    │   │   │   │   ├── inlined-strings.ll
    │   │   │   │   ├── inlined-vars.ll
    │   │   │   │   ├── instcombine-phi.ll
    │   │   │   │   ├── invalid.ll
    │   │   │   │   ├── licm-hoist-debug-loc.ll
    │   │   │   │   ├── linear-dbg-value.ll
    │   │   │   │   ├── linkage-name-abstract.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── location-verifier.ll
    │   │   │   │   ├── lto-comp-dir.ll
    │   │   │   │   ├── mainsubprogram.ll
    │   │   │   │   ├── member-order.ll
    │   │   │   │   ├── member-pointers.ll
    │   │   │   │   ├── missing-abstract-variable.ll
    │   │   │   │   ├── multiline.ll
    │   │   │   │   ├── namespace.ll
    │   │   │   │   ├── namespace_function_definition.ll
    │   │   │   │   ├── namespace_inline_function_definition.ll
    │   │   │   │   ├── noscopes.ll
    │   │   │   │   ├── pass-by-value.ll
    │   │   │   │   ├── piece-verifier.ll
    │   │   │   │   ├── PR20038.ll
    │   │   │   │   ├── PR37395.ll
    │   │   │   │   ├── ptrsize.ll
    │   │   │   │   ├── recursive_inlining.ll
    │   │   │   │   ├── restrict.ll
    │   │   │   │   ├── simplifycfg_sink_last_inst.ll
    │   │   │   │   ├── skeletoncu.ll
    │   │   │   │   ├── sroa-larger.ll
    │   │   │   │   ├── sroa-samesize.ll
    │   │   │   │   ├── store-tail-merge.ll
    │   │   │   │   ├── string-offsets-form.ll
    │   │   │   │   ├── sugared-constants.ll
    │   │   │   │   ├── sunk-compare.ll
    │   │   │   │   ├── template-recursive-void.ll
    │   │   │   │   ├── thrownTypes.ll
    │   │   │   │   ├── tu-composite.ll
    │   │   │   │   ├── tu-member-pointer.ll
    │   │   │   │   ├── two-cus-from-same-file.ll
    │   │   │   │   ├── typedef.ll
    │   │   │   │   ├── unconditional-branch.ll
    │   │   │   │   ├── univariant-discriminated-union.ll
    │   │   │   │   ├── varargs.ll
    │   │   │   │   ├── version.ll
    │   │   │   │   ├── virtual-index.ll
    │   │   │   │   └── volatile-alloca.ll
    │   │   │   ├── Inputs/
    │   │   │   │   ├── arange-overlap.cc
    │   │   │   │   ├── arange-overlap.elf-x86_64
    │   │   │   │   ├── arm-relocs.elf-arm
    │   │   │   │   ├── cross-cu-inlining.c
    │   │   │   │   ├── dwarfdump-decompression-corrupt.elf-x86-64
    │   │   │   │   ├── dwarfdump-decompression-error.elf-x86-64
    │   │   │   │   ├── dwarfdump-gdbindex-v7.elf-x86-64
    │   │   │   │   ├── dwarfdump-inl-test.cc
    │   │   │   │   ├── dwarfdump-inl-test.elf-x86-64
    │   │   │   │   ├── dwarfdump-inl-test.h
    │   │   │   │   ├── dwarfdump-inl-test.high_pc.elf-x86-64
    │   │   │   │   ├── dwarfdump-macro-cmd.h
    │   │   │   │   ├── dwarfdump-macro.cc
    │   │   │   │   ├── dwarfdump-macro.h
    │   │   │   │   ├── dwarfdump-objc.m
    │   │   │   │   ├── dwarfdump-pubnames.cc
    │   │   │   │   ├── dwarfdump-pubnames.elf-x86-64
    │   │   │   │   ├── dwarfdump-ranges-baseaddr-exe.elf-x86-64
    │   │   │   │   ├── dwarfdump-test-32bit.elf.c
    │   │   │   │   ├── dwarfdump-test-loc-list-32bit.elf.cpp
    │   │   │   │   ├── dwarfdump-test-zlib.cc
    │   │   │   │   ├── dwarfdump-test-zlib.elf-x86-64
    │   │   │   │   ├── dwarfdump-test-zlib.o.elf-x86-64
    │   │   │   │   ├── dwarfdump-test-zlibgnu.elf-x86-64
    │   │   │   │   ├── dwarfdump-test.cc
    │   │   │   │   ├── dwarfdump-test.elf-x86-64
    │   │   │   │   ├── dwarfdump-test.elf-x86-64.debuglink
    │   │   │   │   ├── dwarfdump-test2-helper.cc
    │   │   │   │   ├── dwarfdump-test2-main.cc
    │   │   │   │   ├── dwarfdump-test2.elf-x86-64
    │   │   │   │   ├── dwarfdump-test3-decl.h
    │   │   │   │   ├── dwarfdump-test3-decl2.h
    │   │   │   │   ├── dwarfdump-test3.cc
    │   │   │   │   ├── dwarfdump-test3.elf-x86-64-space
    │   │   │   │   ├── dwarfdump-test4-decl.h
    │   │   │   │   ├── dwarfdump-test4-part1.cc
    │   │   │   │   ├── dwarfdump-test4-part2.cc
    │   │   │   │   ├── dwarfdump-test4.elf-x86-64
    │   │   │   │   ├── dwarfdump-type-units.cc
    │   │   │   │   ├── dwarfdump-type-units.elf-x86-64
    │   │   │   │   ├── dwarfdump.elf-mips64-64-bit-dwarf
    │   │   │   │   ├── fission-ranges.cc
    │   │   │   │   ├── fission-ranges.elf-x86_64
    │   │   │   │   ├── gmlt.ll
    │   │   │   │   ├── invalid.elf
    │   │   │   │   ├── invalid.elf.2
    │   │   │   │   ├── invalid.elf.3
    │   │   │   │   ├── invalid.linetable
    │   │   │   │   ├── line.ll
    │   │   │   │   ├── llvm-symbolizer-dwo-test
    │   │   │   │   ├── llvm-symbolizer-dwo-test.cc
    │   │   │   │   ├── llvm-symbolizer-local-mem-func-gcc.elf-x86-64
    │   │   │   │   ├── llvm-symbolizer-test.c
    │   │   │   │   ├── llvm-symbolizer-test.elf-x86-64
    │   │   │   │   ├── llvm-symbolizer-tu.elf-x86-64
    │   │   │   │   ├── loclists-dwp-b.ll
    │   │   │   │   ├── macho-universal
    │   │   │   │   ├── macho-universal.cc
    │   │   │   │   ├── shared-object-stripped.elf-i386
    │   │   │   │   ├── split-dwarf-addr-object-relocation.cpp
    │   │   │   │   ├── split-dwarf-addr-object-relocation.dwo
    │   │   │   │   ├── split-dwarf-dwp.cpp
    │   │   │   │   ├── split-dwarf-dwp.o.dwp
    │   │   │   │   ├── split-dwarf-empty.dwo
    │   │   │   │   ├── split-dwarf-multiple-cu.cpp
    │   │   │   │   ├── split-dwarf-multiple-cu.dwo
    │   │   │   │   ├── split-dwarf-no-skel-address.dwo
    │   │   │   │   ├── split-dwarf-test
    │   │   │   │   ├── split-dwarf-test-nogmlt
    │   │   │   │   ├── split-dwarf-test.cc
    │   │   │   │   ├── split-dwarf-test.cpp
    │   │   │   │   ├── split-dwarf-test.dwo
    │   │   │   │   ├── typeunit-header.elf-x86-64
    │   │   │   │   └── typeunit-header.s
    │   │   │   ├── Lanai/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   └── processes-relocations.ll
    │   │   │   ├── Mips/
    │   │   │   │   ├── delay-slot.ll
    │   │   │   │   ├── dsr-fixed-objects.ll
    │   │   │   │   ├── dsr-non-fixed-objects.ll
    │   │   │   │   ├── dwarfdump-tls.ll
    │   │   │   │   ├── eh_frame.ll
    │   │   │   │   ├── fn-call-line.ll
    │   │   │   │   ├── InlinedFnLocalVar.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── prologue_end.ll
    │   │   │   │   └── tls.ll
    │   │   │   ├── MIR/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── AArch64/
    │   │   │   │   │   ├── clobber-sp.mir
    │   │   │   │   │   ├── implicit-def-dead-scope.mir
    │   │   │   │   │   └── lit.local.cfg
    │   │   │   │   ├── ARM/
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── live-debug-values-reg-copy.mir
    │   │   │   │   │   ├── split-superreg-complex.mir
    │   │   │   │   │   ├── split-superreg-piece.mir
    │   │   │   │   │   └── split-superreg.mir
    │   │   │   │   ├── Mips/
    │   │   │   │   │   ├── last-inst-bundled.mir
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   └── live-debug-values-reg-copy.mir
    │   │   │   │   └── X86/
    │   │   │   │       ├── bit-piece-dh.mir
    │   │   │   │       ├── empty-inline.mir
    │   │   │   │       ├── kill-after-spill.mir
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── live-debug-values-3preds.mir
    │   │   │   │       ├── live-debug-values-reg-copy.mir
    │   │   │   │       ├── live-debug-values-spill.mir
    │   │   │   │       ├── live-debug-values.mir
    │   │   │   │       ├── live-debug-vars-unused-arg-debugonly.mir
    │   │   │   │       ├── live-debug-vars-unused-arg.mir
    │   │   │   │       ├── livedebugvalues-limit.mir
    │   │   │   │       ├── mlicm-hoist.mir
    │   │   │   │       ├── no-cfi-loc.mir
    │   │   │   │       └── regcoalescer.mir
    │   │   │   ├── MSP430/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   └── sdagsplit-1.ll
    │   │   │   ├── NVPTX/
    │   │   │   │   ├── cu-range-hole.ll
    │   │   │   │   ├── dbg-declare-alloca.ll
    │   │   │   │   ├── dbg-value-const-byref.ll
    │   │   │   │   ├── debug-file-loc-only.ll
    │   │   │   │   ├── debug-file-loc.ll
    │   │   │   │   ├── debug-info.ll
    │   │   │   │   ├── debug-loc-offset.ll
    │   │   │   │   └── lit.local.cfg
    │   │   │   ├── PDB/
    │   │   │   │   ├── dbi-bytes.test
    │   │   │   │   ├── dump-fpm.test
    │   │   │   │   ├── every-type.test
    │   │   │   │   ├── just-my-code.test
    │   │   │   │   ├── module-bytes.test
    │   │   │   │   ├── module-stats.test
    │   │   │   │   ├── obj-globalhash.test
    │   │   │   │   ├── pdb-invalid-type.test
    │   │   │   │   ├── pdb-longname-truncation.test
    │   │   │   │   ├── pdb-minimal-construct.test
    │   │   │   │   ├── pdb-resolve-forward-refs.test
    │   │   │   │   ├── pdb-unknown-symbol.test
    │   │   │   │   ├── pdb-yaml-symbols.test
    │   │   │   │   ├── pdbdump-debug-subsections.test
    │   │   │   │   ├── pdbdump-global-lookup.test
    │   │   │   │   ├── pdbdump-globals-empty.test
    │   │   │   │   ├── pdbdump-headers.test
    │   │   │   │   ├── pdbdump-merge-ids-and-types.test
    │   │   │   │   ├── pdbdump-mergeids.test
    │   │   │   │   ├── pdbdump-mergetypes.test
    │   │   │   │   ├── pdbdump-objfilename.yaml
    │   │   │   │   ├── pdbdump-raw-blocks.test
    │   │   │   │   ├── pdbdump-raw-bytes.test
    │   │   │   │   ├── pdbdump-raw-stream.test
    │   │   │   │   ├── pdbdump-readwrite.test
    │   │   │   │   ├── pdbdump-source-names.test
    │   │   │   │   ├── pdbdump-write.test
    │   │   │   │   ├── pdbdump-yaml-types.test
    │   │   │   │   ├── pdbdump-yaml.test
    │   │   │   │   ├── section-headers.test
    │   │   │   │   ├── tpi-bytes.test
    │   │   │   │   ├── udt-stats.test
    │   │   │   │   ├── using-namespace.test
    │   │   │   │   ├── write-fpm.test
    │   │   │   │   ├── DIA/
    │   │   │   │   │   ├── lit.local.cfg
    │   │   │   │   │   ├── pdbdump-flags.test
    │   │   │   │   │   ├── pdbdump-linenumbers.test
    │   │   │   │   │   └── pdbdump-symbol-format.test
    │   │   │   │   ├── Inputs/
    │   │   │   │   │   ├── debug-subsections.yaml
    │   │   │   │   │   ├── empty.cpp
    │   │   │   │   │   ├── every-array.cpp
    │   │   │   │   │   ├── every-class.cpp
    │   │   │   │   │   ├── every-enum.cpp
    │   │   │   │   │   ├── every-function.cpp
    │   │   │   │   │   ├── every-pointer.cpp
    │   │   │   │   │   ├── every-type.cpp
    │   │   │   │   │   ├── every-type.yaml
    │   │   │   │   │   ├── global-name-lookup.cpp
    │   │   │   │   │   ├── longname-truncation.yaml
    │   │   │   │   │   ├── merge-ids-1.yaml
    │   │   │   │   │   ├── merge-ids-2.yaml
    │   │   │   │   │   ├── merge-ids-and-types-1.yaml
    │   │   │   │   │   ├── merge-ids-and-types-2.yaml
    │   │   │   │   │   ├── merge-types-1.yaml
    │   │   │   │   │   ├── merge-types-2.yaml
    │   │   │   │   │   ├── obj-hashes-1.yaml
    │   │   │   │   │   ├── obj-hashes-2.yaml
    │   │   │   │   │   ├── one-symbol.yaml
    │   │   │   │   │   ├── source-names-1.yaml
    │   │   │   │   │   ├── source-names-2.yaml
    │   │   │   │   │   ├── symbolformat-fpo.cpp
    │   │   │   │   │   ├── symbolformat.cpp
    │   │   │   │   │   └── unknown-symbol.yaml
    │   │   │   │   └── Native/
    │   │   │   │       ├── pdb-native-compilands.test
    │   │   │   │       ├── pdb-native-enums.test
    │   │   │   │       ├── pdb-native-function-signatures.test
    │   │   │   │       ├── pdb-native-pointers.test
    │   │   │   │       ├── pdb-native-summary.test
    │   │   │   │       ├── pdb-native-typedefs.test
    │   │   │   │       └── pdb-native-udts.test
    │   │   │   ├── PowerPC/
    │   │   │   │   ├── line.test
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── live-debug-vars-subreg-offset.ll
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── tls-fission.ll
    │   │   │   │   └── tls.ll
    │   │   │   ├── RISCV/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   └── relax-debug-line.ll
    │   │   │   ├── Sparc/
    │   │   │   │   ├── gnu-window-save.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── prologue_end.ll
    │   │   │   │   └── subreg.ll
    │   │   │   ├── SystemZ/
    │   │   │   │   ├── eh_frame.s
    │   │   │   │   ├── eh_frame_personality.ll
    │   │   │   │   ├── eh_frame_personality.s
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── processes-relocations.ll
    │   │   │   │   ├── prologue_end.ll
    │   │   │   │   ├── variable-loc.ll
    │   │   │   │   └── variable-loc.s
    │   │   │   ├── WebAssembly/
    │   │   │   │   ├── dbg-declare.ll
    │   │   │   │   ├── dbg-loop-loc.ll
    │   │   │   │   ├── dbg-value-live-interval.ll
    │   │   │   │   ├── dbg-value-move-2.ll
    │   │   │   │   ├── dbg-value-move-clone.mir
    │   │   │   │   ├── dbg-value-move-reg-stackify.mir
    │   │   │   │   ├── dbg-value-move.ll
    │   │   │   │   └── lit.local.cfg
    │   │   │   └── X86/
    │   │   │       ├── 2010-04-13-PubType.ll
    │   │   │       ├── 2011-09-26-GlobalVarContext.ll
    │   │   │       ├── 2011-12-16-BadStructRef.ll
    │   │   │       ├── abbr_offset.s
    │   │   │       ├── abstract_origin.ll
    │   │   │       ├── accel-tables-dwarf5.ll
    │   │   │       ├── accel-tables.ll
    │   │   │       ├── addr_comments.ll
    │   │   │       ├── align_c11.ll
    │   │   │       ├── align_cpp11.ll
    │   │   │       ├── align_objc.ll
    │   │   │       ├── aligned_stack_var.ll
    │   │   │       ├── arange-and-stub.ll
    │   │   │       ├── arange.ll
    │   │   │       ├── arguments.ll
    │   │   │       ├── array.ll
    │   │   │       ├── array2.ll
    │   │   │       ├── asm-macro-line-number.s
    │   │   │       ├── atomic-c11-dwarf-4.ll
    │   │   │       ├── atomic-c11-dwarf-5.ll
    │   │   │       ├── bbjoin.ll
    │   │   │       ├── bitcast-di.ll
    │   │   │       ├── bitfields-dwarf4.ll
    │   │   │       ├── bitfields.ll
    │   │   │       ├── block-capture.ll
    │   │   │       ├── byvalstruct.ll
    │   │   │       ├── c-type-units.ll
    │   │   │       ├── clang-module.ll
    │   │   │       ├── clone-module-2.ll
    │   │   │       ├── clone-module.ll
    │   │   │       ├── coff_debug_info_type.ll
    │   │   │       ├── coff_relative_names.ll
    │   │   │       ├── concrete_out_of_line.ll
    │   │   │       ├── constant-aggregate.ll
    │   │   │       ├── constant-loclist.ll
    │   │   │       ├── containing-type-extension-rust.ll
    │   │   │       ├── cu-ranges-odr.ll
    │   │   │       ├── cu-ranges.ll
    │   │   │       ├── data_member_location.ll
    │   │   │       ├── dbg-abstract-vars-g-gmlt.ll
    │   │   │       ├── dbg-addr-dse.ll
    │   │   │       ├── dbg-addr.ll
    │   │   │       ├── dbg-asm.s
    │   │   │       ├── dbg-byval-parameter.ll
    │   │   │       ├── dbg-const-int.ll
    │   │   │       ├── dbg-const.ll
    │   │   │       ├── dbg-declare-alloca.ll
    │   │   │       ├── dbg-declare-arg.ll
    │   │   │       ├── dbg-declare-inalloca.ll
    │   │   │       ├── dbg-declare.ll
    │   │   │       ├── dbg-file-name.ll
    │   │   │       ├── dbg-i128-const.ll
    │   │   │       ├── dbg-merge-loc-entry.ll
    │   │   │       ├── dbg-prolog-end.ll
    │   │   │       ├── dbg-subrange.ll
    │   │   │       ├── dbg-value-const-byref.ll
    │   │   │       ├── dbg-value-dag-combine.ll
    │   │   │       ├── dbg-value-frame-index.ll
    │   │   │       ├── dbg-value-g-gmlt.ll
    │   │   │       ├── dbg-value-inlined-parameter.ll
    │   │   │       ├── dbg-value-isel.ll
    │   │   │       ├── dbg-value-location.ll
    │   │   │       ├── dbg-value-range.ll
    │   │   │       ├── dbg-value-regmask-clobber.ll
    │   │   │       ├── dbg-value-terminator.ll
    │   │   │       ├── dbg-value-transfer-order.ll
    │   │   │       ├── dbg-vector-size.ll
    │   │   │       ├── dbg_value_direct.ll
    │   │   │       ├── debug-dead-local-var.ll
    │   │   │       ├── debug-info-access.ll
    │   │   │       ├── debug-info-block-captured-self.ll
    │   │   │       ├── debug-info-blocks.ll
    │   │   │       ├── debug-info-packed-struct.ll
    │   │   │       ├── debug-info-producer-with-flags.ll
    │   │   │       ├── debug-info-static-member.ll
    │   │   │       ├── debug-label-unreached.ll
    │   │   │       ├── debug-loc-asan.mir
    │   │   │       ├── debug-loc-frame.ll
    │   │   │       ├── debug-loc-offset.mir
    │   │   │       ├── debug-macro.ll
    │   │   │       ├── debug-names-ir-disabled.ll
    │   │   │       ├── debug-names-partial.ll
    │   │   │       ├── debug-names-split-dwarf.ll
    │   │   │       ├── debug-ranges-offset.ll
    │   │   │       ├── debug_addr.ll
    │   │   │       ├── debug_and_nodebug_CUs.ll
    │   │   │       ├── debug_frame.ll
    │   │   │       ├── debugger-tune.ll
    │   │   │       ├── decl-derived-member.ll
    │   │   │       ├── default-subrange-array.ll
    │   │   │       ├── deleted-bit-piece.ll
    │   │   │       ├── DIModule.ll
    │   │   │       ├── DIModuleContext.ll
    │   │   │       ├── discriminator.ll
    │   │   │       ├── discriminator2.ll
    │   │   │       ├── discriminator3.ll
    │   │   │       ├── dllimport.ll
    │   │   │       ├── double-declare.ll
    │   │   │       ├── DW_AT_byte_size.ll
    │   │   │       ├── DW_AT_calling-convention.ll
    │   │   │       ├── DW_AT_linkage_name.ll
    │   │   │       ├── DW_AT_location-reference.ll
    │   │   │       ├── DW_AT_object_pointer.ll
    │   │   │       ├── DW_AT_specification.ll
    │   │   │       ├── DW_AT_stmt_list_sec_offset.ll
    │   │   │       ├── dw_op_minus.mir
    │   │   │       ├── dw_op_minus_direct.ll
    │   │   │       ├── DW_TAG_friend.ll
    │   │   │       ├── dwarf-aranges-no-dwarf-labels.ll
    │   │   │       ├── dwarf-aranges.ll
    │   │   │       ├── dwarf-callsite-related-attrs.ll
    │   │   │       ├── dwarf-linkage-names.ll
    │   │   │       ├── dwarf-no-source-loc.ll
    │   │   │       ├── dwarf-public-names.ll
    │   │   │       ├── dwarf-pubnames-split.ll
    │   │   │       ├── dwarfdump-bogus-LNE.s
    │   │   │       ├── dwarfdump-debug-loc-simple.test
    │   │   │       ├── dwarfdump-debug-loclists.test
    │   │   │       ├── dwarfdump-debug-names.s
    │   │   │       ├── dwarfdump-header-64.s
    │   │   │       ├── dwarfdump-header.s
    │   │   │       ├── dwarfdump-line-dwo.s
    │   │   │       ├── dwarfdump-line-mismatch.s
    │   │   │       ├── dwarfdump-line-only.s
    │   │   │       ├── dwarfdump-ranges-baseaddr-exe.s
    │   │   │       ├── dwarfdump-ranges-baseaddr.s
    │   │   │       ├── dwarfdump-ranges-unrelocated.s
    │   │   │       ├── dwarfdump-rnglists.s
    │   │   │       ├── dwarfdump-str-offsets-dwp.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-1.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-2.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-3.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-4.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-5.s
    │   │   │       ├── dwarfdump-str-offsets-invalid-6.s
    │   │   │       ├── dwarfdump-str-offsets-macho.s
    │   │   │       ├── dwarfdump-str-offsets.s
    │   │   │       ├── earlydup-crash.ll
    │   │   │       ├── elf-names.ll
    │   │   │       ├── empty-and-one-elem-array.ll
    │   │   │       ├── empty-array.ll
    │   │   │       ├── empty.ll
    │   │   │       ├── empty_macinfo.ll
    │   │   │       ├── ending-run.ll
    │   │   │       ├── enum-class.ll
    │   │   │       ├── enum-fwd-decl.ll
    │   │   │       ├── fi-expr.ll
    │   │   │       ├── fi-piece.ll
    │   │   │       ├── fission-cu.ll
    │   │   │       ├── fission-hash.ll
    │   │   │       ├── fission-inline.ll
    │   │   │       ├── fission-local-import.ll
    │   │   │       ├── fission-no-inlining.ll
    │   │   │       ├── fission-ranges.ll
    │   │   │       ├── float_const.ll
    │   │   │       ├── float_const_loclist.ll
    │   │   │       ├── formal_parameter.ll
    │   │   │       ├── fragment-offset-order.ll
    │   │   │       ├── frame-register.ll
    │   │   │       ├── FrameIndexExprs.ll
    │   │   │       ├── generate-odr-hash.ll
    │   │   │       ├── ghost-sdnode-dbgvalues.ll
    │   │   │       ├── global-expression.ll
    │   │   │       ├── global-sra-fp80-array.ll
    │   │   │       ├── global-sra-fp80-struct.ll
    │   │   │       ├── gmlt.test
    │   │   │       ├── gnu-public-names-empty.ll
    │   │   │       ├── gnu-public-names-gmlt.ll
    │   │   │       ├── gnu-public-names-multiple-cus-2.s
    │   │   │       ├── gnu-public-names-multiple-cus.ll
    │   │   │       ├── gnu-public-names-tu.ll
    │   │   │       ├── gnu-public-names.ll
    │   │   │       ├── header.ll
    │   │   │       ├── inline-asm-locs.ll
    │   │   │       ├── inline-member-function.ll
    │   │   │       ├── inline-namespace.ll
    │   │   │       ├── inline-seldag-test.ll
    │   │   │       ├── inlined-formal-parameter.ll
    │   │   │       ├── inlined-indirect-value.ll
    │   │   │       ├── InlinedFnLocalVar.ll
    │   │   │       ├── instcombine-instrinsics.ll
    │   │   │       ├── invalid-prologue-end.ll
    │   │   │       ├── isel-cse-line.ll
    │   │   │       ├── lazy-fission-comp-dir.ll
    │   │   │       ├── length_symbol_difference.ll
    │   │   │       ├── lexical-block-file-inline.ll
    │   │   │       ├── lexical_block.ll
    │   │   │       ├── line-info.ll
    │   │   │       ├── line.test
    │   │   │       ├── linkage-name.ll
    │   │   │       ├── lit.local.cfg
    │   │   │       ├── live-debug-values.ll
    │   │   │       ├── live-debug-variables.ll
    │   │   │       ├── live-debug-vars-discard-invalid.mir
    │   │   │       ├── live-debug-vars-dse.mir
    │   │   │       ├── live-debug-vars-index.mir
    │   │   │       ├── live-debug-vars-keep-undef.ll
    │   │   │       ├── loclists-dwp.ll
    │   │   │       ├── low-pc-cu.ll
    │   │   │       ├── main-file-name.s
    │   │   │       ├── mem2reg_fp80.ll
    │   │   │       ├── memberfnptr.ll
    │   │   │       ├── merge_inlined_loc.ll
    │   │   │       ├── mi-print.ll
    │   │   │       ├── misched-dbg-value.ll
    │   │   │       ├── missing-file-line.ll
    │   │   │       ├── mixed-nodebug-cu.ll
    │   │   │       ├── multiple-aranges.ll
    │   │   │       ├── multiple-at-const-val.ll
    │   │   │       ├── no-public-sections-metadata.ll
    │   │   │       ├── no_debug_ranges.ll
    │   │   │       ├── nodebug.ll
    │   │   │       ├── nodebug_with_debug_loc.ll
    │   │   │       ├── nondefault-subrange-array.ll
    │   │   │       ├── nophysreg.ll
    │   │   │       ├── noreturn_c11.ll
    │   │   │       ├── noreturn_cpp11.ll
    │   │   │       ├── noreturn_objc.ll
    │   │   │       ├── objc-fwd-decl.ll
    │   │   │       ├── objc-property-void.ll
    │   │   │       ├── op_deref.ll
    │   │   │       ├── parameters.ll
    │   │   │       ├── partial-constant.ll
    │   │   │       ├── pieces-1.ll
    │   │   │       ├── pieces-2.ll
    │   │   │       ├── pieces-3.ll
    │   │   │       ├── pieces-4.ll
    │   │   │       ├── pointer-type-size.ll
    │   │   │       ├── pr11300.ll
    │   │   │       ├── pr12831.ll
    │   │   │       ├── pr13303.ll
    │   │   │       ├── pr19307.mir
    │   │   │       ├── PR26148.ll
    │   │   │       ├── pr28270.ll
    │   │   │       ├── pr34545.ll
    │   │   │       ├── PR37234.ll
    │   │   │       ├── processes-relocations.ll
    │   │   │       ├── prologue-stack.ll
    │   │   │       ├── range_reloc.ll
    │   │   │       ├── range_reloc_base.ll
    │   │   │       ├── ref_addr_relocation.ll
    │   │   │       ├── reference-argument.ll
    │   │   │       ├── rematerialize.ll
    │   │   │       ├── rnglists_base_attr.ll
    │   │   │       ├── rnglists_curanges.ll
    │   │   │       ├── rvalue-ref.ll
    │   │   │       ├── safestack-byval.ll
    │   │   │       ├── sdag-combine.ll
    │   │   │       ├── sdag-dangling-dbgvalue.ll
    │   │   │       ├── sdag-dbgvalue-phi-use-1.ll
    │   │   │       ├── sdag-dbgvalue-phi-use-2.ll
    │   │   │       ├── sdag-dbgvalue-phi-use-3.ll
    │   │   │       ├── sdag-dbgvalue-phi-use-4.ll
    │   │   │       ├── sdag-legalize-multires.ll
    │   │   │       ├── sdag-salvage-add.ll
    │   │   │       ├── sdag-split-arg.ll
    │   │   │       ├── sdagsplit-1.ll
    │   │   │       ├── sections_as_references.ll
    │   │   │       ├── single-dbg_value.ll
    │   │   │       ├── single-fi.ll
    │   │   │       ├── spill-indirect-nrvo.ll
    │   │   │       ├── spill-nontrivial-param.ll
    │   │   │       ├── spill-nospill.ll
    │   │   │       ├── split-dwarf-cross-unit-reference.ll
    │   │   │       ├── split-dwarf-multiple-cu-hash.ll
    │   │   │       ├── split-dwarf-omit-empty.ll
    │   │   │       ├── split-dwarf-v5-ranges.ll
    │   │   │       ├── split-global.ll
    │   │   │       ├── sret.ll
    │   │   │       ├── sroasplit-1.ll
    │   │   │       ├── sroasplit-2.ll
    │   │   │       ├── sroasplit-3.ll
    │   │   │       ├── sroasplit-4.ll
    │   │   │       ├── sroasplit-5.ll
    │   │   │       ├── sroasplit-dbg-declare.ll
    │   │   │       ├── stack-args.ll
    │   │   │       ├── stack-value-dwarf2.ll
    │   │   │       ├── stack-value-dwarf4.ll
    │   │   │       ├── stack-value-piece.ll
    │   │   │       ├── static_member_array.ll
    │   │   │       ├── stmt-list-multiple-compile-units.ll
    │   │   │       ├── stmt-list.ll
    │   │   │       ├── string-offsets-multiple-cus.ll
    │   │   │       ├── string-offsets-table-order.ll
    │   │   │       ├── string-offsets-table.ll
    │   │   │       ├── stringpool.ll
    │   │   │       ├── strip-broken-debuginfo.ll
    │   │   │       ├── struct-loc.ll
    │   │   │       ├── subrange-type.ll
    │   │   │       ├── subreg.ll
    │   │   │       ├── subregisters.ll
    │   │   │       ├── tail-merge.ll
    │   │   │       ├── template.ll
    │   │   │       ├── this-stack_value.ll
    │   │   │       ├── tls.ll
    │   │   │       ├── type_units_with_addresses.ll
    │   │   │       ├── unattached-global.ll
    │   │   │       ├── union-const.ll
    │   │   │       ├── union-template.ll
    │   │   │       ├── v5-loc.ll
    │   │   │       ├── vector.ll
    │   │   │       ├── vla-dependencies.ll
    │   │   │       ├── vla-global.ll
    │   │   │       ├── vla-multi.ll
    │   │   │       ├── vla.ll
    │   │   │       ├── void-typedef.ll
    │   │   │       ├── xray-split-dwarf-interaction.ll
    │   │   │       └── zextload.ll
    │   │   ├── Examples/
    │   │   │   ├── lit.local.cfg
    │   │   │   └── Kaleidoscope/
    │   │   │       ├── Chapter3.test
    │   │   │       ├── Chapter4.test
    │   │   │       ├── Chapter5.test
    │   │   │       ├── Chapter6.test
    │   │   │       └── Chapter7.test
    │   │   ├── ExecutionEngine/
    │   │   │   ├── 2010-01-15-UndefValue.ll
    │   │   │   ├── fma3-jit.ll
    │   │   │   ├── frem.ll
    │   │   │   ├── lit.local.cfg
    │   │   │   ├── mov64zext32.ll
    │   │   │   ├── test-interp-vec-arithm_float.ll
    │   │   │   ├── test-interp-vec-arithm_int.ll
    │   │   │   ├── test-interp-vec-cast.ll
    │   │   │   ├── test-interp-vec-insertelement.ll
    │   │   │   ├── test-interp-vec-insertextractvalue.ll
    │   │   │   ├── test-interp-vec-loadstore.ll
    │   │   │   ├── test-interp-vec-logical.ll
    │   │   │   ├── test-interp-vec-select.ll
    │   │   │   ├── test-interp-vec-setcond-fp.ll
    │   │   │   ├── test-interp-vec-setcond-int.ll
    │   │   │   ├── test-interp-vec-shift.ll
    │   │   │   ├── test-interp-vec-shuffle.ll
    │   │   │   ├── Interpreter/
    │   │   │   │   ├── alias.ll
    │   │   │   │   ├── call-no-args.ll
    │   │   │   │   ├── intrinsics.ll
    │   │   │   │   └── lit.local.cfg
    │   │   │   ├── MCJIT/
    │   │   │   │   ├── 2002-12-16-ArgTest.ll
    │   │   │   │   ├── 2003-01-04-ArgumentBug.ll
    │   │   │   │   ├── 2003-01-04-LoopTest.ll
    │   │   │   │   ├── 2003-01-04-PhiTest.ll
    │   │   │   │   ├── 2003-01-09-SARTest.ll
    │   │   │   │   ├── 2003-01-10-FUCOM.ll
    │   │   │   │   ├── 2003-01-15-AlignmentTest.ll
    │   │   │   │   ├── 2003-05-06-LivenessClobber.ll
    │   │   │   │   ├── 2003-05-07-ArgumentTest.ll
    │   │   │   │   ├── 2003-05-11-PHIRegAllocBug.ll
    │   │   │   │   ├── 2003-06-04-bzip2-bug.ll
    │   │   │   │   ├── 2003-06-05-PHIBug.ll
    │   │   │   │   ├── 2003-08-15-AllocaAssertion.ll
    │   │   │   │   ├── 2003-08-21-EnvironmentTest.ll
    │   │   │   │   ├── 2003-08-23-RegisterAllocatePhysReg.ll
    │   │   │   │   ├── 2003-10-18-PHINode-ConstantExpr-CondCode-Failure.ll
    │   │   │   │   ├── 2005-12-02-TailCallBug.ll
    │   │   │   │   ├── 2007-12-10-APIntLoadStore.ll
    │   │   │   │   ├── 2008-06-05-APInt-OverAShr.ll
    │   │   │   │   ├── 2013-04-04-RelocAddend.ll
    │   │   │   │   ├── cross-module-a.ll
    │   │   │   │   ├── cross-module-sm-pic-a.ll
    │   │   │   │   ├── eh-lg-pic.ll
    │   │   │   │   ├── eh.ll
    │   │   │   │   ├── fpbitcast.ll
    │   │   │   │   ├── hello.ll
    │   │   │   │   ├── hello2.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── load-object-a.ll
    │   │   │   │   ├── multi-module-a.ll
    │   │   │   │   ├── multi-module-eh-a.ll
    │   │   │   │   ├── multi-module-sm-pic-a.ll
    │   │   │   │   ├── non-extern-addend.ll
    │   │   │   │   ├── pr13727.ll
    │   │   │   │   ├── simplesttest.ll
    │   │   │   │   ├── simpletest.ll
    │   │   │   │   ├── stubs-sm-pic.ll
    │   │   │   │   ├── stubs.ll
    │   │   │   │   ├── test-arith.ll
    │   │   │   │   ├── test-branch.ll
    │   │   │   │   ├── test-call-no-external-funcs.ll
    │   │   │   │   ├── test-call.ll
    │   │   │   │   ├── test-cast.ll
    │   │   │   │   ├── test-common-symbols-alignment.ll
    │   │   │   │   ├── test-common-symbols.ll
    │   │   │   │   ├── test-constantexpr.ll
    │   │   │   │   ├── test-data-align.ll
    │   │   │   │   ├── test-fp-no-external-funcs.ll
    │   │   │   │   ├── test-fp.ll
    │   │   │   │   ├── test-global-ctors.ll
    │   │   │   │   ├── test-global-init-nonzero-sm-pic.ll
    │   │   │   │   ├── test-global-init-nonzero.ll
    │   │   │   │   ├── test-global.ll
    │   │   │   │   ├── test-loadstore.ll
    │   │   │   │   ├── test-local.ll
    │   │   │   │   ├── test-logical.ll
    │   │   │   │   ├── test-loop.ll
    │   │   │   │   ├── test-phi.ll
    │   │   │   │   ├── test-ptr-reloc-sm-pic.ll
    │   │   │   │   ├── test-ptr-reloc.ll
    │   │   │   │   ├── test-ret.ll
    │   │   │   │   ├── test-return.ll
    │   │   │   │   ├── test-setcond-fp.ll
    │   │   │   │   ├── test-setcond-int.ll
    │   │   │   │   ├── test-shift.ll
    │   │   │   │   ├── weak-function.ll
    │   │   │   │   ├── Inputs/
    │   │   │   │   │   ├── cross-module-b.ll
    │   │   │   │   │   ├── multi-module-b.ll
    │   │   │   │   │   ├── multi-module-c.ll
    │   │   │   │   │   ├── multi-module-eh-b.ll
    │   │   │   │   │   └── weak-function-2.ll
    │   │   │   │   └── remote/
    │   │   │   │       ├── cross-module-a.ll
    │   │   │   │       ├── eh.ll
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── multi-module-a.ll
    │   │   │   │       ├── simpletest-remote.ll
    │   │   │   │       ├── stubs-remote.ll
    │   │   │   │       ├── stubs-sm-pic.ll
    │   │   │   │       ├── test-common-symbols-remote.ll
    │   │   │   │       ├── test-data-align-remote.ll
    │   │   │   │       ├── test-fp-no-external-funcs-remote.ll
    │   │   │   │       ├── test-global-init-nonzero-remote.ll
    │   │   │   │       ├── test-global-init-nonzero-sm-pic.ll
    │   │   │   │       ├── test-ptr-reloc-remote.ll
    │   │   │   │       ├── test-ptr-reloc-sm-pic.ll
    │   │   │   │       └── Inputs/
    │   │   │   │           ├── cross-module-b.ll
    │   │   │   │           ├── multi-module-b.ll
    │   │   │   │           └── multi-module-c.ll
    │   │   │   ├── OrcLazy/
    │   │   │   │   ├── anonymous_globals.ll
    │   │   │   │   ├── bad-object-file.ll
    │   │   │   │   ├── basic-object-file-loading.ll
    │   │   │   │   ├── basic-whole-module-partitions.ll
    │   │   │   │   ├── common-symbols.ll
    │   │   │   │   ├── global-ctors-and-dtors.ll
    │   │   │   │   ├── global_aliases.ll
    │   │   │   │   ├── hidden-visibility.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── minimal.ll
    │   │   │   │   ├── module-flags.ll
    │   │   │   │   ├── multiple-compile-threads-basic.ll
    │   │   │   │   ├── private_linkage.ll
    │   │   │   │   ├── single-function-call.ll
    │   │   │   │   ├── weak-function.ll
    │   │   │   │   ├── weak-non-materialization.ll
    │   │   │   │   └── Inputs/
    │   │   │   │       ├── basic-object-source.ll
    │   │   │   │       ├── hidden-definitions.ll
    │   │   │   │       ├── obj-weak-non-materialization-1.ll
    │   │   │   │       ├── obj-weak-non-materialization-2.ll
    │   │   │   │       └── weak-function-2.ll
    │   │   │   ├── OrcMCJIT/
    │   │   │   │   ├── 2002-12-16-ArgTest.ll
    │   │   │   │   ├── 2003-01-04-ArgumentBug.ll
    │   │   │   │   ├── 2003-01-04-LoopTest.ll
    │   │   │   │   ├── 2003-01-04-PhiTest.ll
    │   │   │   │   ├── 2003-01-09-SARTest.ll
    │   │   │   │   ├── 2003-01-10-FUCOM.ll
    │   │   │   │   ├── 2003-01-15-AlignmentTest.ll
    │   │   │   │   ├── 2003-05-06-LivenessClobber.ll
    │   │   │   │   ├── 2003-05-07-ArgumentTest.ll
    │   │   │   │   ├── 2003-05-11-PHIRegAllocBug.ll
    │   │   │   │   ├── 2003-06-04-bzip2-bug.ll
    │   │   │   │   ├── 2003-06-05-PHIBug.ll
    │   │   │   │   ├── 2003-08-15-AllocaAssertion.ll
    │   │   │   │   ├── 2003-08-21-EnvironmentTest.ll
    │   │   │   │   ├── 2003-08-23-RegisterAllocatePhysReg.ll
    │   │   │   │   ├── 2003-10-18-PHINode-ConstantExpr-CondCode-Failure.ll
    │   │   │   │   ├── 2005-12-02-TailCallBug.ll
    │   │   │   │   ├── 2007-12-10-APIntLoadStore.ll
    │   │   │   │   ├── 2008-06-05-APInt-OverAShr.ll
    │   │   │   │   ├── 2013-04-04-RelocAddend.ll
    │   │   │   │   ├── cross-module-a.ll
    │   │   │   │   ├── cross-module-sm-pic-a.ll
    │   │   │   │   ├── eh-lg-pic.ll
    │   │   │   │   ├── eh.ll
    │   │   │   │   ├── fpbitcast.ll
    │   │   │   │   ├── hello.ll
    │   │   │   │   ├── hello2.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── load-object-a.ll
    │   │   │   │   ├── multi-module-a.ll
    │   │   │   │   ├── multi-module-eh-a.ll
    │   │   │   │   ├── multi-module-sm-pic-a.ll
    │   │   │   │   ├── non-extern-addend.ll
    │   │   │   │   ├── pr13727.ll
    │   │   │   │   ├── pr32650.ll
    │   │   │   │   ├── simplesttest.ll
    │   │   │   │   ├── simpletest.ll
    │   │   │   │   ├── stubs-sm-pic.ll
    │   │   │   │   ├── stubs.ll
    │   │   │   │   ├── test-arith.ll
    │   │   │   │   ├── test-branch.ll
    │   │   │   │   ├── test-call-no-external-funcs.ll
    │   │   │   │   ├── test-call.ll
    │   │   │   │   ├── test-cast.ll
    │   │   │   │   ├── test-common-symbols-alignment.ll
    │   │   │   │   ├── test-common-symbols.ll
    │   │   │   │   ├── test-constantexpr.ll
    │   │   │   │   ├── test-data-align.ll
    │   │   │   │   ├── test-fp-no-external-funcs.ll
    │   │   │   │   ├── test-fp.ll
    │   │   │   │   ├── test-global-ctors.ll
    │   │   │   │   ├── test-global-init-nonzero-sm-pic.ll
    │   │   │   │   ├── test-global-init-nonzero.ll
    │   │   │   │   ├── test-global.ll
    │   │   │   │   ├── test-loadstore.ll
    │   │   │   │   ├── test-local.ll
    │   │   │   │   ├── test-logical.ll
    │   │   │   │   ├── test-loop.ll
    │   │   │   │   ├── test-phi.ll
    │   │   │   │   ├── test-ptr-reloc-sm-pic.ll
    │   │   │   │   ├── test-ptr-reloc.ll
    │   │   │   │   ├── test-ret.ll
    │   │   │   │   ├── test-return.ll
    │   │   │   │   ├── test-setcond-fp.ll
    │   │   │   │   ├── test-setcond-int.ll
    │   │   │   │   ├── test-shift.ll
    │   │   │   │   ├── weak-function.ll
    │   │   │   │   ├── Inputs/
    │   │   │   │   │   ├── cross-module-b.ll
    │   │   │   │   │   ├── multi-module-b.ll
    │   │   │   │   │   ├── multi-module-c.ll
    │   │   │   │   │   ├── multi-module-eh-b.ll
    │   │   │   │   │   └── weak-function-2.ll
    │   │   │   │   └── remote/
    │   │   │   │       ├── cross-module-a.ll
    │   │   │   │       ├── eh.ll
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── multi-module-a.ll
    │   │   │   │       ├── simpletest-remote.ll
    │   │   │   │       ├── stubs-remote.ll
    │   │   │   │       ├── stubs-sm-pic.ll
    │   │   │   │       ├── test-common-symbols-remote.ll
    │   │   │   │       ├── test-data-align-remote.ll
    │   │   │   │       ├── test-fp-no-external-funcs-remote.ll
    │   │   │   │       ├── test-global-init-nonzero-remote.ll
    │   │   │   │       ├── test-global-init-nonzero-sm-pic.ll
    │   │   │   │       ├── test-ptr-reloc-remote.ll
    │   │   │   │       ├── test-ptr-reloc-sm-pic.ll
    │   │   │   │       └── Inputs/
    │   │   │   │           ├── cross-module-b.ll
    │   │   │   │           ├── multi-module-b.ll
    │   │   │   │           └── multi-module-c.ll
    │   │   │   └── RuntimeDyld/
    │   │   │       ├── AArch64/
    │   │   │       │   ├── ELF_ARM64_BE-relocations.s
    │   │   │       │   ├── ELF_ARM64_local_branch.s
    │   │   │       │   ├── ELF_ARM64_PIC_relocations.s
    │   │   │       │   ├── ELF_ARM64_relocations.s
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   └── MachO_ARM64_relocations.s
    │   │   │       ├── ARM/
    │   │   │       │   ├── COFF_Thumb.s
    │   │   │       │   ├── ELF_ARM_EXIDX_relocations.s
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   ├── MachO_ARM_PIC_relocations.s
    │   │   │       │   └── MachO_Thumb_Relocations.s
    │   │   │       ├── Mips/
    │   │   │       │   ├── ELF_Mips64r2N64_PIC_relocations.s
    │   │   │       │   ├── ELF_N32_relocations.s
    │   │   │       │   ├── ELF_N64R6_relocations.s
    │   │   │       │   ├── ELF_O32_PIC_relocations.s
    │   │   │       │   ├── ELF_O32R6_relocations.s
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   └── Inputs/
    │   │   │       │       └── ExternalFunction.ll
    │   │   │       ├── PowerPC/
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   ├── ppc32_elf_rel_addr16.s
    │   │   │       │   ├── ppc64_elf.s
    │   │   │       │   ├── ppc64_reloc.s
    │   │   │       │   └── Inputs/
    │   │   │       │       └── ppc64_elf_module_b.s
    │   │   │       ├── SystemZ/
    │   │   │       │   ├── cfi-relo-pc64.s
    │   │   │       │   ├── lit.local.cfg
    │   │   │       │   └── Inputs/
    │   │   │       │       └── rtdyld-globals.ll
    │   │   │       └── X86/
    │   │   │           ├── coff-alignment.ll
    │   │   │           ├── COFF_i386.s
    │   │   │           ├── COFF_x86_64.s
    │   │   │           ├── COFF_x86_64_IMGREL.s
    │   │   │           ├── CommonSymbols_allocation.s
    │   │   │           ├── ELF-large-pic-relocations.s
    │   │   │           ├── ELF-relaxed.s
    │   │   │           ├── ELF_STT_FILE.s
    │   │   │           ├── ELF_x64-64_PC8_relocations.s
    │   │   │           ├── ELF_x64-64_PIC_relocations.s
    │   │   │           ├── ELF_x86-64_debug_frame.s
    │   │   │           ├── ELF_x86-64_none.yaml
    │   │   │           ├── ELF_x86-64_PIC-small-relocations.s
    │   │   │           ├── ELF_x86_64_StubBuf.s
    │   │   │           ├── lit.local.cfg
    │   │   │           ├── MachO_empty_ehframe.s
    │   │   │           ├── MachO_i386_DynNoPIC_relocations.s
    │   │   │           ├── MachO_i386_eh_frame.s
    │   │   │           ├── MachO_x86-64_PIC_relocations.s
    │   │   │           └── Inputs/
    │   │   │               ├── ELF_STT_FILE_FILE.s
    │   │   │               ├── ELF_STT_FILE_GLOBAL.s
    │   │   │               ├── ELF_x86_64_StubBuf.ll
    │   │   │               └── ExternalGlobal.ll
    │   │   ├── Linker/
    │   │   │   ├── 2002-07-17-GlobalFail.ll
    │   │   │   ├── 2002-07-17-LinkTest2.ll
    │   │   │   ├── 2002-08-20-ConstantExpr.ll
    │   │   │   ├── 2003-01-30-LinkerRename.ll
    │   │   │   ├── 2003-01-30-LinkerTypeRename.ll
    │   │   │   ├── 2003-04-23-LinkOnceLost.ll
    │   │   │   ├── 2003-04-26-NullPtrLinkProblem.ll
    │   │   │   ├── 2003-05-15-TypeProblem.ll
    │   │   │   ├── 2003-05-31-LinkerRename.ll
    │   │   │   ├── 2003-06-02-TypeResolveProblem.ll
    │   │   │   ├── 2003-06-02-TypeResolveProblem2.ll
    │   │   │   ├── 2003-08-20-OpaqueTypeResolve.ll
    │   │   │   ├── 2003-08-23-GlobalVarLinking.ll
    │   │   │   ├── 2003-08-23-RecursiveOpaqueTypeResolve.ll
    │   │   │   ├── 2003-08-24-InheritPtrSize.ll
    │   │   │   ├── 2003-08-28-TypeResolvesGlobal.ll
    │   │   │   ├── 2003-08-28-TypeResolvesGlobal2.ll
    │   │   │   ├── 2003-08-28-TypeResolvesGlobal3.ll
    │   │   │   ├── 2003-10-27-LinkOncePromote.ll
    │   │   │   ├── 2003-11-18-TypeResolution.ll
    │   │   │   ├── 2004-02-17-WeakStrongLinkage.ll
    │   │   │   ├── 2004-05-07-TypeResolution1.ll
    │   │   │   ├── 2004-05-07-TypeResolution2.ll
    │   │   │   ├── 2004-12-03-DisagreeingType.ll
    │   │   │   ├── 2005-02-12-ConstantGlobals-2.ll
    │   │   │   ├── 2005-02-12-ConstantGlobals.ll
    │   │   │   ├── 2005-12-06-AppendingZeroLengthArrays.ll
    │   │   │   ├── 2006-01-19-ConstantPacked.ll
    │   │   │   ├── 2008-03-05-AliasReference.ll
    │   │   │   ├── 2008-03-05-AliasReference2.ll
    │   │   │   ├── 2008-03-07-DroppedSection_a.ll
    │   │   │   ├── 2008-03-07-DroppedSection_b.ll
    │   │   │   ├── 2008-06-13-LinkOnceRedefinition.ll
    │   │   │   ├── 2008-06-26-AddressSpace.ll
    │   │   │   ├── 2008-07-06-AliasFnDecl.ll
    │   │   │   ├── 2008-07-06-AliasFnDecl2.ll
    │   │   │   ├── 2008-07-06-AliasWeakDest.ll
    │   │   │   ├── 2008-07-06-AliasWeakDest2.ll
    │   │   │   ├── 2009-09-03-mdnode.ll
    │   │   │   ├── 2009-09-03-mdnode2.ll
    │   │   │   ├── 2011-08-04-DebugLoc.ll
    │   │   │   ├── 2011-08-04-DebugLoc2.ll
    │   │   │   ├── 2011-08-04-Metadata.ll
    │   │   │   ├── 2011-08-04-Metadata2.ll
    │   │   │   ├── 2011-08-18-unique-class-type.ll
    │   │   │   ├── 2011-08-18-unique-class-type2.ll
    │   │   │   ├── 2011-08-18-unique-debug-type.ll
    │   │   │   ├── 2011-08-18-unique-debug-type2.ll
    │   │   │   ├── alias-2.ll
    │   │   │   ├── alias-3.ll
    │   │   │   ├── alias.ll
    │   │   │   ├── alignment.ll
    │   │   │   ├── AppendingLinkage.ll
    │   │   │   ├── AppendingLinkage2.ll
    │   │   │   ├── apple-version.ll
    │   │   │   ├── available_externally_a.ll
    │   │   │   ├── available_externally_b.ll
    │   │   │   ├── available_externally_over_decl.ll
    │   │   │   ├── basiclink.ll
    │   │   │   ├── broken.ll
    │   │   │   ├── comdat-rm-dst.ll
    │   │   │   ├── comdat.ll
    │   │   │   ├── comdat10.ll
    │   │   │   ├── comdat11.ll
    │   │   │   ├── comdat12.ll
    │   │   │   ├── comdat13.ll
    │   │   │   ├── comdat14.ll
    │   │   │   ├── comdat15.ll
    │   │   │   ├── comdat16.ll
    │   │   │   ├── comdat2.ll
    │   │   │   ├── comdat4.ll
    │   │   │   ├── comdat5.ll
    │   │   │   ├── comdat6.ll
    │   │   │   ├── comdat7.ll
    │   │   │   ├── comdat8.ll
    │   │   │   ├── comdat9.ll
    │   │   │   ├── comdat_group.ll
    │   │   │   ├── commandline.ll
    │   │   │   ├── ConstantGlobals.ll
    │   │   │   ├── constructor-comdat.ll
    │   │   │   ├── ctors.ll
    │   │   │   ├── ctors2.ll
    │   │   │   ├── ctors3.ll
    │   │   │   ├── ctors4.ll
    │   │   │   ├── ctors5.ll
    │   │   │   ├── datalayout.ll
    │   │   │   ├── DbgDeclare.ll
    │   │   │   ├── DbgDeclare2.ll
    │   │   │   ├── debug-info-global-var.ll
    │   │   │   ├── debug-info-version-a.ll
    │   │   │   ├── debug-info-version-b.ll
    │   │   │   ├── dicompositetype-unique.ll
    │   │   │   ├── distinct-cycles.ll
    │   │   │   ├── distinct.ll
    │   │   │   ├── dllstorage-a.ll
    │   │   │   ├── dllstorage-b.ll
    │   │   │   ├── drop-debug.ll
    │   │   │   ├── func-attrs-a.ll
    │   │   │   ├── func-attrs-b.ll
    │   │   │   ├── funcimport.ll
    │   │   │   ├── funcimport2.ll
    │   │   │   ├── funcimport_appending_global.ll
    │   │   │   ├── funcimport_comdat.ll
    │   │   │   ├── global_ctors.ll
    │   │   │   ├── ident.ll
    │   │   │   ├── inlineasm.ll
    │   │   │   ├── internalize-lazy.ll
    │   │   │   ├── link-arm-and-thumb-module-inline-asm.ll
    │   │   │   ├── link-arm-and-thumb.ll
    │   │   │   ├── link-flags.ll
    │   │   │   ├── link-global-to-func.ll
    │   │   │   ├── link-type-names.ll
    │   │   │   ├── linkage.ll
    │   │   │   ├── linkage2.ll
    │   │   │   ├── linkmdnode.ll
    │   │   │   ├── linkmdnode2.ll
    │   │   │   ├── linknamedmdnode.ll
    │   │   │   ├── linknamedmdnode2.ll
    │   │   │   ├── LinkOnce.ll
    │   │   │   ├── lto-attributes.ll
    │   │   │   ├── mdlocation.ll
    │   │   │   ├── metadata-a.ll
    │   │   │   ├── metadata-attach.ll
    │   │   │   ├── metadata-b.ll
    │   │   │   ├── metadata-function.ll
    │   │   │   ├── metadata-global.ll
    │   │   │   ├── metadata-mismatch.test
    │   │   │   ├── metadata-source.ll
    │   │   │   ├── metadata-with-global-value-operand.ll
    │   │   │   ├── module-flags-1-a.ll
    │   │   │   ├── module-flags-1-b.ll
    │   │   │   ├── module-flags-2-a.ll
    │   │   │   ├── module-flags-2-b.ll
    │   │   │   ├── module-flags-3-a.ll
    │   │   │   ├── module-flags-3-b.ll
    │   │   │   ├── module-flags-4-a.ll
    │   │   │   ├── module-flags-4-b.ll
    │   │   │   ├── module-flags-5-a.ll
    │   │   │   ├── module-flags-5-b.ll
    │   │   │   ├── module-flags-6-a.ll
    │   │   │   ├── module-flags-6-b.ll
    │   │   │   ├── module-flags-7-a.ll
    │   │   │   ├── module-flags-7-b.ll
    │   │   │   ├── module-flags-8-a.ll
    │   │   │   ├── module-flags-8-b.ll
    │   │   │   ├── module-flags-dont-change-others.ll
    │   │   │   ├── module-flags-pic-1-a.ll
    │   │   │   ├── module-flags-pic-2-a.ll
    │   │   │   ├── multiple-merged-structs.ll
    │   │   │   ├── null_mapping_constant.ll
    │   │   │   ├── objectivec-class-property-flag-mismatch.ll
    │   │   │   ├── odr-lambda-1.ll
    │   │   │   ├── odr.ll
    │   │   │   ├── only-needed-compiler-used.ll
    │   │   │   ├── only-needed-ctors1.ll
    │   │   │   ├── only-needed-ctors2.ll
    │   │   │   ├── only-needed-debug-metadata.ll
    │   │   │   ├── only-needed-dtors1.ll
    │   │   │   ├── only-needed-dtors2.ll
    │   │   │   ├── only-needed-named-metadata.ll
    │   │   │   ├── only-needed-recurse.ll
    │   │   │   ├── only-needed-used.ll
    │   │   │   ├── opaque.ll
    │   │   │   ├── override-different-linkage.ll
    │   │   │   ├── override-with-internal-linkage-2.ll
    │   │   │   ├── override-with-internal-linkage.ll
    │   │   │   ├── override.ll
    │   │   │   ├── partial-type-refinement-link.ll
    │   │   │   ├── partial-type-refinement.ll
    │   │   │   ├── pr21374.ll
    │   │   │   ├── pr21494.ll
    │   │   │   ├── pr22807.ll
    │   │   │   ├── pr26037.ll
    │   │   │   ├── pr27044.ll
    │   │   │   ├── PR8300.ll
    │   │   │   ├── prologuedata.ll
    │   │   │   ├── redefinition.ll
    │   │   │   ├── replaced-function-matches-first-subprogram.ll
    │   │   │   ├── subprogram-linkonce-weak.ll
    │   │   │   ├── syncscopes.ll
    │   │   │   ├── targettriple.ll
    │   │   │   ├── testlink.ll
    │   │   │   ├── thinlto_funcimport_debug.ll
    │   │   │   ├── transitive-lazy-link.ll
    │   │   │   ├── type-unique-alias.ll
    │   │   │   ├── type-unique-dst-types.ll
    │   │   │   ├── type-unique-inheritance.ll
    │   │   │   ├── type-unique-name.ll
    │   │   │   ├── type-unique-odr-a.ll
    │   │   │   ├── type-unique-odr-b.ll
    │   │   │   ├── type-unique-opaque.ll
    │   │   │   ├── type-unique-simple-a.ll
    │   │   │   ├── type-unique-simple-b.ll
    │   │   │   ├── type-unique-simple2-a.ll
    │   │   │   ├── type-unique-simple2-b.ll
    │   │   │   ├── type-unique-simple2.ll
    │   │   │   ├── type-unique-src-type.ll
    │   │   │   ├── type-unique-type-array-a.ll
    │   │   │   ├── type-unique-type-array-b.ll
    │   │   │   ├── type-unique-unrelated.ll
    │   │   │   ├── unique-fwd-decl-a.ll
    │   │   │   ├── unique-fwd-decl-order.ll
    │   │   │   ├── uniqued-distinct-cycles.ll
    │   │   │   ├── unnamed-addr-err-a.ll
    │   │   │   ├── unnamed-addr-err-b.ll
    │   │   │   ├── unnamed-addr1-a.ll
    │   │   │   ├── unnamed-addr1-b.ll
    │   │   │   ├── visibility.ll
    │   │   │   ├── weakextern.ll
    │   │   │   ├── wrong-addrspace-gv-declaration.ll
    │   │   │   └── Inputs/
    │   │   │       ├── 2003-01-30-LinkerRename.ll
    │   │   │       ├── 2003-05-31-LinkerRename.ll
    │   │   │       ├── alias-2.ll
    │   │   │       ├── alias.ll
    │   │   │       ├── alignment.ll
    │   │   │       ├── available_externally_over_decl.ll
    │   │   │       ├── basiclink.a.ll
    │   │   │       ├── basiclink.b.ll
    │   │   │       ├── comdat-rm-dst.ll
    │   │   │       ├── comdat.ll
    │   │   │       ├── comdat11.ll
    │   │   │       ├── comdat13.ll
    │   │   │       ├── comdat14.ll
    │   │   │       ├── comdat15.ll
    │   │   │       ├── comdat16.ll
    │   │   │       ├── comdat2.ll
    │   │   │       ├── comdat3.ll
    │   │   │       ├── comdat4.ll
    │   │   │       ├── comdat5.ll
    │   │   │       ├── comdat8.ll
    │   │   │       ├── commandline.a.ll
    │   │   │       ├── commandline.b.ll
    │   │   │       ├── ConstantGlobals.ll
    │   │   │       ├── constructor-comdat.ll
    │   │   │       ├── ctors.ll
    │   │   │       ├── ctors2.ll
    │   │   │       ├── ctors3.ll
    │   │   │       ├── datalayout-a.ll
    │   │   │       ├── datalayout-b.ll
    │   │   │       ├── dicompositetype-unique.ll
    │   │   │       ├── distinct.ll
    │   │   │       ├── drop-debug.bc
    │   │   │       ├── funcimport.ll
    │   │   │       ├── funcimport2.ll
    │   │   │       ├── funcimport_appending_global.ll
    │   │   │       ├── funcimport_comdat.ll
    │   │   │       ├── ident.a.ll
    │   │   │       ├── ident.b.ll
    │   │   │       ├── internalize-lazy.ll
    │   │   │       ├── linkage.a.ll
    │   │   │       ├── linkage.b.ll
    │   │   │       ├── linkage.c.ll
    │   │   │       ├── linkage.d.ll
    │   │   │       ├── linkage2.ll
    │   │   │       ├── mdlocation.ll
    │   │   │       ├── metadata-attach.ll
    │   │   │       ├── metadata-function.ll
    │   │   │       ├── metadata-mismatch-a.ll
    │   │   │       ├── metadata-mismatch-b.ll
    │   │   │       ├── metadata-source-a.ll
    │   │   │       ├── metadata-source-b.ll
    │   │   │       ├── metadata-with-global-value-operand.ll
    │   │   │       ├── module-flags-dont-change-others.ll
    │   │   │       ├── module-flags-pic-1-b.ll
    │   │   │       ├── module-flags-pic-2-b.ll
    │   │   │       ├── objectivec-class-property-flag-mismatch.ll
    │   │   │       ├── odr-lambda-2.ll
    │   │   │       ├── odr.ll
    │   │   │       ├── old_global_ctors.3.4.bc
    │   │   │       ├── only-needed-compiler-used.ll
    │   │   │       ├── only-needed-ctors.ll
    │   │   │       ├── only-needed-debug-metadata.ll
    │   │   │       ├── only-needed-dtors.ll
    │   │   │       ├── only-needed-named-metadata.ll
    │   │   │       ├── only-needed-recurse.ll
    │   │   │       ├── only-needed-used.ll
    │   │   │       ├── opaque.ll
    │   │   │       ├── override-different-linkage.ll
    │   │   │       ├── override-with-internal-linkage-2.ll
    │   │   │       ├── override-with-internal-linkage.ll
    │   │   │       ├── override.ll
    │   │   │       ├── PR11464.a.ll
    │   │   │       ├── PR11464.b.ll
    │   │   │       ├── pr21374.ll
    │   │   │       ├── pr22807-1.ll
    │   │   │       ├── pr22807-2.ll
    │   │   │       ├── pr26037.ll
    │   │   │       ├── pr27044.ll
    │   │   │       ├── PR8300.a.ll
    │   │   │       ├── PR8300.b.ll
    │   │   │       ├── redefinition.ll
    │   │   │       ├── replaced-function-matches-first-subprogram.ll
    │   │   │       ├── subprogram-linkonce-weak.ll
    │   │   │       ├── syncscope-1.ll
    │   │   │       ├── syncscope-2.ll
    │   │   │       ├── targettriple-a.ll
    │   │   │       ├── targettriple-b.ll
    │   │   │       ├── targettriple-c.ll
    │   │   │       ├── testlink.ll
    │   │   │       ├── thinlto_funcimport_debug.ll
    │   │   │       ├── thumb-module-inline-asm.ll
    │   │   │       ├── thumb.ll
    │   │   │       ├── type-unique-alias.ll
    │   │   │       ├── type-unique-dst-types2.ll
    │   │   │       ├── type-unique-dst-types3.ll
    │   │   │       ├── type-unique-inheritance-a.ll
    │   │   │       ├── type-unique-inheritance-b.ll
    │   │   │       ├── type-unique-name.ll
    │   │   │       ├── type-unique-opaque.ll
    │   │   │       ├── type-unique-simple2-a.ll
    │   │   │       ├── type-unique-simple2-b.ll
    │   │   │       ├── type-unique-unrelated2.ll
    │   │   │       ├── type-unique-unrelated3.ll
    │   │   │       ├── unique-fwd-decl-b.ll
    │   │   │       ├── unique-fwd-decl-order.ll
    │   │   │       ├── visibility.ll
    │   │   │       ├── wrong-addrspace-gv-declaration.ll
    │   │   │       └── apple-version/
    │   │   │           ├── 1.ll
    │   │   │           ├── 2.ll
    │   │   │           ├── 3.ll
    │   │   │           └── 4.ll
    │   │   ├── LTO/
    │   │   │   ├── ARM/
    │   │   │   │   ├── inline-asm.ll
    │   │   │   │   ├── link-arm-and-thumb.ll
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── runtime-library-subtarget.ll
    │   │   │   │   └── Inputs/
    │   │   │   │       └── thumb.ll
    │   │   │   ├── Resolution/
    │   │   │   │   └── X86/
    │   │   │   │       ├── alias-alias.ll
    │   │   │   │       ├── alias.ll
    │   │   │   │       ├── asm-output.ll
    │   │   │   │       ├── available-externally.ll
    │   │   │   │       ├── cache-dso-local.ll
    │   │   │   │       ├── cache-dso-local2.ll
    │   │   │   │       ├── cache-prevailing.ll
    │   │   │   │       ├── comdat-mixed-lto.ll
    │   │   │   │       ├── comdat.ll
    │   │   │   │       ├── common2.ll
    │   │   │   │       ├── commons.ll
    │   │   │   │       ├── dead-strip-alias.ll
    │   │   │   │       ├── dead-strip-fulllto.ll
    │   │   │   │       ├── diagnostic-handler-remarks-with-hotness.ll
    │   │   │   │       ├── diagnostic-handler-remarks.ll
    │   │   │   │       ├── empty-bitcode.test
    │   │   │   │       ├── export-jumptable.ll
    │   │   │   │       ├── function-alias-non-prevailing.ll
    │   │   │   │       ├── ifunc.ll
    │   │   │   │       ├── intrinsic.ll
    │   │   │   │       ├── link-odr-availextern.ll
    │   │   │   │       ├── linker-redef-thin.ll
    │   │   │   │       ├── linker-redef.ll
    │   │   │   │       ├── linkonce.ll
    │   │   │   │       ├── lit.local.cfg
    │   │   │   │       ├── load-sample-prof-icp.ll
    │   │   │   │       ├── load-sample-prof-lto.ll
    │   │   │   │       ├── load-sample-prof.ll
    │   │   │   │       ├── local-def-dllimport.ll
    │   │   │   │       ├── lowertypetests.ll
    │   │   │   │       ├── lto-unit-check.ll
    │   │   │   │       ├── mixed_lto.ll
    │   │   │   │       ├── mod-asm-used.ll
    │   │   │   │       ├── multi-thinlto.ll
    │   │   │   │       ├── not-prevailing-alias.ll
    │   │   │   │       ├── not-prevailing-variables.ll
    │   │   │   │       ├── not-prevailing.ll
    │   │   │   │       ├── setting-dso-local.ll
    │   │   │   │       ├── symtab-elf.ll
    │   │   │   │       ├── symtab.ll
    │   │   │   │       ├── type-checked-load.ll
    │   │   │   │       └── Inputs/
    │   │   │   │           ├── alias-1.ll
    │   │   │   │           ├── alias-alias-1.ll
    │   │   │   │           ├── comdat-mixed-lto.ll
    │   │   │   │           ├── comdat.ll
    │   │   │   │           ├── common2.ll
    │   │   │   │           ├── commons.ll
    │   │   │   │           ├── dead-strip-alias.ll
    │   │   │   │           ├── dead-strip-fulllto.ll
    │   │   │   │           ├── intrinsic.ll
    │   │   │   │           ├── link-odr-availextern-ae.ll
    │   │   │   │           ├── link-odr-availextern-odr.ll
    │   │   │   │           ├── load-sample-prof-icp.prof
    │   │   │   │           ├── load-sample-prof.prof
    │   │   │   │           ├── mixed_lto.ll
    │   │   │   │           ├── mod-asm-used.ll
    │   │   │   │           └── not-prevailing.ll
    │   │   │   └── X86/
    │   │   │       ├── attrs.ll
    │   │   │       ├── bcsection.ll
    │   │   │       ├── cfi_endproc.ll
    │   │   │       ├── codemodel-1.ll
    │   │   │       ├── codemodel-2.ll
    │   │   │       ├── codemodel-3.ll
    │   │   │       ├── current-section.ll
    │   │   │       ├── diagnostic-handler-noexit.ll
    │   │   │       ├── diagnostic-handler-remarks-with-hotness.ll
    │   │   │       ├── diagnostic-handler-remarks.ll
    │   │   │       ├── disable-verify.ll
    │   │   │       ├── dllimport.ll
    │   │   │       ├── internalize.ll
    │   │   │       ├── invalid.ll
    │   │   │       ├── keep-used-puts-during-instcombine.ll
    │   │   │       ├── libcall-overridden-via-alias.ll
    │   │   │       ├── linkonce_odr_func.ll
    │   │   │       ├── list-symbols.ll
    │   │   │       ├── lit.local.cfg
    │   │   │       ├── llvm-lto-output.ll
    │   │   │       ├── no-undefined-puts-when-implemented.ll
    │   │   │       ├── objc-detection-i386.ll
    │   │   │       ├── objc-detection.ll
    │   │   │       ├── parallel.ll
    │   │   │       ├── pr25919.ll
    │   │   │       ├── pr38046.ll
    │   │   │       ├── private-symbol.ll
    │   │   │       ├── remangle_intrinsics.ll
    │   │   │       ├── remangle_intrinsics_tbaa.ll
    │   │   │       ├── restore-externals.ll
    │   │   │       ├── runtime-library.ll
    │   │   │       ├── set-merged.ll
    │   │   │       ├── stdcall.ll
    │   │   │       ├── strip-debug-info-no-call-loc.ll
    │   │   │       ├── strip-debug-info.ll
    │   │   │       ├── symver-asm.ll
    │   │   │       ├── symver-asm2.ll
    │   │   │       ├── symver-asm3.ll
    │   │   │       ├── triple-init.ll
    │   │   │       ├── triple-init2.ll
    │   │   │       ├── type-mapping-bug.ll
    │   │   │       ├── type-mapping-bug2.ll
    │   │   │       ├── unnamed.ll
    │   │   │       └── Inputs/
    │   │   │           ├── bcsection.macho.s
    │   │   │           ├── bcsection.s
    │   │   │           ├── codemodel-3.ll
    │   │   │           ├── dllimport.ll
    │   │   │           ├── invalid.ll.bc
    │   │   │           ├── list-symbols.ll
    │   │   │           ├── remangle_intrinsics.ll
    │   │   │           ├── remangle_intrinsics_tbaa.ll
    │   │   │           ├── strip-debug-info-bar.ll
    │   │   │           ├── type-mapping-bug2.ll
    │   │   │           └── type-mapping-src.ll
    │   │   ├── Object/
    │   │   │   ├── ar-create.test
    │   │   │   ├── ar-error.test
    │   │   │   ├── archive-darwin-duplicates.test
    │   │   │   ├── archive-delete.test
    │   │   │   ├── archive-error-tmp.txt
    │   │   │   ├── archive-extract-dir.test
    │   │   │   ├── archive-extract.test
    │   │   │   ├── archive-format.test
    │   │   │   ├── archive-long-filenames-no-null-terminator.test
    │   │   │   ├── archive-long-index.test
    │   │   │   ├── archive-move.test
    │   │   │   ├── archive-pad.test
    │   │   │   ├── archive-replace-pos.test
    │   │   │   ├── archive-symtab.test
    │   │   │   ├── archive-thin-create.test
    │   │   │   ├── archive-thin-paths.test
    │   │   │   ├── archive-thin-read.test
    │   │   │   ├── archive-toc.test
    │   │   │   ├── archive-update.test
    │   │   │   ├── check_binary_output.ll
    │   │   │   ├── coff-archive-short.test
    │   │   │   ├── coff-archive.test
    │   │   │   ├── coff-empty-drectve.test
    │   │   │   ├── coff-invalid.test
    │   │   │   ├── coff-weak-externals.test
    │   │   │   ├── corrupt.test
    │   │   │   ├── directory.ll
    │   │   │   ├── dllimport-globalref.ll
    │   │   │   ├── dllimport.ll
    │   │   │   ├── dyn-rel-relocation.test
    │   │   │   ├── dynamic-reloc.test
    │   │   │   ├── elf-invalid-phdr.test
    │   │   │   ├── elf-reloc-no-sym.test
    │   │   │   ├── elf-unknown-type.test
    │   │   │   ├── invalid-alignment.test
    │   │   │   ├── invalid.test
    │   │   │   ├── kext.test
    │   │   │   ├── lit.local.cfg
    │   │   │   ├── macho-invalid.test
    │   │   │   ├── mangle-ir.ll
    │   │   │   ├── mri-addlib.test
    │   │   │   ├── mri-addmod.test
    │   │   │   ├── mri-crlf.test
    │   │   │   ├── mri1.test
    │   │   │   ├── mri2.test
    │   │   │   ├── mri3.test
    │   │   │   ├── mri4.test
    │   │   │   ├── mri5.test
    │   │   │   ├── multi-module.ll
    │   │   │   ├── nm-archive.test
    │   │   │   ├── nm-darwin-m.test
    │   │   │   ├── nm-error.test
    │   │   │   ├── nm-irix6.test
    │   │   │   ├── nm-pe-image.test
    │   │   │   ├── nm-shared-object.test
    │   │   │   ├── nm-trivial-object.test
    │   │   │   ├── nm-universal-binary.test
    │   │   │   ├── nm-weak-global-macho.test
    │   │   │   ├── no-section-header-string-table.test
    │   │   │   ├── no-section-table.test
    │   │   │   ├── obj2yaml-coff-long-file-symbol.test
    │   │   │   ├── obj2yaml-coff-long-section-name.test
    │   │   │   ├── obj2yaml-coff-section-aux-symbol.test
    │   │   │   ├── obj2yaml-coff-weak-external.test
    │   │   │   ├── obj2yaml-invalid-reloc.test
    │   │   │   ├── obj2yaml-sectiongroup.test
    │   │   │   ├── obj2yaml.test
    │   │   │   ├── objc-imageinfo-coff.ll
    │   │   │   ├── objc-imageinfo-elf.ll
    │   │   │   ├── objc-imageinfo-macho.ll
    │   │   │   ├── objdump-export-list.test
    │   │   │   ├── objdump-file-header.test
    │   │   │   ├── objdump-no-sectionheaders.test
    │   │   │   ├── objdump-private-headers.test
    │   │   │   ├── objdump-reloc-shared.test
    │   │   │   ├── objdump-relocations.test
    │   │   │   ├── objdump-section-content.test
    │   │   │   ├── objdump-sectionheaders.test
    │   │   │   ├── objdump-shndx.test
    │   │   │   ├── objdump-symbol-table.test
    │   │   │   ├── pr25877.test
    │   │   │   ├── readobj-absent.test
    │   │   │   ├── readobj-elf-versioning.test
    │   │   │   ├── readobj-shared-object.test
    │   │   │   ├── readobj.test
    │   │   │   ├── relocation-executable.test
    │   │   │   ├── simple-archive.test
    │   │   │   ├── size-trivial-macho.test
    │   │   │   ├── stackmap-dump.test
    │   │   │   ├── wasm-bad-metadata-version.yaml
    │   │   │   ├── wasm-duplicate-name.test
    │   │   │   ├── wasm-invalid-file.yaml
    │   │   │   ├── wasm-invalid-section-order.test
    │   │   │   ├── wasm-invalid-start.test
    │   │   │   ├── wasm-missing-version.test
    │   │   │   ├── wasm-string-outside-section.test
    │   │   │   ├── yaml2obj-coff-invalid-alignment.test
    │   │   │   ├── yaml2obj-coff-multi-doc.test
    │   │   │   ├── yaml2obj-elf-alignment.yaml
    │   │   │   ├── yaml2obj-elf-bits-endian.test
    │   │   │   ├── yaml2obj-elf-file-headers-with-e_flags.yaml
    │   │   │   ├── yaml2obj-elf-file-headers.yaml
    │   │   │   ├── yaml2obj-elf-multi-doc.test
    │   │   │   ├── yaml2obj-elf-rel-noref.yaml
    │   │   │   ├── yaml2obj-elf-rel.yaml
    │   │   │   ├── yaml2obj-elf-section-basic.yaml
    │   │   │   ├── yaml2obj-elf-section-invalid-size.yaml
    │   │   │   ├── yaml2obj-elf-symbol-basic.yaml
    │   │   │   ├── yaml2obj-elf-symbol-LocalGlobalWeak.yaml
    │   │   │   ├── yaml2obj-elf-symbol-visibility.yaml
    │   │   │   ├── yaml2obj-invalid.yaml
    │   │   │   ├── yaml2obj-readobj.test
    │   │   │   ├── AArch64/
    │   │   │   │   └── yaml2obj-elf-aarch64-rel.yaml
    │   │   │   ├── AMDGPU/
    │   │   │   │   ├── elf-header-flags-mach.yaml
    │   │   │   │   ├── elf-header-flags-sram-ecc.yaml
    │   │   │   │   ├── elf-header-flags-xnack.yaml
    │   │   │   │   ├── elf-header-osabi.yaml
    │   │   │   │   ├── elf32-unknown.yaml
    │   │   │   │   ├── elf64-relocs.yaml
    │   │   │   │   ├── elf64-unknown.yaml
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   └── objdump.s
    │   │   │   ├── ARM/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── macho-data-in-code.test
    │   │   │   │   ├── nm-mapping-symbol.s
    │   │   │   │   ├── objdump-thumb.test
    │   │   │   │   └── symbol-addr.ll
    │   │   │   ├── Inputs/
    │   │   │   │   ├── absolute.elf-x86-64
    │   │   │   │   ├── archive-test.a-coff-i386
    │   │   │   │   ├── archive-test.a-corrupt-symbol-table
    │   │   │   │   ├── archive-test.a-empty
    │   │   │   │   ├── archive-test.a-gnu-minimal
    │   │   │   │   ├── archive-test.a-gnu-no-symtab
    │   │   │   │   ├── archive-test.a-irix6-mips64el
    │   │   │   │   ├── coff-short-import-code
    │   │   │   │   ├── coff-short-import-data
    │   │   │   │   ├── common.coff-i386
    │   │   │   │   ├── corrupt-invalid-dynamic-table-offset.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-dynamic-table-size.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-dynamic-table-too-large.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-phentsize.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-relocation-size.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-strtab.elf.x86-64
    │   │   │   │   ├── corrupt-invalid-virtual-addr.elf.x86-64
    │   │   │   │   ├── corrupt-version.elf-x86_64
    │   │   │   │   ├── corrupt.elf-x86-64
    │   │   │   │   ├── darwin-m-test1.mach0-armv7
    │   │   │   │   ├── darwin-m-test2.macho-i386
    │   │   │   │   ├── darwin-m-test3.macho-x86-64
    │   │   │   │   ├── dext-test.elf-mips64r2
    │   │   │   │   ├── dyn-rel.so.elf-mips
    │   │   │   │   ├── elf-reloc-no-sym.x86_64
    │   │   │   │   ├── elf-versioning-test.i386
    │   │   │   │   ├── elf-versioning-test.x86_64
    │   │   │   │   ├── elfver.S
    │   │   │   │   ├── elfver.script
    │   │   │   │   ├── evenlen
    │   │   │   │   ├── hello-world.elf-x86-64
    │   │   │   │   ├── hello-world.macho-x86_64
    │   │   │   │   ├── invalid-bad-rel-type.elf
    │   │   │   │   ├── invalid-bad-section-address.coff
    │   │   │   │   ├── invalid-buffer.elf
    │   │   │   │   ├── invalid-coff-header-too-small
    │   │   │   │   ├── invalid-e_shnum.elf
    │   │   │   │   ├── invalid-ext-symtab-index.elf-x86-64
    │   │   │   │   ├── invalid-phdr.elf
    │   │   │   │   ├── invalid-rel-sym.elf
    │   │   │   │   ├── invalid-reloc.elf-x86-64
    │   │   │   │   ├── invalid-relocation-sec-sh_offset.elf-i386
    │   │   │   │   ├── invalid-relocation-sec-sh_offset.elf-x86-64
    │   │   │   │   ├── invalid-section-index.elf
    │   │   │   │   ├── invalid-section-size.elf
    │   │   │   │   ├── invalid-section-size2.elf
    │   │   │   │   ├── invalid-sections-num.elf
    │   │   │   │   ├── invalid-sh_entsize.elf
    │   │   │   │   ├── invalid-strtab-non-null.elf
    │   │   │   │   ├── invalid-strtab-size.elf
    │   │   │   │   ├── invalid-strtab-type.elf
    │   │   │   │   ├── invalid-strtab-zero-size.elf
    │   │   │   │   ├── invalid-symbol-table-size.elf
    │   │   │   │   ├── invalid-xindex-size.elf
    │   │   │   │   ├── macho-data-in-code.macho-thumbv7
    │   │   │   │   ├── macho-empty-kext-bundle-x86-64
    │   │   │   │   ├── macho-hello-g.macho-x86_64
    │   │   │   │   ├── macho-invalid-bad-symbol-index
    │   │   │   │   ├── macho-invalid-bind-overlap
    │   │   │   │   ├── macho-invalid-codesig-overlap
    │   │   │   │   ├── macho-invalid-codesign-bad-size
    │   │   │   │   ├── macho-invalid-dataincode-bad-size
    │   │   │   │   ├── macho-invalid-dataincode-dataoff-datasize
    │   │   │   │   ├── macho-invalid-dataincode-more-than-one
    │   │   │   │   ├── macho-invalid-dyld-name_offset-toobig
    │   │   │   │   ├── macho-invalid-dyld-name_toobig
    │   │   │   │   ├── macho-invalid-dyld-small
    │   │   │   │   ├── macho-invalid-dyldinfo-bind_off-bind_size
    │   │   │   │   ├── macho-invalid-dyldinfo-export_off-export_size
    │   │   │   │   ├── macho-invalid-dyldinfo-lazy_bind_off-lazy_bind_size
    │   │   │   │   ├── macho-invalid-dyldinfo-more-than-one
    │   │   │   │   ├── macho-invalid-dyldinfo-rebase_off
    │   │   │   │   ├── macho-invalid-dyldinfo-rebase_off-rebase_size
    │   │   │   │   ├── macho-invalid-dyldinfo-small
    │   │   │   │   ├── macho-invalid-dyldinfo-weak_bind_off-weak_bind_size
    │   │   │   │   ├── macho-invalid-dyldinfoonly-bad-size
    │   │   │   │   ├── macho-invalid-dyldinfoonly-bind_off
    │   │   │   │   ├── macho-invalid-dyldinfoonly-export_off
    │   │   │   │   ├── macho-invalid-dyldinfoonly-lazy_bind_off
    │   │   │   │   ├── macho-invalid-dyldinfoonly-weak_bind_off
    │   │   │   │   ├── macho-invalid-dylib-cmdsize-past-eof
    │   │   │   │   ├── macho-invalid-dylib-id-more-than-one
    │   │   │   │   ├── macho-invalid-dylib-name_offset-toobig
    │   │   │   │   ├── macho-invalid-dylib-name_offset-toosmall
    │   │   │   │   ├── macho-invalid-dylib-name_toobig
    │   │   │   │   ├── macho-invalid-dylib-no-id
    │   │   │   │   ├── macho-invalid-dylib-small
    │   │   │   │   ├── macho-invalid-dylib-wrong-filetype
    │   │   │   │   ├── macho-invalid-dylib_code_sign_drs-bad-size
    │   │   │   │   ├── macho-invalid-dysymtab-bad-size
    │   │   │   │   ├── macho-invalid-dysymtab-extrefsymoff
    │   │   │   │   ├── macho-invalid-dysymtab-extrefsymoff-nextrefsyms
    │   │   │   │   ├── macho-invalid-dysymtab-extreloff
    │   │   │   │   ├── macho-invalid-dysymtab-extreloff-nextrel
    │   │   │   │   ├── macho-invalid-dysymtab-indirectsymoff
    │   │   │   │   ├── macho-invalid-dysymtab-indirectsymoff-nindirectsyms
    │   │   │   │   ├── macho-invalid-dysymtab-locreloff
    │   │   │   │   ├── macho-invalid-dysymtab-locreloff-nlocrel
    │   │   │   │   ├── macho-invalid-dysymtab-modtaboff
    │   │   │   │   ├── macho-invalid-dysymtab-modtaboff-nmodtab
    │   │   │   │   ├── macho-invalid-dysymtab-more-than-one
    │   │   │   │   ├── macho-invalid-dysymtab-small
    │   │   │   │   ├── macho-invalid-dysymtab-tocoff
    │   │   │   │   ├── macho-invalid-dysymtab-tocoff-ntoc
    │   │   │   │   ├── macho-invalid-encrypt-bad-size
    │   │   │   │   ├── macho-invalid-encrypt-cryptoff
    │   │   │   │   ├── macho-invalid-encrypt-more-than-one
    │   │   │   │   ├── macho-invalid-encrypt64-bad-size
    │   │   │   │   ├── macho-invalid-encrypt64-cryptoff-cryptsize
    │   │   │   │   ├── macho-invalid-entry-bad-size
    │   │   │   │   ├── macho-invalid-entry-more-than-one
    │   │   │   │   ├── macho-invalid-export-overlap
    │   │   │   │   ├── macho-invalid-extrefsyms-overlap
    │   │   │   │   ├── macho-invalid-extreloff-overlap
    │   │   │   │   ├── macho-invalid-fat
    │   │   │   │   ├── macho-invalid-fat-arch-badalign
    │   │   │   │   ├── macho-invalid-fat-arch-bigalign
    │   │   │   │   ├── macho-invalid-fat-arch-overlap
    │   │   │   │   ├── macho-invalid-fat-arch-overlapheaders
    │   │   │   │   ├── macho-invalid-fat-arch-size
    │   │   │   │   ├── macho-invalid-fat-arch-twosame
    │   │   │   │   ├── macho-invalid-fat-header
    │   │   │   │   ├── macho-invalid-fat.obj.elf-x86_64
    │   │   │   │   ├── macho-invalid-fat_cputype
    │   │   │   │   ├── macho-invalid-function_starts-dataoff
    │   │   │   │   ├── macho-invalid-fvmfile-obsolete
    │   │   │   │   ├── macho-invalid-header
    │   │   │   │   ├── macho-invalid-hints-overlap
    │   │   │   │   ├── macho-invalid-ident-obsolete
    │   │   │   │   ├── macho-invalid-idfvmlib-obsolete
    │   │   │   │   ├── macho-invalid-indirectsyms-overlap
    │   │   │   │   ├── macho-invalid-lazy_bind-overlap
    │   │   │   │   ├── macho-invalid-linkopt-bad-count
    │   │   │   │   ├── macho-invalid-linkopt-bad-size
    │   │   │   │   ├── macho-invalid-linkopthint-dataoff
    │   │   │   │   ├── macho-invalid-linkopthint-small
    │   │   │   │   ├── macho-invalid-loadfvmlib-obsolete
    │   │   │   │   ├── macho-invalid-locreloff-overlap
    │   │   │   │   ├── macho-invalid-modtab-overlap
    │   │   │   │   ├── macho-invalid-no-size-for-sections
    │   │   │   │   ├── macho-invalid-note
    │   │   │   │   ├── macho-invalid-prebind_cksum-obsolete
    │   │   │   │   ├── macho-invalid-prebound_dylib-obsolete
    │   │   │   │   ├── macho-invalid-prepage-obsolete
    │   │   │   │   ├── macho-invalid-rebase-overlap
    │   │   │   │   ├── macho-invalid-reloc-overlap
    │   │   │   │   ├── macho-invalid-routines-bad-size
    │   │   │   │   ├── macho-invalid-routines64-more-than-one
    │   │   │   │   ├── macho-invalid-rpath-name_offset-toobig
    │   │   │   │   ├── macho-invalid-rpath-name_toobig
    │   │   │   │   ├── macho-invalid-rpath-small
    │   │   │   │   ├── macho-invalid-section-addr
    │   │   │   │   ├── macho-invalid-section-addr-size
    │   │   │   │   ├── macho-invalid-section-index-getSectionRawName
    │   │   │   │   ├── macho-invalid-section-offset
    │   │   │   │   ├── macho-invalid-section-offset-in-headers
    │   │   │   │   ├── macho-invalid-section-offset-size
    │   │   │   │   ├── macho-invalid-section-overlap
    │   │   │   │   ├── macho-invalid-section-reloff
    │   │   │   │   ├── macho-invalid-section-reloff-nrelocs
    │   │   │   │   ├── macho-invalid-section-size-filesize
    │   │   │   │   ├── macho-invalid-segment-fileoff
    │   │   │   │   ├── macho-invalid-segment-filesize
    │   │   │   │   ├── macho-invalid-segment-vmsize
    │   │   │   │   ├── macho-invalid-source-bad-size
    │   │   │   │   ├── macho-invalid-source-more-than-one
    │   │   │   │   ├── macho-invalid-splitinfo-dataoff-datasize
    │   │   │   │   ├── macho-invalid-strtab-overlap
    │   │   │   │   ├── macho-invalid-subclient-name_toobig
    │   │   │   │   ├── macho-invalid-subframe-small
    │   │   │   │   ├── macho-invalid-sublibrary-name_offset-toobig
    │   │   │   │   ├── macho-invalid-subumbrella-offset-small
    │   │   │   │   ├── macho-invalid-symbol-name-past-eof
    │   │   │   │   ├── macho-invalid-symseg-obsolete
    │   │   │   │   ├── macho-invalid-symtab-bad-size
    │   │   │   │   ├── macho-invalid-symtab-more-than-one
    │   │   │   │   ├── macho-invalid-symtab-overlap
    │   │   │   │   ├── macho-invalid-symtab-small
    │   │   │   │   ├── macho-invalid-symtab-stroff
    │   │   │   │   ├── macho-invalid-symtab-stroff-strsize
    │   │   │   │   ├── macho-invalid-symtab-symoff
    │   │   │   │   ├── macho-invalid-symtab-symoff-nsyms
    │   │   │   │   ├── macho-invalid-thread-count-pastend
    │   │   │   │   ├── macho-invalid-thread-count-wrong
    │   │   │   │   ├── macho-invalid-thread-flavor-unknown
    │   │   │   │   ├── macho-invalid-thread-state-pastend
    │   │   │   │   ├── macho-invalid-thread-unknown-cputype
    │   │   │   │   ├── macho-invalid-toc-overlap
    │   │   │   │   ├── macho-invalid-too-small-load-command
    │   │   │   │   ├── macho-invalid-too-small-segment-load-command
    │   │   │   │   ├── macho-invalid-too-small-segment-load-command.1
    │   │   │   │   ├── macho-invalid-twolevelhints-bad-size
    │   │   │   │   ├── macho-invalid-twolevelhints-more-than-one
    │   │   │   │   ├── macho-invalid-twolevelhints-offset
    │   │   │   │   ├── macho-invalid-twolevelhints-offset-nhints
    │   │   │   │   ├── macho-invalid-unixthread-more-than-one
    │   │   │   │   ├── macho-invalid-uuid-bad-size
    │   │   │   │   ├── macho-invalid-uuid-more-than-one
    │   │   │   │   ├── macho-invalid-vers-more-than-one
    │   │   │   │   ├── macho-invalid-vers-small
    │   │   │   │   ├── macho-invalid-weak_bind-overlap
    │   │   │   │   ├── macho-invalid-zero-ncmds
    │   │   │   │   ├── macho-rpath-x86_64
    │   │   │   │   ├── macho-text-data-bss.macho-x86_64
    │   │   │   │   ├── macho-text-sections.macho-x86_64
    │   │   │   │   ├── macho-text.thumb
    │   │   │   │   ├── macho-universal-archive-bad1.x86_64.i386
    │   │   │   │   ├── macho-universal-archive-bad2.x86_64.i386
    │   │   │   │   ├── macho-universal-archive.x86_64.i386
    │   │   │   │   ├── macho-universal-bad1.x86_64.i386
    │   │   │   │   ├── macho-universal-bad2.x86_64.i386
    │   │   │   │   ├── macho-universal.x86_64.i386
    │   │   │   │   ├── macho-universal64-archive.x86_64.i386
    │   │   │   │   ├── macho-universal64.x86_64.i386
    │   │   │   │   ├── macho-valid-0-nsyms
    │   │   │   │   ├── macho64-invalid-incomplete-load-command
    │   │   │   │   ├── macho64-invalid-incomplete-load-command.1
    │   │   │   │   ├── macho64-invalid-incomplete-segment-load-command
    │   │   │   │   ├── macho64-invalid-no-size-for-sections
    │   │   │   │   ├── macho64-invalid-too-small-load-command
    │   │   │   │   ├── macho64-invalid-too-small-load-command.1
    │   │   │   │   ├── macho64-invalid-too-small-segment-load-command
    │   │   │   │   ├── micro-mips.elf-mipsel
    │   │   │   │   ├── mri-crlf.mri
    │   │   │   │   ├── multi-module.ll
    │   │   │   │   ├── no-section-header-string-table.elf-x86-64
    │   │   │   │   ├── no-sections.elf-x86-64
    │   │   │   │   ├── no-start-symbol.elf-x86_64
    │   │   │   │   ├── oddlen
    │   │   │   │   ├── openbsd-phdrs.elf-x86-64
    │   │   │   │   ├── phdr-note.elf-x86-64
    │   │   │   │   ├── phdrs.elf-x86-64
    │   │   │   │   ├── program-headers.elf-i386
    │   │   │   │   ├── program-headers.elf-x86-64
    │   │   │   │   ├── program-headers.mips
    │   │   │   │   ├── program-headers.mips64
    │   │   │   │   ├── rel-no-sec-table.elf-x86-64
    │   │   │   │   ├── relocatable-with-section-address.elf-x86-64
    │   │   │   │   ├── relocation-dynamic.elf-i386
    │   │   │   │   ├── relocation-relocatable.elf-i386
    │   │   │   │   ├── relocations.elf-x86-64
    │   │   │   │   ├── sectionGroup.elf.x86-64
    │   │   │   │   ├── shared-object-test.elf-i386
    │   │   │   │   ├── shared-object-test.elf-x86-64
    │   │   │   │   ├── shared.ll
    │   │   │   │   ├── shndx.elf
    │   │   │   │   ├── solaris-nosymbols.yaml
    │   │   │   │   ├── stackmap-test.macho-x86-64
    │   │   │   │   ├── thumb-symbols.elf.arm
    │   │   │   │   ├── trivial-executable-test.macho-x86-64
    │   │   │   │   ├── trivial-label-test.elf-x86-64
    │   │   │   │   ├── trivial-object-test.coff-arm64
    │   │   │   │   ├── trivial-object-test.coff-armnt
    │   │   │   │   ├── trivial-object-test.coff-i386
    │   │   │   │   ├── trivial-object-test.coff-x86-64
    │   │   │   │   ├── trivial-object-test.elf-avr
    │   │   │   │   ├── trivial-object-test.elf-hexagon
    │   │   │   │   ├── trivial-object-test.elf-i386
    │   │   │   │   ├── trivial-object-test.elf-mips64el
    │   │   │   │   ├── trivial-object-test.elf-mipsel
    │   │   │   │   ├── trivial-object-test.elf-x86-64
    │   │   │   │   ├── trivial-object-test.macho-i386
    │   │   │   │   ├── trivial-object-test.macho-x86-64
    │   │   │   │   ├── trivial-object-test.wasm
    │   │   │   │   ├── trivial-object-test2.elf-x86-64
    │   │   │   │   ├── trivial-object-test2.macho-x86-64
    │   │   │   │   ├── trivial.ll
    │   │   │   │   ├── unwind-section.elf-x86-64
    │   │   │   │   ├── very_long_bytecode_file_name.bc
    │   │   │   │   ├── weak-global-symbol.macho-i386
    │   │   │   │   ├── weak.elf-x86-64
    │   │   │   │   ├── COFF/
    │   │   │   │   │   ├── empty-drectve.yaml
    │   │   │   │   │   ├── i386.yaml
    │   │   │   │   │   ├── long-file-symbol.yaml
    │   │   │   │   │   ├── long-section-name.yaml
    │   │   │   │   │   ├── section-aux-symbol.yaml
    │   │   │   │   │   ├── weak-external.yaml
    │   │   │   │   │   ├── weak-externals.yaml
    │   │   │   │   │   └── x86-64.yaml
    │   │   │   │   ├── ELF/
    │   │   │   │   │   ├── BE32.yaml
    │   │   │   │   │   ├── BE64.yaml
    │   │   │   │   │   ├── LE32.yaml
    │   │   │   │   │   └── LE64.yaml
    │   │   │   │   └── WASM/
    │   │   │   │       ├── invalid-section-order.wasm
    │   │   │   │       ├── missing-version.wasm
    │   │   │   │       └── string-outside-section.wasm
    │   │   │   ├── Lanai/
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   └── yaml2obj-elf-lanai-rel.yaml
    │   │   │   ├── Mips/
    │   │   │   │   ├── abi-flags.yaml
    │   │   │   │   ├── elf-abi.yaml
    │   │   │   │   ├── elf-flags.yaml
    │   │   │   │   ├── elf-mips64-rel.yaml
    │   │   │   │   ├── feature.test
    │   │   │   │   ├── lit.local.cfg
    │   │   │   │   ├── objdump-micro-mips.test
    │   │   │   │   └── reloc-visit.test
    │   │   │   ├── RISCV/
    │   │   │   │   ├── elf-flags.yaml
    │   │   │   │   └── lit.local.cfg
    │   │   │   └── X86/
    │   │   │       ├── archive-ir-asm.ll
    │   │   │       ├── archive-symbol-table.s
    │   │   │       ├── asm-lazy-reference.ll
    │   │   │       ├── irsymtab-asm.ll
    │   │   │       ├── irsymtab-bad-alias.ll
    │   │   │       ├── irsymtab.ll
    │   │   │       ├── lit.local.cfg
    │   │   │       ├── macho-text-sections.test
    │   │   │       ├── nm-bitcodeweak.test
    │   │   │       ├── nm-coff.s
    │   │   │       ├── nm-ir.ll
    │   │   │       ├── nm-macho.s
    │   │   │       ├── nm-print-size.s
    │   │   │       ├── nm-undefinedweak.test
    │   │   │       ├── no-start-symbol.test
    │   │   │       ├── obj2yaml-dup-section-name.s
    │   │   │       ├── obj2yaml-dup-symbol-name.s
    │   │   │       ├── objdump-disassembly-inline-relocations.test
    │   │   │       ├── objdump-label.test
    │   │   │       ├── objdump-trivial-object.test
    │   │   │       ├── yaml-elf-x86-rel-broken.yaml
    │   │   │       └── yaml2obj-elf-x86-rel.yaml
    │   │   ├── Other/
    │   │   │   ├── 2002-01-31-CallGraph.ll
    │   │   │   ├── 2002-02-24-InlineBrokePHINodes.ll
    │   │   │   ├── 2002-03-11-ConstPropCrash.ll
    │   │   │   ├── 2003-02-19-LoopInfoNestingBug.ll
    │   │   │   ├── 2004-08-16-PackedConstantInlineStore.ll
    │   │   │   ├── 2004-08-16-PackedGlobalConstant.ll
    │   │   │   ├── 2004-08-16-PackedSelect.ll
    │   │   │   ├── 2004-08-16-PackedSimple.ll
    │   │   │   ├── 2004-08-20-PackedControlFlow.ll
    │   │   │   ├── 2006-02-05-PassManager.ll
    │   │   │   ├── 2007-04-24-eliminate-mostly-empty-blocks.ll
    │   │   │   ├── 2007-06-05-PassID.ll
    │   │   │   ├── 2007-06-28-PassManager.ll
    │   │   │   ├── 2007-09-10-PassManager.ll
    │   │   │   ├── 2008-02-14-PassManager.ll
    │   │   │   ├── 2008-06-04-FieldSizeInPacked.ll
    │   │   │   ├── 2008-10-06-RemoveDeadPass.ll
    │   │   │   ├── 2008-10-15-MissingSpace.ll
    │   │   │   ├── 2009-03-31-CallGraph.ll
    │   │   │   ├── 2009-06-05-no-implicit-float.ll
    │   │   │   ├── 2009-09-14-function-elements.ll
    │   │   │   ├── 2010-05-06-Printer.ll
    │   │   │   ├── attribute-comment.ll
    │   │   │   ├── bcanalyzer-block-info.txt
    │   │   │   ├── can-execute.txt
    │   │   │   ├── cfg-printer-branch-weights.ll
    │   │   │   ├── cgscc-devirt-iteration.ll
    │   │   │   ├── cgscc-disconnected-invalidation.ll
    │   │   │   ├── cgscc-iterate-function-mutation.ll
    │   │   │   ├── cgscc-libcall-update.ll
    │   │   │   ├── cgscc-observe-devirt.ll
    │   │   │   ├── cleanup-lcssa.ll
    │   │   │   ├── close-stderr.ll
    │   │   │   ├── codegenprepare-and-debug.ll
    │   │   │   ├── constant-fold-gep-address-spaces.ll
    │   │   │   ├── constant-fold-gep.ll
    │   │   │   ├── debugcounter-dce.ll
    │   │   │   ├── debugcounter-earlycse.ll
    │   │   │   ├── debugcounter-newgvn.ll
    │   │   │   ├── debugcounter-predicateinfo.ll
    │   │   │   ├── extract-alias.ll
    │   │   │   ├── extract-linkonce.ll
    │   │   │   ├── extract-weak-odr.ll
    │   │   │   ├── extract.ll
    │   │   │   ├── FileCheck-space.txt
    │   │   │   ├── invalid-commandline-option.ll
    │   │   │   ├── invariant.group.ll
    │   │   │   ├── lint.ll
    │   │   │   ├── lit-globbing.ll
    │   │   │   ├── lit-quoting.txt
    │   │   │   ├── lit-unicode.txt
    │   │   │   ├── llvm-nm-without-aliases.ll
    │   │   │   ├── loop-deletion-printer.ll
    │   │   │   ├── loop-pass-ordering.ll
    │   │   │   ├── loop-pass-printer.ll
    │   │   │   ├── loop-pm-invalidation.ll
    │   │   │   ├── machine-size-remarks.ll
    │   │   │   ├── new-pass-manager.ll
    │   │   │   ├── new-pm-defaults.ll
    │   │   │   ├── new-pm-lto-defaults.ll
    │   │   │   ├── new-pm-pgo.ll
    │   │   │   ├── new-pm-thinlto-defaults.ll
    │   │   │   ├── opt-bisect-helper.py
    │   │   │   ├── opt-bisect-legacy-pass-manager.ll
    │   │   │   ├── opt-hot-cold-split.ll
    │   │   │   ├── opt-O0-pipeline.ll
    │   │   │   ├── opt-O2-pipeline.ll
    │   │   │   ├── opt-O3-pipeline.ll
    │   │   │   ├── opt-Os-pipeline.ll
    │   │   │   ├── opt-override-mcpu-mattr.ll
    │   │   │   ├── opt-twice.ll
    │   │   │   ├── optimization-remarks-inline.ll
    │   │   │   ├── optimization-remarks-invalidation.ll
    │   │   │   ├── optimization-remarks-lazy-bfi.ll
    │   │   │   ├── optimize-inrange-gep.ll
    │   │   │   ├── optimize-options.ll
    │   │   │   ├── pass-pipeline-parsing.ll
    │   │   │   ├── pass-pipelines.ll
    │   │   │   ├── pipefail.txt
    │   │   │   ├── pr32085.ll
    │   │   │   ├── print-debug-counter.ll
    │   │   │   ├── print-module-scope.ll
    │   │   │   ├── printer.ll
    │   │   │   ├── ResponseFile.ll
    │   │   │   ├── scc-deleted-printer.ll
    │   │   │   ├── scc-pass-printer.ll
    │   │   │   ├── size-remarks.ll
    │   │   │   ├── spir_cc.ll
    │   │   │   ├── statistic.ll
    │   │   │   ├── time-passes.ll
    │   │   │   ├── umask.ll
    │   │   │   ├── writing-to-stdout.ll
    │   │   │   ├── Inputs/
    │   │   │   │   ├── block-info-only.bc
    │   │   │   │   ├── glob-input
    │   │   │   │   ├── has-block-info.bc
    │   │   │   │   ├── new-pm-pgo.prof
    │   │   │   │   ├── new-pm-pgo.proftext
    │   │   │   │   ├── no-block-info.bc
    │   │   │   │   ├── utf8-bom-response
    │   │   │   │   ├── utf8-response
    │   │   │   │   └── TestProg/
    │   │   │   │       └── TestProg
    │   │   │   └── X86/
    │   │   │       ├── debugcounter-divrempairs.ll
    │   │   │       ├── debugcounter-partiallyinlinelibcalls.ll
    │   │   │       ├── inline-asm-newline-terminator.ll
    │   │   │       ├── lit.local.cfg
    │   │   │       ├── mbb-dump.ll
    │   │   │       └── opt-bisect-isel.ll
    │   │   ├── SafepointIRVerifier/
    │   │   │   ├── basic-use-after-reloc.ll
    │   │   │   ├── compares.ll
    │   │   │   ├── constant-bases.ll
    │   │   │   ├── from-same-relocation-in-phi-nodes.ll
    │   │   │   ├── unreachable-block-tolerant.ll
    │   │   │   ├── unrecorded-live-at-sp.ll
    │   │   │   ├── use-derived-unrelocated.ll
    │   │   │   └── uses-in-phi-nodes.ll
    │   │   ├── SymbolRewriter/
    │   │   │   └── rewrite.ll
    │   │   └── TableGen/
    │   │       ├── 2003-08-03-PassCode.td
    │   │       ├── 2006-09-18-LargeInt.td
    │   │       ├── 2010-03-24-PrematureDefaults.td
    │   │       ├── AllowDuplicateRegisterNames.td
    │   │       ├── ambiguous-composition.td
    │   │       ├── AnonDefinitionOnDemand.td
    │   │       ├── arithmetic.td
    │   │       ├── AsmPredicateCondsEmission.td
    │   │       ├── AsmVariant.td
    │   │       ├── BitOffsetDecoder.td
    │   │       ├── BitsInit.td
    │   │       ├── BitsInitOverflow.td
    │   │       ├── cast-list-initializer.td
    │   │       ├── cast-multiclass.td
    │   │       ├── cast-typeerror.td
    │   │       ├── cast.td
    │   │       ├── ClassInstanceValue.td
    │   │       ├── code.td
    │   │       ├── compare.td
    │   │       ├── ConcatenatedSubregs.td
    │   │       ├── ConstraintChecking.inc
    │   │       ├── ConstraintChecking1.td
    │   │       ├── ConstraintChecking2.td
    │   │       ├── ConstraintChecking3.td
    │   │       ├── ConstraintChecking4.td
    │   │       ├── ConstraintChecking5.td
    │   │       ├── ConstraintChecking6.td
    │   │       ├── ConstraintChecking7.td
    │   │       ├── CStyleComment.td
    │   │       ├── dag-functional.td
    │   │       ├── dag-isel-res-order.td
    │   │       ├── Dag.td
    │   │       ├── defmclass.td
    │   │       ├── DefmInherit.td
    │   │       ├── DefmInsideMultiClass.td
    │   │       ├── defset-typeerror.td
    │   │       ├── defset.td
    │   │       ├── DuplicateFieldValues.td
    │   │       ├── eq.td
    │   │       ├── eqbit.td
    │   │       ├── FastISelEmitter.td
    │   │       ├── FieldAccess.td
    │   │       ├── foldl.td
    │   │       ├── foreach-eval.td
    │   │       ├── foreach-leak.td
    │   │       ├── foreach-multiclass.td
    │   │       ├── foreach.td
    │   │       ├── ForeachList.td
    │   │       ├── ForeachLoop.td
    │   │       ├── ForwardRef.td
    │   │       ├── GeneralList.td
    │   │       ├── generic-tables-instruction.td
    │   │       ├── generic-tables.td
    │   │       ├── GlobalISelEmitter-PR39045.td
    │   │       ├── GlobalISelEmitter.td
    │   │       ├── HwModeSelect.td
    │   │       ├── if-empty-list-arg.td
    │   │       ├── if-type.td
    │   │       ├── if.td
    │   │       ├── ifbit.td
    │   │       ├── Include.inc
    │   │       ├── Include.td
    │   │       ├── IntBitInit.td
    │   │       ├── intrinsic-long-name.td
    │   │       ├── intrinsic-struct.td
    │   │       ├── intrinsic-varargs.td
    │   │       ├── isa.td
    │   │       ├── JSON-check.py
    │   │       ├── JSON.td
    │   │       ├── LazyChange.td
    │   │       ├── LetInsideMultiClasses.td
    │   │       ├── lisp.td
    │   │       ├── list-element-bitref.td
    │   │       ├── ListArgs.td
    │   │       ├── ListArgsSimple.td
    │   │       ├── listconcat.td
    │   │       ├── ListConversion.td
    │   │       ├── ListManip.td
    │   │       ├── ListOfList.td
    │   │       ├── ListSlices.td
    │   │       ├── lit.local.cfg
    │   │       ├── LoLoL.td
    │   │       ├── math.td
    │   │       ├── MultiClass-defm-fail.td
    │   │       ├── MultiClass-defm.td
    │   │       ├── MultiClass.td
    │   │       ├── MultiClassDefName.td
    │   │       ├── MultiClassInherit.td
    │   │       ├── MultiPat.td
    │   │       ├── name-resolution-consistency.td
    │   │       ├── nested-comment.td
    │   │       ├── NestedForeach.td
    │   │       ├── Paste.td
    │   │       ├── pr8330.td
    │   │       ├── prep-diag1.td
    │   │       ├── prep-diag10.td
    │   │       ├── prep-diag11-include.inc
    │   │       ├── prep-diag11.td
    │   │       ├── prep-diag12-include.inc
    │   │       ├── prep-diag12.td
    │   │       ├── prep-diag13.td
    │   │       ├── prep-diag14.td
    │   │       ├── prep-diag2.td
    │   │       ├── prep-diag3.td
    │   │       ├── prep-diag4.td
    │   │       ├── prep-diag5.td
    │   │       ├── prep-diag6.td
    │   │       ├── prep-diag7.td
    │   │       ├── prep-diag8.td
    │   │       ├── prep-diag9.td
    │   │       ├── prep-region-include.inc
    │   │       ├── prep-region-processing.td
    │   │       ├── RegisterBankEmitter.td
    │   │       ├── RegisterEncoder.td
    │   │       ├── RelTest.td
    │   │       ├── searchabletables-intrinsic.td
    │   │       ├── self-reference-recursion.td
    │   │       ├── self-reference-typeerror.td
    │   │       ├── self-reference.td
    │   │       ├── SetTheory.td
    │   │       ├── SiblingForeach.td
    │   │       ├── size.td
    │   │       ├── Slice.td
    │   │       ├── strconcat.td
    │   │       ├── String.td
    │   │       ├── subst.td
    │   │       ├── subst2.td
    │   │       ├── SuperSubclassSameName.td
    │   │       ├── TargetInstrInfo.td
    │   │       ├── TargetInstrSpec.td
    │   │       ├── template-arg-dependency.td
    │   │       ├── TemplateArgRename.td
    │   │       ├── Tree.td
    │   │       ├── TreeNames.td
    │   │       ├── trydecode-emission.td
    │   │       ├── trydecode-emission2.td
    │   │       ├── trydecode-emission3.td
    │   │       ├── TwoLevelName.td
    │   │       ├── UnsetBitInit.td
    │   │       ├── unterminated-c-comment-include.inc
    │   │       ├── unterminated-c-comment.td
    │   │       ├── unterminated-code-block-include.inc
    │   │       ├── unterminated-code-block.td
    │   │       ├── UnterminatedComment.td
    │   │       ├── usevalname.td
    │   │       ├── ValidIdentifiers.td
    │   │       └── FixedLenDecoderEmitter/
    │   │           └── conflict.td
    │   └── unittests/
    │       ├── CMakeLists.txt
    │       ├── unittest.cfg.in
    │       ├── ADT/
    │       │   ├── AnyTest.cpp
    │       │   ├── APFloatTest.cpp
    │       │   ├── APIntTest.cpp
    │       │   ├── APSIntTest.cpp
    │       │   ├── ArrayRefTest.cpp
    │       │   ├── BitmaskEnumTest.cpp
    │       │   ├── BitVectorTest.cpp
    │       │   ├── BreadthFirstIteratorTest.cpp
    │       │   ├── BumpPtrListTest.cpp
    │       │   ├── CMakeLists.txt
    │       │   ├── DAGDeltaAlgorithmTest.cpp
    │       │   ├── DeltaAlgorithmTest.cpp
    │       │   ├── DenseMapTest.cpp
    │       │   ├── DenseSetTest.cpp
    │       │   ├── DepthFirstIteratorTest.cpp
    │       │   ├── EquivalenceClassesTest.cpp
    │       │   ├── FoldingSet.cpp
    │       │   ├── FunctionExtrasTest.cpp
    │       │   ├── FunctionRefTest.cpp
    │       │   ├── HashingTest.cpp
    │       │   ├── IListBaseTest.cpp
    │       │   ├── IListIteratorTest.cpp
    │       │   ├── IListNodeBaseTest.cpp
    │       │   ├── IListNodeTest.cpp
    │       │   ├── IListSentinelTest.cpp
    │       │   ├── IListTest.cpp
    │       │   ├── ImmutableListTest.cpp
    │       │   ├── ImmutableMapTest.cpp
    │       │   ├── ImmutableSetTest.cpp
    │       │   ├── IntEqClassesTest.cpp
    │       │   ├── IntervalMapTest.cpp
    │       │   ├── IntrusiveRefCntPtrTest.cpp
    │       │   ├── IteratorTest.cpp
    │       │   ├── MakeUniqueTest.cpp
    │       │   ├── MappedIteratorTest.cpp
    │       │   ├── MapVectorTest.cpp
    │       │   ├── OptionalTest.cpp
    │       │   ├── PackedVectorTest.cpp
    │       │   ├── PointerEmbeddedIntTest.cpp
    │       │   ├── PointerIntPairTest.cpp
    │       │   ├── PointerSumTypeTest.cpp
    │       │   ├── PointerUnionTest.cpp
    │       │   ├── PostOrderIteratorTest.cpp
    │       │   ├── PriorityWorklistTest.cpp
    │       │   ├── RangeAdapterTest.cpp
    │       │   ├── SCCIteratorTest.cpp
    │       │   ├── ScopeExitTest.cpp
    │       │   ├── SequenceTest.cpp
    │       │   ├── SetVectorTest.cpp
    │       │   ├── SimpleIListTest.cpp
    │       │   ├── SmallPtrSetTest.cpp
    │       │   ├── SmallSetTest.cpp
    │       │   ├── SmallStringTest.cpp
    │       │   ├── SmallVectorTest.cpp
    │       │   ├── SparseBitVectorTest.cpp
    │       │   ├── SparseMultiSetTest.cpp
    │       │   ├── SparseSetTest.cpp
    │       │   ├── StatisticTest.cpp
    │       │   ├── STLExtrasTest.cpp
    │       │   ├── StringExtrasTest.cpp
    │       │   ├── StringMapTest.cpp
    │       │   ├── StringRefTest.cpp
    │       │   ├── StringSwitchTest.cpp
    │       │   ├── TestGraph.h
    │       │   ├── TinyPtrVectorTest.cpp
    │       │   ├── TripleTest.cpp
    │       │   ├── TwineTest.cpp
    │       │   └── VariadicFunctionTest.cpp
    │       ├── Analysis/
    │       │   ├── AliasAnalysisTest.cpp
    │       │   ├── AliasSetTrackerTest.cpp
    │       │   ├── BasicAliasAnalysisTest.cpp
    │       │   ├── BlockFrequencyInfoTest.cpp
    │       │   ├── BranchProbabilityInfoTest.cpp
    │       │   ├── CallGraphTest.cpp
    │       │   ├── CaptureTrackingTest.cpp
    │       │   ├── CFGTest.cpp
    │       │   ├── CGSCCPassManagerTest.cpp
    │       │   ├── CMakeLists.txt
    │       │   ├── DivergenceAnalysisTest.cpp
    │       │   ├── GlobalsModRefTest.cpp
    │       │   ├── LazyCallGraphTest.cpp
    │       │   ├── LoopInfoTest.cpp
    │       │   ├── MemoryBuiltinsTest.cpp
    │       │   ├── MemorySSATest.cpp
    │       │   ├── OrderedBasicBlockTest.cpp
    │       │   ├── OrderedInstructionsTest.cpp
    │       │   ├── PhiValuesTest.cpp
    │       │   ├── ProfileSummaryInfoTest.cpp
    │       │   ├── ScalarEvolutionTest.cpp
    │       │   ├── SparsePropagation.cpp
    │       │   ├── TargetLibraryInfoTest.cpp
    │       │   ├── TBAATest.cpp
    │       │   ├── UnrollAnalyzerTest.cpp
    │       │   ├── ValueLatticeTest.cpp
    │       │   └── ValueTrackingTest.cpp
    │       ├── AsmParser/
    │       │   ├── AsmParserTest.cpp
    │       │   └── CMakeLists.txt
    │       ├── BinaryFormat/
    │       │   ├── CMakeLists.txt
    │       │   ├── DwarfTest.cpp
    │       │   ├── MachOTest.cpp
    │       │   ├── MsgPackReaderTest.cpp
    │       │   ├── MsgPackTypesTest.cpp
    │       │   ├── MsgPackWriterTest.cpp
    │       │   └── TestFileMagic.cpp
    │       ├── Bitcode/
    │       │   ├── BitReaderTest.cpp
    │       │   ├── BitstreamReaderTest.cpp
    │       │   ├── BitstreamWriterTest.cpp
    │       │   └── CMakeLists.txt
    │       ├── CodeGen/
    │       │   ├── AArch64SelectionDAGTest.cpp
    │       │   ├── CMakeLists.txt
    │       │   ├── DIEHashTest.cpp
    │       │   ├── LowLevelTypeTest.cpp
    │       │   ├── MachineInstrBundleIteratorTest.cpp
    │       │   ├── MachineInstrTest.cpp
    │       │   ├── MachineOperandTest.cpp
    │       │   ├── ScalableVectorMVTsTest.cpp
    │       │   └── GlobalISel/
    │       │       ├── CMakeLists.txt
    │       │       ├── CSETest.cpp
    │       │       ├── GISelMITest.h
    │       │       ├── LegalizerHelperTest.cpp
    │       │       ├── LegalizerInfoTest.cpp
    │       │       └── PatternMatchTest.cpp
    │       ├── DebugInfo/
    │       │   ├── CMakeLists.txt
    │       │   ├── CodeView/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── RandomAccessVisitorTest.cpp
    │       │   │   ├── TypeHashingTest.cpp
    │       │   │   └── TypeIndexDiscoveryTest.cpp
    │       │   ├── DWARF/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── DWARFDebugInfoTest.cpp
    │       │   │   ├── DWARFDebugLineTest.cpp
    │       │   │   ├── DWARFFormValueTest.cpp
    │       │   │   ├── DwarfGenerator.cpp
    │       │   │   ├── DwarfGenerator.h
    │       │   │   ├── DwarfUtils.cpp
    │       │   │   └── DwarfUtils.h
    │       │   ├── MSF/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── MappedBlockStreamTest.cpp
    │       │   │   ├── MSFBuilderTest.cpp
    │       │   │   └── MSFCommonTest.cpp
    │       │   └── PDB/
    │       │       ├── CMakeLists.txt
    │       │       ├── HashTableTest.cpp
    │       │       ├── NativeSymbolReuseTest.cpp
    │       │       ├── PDBApiTest.cpp
    │       │       └── StringTableBuilderTest.cpp
    │       ├── Demangle/
    │       │   ├── CMakeLists.txt
    │       │   ├── ItaniumDemangleTest.cpp
    │       │   └── PartialDemangleTest.cpp
    │       ├── ExecutionEngine/
    │       │   ├── CMakeLists.txt
    │       │   ├── ExecutionEngineTest.cpp
    │       │   ├── MCJIT/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── MCJITCAPITest.cpp
    │       │   │   ├── MCJITMemoryManagerTest.cpp
    │       │   │   ├── MCJITMultipleModuleTest.cpp
    │       │   │   ├── MCJITObjectCacheTest.cpp
    │       │   │   ├── MCJITTest.cpp
    │       │   │   ├── MCJITTestAPICommon.h
    │       │   │   ├── MCJITTestBase.h
    │       │   │   └── MCJITTests.def
    │       │   └── Orc/
    │       │       ├── CMakeLists.txt
    │       │       ├── CoreAPIsTest.cpp
    │       │       ├── GlobalMappingLayerTest.cpp
    │       │       ├── IndirectionUtilsTest.cpp
    │       │       ├── JITTargetMachineBuilderTest.cpp
    │       │       ├── LazyCallThroughAndReexportsTest.cpp
    │       │       ├── LazyEmittingLayerTest.cpp
    │       │       ├── LegacyAPIInteropTest.cpp
    │       │       ├── LegacyCompileOnDemandLayerTest.cpp
    │       │       ├── LegacyRTDyldObjectLinkingLayerTest.cpp
    │       │       ├── ObjectTransformLayerTest.cpp
    │       │       ├── OrcCAPITest.cpp
    │       │       ├── OrcTestCommon.cpp
    │       │       ├── OrcTestCommon.h
    │       │       ├── QueueChannel.cpp
    │       │       ├── QueueChannel.h
    │       │       ├── RemoteObjectLayerTest.cpp
    │       │       ├── RPCUtilsTest.cpp
    │       │       ├── RTDyldObjectLinkingLayerTest.cpp
    │       │       ├── SymbolStringPoolTest.cpp
    │       │       └── ThreadSafeModuleTest.cpp
    │       ├── FuzzMutate/
    │       │   ├── CMakeLists.txt
    │       │   ├── OperationsTest.cpp
    │       │   ├── RandomIRBuilderTest.cpp
    │       │   ├── ReservoirSamplerTest.cpp
    │       │   └── StrategiesTest.cpp
    │       ├── IR/
    │       │   ├── AsmWriterTest.cpp
    │       │   ├── AttributesTest.cpp
    │       │   ├── BasicBlockTest.cpp
    │       │   ├── CFGBuilder.cpp
    │       │   ├── CFGBuilder.h
    │       │   ├── CMakeLists.txt
    │       │   ├── ConstantRangeTest.cpp
    │       │   ├── ConstantsTest.cpp
    │       │   ├── DebugInfoTest.cpp
    │       │   ├── DebugTypeODRUniquingTest.cpp
    │       │   ├── DominatorTreeBatchUpdatesTest.cpp
    │       │   ├── DominatorTreeTest.cpp
    │       │   ├── DomTreeUpdaterTest.cpp
    │       │   ├── FunctionTest.cpp
    │       │   ├── InstructionsTest.cpp
    │       │   ├── IntrinsicsTest.cpp
    │       │   ├── IRBuilderTest.cpp
    │       │   ├── LegacyPassManagerTest.cpp
    │       │   ├── ManglerTest.cpp
    │       │   ├── MDBuilderTest.cpp
    │       │   ├── MetadataTest.cpp
    │       │   ├── ModuleTest.cpp
    │       │   ├── PassBuilderCallbacksTest.cpp
    │       │   ├── PassManagerTest.cpp
    │       │   ├── PatternMatch.cpp
    │       │   ├── TypesTest.cpp
    │       │   ├── UserTest.cpp
    │       │   ├── UseTest.cpp
    │       │   ├── ValueHandleTest.cpp
    │       │   ├── ValueMapTest.cpp
    │       │   ├── ValueTest.cpp
    │       │   ├── VerifierTest.cpp
    │       │   └── WaymarkTest.cpp
    │       ├── LineEditor/
    │       │   ├── CMakeLists.txt
    │       │   └── LineEditor.cpp
    │       ├── Linker/
    │       │   ├── CMakeLists.txt
    │       │   └── LinkModulesTest.cpp
    │       ├── MC/
    │       │   ├── CMakeLists.txt
    │       │   ├── Disassembler.cpp
    │       │   ├── DwarfLineTables.cpp
    │       │   ├── StringTableBuilderTest.cpp
    │       │   └── TargetRegistry.cpp
    │       ├── MI/
    │       │   ├── CMakeLists.txt
    │       │   └── LiveIntervalTest.cpp
    │       ├── Object/
    │       │   ├── CMakeLists.txt
    │       │   ├── SymbolicFileTest.cpp
    │       │   └── SymbolSizeTest.cpp
    │       ├── ObjectYAML/
    │       │   ├── CMakeLists.txt
    │       │   └── YAMLTest.cpp
    │       ├── Option/
    │       │   ├── CMakeLists.txt
    │       │   ├── OptionParsingTest.cpp
    │       │   └── Opts.td
    │       ├── OptRemarks/
    │       │   ├── CMakeLists.txt
    │       │   └── OptRemarksParsingTest.cpp
    │       ├── Passes/
    │       │   ├── CMakeLists.txt
    │       │   ├── PluginsTest.cpp
    │       │   ├── TestPlugin.cpp
    │       │   └── TestPlugin.h
    │       ├── ProfileData/
    │       │   ├── CMakeLists.txt
    │       │   ├── CoverageMappingTest.cpp
    │       │   ├── InstrProfTest.cpp
    │       │   └── SampleProfTest.cpp
    │       ├── Support/
    │       │   ├── AlignOfTest.cpp
    │       │   ├── AllocatorTest.cpp
    │       │   ├── ARMAttributeParser.cpp
    │       │   ├── ArrayRecyclerTest.cpp
    │       │   ├── BinaryStreamTest.cpp
    │       │   ├── BlockFrequencyTest.cpp
    │       │   ├── BranchProbabilityTest.cpp
    │       │   ├── CachePruningTest.cpp
    │       │   ├── Casting.cpp
    │       │   ├── CheckedArithmeticTest.cpp
    │       │   ├── Chrono.cpp
    │       │   ├── CMakeLists.txt
    │       │   ├── CommandLineTest.cpp
    │       │   ├── CompressionTest.cpp
    │       │   ├── ConvertUTFTest.cpp
    │       │   ├── CrashRecoveryTest.cpp
    │       │   ├── DataExtractorTest.cpp
    │       │   ├── DebugCounterTest.cpp
    │       │   ├── DebugTest.cpp
    │       │   ├── DJBTest.cpp
    │       │   ├── EndianStreamTest.cpp
    │       │   ├── EndianTest.cpp
    │       │   ├── ErrnoTest.cpp
    │       │   ├── ErrorOrTest.cpp
    │       │   ├── ErrorTest.cpp
    │       │   ├── FileOutputBufferTest.cpp
    │       │   ├── formatted_raw_ostream_test.cpp
    │       │   ├── FormatVariadicTest.cpp
    │       │   ├── GlobPatternTest.cpp
    │       │   ├── Host.cpp
    │       │   ├── ItaniumManglingCanonicalizerTest.cpp
    │       │   ├── JSONTest.cpp
    │       │   ├── LEB128Test.cpp
    │       │   ├── LineIteratorTest.cpp
    │       │   ├── LockFileManagerTest.cpp
    │       │   ├── ManagedStatic.cpp
    │       │   ├── MathExtrasTest.cpp
    │       │   ├── MD5Test.cpp
    │       │   ├── MemoryBufferTest.cpp
    │       │   ├── MemoryTest.cpp
    │       │   ├── NativeFormatTests.cpp
    │       │   ├── ParallelTest.cpp
    │       │   ├── Path.cpp
    │       │   ├── ProcessTest.cpp
    │       │   ├── ProgramTest.cpp
    │       │   ├── raw_ostream_test.cpp
    │       │   ├── raw_pwrite_stream_test.cpp
    │       │   ├── raw_sha1_ostream_test.cpp
    │       │   ├── RegexTest.cpp
    │       │   ├── ReplaceFileTest.cpp
    │       │   ├── ReverseIterationTest.cpp
    │       │   ├── ScaledNumberTest.cpp
    │       │   ├── SourceMgrTest.cpp
    │       │   ├── SpecialCaseListTest.cpp
    │       │   ├── StringPool.cpp
    │       │   ├── SwapByteOrderTest.cpp
    │       │   ├── SymbolRemappingReaderTest.cpp
    │       │   ├── TargetParserTest.cpp
    │       │   ├── TarWriterTest.cpp
    │       │   ├── TaskQueueTest.cpp
    │       │   ├── Threading.cpp
    │       │   ├── ThreadLocalTest.cpp
    │       │   ├── ThreadPool.cpp
    │       │   ├── TimerTest.cpp
    │       │   ├── TrailingObjectsTest.cpp
    │       │   ├── TrigramIndexTest.cpp
    │       │   ├── TypeNameTest.cpp
    │       │   ├── TypeTraitsTest.cpp
    │       │   ├── UnicodeTest.cpp
    │       │   ├── VersionTupleTest.cpp
    │       │   ├── VirtualFileSystemTest.cpp
    │       │   ├── xxhashTest.cpp
    │       │   ├── YAMLIOTest.cpp
    │       │   ├── YAMLParserTest.cpp
    │       │   └── DynamicLibrary/
    │       │       ├── CMakeLists.txt
    │       │       ├── DynamicLibraryTest.cpp
    │       │       ├── ExportedFuncs.cpp
    │       │       ├── PipSqueak.cpp
    │       │       └── PipSqueak.h
    │       ├── Target/
    │       │   ├── CMakeLists.txt
    │       │   ├── AArch64/
    │       │   │   ├── CMakeLists.txt
    │       │   │   └── InstSizes.cpp
    │       │   └── WebAssembly/
    │       │       ├── CMakeLists.txt
    │       │       └── WebAssemblyExceptionInfoTest.cpp
    │       ├── TextAPI/
    │       │   ├── CMakeLists.txt
    │       │   └── ELFYAMLTest.cpp
    │       ├── tools/
    │       │   ├── CMakeLists.txt
    │       │   ├── llvm-cfi-verify/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── FileAnalysis.cpp
    │       │   │   └── GraphBuilder.cpp
    │       │   └── llvm-exegesis/
    │       │       ├── BenchmarkRunnerTest.cpp
    │       │       ├── ClusteringTest.cpp
    │       │       ├── CMakeLists.txt
    │       │       ├── PerfHelperTest.cpp
    │       │       ├── RegisterValueTest.cpp
    │       │       ├── AArch64/
    │       │       │   ├── CMakeLists.txt
    │       │       │   └── TargetTest.cpp
    │       │       ├── ARM/
    │       │       │   ├── AssemblerTest.cpp
    │       │       │   └── CMakeLists.txt
    │       │       ├── Common/
    │       │       │   └── AssemblerUtils.h
    │       │       ├── PowerPC/
    │       │       │   ├── AnalysisTest.cpp
    │       │       │   ├── CMakeLists.txt
    │       │       │   └── TargetTest.cpp
    │       │       └── X86/
    │       │           ├── AnalysisTest.cpp
    │       │           ├── AssemblerTest.cpp
    │       │           ├── BenchmarkResultTest.cpp
    │       │           ├── CMakeLists.txt
    │       │           ├── RegisterAliasingTest.cpp
    │       │           ├── SnippetGeneratorTest.cpp
    │       │           └── TargetTest.cpp
    │       ├── Transforms/
    │       │   ├── CMakeLists.txt
    │       │   ├── IPO/
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── LowerTypeTests.cpp
    │       │   │   └── WholeProgramDevirt.cpp
    │       │   ├── Scalar/
    │       │   │   ├── CMakeLists.txt
    │       │   │   └── LoopPassManagerTest.cpp
    │       │   ├── Utils/
    │       │   │   ├── ASanStackFrameLayoutTest.cpp
    │       │   │   ├── BasicBlockUtilsTest.cpp
    │       │   │   ├── CloningTest.cpp
    │       │   │   ├── CMakeLists.txt
    │       │   │   ├── CodeExtractorTest.cpp
    │       │   │   ├── FunctionComparatorTest.cpp
    │       │   │   ├── IntegerDivisionTest.cpp
    │       │   │   ├── LocalTest.cpp
    │       │   │   ├── SSAUpdaterBulkTest.cpp
    │       │   │   ├── UnrollLoopTest.cpp
    │       │   │   └── ValueMapperTest.cpp
    │       │   └── Vectorize/
    │       │       ├── CMakeLists.txt
    │       │       ├── VPlanDominatorTreeTest.cpp
    │       │       ├── VPlanHCFGTest.cpp
    │       │       ├── VPlanLoopInfoTest.cpp
    │       │       ├── VPlanSlpTest.cpp
    │       │       ├── VPlanTest.cpp
    │       │       └── VPlanTestBase.h
    │       └── XRay/
    │           ├── CMakeLists.txt
    │           ├── FDRBlockIndexerTest.cpp
    │           ├── FDRBlockVerifierTest.cpp
    │           ├── FDRProducerConsumerTest.cpp
    │           ├── FDRRecordPrinterTest.cpp
    │           ├── FDRRecordsTest.cpp
    │           ├── FDRTraceWriterTest.cpp
    │           ├── GraphTest.cpp
    │           └── ProfileTest.cpp
    └── tests/
        ├── build.py
        └── samples/
            ├── sample1.c
            ├── sample10.c
            ├── sample10.h
            ├── sample11.c
            ├── sample12.c
            ├── sample13.c
            ├── sample13.h
            ├── sample14.c
            ├── sample14.h
            ├── sample15.c
            ├── sample15.h
            ├── sample16.c
            ├── sample17.c
            ├── sample18.c
            ├── sample19.c
            ├── sample2.c
            ├── sample20.c
            ├── sample21.c
            ├── sample3.c
            ├── sample4.c
            ├── sample5.c
            ├── sample6.c
            ├── sample7.c
            ├── sample8.c
            └── sample9.c


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
# xVMP

xVMP is an LLVM IR-based code virtualization tool, which fulfilled a scalable and virtualized instruction-hardened obfuscation. It supports multiple programming languages, and architectures. It is also compatible with existing LLVM IR-based obfuscation schemes (such as Obfuscator-LLVM).

xVMP is developer friendly. You only need to add annotations to the to-be-protected function in the source code, and xVMP can perform virtualization protection on the function during compilation.



## Table of Contents

- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [Examples](#examples)
- [Precautions](#Precautions)
- [Maintainers](#maintainers)
- [Contributing](#contributing)



## Background

Virtualization-based software protection schemes protect the logic and data in the program by converting the original code into a new bytecode based on the custom instruction set architecture (ISA). The new bytecode is emulated via an embedded virtual machine (i.e. interpreter) at runtime. Since a lot of reverse engineering is required for attackers to learn the custom ISA, virtualization obfuscation could hide valuable assets in software.

To meet the requirements in real-world software development, the virtualization obfuscator should achieve the following three goals:

- i) Strong protection, which means that virtualized code should resist various de-virtualization techniques such as symbolic execution, frequency analysis, etc.
- ii) Compatibility, which means the virtualization obfuscator should support different source code types, platforms, instruction sets, and various code obfuscation schemes.
- iii) Ease of use, i.e., developers only need to make simple marks to complete the obfuscation.

Unfortunately, the state-of-the-art virtualization obfuscators cannot fulfill the above requirements. On the one hand, they lack effective protection for virtualization instructions (Tigress only xors a constant for all instructions) and many works in recent years have broken through them by using frequency analysis and symbolic execution. On the other hand, VMProtect and Themida only support virtualize executables on X86 and X64 architectures, and they are not open source. The most advanced academic virtualization scheme Tigress can only support C language source code, and since its input must be a single file containing the full program source code, it is difficult to blend in the software development cycle.

Therefore, we present xVMP, an LLVM-based code virtualization obfuscator fulfills these goals. It incorporates the obfuscation process of code virtualization into the compilation to mask the effects of different architectures and program languages. xVMP generates virtualized code based on LLVM IR and embeds the interpreter of virtualized code into the IR and compiles to an executable. To enhance the security, xVMP encrypts virtualized instructions in each basic block and decrypts them at runtime to enhance the security of obfuscation. In addition, it supports specified function obfuscation. xVMP identifies the function annotations marked by the developer in the source code to locate the function to protect.



## Install

### Prebuilt Binaries

Please download the latest prebuilt binaries from [Release](https://github.com/GANGE666/xVMP/releases).

### Building from source with Obfuscator-LLVM

The code in the master branch is xVMP mixed with obfuscator-llvm based on LLLVM 8.0.

0. Prerequisites. Same as [LLVM building requirements](https://llvm.org/docs/GettingStarted.html#requirements).

1. Use the building script. It will build xVMP and compatible obfuscator-llvm in the `build` directory.

```bash
$ bash ./build.sh
```

### Building as a plugin for LLVM

TBD

### Docker

TBD



## Usage

You only need to add the annotation before the definition of the to-be-protected function. As shown in the following code.

```c
__attribute((__annotate__("vmp"))) 	// add this annotation
void gen_deckey (unsigned char *decrypt_key, char *passwd) {
  // generate decrypt key from the password
}
```

Then compile the source code using the LLVM toolchain with xVMP.

But please heed these [precautions](#Precautions).



## Examples

We have prepared three examples in the [examples](./examples/) directory to show how to use xVMP.
In these examples, you can use xVMP alone or use xVMP with ollvm to protect specific functions easily, and you can also see the advantages of xVMP over Tigress.

We use `/examples/test/test2` as an example. Part of the source code is shown below.

```c
#ifdef ENABLE_OLLVM
__attribute((__annotate__(("fla"))))
__attribute((__annotate__(("bcf"))))
#endif
#ifdef ENABLE_XVMP
__attribute((__annotate__(("vmp"))))
#endif
uint32_t tea_decrypt (uint32_t* v) {
    uint32_t v0=v[0], v1=v[1], sum=0xC6EF3720, i;  /* set up */
    uint32_t delta=0x9e3779b9;                     /* a key schedule constant */
    uint32_t k0=0x94C36D33, k1=0x164512A3, k2=0xFEEEDA59, k3=0x87BD19BD;   /* cache key */
    for (i=0; i<32; i++) {                         /* basic cycle start */
        v1 -= ((v0<<4) + k2) ^ (v0 + sum) ^ ((v0>>5) + k3);
        v0 -= ((v1<<4) + k0) ^ (v1 + sum) ^ ((v1>>5) + k1);
        sum -= delta;
    }                                              /* end cycle */
    v[0]=v0; v[1]=v1;
    return v[0];
}
```

We will show the protection effects after four compilation schemes:

- Original build
- Tigress protection
- xVMP protection
- xVMP combined with Obfuscator-LLVM protection



#### Original build

Use `clang test2.c -o test2` to build an unprotected program. The unprotected programs can be easily analyzed for original logic using reverse engineering tools, like IDA Pro.

<img src="imgs/image-20230212154152017.png" alt="image-20230212154152017" style="zoom:50%;" />

#### Tigress Protection

Use `tigress --Environment=x86_64:Linux:Gcc:4.6 --Seed=0  --Transform=Virtualize   --VirtualizeDispatch=interpolation --Functions=tea_decrypt --VirtualizeEncodeByteArray=true test2.c --out=test2_tigress.c` to protect the `test2` with Tigress.

In IDA, we can clearly see that the virtualized code only XORs a constant for protection, which is very easy to be broken. The length of virtualized function is 0x7CA.

<img src="imgs/image-20230212154624109.png" alt="image-20230212154624109" style="zoom:50%;" />

<img src="imgs/image-20230212154747677.png" alt="image-20230212154747677" style="zoom:50%;" />

#### xVMP Protection

Use `clang -DENABLE_XVMP test2.c -o test2_xvmp `  to protect the `test2` with xVMP.

The virtualization code of program protected by xVMP is more hardened and protected, and the interpreter is more complicated.

The length of function `vm_interpreter_tea_decrypt` is 0x5A71.

<img src="imgs/image-20230212155037488.png" alt="image-20230212155037488" style="zoom:50%;" />

<img src="imgs/image-20230212155055490.png" alt="image-20230212155055490" style="zoom:50%;" />

#### xVMP+Obfuscator-LLVM

Use  `clang -DENABLE_XVMP -DENABLE_OLLVM test2.c -o test2_xvmp_ollvm`  to protect the `test2` with xVMP and obfuscator-LLVM.

The protection of xVMP+oLLVM makes it more difficult for attackers to be reversed.

The length of function `vm_interpreter_tea_decrypt` is 0x149F2.

<img src="imgs/image-20230212155110480.png" alt="image-20230212155110480" style="zoom:50%;" />



## Precautions

- Code optimization. Virtualization is unsound because code optimization may introduces instructions that xVMP cannot handle. So please compile with the `-O0` option, or optimize after xVMP virtualization is complete. Please do not use the `-O3`, `-O2` option.
- Please do not use the `-g` option. Because it will introduce instructions such as `@llvm.dbg.declare`.
- If you want to modify the interpreter, please run the `scripts/rebuild-with-interpreter.sh` script after installing python2 to update the hard-coded interpreter. The interpreter source code is in the `src/xVMPInterpreter` directory.
- SWITCH, PHI statement is not support yet.



## Maintainers

[@G6](https://github.com/GANGE666).

## Contributing

Feel free to dive in! [Open an issue](https://github.com/GANGE666/xVMP/issues/new) or submit PRs.




================================================
FILE: build.sh
================================================
#!/bin/bash
cd "$(dirname "$0")"

if [ ! -d "build" ]; then
    mkdir build
    cd build
#    cmake -DCMAKE_C_COMPILER=gcc -DCMAKE_CXX_COMPILER=g++ -DCMAKE_BUILD_TYPE=Release -GNinja -DCMAKE_BUILD_TYPE="Release" ../src
    cmake -DCMAKE_C_COMPILER=gcc -DCMAKE_CXX_COMPILER=g++ -DCMAKE_BUILD_TYPE=Release -DCMAKE_BUILD_TYPE="Release" ../src
else
    cd build
fi


cmake --build .




================================================
FILE: examples/test1/README.md
================================================
# Original
`clang test1.c -o test1`

# xVMP
xvmp:
`clang -DENABLE_XVMP test1.c -o test1_xvmp`

xvmp+ollvm:
`clang -DENABLE_XVMP -DENABLE_OLLVM test1.c -o test1_xvmp_ollvm`

# Tigress
`tigress --Environment=x86_64:Linux:Gcc:4.6 --Seed=0  --Transform=Virtualize   --VirtualizeDispatch=interpolation --Functions=vm_test --VirtualizeEncodeByteArray=true test1.c --out=test1_tigress.c`
`clang test1_tigress.c -o test1_tigress`




================================================
FILE: examples/test1/test1.c
================================================
#include<stdio.h>

#ifdef ENABLE_OLLVM
__attribute((__annotate__(("fla"))))
__attribute((__annotate__(("bcf"))))
#endif
#ifdef ENABLE_XVMP
__attribute((__annotate__(("vmp"))))
#endif
void vm_test(char * buf, int len){
        for(int i = 0; i < len; i++)
                buf[i] ^= 0x3A;
}

int main() {
    char array[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    vm_test(array, 10);

    for (int i=0; i<10; i++) {
        printf("%d, ", array[i]);
    }
    printf("\n");
}




================================================
FILE: examples/test2/README.md
================================================
# Original
`clang test2.c -o test2`

# xVMP
xvmp:
`clang -DENABLE_XVMP test2.c -o test2_xvmp`

xvmp+ollvm:
`clang -DENABLE_XVMP -DENABLE_OLLVM test2.c -o test2_xvmp_ollvm`

# Tigress
`tigress --Environment=x86_64:Linux:Gcc:4.6 --Seed=0  --Transform=Virtualize   --VirtualizeDispatch=interpolation --Functions=tea_decrypt --VirtualizeEncodeByteArray=true test2.c --out=test2_tigress.c`
`clang test2_tigress.c -o test2_tigress`




================================================
FILE: examples/test2/test2.c
================================================
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <stdint.h>

void tea_encrypt (uint32_t* v, uint32_t* k) {
    uint32_t v0=v[0], v1=v[1], sum=0, i;           /* set up */
    uint32_t delta=0x9e3779b9;                     /* a key schedule constant */
    uint32_t k0=k[0], k1=k[1], k2=k[2], k3=k[3];   /* cache key */
    for (i=0; i < 32; i++) {                       /* basic cycle start */
        sum += delta;
        v0 += ((v1<<4) + k0) ^ (v1 + sum) ^ ((v1>>5) + k1);
        v1 += ((v0<<4) + k2) ^ (v0 + sum) ^ ((v0>>5) + k3);
    }                                              /* end cycle */
    v[0]=v0; v[1]=v1;
}

#ifdef ENABLE_OLLVM
__attribute((__annotate__(("fla"))))
__attribute((__annotate__(("bcf"))))
#endif
#ifdef ENABLE_XVMP
__attribute((__annotate__(("vmp"))))
#endif
uint32_t tea_decrypt (uint32_t* v) {
    // uint32_t* v = &input;
    uint32_t v0=v[0], v1=v[1], sum=0xC6EF3720, i;  /* set up */
    uint32_t delta=0x9e3779b9;                     /* a key schedule constant */
    uint32_t k0=0x94C36D33, k1=0x164512A3, k2=0xFEEEDA59, k3=0x87BD19BD;   /* cache key */
    for (i=0; i<32; i++) {                         /* basic cycle start */
        v1 -= ((v0<<4) + k2) ^ (v0 + sum) ^ ((v0>>5) + k3);
        v0 -= ((v1<<4) + k0) ^ (v1 + sum) ^ ((v1>>5) + k1);
        sum -= delta;
    }                                              /* end cycle */
    v[0]=v0; v[1]=v1;
    return v[0];
}

int main(int argc, char **argv) {
    if (argc < 2) {
        printf("Call this program with 1 arguments\n");
        return 1;
    }

    unsigned long input = strtoul(argv[1], 0, 10);
    uint32_t v[2] = {0};
    v[0] = input & 0xFFFFFFFF;
    v[1] = 0;

    // uint32_t output = SECRET(input);
    uint32_t output = tea_decrypt(v);

    printf("%u\n", output);

    return 0;
}




================================================
FILE: examples/test3/README.md
================================================
# Original
`clang test3_main.c test3_foo.c -o test3`

# xVMP
xvmp:
`clang -DENABLE_XVMP test3_main.c test3_foo.c -o test3_xvmp`

xvmp+ollvm:
`clang -DENABLE_XVMP -DENABLE_OLLVM test3_main.c test3_foo.c -o test3_xvmp_ollvm`

# Tigress
Because Tigress can only accept a whole program single C file as input, which means that the original compilation process needs to be broken and is very unfriendly to developers.
And you need merge all C file into one as following.
`tigress-merge test3_main.c test3_foo.c --out=test3_tigress.c`
`tigress --Environment=x86_64:Linux:Gcc:4.6 --Seed=0  --Transform=Virtualize   --VirtualizeDispatch=interpolation --Functions=foo --VirtualizeEncodeByteArray=true test3_tigress.c --out=test3_tigress_obf.c`
`clang test3_tigress_obf.c -o test3_tigress_obf`

If you directly obfuscate `test3_foo.c` by Tigress, a new `main` function will be introduced in the output file of `test_foo.c`.





================================================
FILE: examples/test3/test3_foo.c
================================================

#ifdef ENABLE_OLLVM
__attribute((__annotate__(("fla"))))
__attribute((__annotate__(("bcf"))))
#endif
#ifdef ENABLE_XVMP
__attribute((__annotate__(("vmp"))))
#endif
int foo(int a, int b) {
    return a+b;
}



================================================
FILE: examples/test3/test3_foo.h
================================================
int foo(int a, int b);



================================================
FILE: examples/test3/test3_main.c
================================================
#include "test3_foo.h"

int main(int argc, char **argv) {
    if (argc < 2) {
        printf("Call this program with 1 arguments\n");
        return 1;
    }

    int input = atoi(argv[1]);

    int res = foo(input, 0xdeadbeef);
    printf("%d\n", res);

    return 0;
}




================================================
FILE: scripts/interpreter-ir2str.py
================================================
import binascii
import os

def cut(obj, sec):
    return [obj[i:i+sec] for i in range(0,len(obj),sec)]


def bytecode2string2():

    # tranverse .bc to hex output
    f = open("/tmp/xVMPInterpreter.bc", "rb")
    data = f.read()
    data_hex = binascii.b2a_hex(data)
    f.close()

    # f = open("/tmp/vm.h", "w")
    currpath = os.path.dirname(os.path.abspath(__file__))
    f = open(currpath+"/../src/include/llvm/Transforms/Obfuscation/vm.h", "w")

    f.write("#include <string>\n")
    f.write("const int binary_ir_length = " + str(len(data)) +";\n")

    f.write("std::vector<std::string> binary_ir_vector = \n{")

    for data_cut in cut(data_hex, 10000):
        f.write("\tstd::string(\"")
        for i in range(len(data_cut)//2):
            f.write("\\x" + data_cut[2*i: 2*(i+1)])
        f.write("\", %d),\n" % (len(data_cut)//2))

    f.write("\n};\n\n")

    f.write("std::string binary_ir;")

    # f.write("""
    # binary_ir.resize(binary_ir_length);
    # int binary_ir_idx = 0;
    # for(auto s: binary_ir_vector) {
    #     for (int i = 0; i < s.size(); i++) {
    #         binary_ir[binary_ir_idx++] = s[i];
    #     }
    # }
    # """)

    f.close()


bytecode2string2()

print("[*] finish!")




================================================
FILE: scripts/rebuild-with-interpreter.sh
================================================
#!/bin/bash
set -ex

ROOT_PATH=$(cd $(dirname $0)/../; pwd)
# echo $ROOT_PATH

# use clang-8 to compile interpreter first.
# CLANG_PATH=/ollvm/ollvm/llvm-8/llvm-project/build/bin/
CLANG_PATH=./build/bin/

$CLANG_PATH/clang-8 -O0 -Xclang -disable-O0-optnone -emit-llvm -c $ROOT_PATH/src/xVMPInterpreter/xVMPInterpreter.c -o /tmp/xVMPInterpreter.bc
$CLANG_PATH/llvm-dis /tmp/xVMPInterpreter.bc -o /tmp/xVMPInterpreter.ll

python2 $ROOT_PATH/scripts/interpreter-ir2str.py





================================================
FILE: src/llvm.spec.in
================================================
Name: @PACKAGE_NAME@
Version: @PACKAGE_VERSION@
Release: 0
Summary: LLVM (An Optimizing Compiler Infrastructure)
License: University of Illinois/NCSA Open Source License
Vendor: None (open source)
Group: Development/Compilers
URL: http://llvm..org/
Source: http://llvm.org/releases/@PACKAGE_VERSION@/@PACKAGE_NAME@-@PACKAGE_VERSION@.tar.gz
BuildRoot: %{_tmppath}/%{name}-root
Requires: /sbin/ldconfig
BuildRequires: gcc >= 3.4

%description
LLVM is a compiler infrastructure designed for compile-time, link-time, runtime,
and idle-time optimization of programs from arbitrary programming languages.
LLVM is written in C++ and has been developed since 2000 at the University of
Illinois and Apple. It currently supports compilation of C and C++ programs,
using front-ends derived from GCC 4.0.1. A new front-end for the C family of
languages is in development. The compiler infrastructure
includes mirror sets of programming tools as well as libraries with equivalent
functionality.

%prep
%setup -q -n @PACKAGE_NAME@-@PACKAGE_VERSION@

%build
./configure \
--prefix=%{_prefix} \
--bindir=%{_bindir} \
--datadir=%{_datadir} \
--includedir=%{_includedir} \
--libdir=%{_libdir} \
--enable-optimized \
--enable-assertions
make tools-only

%install
rm -rf %{buildroot}
make install DESTDIR=%{buildroot}

%clean
rm -rf %{buildroot}

%post -p /sbin/ldconfig

%postun -p /sbin/ldconfig

%files
%defattr(-, root, root)
%doc CREDITS.TXT LICENSE.TXT README.txt docs/*.{html,css,gif,jpg} docs/CommandGuide
%{_bindir}/*
%{_libdir}/*.o
%{_libdir}/*.a
%{_libdir}/*.so
%{_includedir}/llvm

%changelog
* Fri Aug 04 2006 Reid Spencer
- Updates for release 1.8
* Fri Apr 07 2006 Reid Spencer
- Make the build be optimized+assertions
* Fri May 13 2005 Reid Spencer
- Minor adjustments for the 1.5 release
* Mon Feb 09 2003 Brian R. Gaeke
- Initial working version of RPM spec file.





================================================
FILE: src/RELEASE_TESTERS.TXT
================================================
This file is a list of the people responsible for ensuring that targets and
environments get tested and validated during the release process.

They will also, in conjunction with the release manager and the code owners,
accept patches into stable release branches, tag critical bugs and release
stoppers as well as make sure that no regressions were observed on their
targets since the last release.

N: Ben Pope
E: benpope81@gmail.com
T: x86
O: Ubuntu

N: Sylvestre Ledru
E: sylvestre@debian.org
T: All supported archs Debian/Ubuntu
O: Debian/Ubuntu packages

N: Nikola Smiljanic
E: popizdeh@gmail.com
T: x86
O: OpenSUSE, Fedora

N: Brian Cain
E: brian.cain@gmail.com
T: x86
O: SuSE Enterprise, CentOS

N: Bernhard Rosenkränzer
E: bero@linaro.org
T: x86
O: OpenMandriva

N: Dimitry Andric
E: dimitry@andric.com
T: x86
O: FreeBSD

N: Hans Wennborg
E: hans@chromium.org
T: x86
O: Windows

N: Diana Picus, Yvan Roux
E: diana.picus@linaro.org, yvan.roux@linaro.org
T: ARM, AArch64
O: Linux



================================================
FILE: src/bindings/LLVMBuild.txt
================================================
;===- ./bindings/LLVMBuild.txt ---------------------------------*- Conf -*--===;
;
;                     The LLVM Compiler Infrastructure
;
; This file is distributed under the University of Illinois Open Source
; License. See LICENSE.TXT for details.
;
;===------------------------------------------------------------------------===;
;
; This is an LLVMBuild description file for the components in this subdirectory.
;
; For more information on the LLVMBuild system, please see:
;
;   http://llvm.org/docs/LLVMBuild.html
;
;===------------------------------------------------------------------------===;

[component_0]
type = Group
name = Bindings
parent = $ROOT



================================================
FILE: src/bindings/README.txt
================================================
This directory contains bindings for the LLVM compiler infrastructure to allow
programs written in languages other than C or C++ to take advantage of the LLVM
infrastructure--for instance, a self-hosted compiler front-end.



================================================
FILE: src/bindings/go/build.sh
================================================
#!/bin/sh -xe

gollvmdir=$(dirname "$0")/llvm

workdir=$gollvmdir/workdir
llvmdir=$gollvmdir/../../..
llvm_builddir=$workdir/llvm_build

mkdir -p $llvm_builddir

cmake_flags="../../../../.. $@"
llvm_config="$llvm_builddir/bin/llvm-config"
llvm_go="$llvm_builddir/bin/llvm-go"

if test -n "`which ninja`" ; then
  # If Ninja is available, we can speed up the build by building only the
  # required subset of LLVM.
  (cd $llvm_builddir && cmake -G Ninja $cmake_flags)
  ninja -C $llvm_builddir llvm-config llvm-go
  llvm_components="$($llvm_go print-components)"
  llvm_buildtargets="$($llvm_config --libs $llvm_components | sed -e 's/-l//g')"
  ninja -C $llvm_builddir $llvm_buildtargets FileCheck
else
  (cd $llvm_builddir && cmake $cmake_flags)
  make -C $llvm_builddir -j4
fi

$llvm_go print-config > $gollvmdir/llvm_config.go



================================================
FILE: src/bindings/go/conftest.go
================================================
package main

import (
	"go/build"
	"os"
)

// Tests that the Go compiler is at least version 1.2.
func main() {
	for _, tag := range build.Default.ReleaseTags {
		if tag == "go1.2" {
			os.Exit(0)
		}
	}
	os.Exit(1)
}



================================================
FILE: src/bindings/go/README.txt
================================================
This directory contains LLVM bindings for the Go programming language
(http://golang.org).

Prerequisites
-------------

* Go 1.2+.
* CMake (to build LLVM).

Using the bindings
------------------

The package path "llvm.org/llvm/bindings/go/llvm" can be used to
import the latest development version of LLVM from SVN. Paths such as
"llvm.org/llvm.v36/bindings/go/llvm" refer to released versions of LLVM.

It is recommended to use the "-d" flag with "go get" to download the
package or a dependency, as an additional step is required to build LLVM
(see "Building LLVM" below).

Building LLVM
-------------

The script "build.sh" in this directory can be used to build LLVM and prepare
it to be used by the bindings. If you receive an error message from "go build"
like this:

    ./analysis.go:4:84: fatal error: llvm-c/Analysis.h: No such file or directory
     #include <llvm-c/Analysis.h> // If you are getting an error here read bindings/go/README.txt

or like this:

    ./llvm_dep.go:5: undefined: run_build_sh

it means that LLVM needs to be built or updated by running the script.

    $ $GOPATH/src/llvm.org/llvm/bindings/go/build.sh

Any command line arguments supplied to the script are passed to LLVM's CMake
build system. A good set of arguments to use during development are:

    $ $GOPATH/src/llvm.org/llvm/bindings/go/build.sh -DCMAKE_BUILD_TYPE=Debug -DLLVM_TARGETS_TO_BUILD=host -DBUILD_SHARED_LIBS=ON

Note that CMake keeps a cache of build settings so once you have built
LLVM there is no need to pass these arguments again after updating.

Alternatively, you can build LLVM yourself, but you must then set the
CGO_CPPFLAGS, CGO_CXXFLAGS and CGO_LDFLAGS environment variables:

    $ export CGO_CPPFLAGS="`/path/to/llvm-build/bin/llvm-config --cppflags`"
    $ export CGO_CXXFLAGS=-std=c++11
    $ export CGO_LDFLAGS="`/path/to/llvm-build/bin/llvm-config --ldflags --libs --system-libs all`"
    $ go build -tags byollvm

If you see a compilation error while compiling your code with Go 1.9.4 or later as follows,

    go build llvm.org/llvm/bindings/go/llvm: invalid flag in #cgo LDFLAGS: -Wl,-headerpad_max_install_names

you need to setup $CGO_LDFLAGS_ALLOW to allow a compiler to specify some linker options:

    $ export CGO_LDFLAGS_ALLOW='-Wl,(-search_paths_first|-headerpad_max_install_names)'



================================================
FILE: src/bindings/go/llvm/analysis.go
================================================
//===- analysis.go - Bindings for analysis --------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the analysis component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Analysis.h" // If you are getting an error here read bindings/go/README.txt
#include "llvm-c/Core.h"
#include <stdlib.h>
*/
import "C"
import "errors"

type VerifierFailureAction C.LLVMVerifierFailureAction

const (
	// verifier will print to stderr and abort()
	AbortProcessAction VerifierFailureAction = C.LLVMAbortProcessAction
	// verifier will print to stderr and return 1
	PrintMessageAction VerifierFailureAction = C.LLVMPrintMessageAction
	// verifier will just return 1
	ReturnStatusAction VerifierFailureAction = C.LLVMReturnStatusAction
)

// Verifies that a module is valid, taking the specified action if not.
// Optionally returns a human-readable description of any invalid constructs.
func VerifyModule(m Module, a VerifierFailureAction) error {
	var cmsg *C.char
	broken := C.LLVMVerifyModule(m.C, C.LLVMVerifierFailureAction(a), &cmsg)

	// C++'s verifyModule means isModuleBroken, so it returns false if
	// there are no errors
	if broken != 0 {
		err := errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
		return err
	}
	return nil
}

var verifyFunctionError = errors.New("Function is broken")

// Verifies that a single function is valid, taking the specified action.
// Useful for debugging.
func VerifyFunction(f Value, a VerifierFailureAction) error {
	broken := C.LLVMVerifyFunction(f.C, C.LLVMVerifierFailureAction(a))

	// C++'s verifyFunction means isFunctionBroken, so it returns false if
	// there are no errors
	if broken != 0 {
		return verifyFunctionError
	}
	return nil
}

// Open up a ghostview window that displays the CFG of the current function.
// Useful for debugging.
func ViewFunctionCFG(f Value)     { C.LLVMViewFunctionCFG(f.C) }
func ViewFunctionCFGOnly(f Value) { C.LLVMViewFunctionCFGOnly(f.C) }



================================================
FILE: src/bindings/go/llvm/bitreader.go
================================================
//===- bitreader.go - Bindings for bitreader ------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the bitreader component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/BitReader.h"
#include "llvm-c/Core.h"
#include <stdlib.h>
*/
import "C"

import (
	"errors"
	"unsafe"
)

// ParseBitcodeFile parses the LLVM IR (bitcode) in the file with the
// specified name, and returns a new LLVM module.
func ParseBitcodeFile(name string) (Module, error) {
	var buf C.LLVMMemoryBufferRef
	var errmsg *C.char
	var cfilename *C.char = C.CString(name)
	defer C.free(unsafe.Pointer(cfilename))
	result := C.LLVMCreateMemoryBufferWithContentsOfFile(cfilename, &buf, &errmsg)
	if result != 0 {
		err := errors.New(C.GoString(errmsg))
		C.free(unsafe.Pointer(errmsg))
		return Module{}, err
	}
	defer C.LLVMDisposeMemoryBuffer(buf)

	var m Module
	if C.LLVMParseBitcode2(buf, &m.C) == 0 {
		return m, nil
	}

	err := errors.New(C.GoString(errmsg))
	C.free(unsafe.Pointer(errmsg))
	return Module{}, err
}



================================================
FILE: src/bindings/go/llvm/bitwriter.go
================================================
//===- bitwriter.go - Bindings for bitwriter ------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the bitwriter component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/BitWriter.h"
#include <stdlib.h>
*/
import "C"
import "os"
import "errors"

var writeBitcodeToFileErr = errors.New("Failed to write bitcode to file")

func WriteBitcodeToFile(m Module, file *os.File) error {
	fail := C.LLVMWriteBitcodeToFD(m.C, C.int(file.Fd()), C.int(0), C.int(0))
	if fail != 0 {
		return writeBitcodeToFileErr
	}
	return nil
}

func WriteBitcodeToMemoryBuffer(m Module) MemoryBuffer {
	mb := C.LLVMWriteBitcodeToMemoryBuffer(m.C)
	return MemoryBuffer{mb}
}

// TODO(nsf): Figure out way how to make it work with io.Writer



================================================
FILE: src/bindings/go/llvm/dibuilder.go
================================================
//===- dibuilder.go - Bindings for DIBuilder ------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the DIBuilder class.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "IRBindings.h"
#include <stdlib.h>
*/
import "C"

import (
	"debug/dwarf"
	"unsafe"
)

type DwarfTag uint32

const (
	DW_TAG_lexical_block   DwarfTag = 0x0b
	DW_TAG_compile_unit    DwarfTag = 0x11
	DW_TAG_variable        DwarfTag = 0x34
	DW_TAG_base_type       DwarfTag = 0x24
	DW_TAG_pointer_type    DwarfTag = 0x0F
	DW_TAG_structure_type  DwarfTag = 0x13
	DW_TAG_subroutine_type DwarfTag = 0x15
	DW_TAG_file_type       DwarfTag = 0x29
	DW_TAG_subprogram      DwarfTag = 0x2E
	DW_TAG_auto_variable   DwarfTag = 0x100
	DW_TAG_arg_variable    DwarfTag = 0x101
)

const (
	FlagPrivate = 1 << iota
	FlagProtected
	FlagFwdDecl
	FlagAppleBlock
	FlagBlockByrefStruct
	FlagVirtual
	FlagArtificial
	FlagExplicit
	FlagPrototyped
	FlagObjcClassComplete
	FlagObjectPointer
	FlagVector
	FlagStaticMember
	FlagIndirectVariable
)

type DwarfLang uint32

const (
	// http://dwarfstd.org/ShowIssue.php?issue=101014.1&type=open
	DW_LANG_Go DwarfLang = 0x0016
)

type DwarfTypeEncoding uint32

const (
	DW_ATE_address         DwarfTypeEncoding = 0x01
	DW_ATE_boolean         DwarfTypeEncoding = 0x02
	DW_ATE_complex_float   DwarfTypeEncoding = 0x03
	DW_ATE_float           DwarfTypeEncoding = 0x04
	DW_ATE_signed          DwarfTypeEncoding = 0x05
	DW_ATE_signed_char     DwarfTypeEncoding = 0x06
	DW_ATE_unsigned        DwarfTypeEncoding = 0x07
	DW_ATE_unsigned_char   DwarfTypeEncoding = 0x08
	DW_ATE_imaginary_float DwarfTypeEncoding = 0x09
	DW_ATE_packed_decimal  DwarfTypeEncoding = 0x0a
	DW_ATE_numeric_string  DwarfTypeEncoding = 0x0b
	DW_ATE_edited          DwarfTypeEncoding = 0x0c
	DW_ATE_signed_fixed    DwarfTypeEncoding = 0x0d
	DW_ATE_unsigned_fixed  DwarfTypeEncoding = 0x0e
	DW_ATE_decimal_float   DwarfTypeEncoding = 0x0f
	DW_ATE_UTF             DwarfTypeEncoding = 0x10
	DW_ATE_lo_user         DwarfTypeEncoding = 0x80
	DW_ATE_hi_user         DwarfTypeEncoding = 0xff
)

// DIBuilder is a wrapper for the LLVM DIBuilder class.
type DIBuilder struct {
	ref C.LLVMDIBuilderRef
	m   Module
}

// NewDIBuilder creates a new DIBuilder, associated with the given module.
func NewDIBuilder(m Module) *DIBuilder {
	d := C.LLVMCreateDIBuilder(m.C)
	return &DIBuilder{ref: d, m: m}
}

// Destroy destroys the DIBuilder.
func (d *DIBuilder) Destroy() {
	C.LLVMDisposeDIBuilder(d.ref)
}

// FInalize finalizes the debug information generated by the DIBuilder.
func (d *DIBuilder) Finalize() {
	C.LLVMDIBuilderFinalize(d.ref)
}

// DICompileUnit holds the values for creating compile unit debug metadata.
type DICompileUnit struct {
	Language       DwarfLang
	File           string
	Dir            string
	Producer       string
	Optimized      bool
	Flags          string
	RuntimeVersion int
}

// CreateCompileUnit creates compile unit debug metadata.
func (d *DIBuilder) CreateCompileUnit(cu DICompileUnit) Metadata {
	file := C.CString(cu.File)
	defer C.free(unsafe.Pointer(file))
	dir := C.CString(cu.Dir)
	defer C.free(unsafe.Pointer(dir))
	producer := C.CString(cu.Producer)
	defer C.free(unsafe.Pointer(producer))
	flags := C.CString(cu.Flags)
	defer C.free(unsafe.Pointer(flags))
	result := C.LLVMDIBuilderCreateCompileUnit(
		d.ref,
		C.LLVMDWARFSourceLanguage(cu.Language),
		C.LLVMDIBuilderCreateFile(d.ref, file, C.size_t(len(cu.File)), dir, C.size_t(len(cu.Dir))),
		producer, C.size_t(len(cu.Producer)),
		C.LLVMBool(boolToCInt(cu.Optimized)),
		flags, C.size_t(len(cu.Flags)),
		C.unsigned(cu.RuntimeVersion),
		/*SplitName=*/ nil, 0,
		C.LLVMDWARFEmissionFull,
		/*DWOId=*/ 0,
		/*SplitDebugInlining*/ C.LLVMBool(boolToCInt(true)),
		/*DebugInfoForProfiling*/ C.LLVMBool(boolToCInt(false)),
	)
	return Metadata{C: result}
}

// CreateFile creates file debug metadata.
func (d *DIBuilder) CreateFile(filename, dir string) Metadata {
	cfilename := C.CString(filename)
	defer C.free(unsafe.Pointer(cfilename))
	cdir := C.CString(dir)
	defer C.free(unsafe.Pointer(cdir))
	result := C.LLVMDIBuilderCreateFile(d.ref,
		cfilename, C.size_t(len(filename)),
		cdir, C.size_t(len(dir)))
	return Metadata{C: result}
}

// DILexicalBlock holds the values for creating lexical block debug metadata.
type DILexicalBlock struct {
	File   Metadata
	Line   int
	Column int
}

// CreateLexicalBlock creates lexical block debug metadata.
func (d *DIBuilder) CreateLexicalBlock(diScope Metadata, b DILexicalBlock) Metadata {
	result := C.LLVMDIBuilderCreateLexicalBlock(
		d.ref,
		diScope.C,
		b.File.C,
		C.unsigned(b.Line),
		C.unsigned(b.Column),
	)
	return Metadata{C: result}
}

func (d *DIBuilder) CreateLexicalBlockFile(diScope Metadata, diFile Metadata, discriminator int) Metadata {
	result := C.LLVMDIBuilderCreateLexicalBlockFile(d.ref, diScope.C, diFile.C,
		C.unsigned(discriminator))
	return Metadata{C: result}
}

// DIFunction holds the values for creating function debug metadata.
type DIFunction struct {
	Name         string
	LinkageName  string
	File         Metadata
	Line         int
	Type         Metadata
	LocalToUnit  bool
	IsDefinition bool
	ScopeLine    int
	Flags        int
	Optimized    bool
}

// CreateFunction creates function debug metadata.
func (d *DIBuilder) CreateFunction(diScope Metadata, f DIFunction) Metadata {
	name := C.CString(f.Name)
	defer C.free(unsafe.Pointer(name))
	linkageName := C.CString(f.LinkageName)
	defer C.free(unsafe.Pointer(linkageName))
	result := C.LLVMDIBuilderCreateFunction(
		d.ref,
		diScope.C,
		name, C.size_t(len(f.Name)),
		linkageName, C.size_t(len(f.LinkageName)),
		f.File.C,
		C.unsigned(f.Line),
		f.Type.C,
		C.LLVMBool(boolToCInt(f.LocalToUnit)),
		C.LLVMBool(boolToCInt(f.IsDefinition)),
		C.unsigned(f.ScopeLine),
		C.LLVMDIFlags(f.Flags),
		C.LLVMBool(boolToCInt(f.Optimized)),
	)
	return Metadata{C: result}
}

// DIAutoVariable holds the values for creating auto variable debug metadata.
type DIAutoVariable struct {
	Name           string
	File           Metadata
	Line           int
	Type           Metadata
	AlwaysPreserve bool
	Flags          int
	AlignInBits    uint32
}

// CreateAutoVariable creates local variable debug metadata.
func (d *DIBuilder) CreateAutoVariable(scope Metadata, v DIAutoVariable) Metadata {
	name := C.CString(v.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreateAutoVariable(
		d.ref,
		scope.C,
		name, C.size_t(len(v.Name)),
		v.File.C,
		C.unsigned(v.Line),
		v.Type.C,
		C.LLVMBool(boolToCInt(v.AlwaysPreserve)),
		C.LLVMDIFlags(v.Flags),
		C.uint32_t(v.AlignInBits),
	)
	return Metadata{C: result}
}

// DIParameterVariable holds the values for creating parameter variable debug metadata.
type DIParameterVariable struct {
	Name           string
	File           Metadata
	Line           int
	Type           Metadata
	AlwaysPreserve bool
	Flags          int

	// ArgNo is the 1-based index of the argument in the function's
	// parameter list.
	ArgNo int
}

// CreateParameterVariable creates parameter variable debug metadata.
func (d *DIBuilder) CreateParameterVariable(scope Metadata, v DIParameterVariable) Metadata {
	name := C.CString(v.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreateParameterVariable(
		d.ref,
		scope.C,
		name, C.size_t(len(v.Name)),
		C.unsigned(v.ArgNo),
		v.File.C,
		C.unsigned(v.Line),
		v.Type.C,
		C.LLVMBool(boolToCInt(v.AlwaysPreserve)),
		C.LLVMDIFlags(v.Flags),
	)
	return Metadata{C: result}
}

// DIBasicType holds the values for creating basic type debug metadata.
type DIBasicType struct {
	Name       string
	SizeInBits uint64
	Encoding   DwarfTypeEncoding
}

// CreateBasicType creates basic type debug metadata.
func (d *DIBuilder) CreateBasicType(t DIBasicType) Metadata {
	name := C.CString(t.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreateBasicType(
		d.ref,
		name,
		C.size_t(len(t.Name)),
		C.uint64_t(t.SizeInBits),
		C.LLVMDWARFTypeEncoding(t.Encoding),
		C.LLVMDIFlags(0),
	)
	return Metadata{C: result}
}

// DIPointerType holds the values for creating pointer type debug metadata.
type DIPointerType struct {
	Pointee     Metadata
	SizeInBits  uint64
	AlignInBits uint32 // optional
	AddressSpace uint32
	Name        string // optional
}

// CreatePointerType creates a type that represents a pointer to another type.
func (d *DIBuilder) CreatePointerType(t DIPointerType) Metadata {
	name := C.CString(t.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreatePointerType(
		d.ref,
		t.Pointee.C,
		C.uint64_t(t.SizeInBits),
		C.uint32_t(t.AlignInBits),
		C.unsigned(t.AddressSpace),
		name,
		C.size_t(len(t.Name)),
	)
	return Metadata{C: result}
}

// DISubroutineType holds the values for creating subroutine type debug metadata.
type DISubroutineType struct {
	// File is the file in which the subroutine type is defined.
	File Metadata

	// Parameters contains the subroutine parameter types,
	// including the return type at the 0th index.
	Parameters []Metadata

	Flags int
}

// CreateSubroutineType creates subroutine type debug metadata.
func (d *DIBuilder) CreateSubroutineType(t DISubroutineType) Metadata {
	params, length := llvmMetadataRefs(t.Parameters)
	result := C.LLVMDIBuilderCreateSubroutineType(
		d.ref,
		t.File.C,
		params,
		length,
		C.LLVMDIFlags(t.Flags),
	)
	return Metadata{C: result}
}

// DIStructType holds the values for creating struct type debug metadata.
type DIStructType struct {
	Name        string
	File        Metadata
	Line        int
	SizeInBits  uint64
	AlignInBits uint32
	Flags       int
	DerivedFrom Metadata
	Elements    []Metadata
	VTableHolder Metadata // optional
	UniqueID     string
}

// CreateStructType creates struct type debug metadata.
func (d *DIBuilder) CreateStructType(scope Metadata, t DIStructType) Metadata {
	elements, length := llvmMetadataRefs(t.Elements)
	name := C.CString(t.Name)
	uniqueID := C.CString(t.UniqueID)
	defer C.free(unsafe.Pointer(name))
	defer C.free(unsafe.Pointer(uniqueID))
	result := C.LLVMDIBuilderCreateStructType(
		d.ref,
		scope.C,
		name,
		C.size_t(len(t.Name)),
		t.File.C,
		C.unsigned(t.Line),
		C.uint64_t(t.SizeInBits),
		C.uint32_t(t.AlignInBits),
		C.LLVMDIFlags(t.Flags),
		t.DerivedFrom.C,
		elements,
		length,
		C.unsigned(0), // Optional Objective-C runtime version.
		t.VTableHolder.C,
		uniqueID,
		C.size_t(len(t.UniqueID)),
	)
	return Metadata{C: result}
}

// DIReplaceableCompositeType holds the values for creating replaceable
// composite type debug metadata.
type DIReplaceableCompositeType struct {
	Tag         dwarf.Tag
	Name        string
	File        Metadata
	Line        int
	RuntimeLang int
	SizeInBits  uint64
	AlignInBits uint32
	Flags       int
	UniqueID    string
}

// CreateReplaceableCompositeType creates replaceable composite type debug metadata.
func (d *DIBuilder) CreateReplaceableCompositeType(scope Metadata, t DIReplaceableCompositeType) Metadata {
	name := C.CString(t.Name)
	uniqueID := C.CString(t.UniqueID)
	defer C.free(unsafe.Pointer(name))
	defer C.free(unsafe.Pointer(uniqueID))
	result := C.LLVMDIBuilderCreateReplaceableCompositeType(
		d.ref,
		C.unsigned(t.Tag),
		name,
		C.size_t(len(t.Name)),
		scope.C,
		t.File.C,
		C.unsigned(t.Line),
		C.unsigned(t.RuntimeLang),
		C.uint64_t(t.SizeInBits),
		C.uint32_t(t.AlignInBits),
		C.LLVMDIFlags(t.Flags),
		uniqueID,
		C.size_t(len(t.UniqueID)),
	)
	return Metadata{C: result}
}

// DIMemberType holds the values for creating member type debug metadata.
type DIMemberType struct {
	Name         string
	File         Metadata
	Line         int
	SizeInBits   uint64
	AlignInBits  uint32
	OffsetInBits uint64
	Flags        int
	Type         Metadata
}

// CreateMemberType creates struct type debug metadata.
func (d *DIBuilder) CreateMemberType(scope Metadata, t DIMemberType) Metadata {
	name := C.CString(t.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreateMemberType(
		d.ref,
		scope.C,
		name,
		C.size_t(len(t.Name)),
		t.File.C,
		C.unsigned(t.Line),
		C.uint64_t(t.SizeInBits),
		C.uint32_t(t.AlignInBits),
		C.uint64_t(t.OffsetInBits),
		C.LLVMDIFlags(t.Flags),
		t.Type.C,
	)
	return Metadata{C: result}
}

// DISubrange describes an integer value range.
type DISubrange struct {
	Lo    int64
	Count int64
}

// DIArrayType holds the values for creating array type debug metadata.
type DIArrayType struct {
	SizeInBits  uint64
	AlignInBits uint32
	ElementType Metadata
	Subscripts  []DISubrange
}

// CreateArrayType creates struct type debug metadata.
func (d *DIBuilder) CreateArrayType(t DIArrayType) Metadata {
	subscriptsSlice := make([]Metadata, len(t.Subscripts))
	for i, s := range t.Subscripts {
		subscriptsSlice[i] = d.getOrCreateSubrange(s.Lo, s.Count)
	}
	subscripts, length := llvmMetadataRefs(subscriptsSlice)
	result := C.LLVMDIBuilderCreateArrayType(
		d.ref,
		C.uint64_t(t.SizeInBits),
		C.uint32_t(t.AlignInBits),
		t.ElementType.C,
		subscripts,
		length,
	)
	return Metadata{C: result}
}

// DITypedef holds the values for creating typedef type debug metadata.
type DITypedef struct {
	Type    Metadata
	Name    string
	File    Metadata
	Line    int
	Context Metadata
}

// CreateTypedef creates typedef type debug metadata.
func (d *DIBuilder) CreateTypedef(t DITypedef) Metadata {
	name := C.CString(t.Name)
	defer C.free(unsafe.Pointer(name))
	result := C.LLVMDIBuilderCreateTypedef(
		d.ref,
		t.Type.C,
		name,
		C.size_t(len(t.Name)),
		t.File.C,
		C.unsigned(t.Line),
		t.Context.C,
	)
	return Metadata{C: result}
}

// getOrCreateSubrange gets a metadata node for the specified subrange,
// creating if required.
func (d *DIBuilder) getOrCreateSubrange(lo, count int64) Metadata {
	result := C.LLVMDIBuilderGetOrCreateSubrange(d.ref, C.int64_t(lo), C.int64_t(count))
	return Metadata{C: result}
}

// getOrCreateArray gets a metadata node containing the specified values,
// creating if required.
func (d *DIBuilder) getOrCreateArray(values []Metadata) Metadata {
	if len(values) == 0 {
		return Metadata{}
	}
	data, length := llvmMetadataRefs(values)
	result := C.LLVMDIBuilderGetOrCreateArray(d.ref, data, C.size_t(length))
	return Metadata{C: result}
}

// getOrCreateTypeArray gets a metadata node for a type array containing the
// specified values, creating if required.
func (d *DIBuilder) getOrCreateTypeArray(values []Metadata) Metadata {
	if len(values) == 0 {
		return Metadata{}
	}
	data, length := llvmMetadataRefs(values)
	result := C.LLVMDIBuilderGetOrCreateTypeArray(d.ref, data, C.size_t(length))
	return Metadata{C: result}
}

// CreateExpression creates a new descriptor for the specified
// variable which has a complex address expression for its address.
func (d *DIBuilder) CreateExpression(addr []int64) Metadata {
	var data *C.int64_t
	if len(addr) > 0 {
		data = (*C.int64_t)(unsafe.Pointer(&addr[0]))
	}
	result := C.LLVMDIBuilderCreateExpression(d.ref, data, C.size_t(len(addr)))
	return Metadata{C: result}
}

// InsertDeclareAtEnd inserts a call to llvm.dbg.declare at the end of the
// specified basic block for the given value and associated debug metadata.
func (d *DIBuilder) InsertDeclareAtEnd(v Value, diVarInfo, expr Metadata, l DebugLoc, bb BasicBlock) Value {
	loc := C.LLVMDIBuilderCreateDebugLocation(
		d.m.Context().C, C.uint(l.Line), C.uint(l.Col), l.Scope.C, l.InlinedAt.C)
	result := C.LLVMDIBuilderInsertDeclareAtEnd(d.ref, v.C, diVarInfo.C, expr.C, loc, bb.C)
	return Value{C: result}
}

// InsertValueAtEnd inserts a call to llvm.dbg.value at the end of the
// specified basic block for the given value and associated debug metadata.
func (d *DIBuilder) InsertValueAtEnd(v Value, diVarInfo, expr Metadata, l DebugLoc, bb BasicBlock) Value {
	loc := C.LLVMDIBuilderCreateDebugLocation(
		d.m.Context().C, C.uint(l.Line), C.uint(l.Col), l.Scope.C, l.InlinedAt.C)
	result := C.LLVMDIBuilderInsertDbgValueAtEnd(d.ref, v.C, diVarInfo.C, expr.C, loc, bb.C)
	return Value{C: result}
}

func (v Value) SetSubprogram(sp Metadata) {
  C.LLVMSetSubprogram(v.C, sp.C)
}

func boolToCInt(v bool) C.int {
	if v {
		return 1
	}
	return 0
}

//-------------------------------------------------------------------------
// llvm.Metadata
//-------------------------------------------------------------------------

func (c Context) TemporaryMDNode(mds []Metadata) (md Metadata) {
	ptr, nvals := llvmMetadataRefs(mds)
	md.C = C.LLVMTemporaryMDNode(c.C, ptr, C.size_t(nvals))
	return
}

func (md Metadata) ReplaceAllUsesWith(new Metadata) {
	C.LLVMMetadataReplaceAllUsesWith(md.C, new.C)
}



================================================
FILE: src/bindings/go/llvm/executionengine.go
================================================
//===- executionengine.go - Bindings for executionengine ------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the executionengine component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Core.h"
#include "llvm-c/ExecutionEngine.h"
#include <stdlib.h>
*/
import "C"
import "unsafe"
import "errors"

func LinkInMCJIT()       { C.LLVMLinkInMCJIT() }
func LinkInInterpreter() { C.LLVMLinkInInterpreter() }

type GenericValue struct {
	C C.LLVMGenericValueRef
}
type ExecutionEngine struct {
	C C.LLVMExecutionEngineRef
}

type MCJITCompilerOptions struct {
	C C.struct_LLVMMCJITCompilerOptions
}

func (options *MCJITCompilerOptions) SetMCJITOptimizationLevel(level uint) {
	options.C.OptLevel = C.uint(level)
}

func (options *MCJITCompilerOptions) SetMCJITNoFramePointerElim(nfp bool) {
	options.C.NoFramePointerElim = boolToLLVMBool(nfp)
}

func (options *MCJITCompilerOptions) SetMCJITEnableFastISel(fastisel bool) {
	options.C.EnableFastISel = boolToLLVMBool(fastisel)
}

func (options *MCJITCompilerOptions) SetMCJITCodeModel(CodeModel CodeModel) {
	options.C.CodeModel = C.LLVMCodeModel(CodeModel)
}

// helpers
func llvmGenericValueRefPtr(t *GenericValue) *C.LLVMGenericValueRef {
	return (*C.LLVMGenericValueRef)(unsafe.Pointer(t))
}

//-------------------------------------------------------------------------
// llvm.GenericValue
//-------------------------------------------------------------------------

func NewGenericValueFromInt(t Type, n uint64, signed bool) (g GenericValue) {
	g.C = C.LLVMCreateGenericValueOfInt(t.C, C.ulonglong(n), boolToLLVMBool(signed))
	return
}
func NewGenericValueFromPointer(p unsafe.Pointer) (g GenericValue) {
	g.C = C.LLVMCreateGenericValueOfPointer(p)
	return
}
func NewGenericValueFromFloat(t Type, n float64) (g GenericValue) {
	g.C = C.LLVMCreateGenericValueOfFloat(t.C, C.double(n))
	return
}
func (g GenericValue) IntWidth() int { return int(C.LLVMGenericValueIntWidth(g.C)) }
func (g GenericValue) Int(signed bool) uint64 {
	return uint64(C.LLVMGenericValueToInt(g.C, boolToLLVMBool(signed)))
}
func (g GenericValue) Float(t Type) float64 {
	return float64(C.LLVMGenericValueToFloat(t.C, g.C))
}
func (g GenericValue) Pointer() unsafe.Pointer {
	return C.LLVMGenericValueToPointer(g.C)
}
func (g GenericValue) Dispose() { C.LLVMDisposeGenericValue(g.C) }

//-------------------------------------------------------------------------
// llvm.ExecutionEngine
//-------------------------------------------------------------------------

func NewExecutionEngine(m Module) (ee ExecutionEngine, err error) {
	var cmsg *C.char
	fail := C.LLVMCreateExecutionEngineForModule(&ee.C, m.C, &cmsg)
	if fail != 0 {
		ee.C = nil
		err = errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
	}
	return
}

func NewInterpreter(m Module) (ee ExecutionEngine, err error) {
	var cmsg *C.char
	fail := C.LLVMCreateInterpreterForModule(&ee.C, m.C, &cmsg)
	if fail != 0 {
		ee.C = nil
		err = errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
	}
	return
}

func NewMCJITCompilerOptions() MCJITCompilerOptions {
	var options C.struct_LLVMMCJITCompilerOptions
	C.LLVMInitializeMCJITCompilerOptions(&options, C.size_t(unsafe.Sizeof(C.struct_LLVMMCJITCompilerOptions{})))
	return MCJITCompilerOptions{options}
}

func NewMCJITCompiler(m Module, options MCJITCompilerOptions) (ee ExecutionEngine, err error) {
	var cmsg *C.char
	fail := C.LLVMCreateMCJITCompilerForModule(&ee.C, m.C, &options.C, C.size_t(unsafe.Sizeof(C.struct_LLVMMCJITCompilerOptions{})), &cmsg)
	if fail != 0 {
		ee.C = nil
		err = errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
	}
	return
}

func (ee ExecutionEngine) Dispose()               { C.LLVMDisposeExecutionEngine(ee.C) }
func (ee ExecutionEngine) RunStaticConstructors() { C.LLVMRunStaticConstructors(ee.C) }
func (ee ExecutionEngine) RunStaticDestructors()  { C.LLVMRunStaticDestructors(ee.C) }

func (ee ExecutionEngine) RunFunction(f Value, args []GenericValue) (g GenericValue) {
	nargs := len(args)
	var argptr *GenericValue
	if nargs > 0 {
		argptr = &args[0]
	}
	g.C = C.LLVMRunFunction(ee.C, f.C,
		C.unsigned(nargs), llvmGenericValueRefPtr(argptr))
	return
}

func (ee ExecutionEngine) FreeMachineCodeForFunction(f Value) {
	C.LLVMFreeMachineCodeForFunction(ee.C, f.C)
}
func (ee ExecutionEngine) AddModule(m Module) { C.LLVMAddModule(ee.C, m.C) }

func (ee ExecutionEngine) RemoveModule(m Module) {
	var modtmp C.LLVMModuleRef
	C.LLVMRemoveModule(ee.C, m.C, &modtmp, nil)
}

func (ee ExecutionEngine) FindFunction(name string) (f Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	C.LLVMFindFunction(ee.C, cname, &f.C)
	return
}

func (ee ExecutionEngine) RecompileAndRelinkFunction(f Value) unsafe.Pointer {
	return C.LLVMRecompileAndRelinkFunction(ee.C, f.C)
}

func (ee ExecutionEngine) TargetData() (td TargetData) {
	td.C = C.LLVMGetExecutionEngineTargetData(ee.C)
	return
}

func (ee ExecutionEngine) AddGlobalMapping(global Value, addr unsafe.Pointer) {
	C.LLVMAddGlobalMapping(ee.C, global.C, addr)
}

func (ee ExecutionEngine) PointerToGlobal(global Value) unsafe.Pointer {
	return C.LLVMGetPointerToGlobal(ee.C, global.C)
}



================================================
FILE: src/bindings/go/llvm/executionengine_test.go
================================================
//===- executionengine_test.go - Tests for executionengine ----------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file tests bindings for the executionengine component.
//
//===----------------------------------------------------------------------===//

package llvm

import (
	"testing"
)

func TestFactorial(t *testing.T) {
	LinkInMCJIT()
	InitializeNativeTarget()
	InitializeNativeAsmPrinter()

	mod := NewModule("fac_module")

	fac_args := []Type{Int32Type()}
	fac_type := FunctionType(Int32Type(), fac_args, false)
	fac := AddFunction(mod, "fac", fac_type)
	fac.SetFunctionCallConv(CCallConv)
	n := fac.Param(0)

	entry := AddBasicBlock(fac, "entry")
	iftrue := AddBasicBlock(fac, "iftrue")
	iffalse := AddBasicBlock(fac, "iffalse")
	end := AddBasicBlock(fac, "end")

	builder := NewBuilder()
	defer builder.Dispose()

	builder.SetInsertPointAtEnd(entry)
	If := builder.CreateICmp(IntEQ, n, ConstInt(Int32Type(), 0, false), "cmptmp")
	builder.CreateCondBr(If, iftrue, iffalse)

	builder.SetInsertPointAtEnd(iftrue)
	res_iftrue := ConstInt(Int32Type(), 1, false)
	builder.CreateBr(end)

	builder.SetInsertPointAtEnd(iffalse)
	n_minus := builder.CreateSub(n, ConstInt(Int32Type(), 1, false), "subtmp")
	call_fac_args := []Value{n_minus}
	call_fac := builder.CreateCall(fac, call_fac_args, "calltmp")
	res_iffalse := builder.CreateMul(n, call_fac, "multmp")
	builder.CreateBr(end)

	builder.SetInsertPointAtEnd(end)
	res := builder.CreatePHI(Int32Type(), "result")
	phi_vals := []Value{res_iftrue, res_iffalse}
	phi_blocks := []BasicBlock{iftrue, iffalse}
	res.AddIncoming(phi_vals, phi_blocks)
	builder.CreateRet(res)

	err := VerifyModule(mod, ReturnStatusAction)
	if err != nil {
		t.Errorf("Error verifying module: %s", err)
		return
	}

	options := NewMCJITCompilerOptions()
	options.SetMCJITOptimizationLevel(2)
	options.SetMCJITEnableFastISel(true)
	options.SetMCJITNoFramePointerElim(true)
	options.SetMCJITCodeModel(CodeModelJITDefault)
	engine, err := NewMCJITCompiler(mod, options)
	if err != nil {
		t.Errorf("Error creating JIT: %s", err)
		return
	}
	defer engine.Dispose()

	pass := NewPassManager()
	defer pass.Dispose()

	pass.AddConstantPropagationPass()
	pass.AddInstructionCombiningPass()
	pass.AddPromoteMemoryToRegisterPass()
	pass.AddGVNPass()
	pass.AddCFGSimplificationPass()
	pass.Run(mod)

	exec_args := []GenericValue{NewGenericValueFromInt(Int32Type(), 10, false)}
	exec_res := engine.RunFunction(fac, exec_args)
	var fac10 uint64 = 10 * 9 * 8 * 7 * 6 * 5 * 4 * 3 * 2 * 1
	if exec_res.Int(false) != fac10 {
		t.Errorf("Expected %d, got %d", fac10, exec_res.Int(false))
	}
}



================================================
FILE: src/bindings/go/llvm/InstrumentationBindings.cpp
================================================
//===- InstrumentationBindings.cpp - instrumentation bindings -------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines C bindings for the instrumentation component.
//
//===----------------------------------------------------------------------===//

#include "InstrumentationBindings.h"
#include "llvm-c/Core.h"
#include "llvm/IR/LegacyPassManager.h"
#include "llvm/IR/Module.h"
#include "llvm/Transforms/Instrumentation.h"
#include "llvm/Transforms/Instrumentation/MemorySanitizer.h"
#include "llvm/Transforms/Instrumentation/ThreadSanitizer.h"

using namespace llvm;

void LLVMAddAddressSanitizerFunctionPass(LLVMPassManagerRef PM) {
  unwrap(PM)->add(createAddressSanitizerFunctionPass());
}

void LLVMAddAddressSanitizerModulePass(LLVMPassManagerRef PM) {
  unwrap(PM)->add(createAddressSanitizerModulePass());
}

void LLVMAddThreadSanitizerPass(LLVMPassManagerRef PM) {
  unwrap(PM)->add(createThreadSanitizerLegacyPassPass());
}

void LLVMAddMemorySanitizerLegacyPassPass(LLVMPassManagerRef PM) {
  unwrap(PM)->add(createMemorySanitizerLegacyPassPass());
}

void LLVMAddDataFlowSanitizerPass(LLVMPassManagerRef PM,
                                  int ABIListFilesNum,
                                  const char **ABIListFiles) {
  std::vector<std::string> ABIListFilesVec;
  for (int i = 0; i != ABIListFilesNum; ++i) {
    ABIListFilesVec.push_back(ABIListFiles[i]);
  }
  unwrap(PM)->add(createDataFlowSanitizerPass(ABIListFilesVec));
}



================================================
FILE: src/bindings/go/llvm/InstrumentationBindings.h
================================================
//===- InstrumentationBindings.h - instrumentation bindings -----*- C++ -*-===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines C bindings for the Transforms/Instrumentation component.
//
//===----------------------------------------------------------------------===//

#ifndef LLVM_BINDINGS_GO_LLVM_INSTRUMENTATIONBINDINGS_H
#define LLVM_BINDINGS_GO_LLVM_INSTRUMENTATIONBINDINGS_H

#include "llvm-c/Core.h"

#ifdef __cplusplus
extern "C" {
#endif

// FIXME: These bindings shouldn't be Go-specific and should eventually move to
// a (somewhat) less stable collection of C APIs for use in creating bindings of
// LLVM in other languages.

void LLVMAddAddressSanitizerFunctionPass(LLVMPassManagerRef PM);
void LLVMAddAddressSanitizerModulePass(LLVMPassManagerRef PM);
void LLVMAddThreadSanitizerPass(LLVMPassManagerRef PM);
void LLVMAddMemorySanitizerLegacyPassPass(LLVMPassManagerRef PM);
void LLVMAddDataFlowSanitizerPass(LLVMPassManagerRef PM, int ABIListFilesNum,
                                  const char **ABIListFiles);

#ifdef __cplusplus
}
#endif

#endif



================================================
FILE: src/bindings/go/llvm/ir.go
================================================
//===- ir.go - Bindings for ir --------------------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the ir component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Core.h"
#include "llvm-c/Comdat.h"
#include "IRBindings.h"
#include <stdlib.h>
*/
import "C"
import "unsafe"
import "errors"

type (
	// We use these weird structs here because *Ref types are pointers and
	// Go's spec says that a pointer cannot be used as a receiver base type.
	Context struct {
		C C.LLVMContextRef
	}
	Module struct {
		C C.LLVMModuleRef
	}
	Type struct {
		C C.LLVMTypeRef
	}
	Value struct {
		C C.LLVMValueRef
	}
	Comdat struct {
		C C.LLVMComdatRef
	}
	BasicBlock struct {
		C C.LLVMBasicBlockRef
	}
	Builder struct {
		C C.LLVMBuilderRef
	}
	ModuleProvider struct {
		C C.LLVMModuleProviderRef
	}
	MemoryBuffer struct {
		C C.LLVMMemoryBufferRef
	}
	PassManager struct {
		C C.LLVMPassManagerRef
	}
	Use struct {
		C C.LLVMUseRef
	}
	Metadata struct {
		C C.LLVMMetadataRef
	}
	Attribute struct {
		C C.LLVMAttributeRef
	}
	Opcode              C.LLVMOpcode
	TypeKind            C.LLVMTypeKind
	Linkage             C.LLVMLinkage
	Visibility          C.LLVMVisibility
	CallConv            C.LLVMCallConv
	ComdatSelectionKind C.LLVMComdatSelectionKind
	IntPredicate        C.LLVMIntPredicate
	FloatPredicate      C.LLVMRealPredicate
	LandingPadClause    C.LLVMLandingPadClauseTy
	InlineAsmDialect    C.LLVMInlineAsmDialect
)

func (c Context) IsNil() bool        { return c.C == nil }
func (c Module) IsNil() bool         { return c.C == nil }
func (c Type) IsNil() bool           { return c.C == nil }
func (c Value) IsNil() bool          { return c.C == nil }
func (c BasicBlock) IsNil() bool     { return c.C == nil }
func (c Builder) IsNil() bool        { return c.C == nil }
func (c ModuleProvider) IsNil() bool { return c.C == nil }
func (c MemoryBuffer) IsNil() bool   { return c.C == nil }
func (c PassManager) IsNil() bool    { return c.C == nil }
func (c Use) IsNil() bool            { return c.C == nil }
func (c Attribute) IsNil() bool      { return c.C == nil }

// helpers
func llvmTypeRefPtr(t *Type) *C.LLVMTypeRef    { return (*C.LLVMTypeRef)(unsafe.Pointer(t)) }
func llvmValueRefPtr(t *Value) *C.LLVMValueRef { return (*C.LLVMValueRef)(unsafe.Pointer(t)) }
func llvmMetadataRefPtr(t *Metadata) *C.LLVMMetadataRef {
	return (*C.LLVMMetadataRef)(unsafe.Pointer(t))
}
func llvmBasicBlockRefPtr(t *BasicBlock) *C.LLVMBasicBlockRef {
	return (*C.LLVMBasicBlockRef)(unsafe.Pointer(t))
}
func boolToLLVMBool(b bool) C.LLVMBool {
	if b {
		return C.LLVMBool(1)
	}
	return C.LLVMBool(0)
}

func llvmValueRefs(values []Value) (*C.LLVMValueRef, C.unsigned) {
	var pt *C.LLVMValueRef
	ptlen := C.unsigned(len(values))
	if ptlen > 0 {
		pt = llvmValueRefPtr(&values[0])
	}
	return pt, ptlen
}

func llvmMetadataRefs(mds []Metadata) (*C.LLVMMetadataRef, C.unsigned) {
	var pt *C.LLVMMetadataRef
	ptlen := C.unsigned(len(mds))
	if ptlen > 0 {
		pt = llvmMetadataRefPtr(&mds[0])
	}
	return pt, ptlen
}

//-------------------------------------------------------------------------
// llvm.Opcode
//-------------------------------------------------------------------------

const (
	Ret         Opcode = C.LLVMRet
	Br          Opcode = C.LLVMBr
	Switch      Opcode = C.LLVMSwitch
	IndirectBr  Opcode = C.LLVMIndirectBr
	Invoke      Opcode = C.LLVMInvoke
	Unreachable Opcode = C.LLVMUnreachable

	// Standard Binary Operators
	Add  Opcode = C.LLVMAdd
	FAdd Opcode = C.LLVMFAdd
	Sub  Opcode = C.LLVMSub
	FSub Opcode = C.LLVMFSub
	Mul  Opcode = C.LLVMMul
	FMul Opcode = C.LLVMFMul
	UDiv Opcode = C.LLVMUDiv
	SDiv Opcode = C.LLVMSDiv
	FDiv Opcode = C.LLVMFDiv
	URem Opcode = C.LLVMURem
	SRem Opcode = C.LLVMSRem
	FRem Opcode = C.LLVMFRem

	// Logical Operators
	Shl  Opcode = C.LLVMShl
	LShr Opcode = C.LLVMLShr
	AShr Opcode = C.LLVMAShr
	And  Opcode = C.LLVMAnd
	Or   Opcode = C.LLVMOr
	Xor  Opcode = C.LLVMXor

	// Memory Operators
	Alloca        Opcode = C.LLVMAlloca
	Load          Opcode = C.LLVMLoad
	Store         Opcode = C.LLVMStore
	GetElementPtr Opcode = C.LLVMGetElementPtr

	// Cast Operators
	Trunc    Opcode = C.LLVMTrunc
	ZExt     Opcode = C.LLVMZExt
	SExt     Opcode = C.LLVMSExt
	FPToUI   Opcode = C.LLVMFPToUI
	FPToSI   Opcode = C.LLVMFPToSI
	UIToFP   Opcode = C.LLVMUIToFP
	SIToFP   Opcode = C.LLVMSIToFP
	FPTrunc  Opcode = C.LLVMFPTrunc
	FPExt    Opcode = C.LLVMFPExt
	PtrToInt Opcode = C.LLVMPtrToInt
	IntToPtr Opcode = C.LLVMIntToPtr
	BitCast  Opcode = C.LLVMBitCast

	// Other Operators
	ICmp   Opcode = C.LLVMICmp
	FCmp   Opcode = C.LLVMFCmp
	PHI    Opcode = C.LLVMPHI
	Call   Opcode = C.LLVMCall
	Select Opcode = C.LLVMSelect
	// UserOp1
	// UserOp2
	VAArg          Opcode = C.LLVMVAArg
	ExtractElement Opcode = C.LLVMExtractElement
	InsertElement  Opcode = C.LLVMInsertElement
	ShuffleVector  Opcode = C.LLVMShuffleVector
	ExtractValue   Opcode = C.LLVMExtractValue
	InsertValue    Opcode = C.LLVMInsertValue
)

//-------------------------------------------------------------------------
// llvm.TypeKind
//-------------------------------------------------------------------------

const (
	VoidTypeKind      TypeKind = C.LLVMVoidTypeKind
	FloatTypeKind     TypeKind = C.LLVMFloatTypeKind
	DoubleTypeKind    TypeKind = C.LLVMDoubleTypeKind
	X86_FP80TypeKind  TypeKind = C.LLVMX86_FP80TypeKind
	FP128TypeKind     TypeKind = C.LLVMFP128TypeKind
	PPC_FP128TypeKind TypeKind = C.LLVMPPC_FP128TypeKind
	LabelTypeKind     TypeKind = C.LLVMLabelTypeKind
	IntegerTypeKind   TypeKind = C.LLVMIntegerTypeKind
	FunctionTypeKind  TypeKind = C.LLVMFunctionTypeKind
	StructTypeKind    TypeKind = C.LLVMStructTypeKind
	ArrayTypeKind     TypeKind = C.LLVMArrayTypeKind
	PointerTypeKind   TypeKind = C.LLVMPointerTypeKind
	VectorTypeKind    TypeKind = C.LLVMVectorTypeKind
	MetadataTypeKind  TypeKind = C.LLVMMetadataTypeKind
	TokenTypeKind     TypeKind = C.LLVMTokenTypeKind
)

//-------------------------------------------------------------------------
// llvm.Linkage
//-------------------------------------------------------------------------

const (
	ExternalLinkage            Linkage = C.LLVMExternalLinkage
	AvailableExternallyLinkage Linkage = C.LLVMAvailableExternallyLinkage
	LinkOnceAnyLinkage         Linkage = C.LLVMLinkOnceAnyLinkage
	LinkOnceODRLinkage         Linkage = C.LLVMLinkOnceODRLinkage
	WeakAnyLinkage             Linkage = C.LLVMWeakAnyLinkage
	WeakODRLinkage             Linkage = C.LLVMWeakODRLinkage
	AppendingLinkage           Linkage = C.LLVMAppendingLinkage
	InternalLinkage            Linkage = C.LLVMInternalLinkage
	PrivateLinkage             Linkage = C.LLVMPrivateLinkage
	ExternalWeakLinkage        Linkage = C.LLVMExternalWeakLinkage
	CommonLinkage              Linkage = C.LLVMCommonLinkage
)

//-------------------------------------------------------------------------
// llvm.Visibility
//-------------------------------------------------------------------------

const (
	DefaultVisibility   Visibility = C.LLVMDefaultVisibility
	HiddenVisibility    Visibility = C.LLVMHiddenVisibility
	ProtectedVisibility Visibility = C.LLVMProtectedVisibility
)

//-------------------------------------------------------------------------
// llvm.CallConv
//-------------------------------------------------------------------------

const (
	CCallConv           CallConv = C.LLVMCCallConv
	FastCallConv        CallConv = C.LLVMFastCallConv
	ColdCallConv        CallConv = C.LLVMColdCallConv
	X86StdcallCallConv  CallConv = C.LLVMX86StdcallCallConv
	X86FastcallCallConv CallConv = C.LLVMX86FastcallCallConv
)

//-------------------------------------------------------------------------
// llvm.ComdatSelectionKind
//-------------------------------------------------------------------------

const (
	AnyComdatSelectionKind          ComdatSelectionKind = C.LLVMAnyComdatSelectionKind
	ExactMatchComdatSelectionKind   ComdatSelectionKind = C.LLVMExactMatchComdatSelectionKind
	LargestComdatSelectionKind      ComdatSelectionKind = C.LLVMLargestComdatSelectionKind
	NoDuplicatesComdatSelectionKind ComdatSelectionKind = C.LLVMNoDuplicatesComdatSelectionKind
	SameSizeComdatSelectionKind     ComdatSelectionKind = C.LLVMSameSizeComdatSelectionKind
)

//-------------------------------------------------------------------------
// llvm.IntPredicate
//-------------------------------------------------------------------------

const (
	IntEQ  IntPredicate = C.LLVMIntEQ
	IntNE  IntPredicate = C.LLVMIntNE
	IntUGT IntPredicate = C.LLVMIntUGT
	IntUGE IntPredicate = C.LLVMIntUGE
	IntULT IntPredicate = C.LLVMIntULT
	IntULE IntPredicate = C.LLVMIntULE
	IntSGT IntPredicate = C.LLVMIntSGT
	IntSGE IntPredicate = C.LLVMIntSGE
	IntSLT IntPredicate = C.LLVMIntSLT
	IntSLE IntPredicate = C.LLVMIntSLE
)

//-------------------------------------------------------------------------
// llvm.FloatPredicate
//-------------------------------------------------------------------------

const (
	FloatPredicateFalse FloatPredicate = C.LLVMRealPredicateFalse
	FloatOEQ            FloatPredicate = C.LLVMRealOEQ
	FloatOGT            FloatPredicate = C.LLVMRealOGT
	FloatOGE            FloatPredicate = C.LLVMRealOGE
	FloatOLT            FloatPredicate = C.LLVMRealOLT
	FloatOLE            FloatPredicate = C.LLVMRealOLE
	FloatONE            FloatPredicate = C.LLVMRealONE
	FloatORD            FloatPredicate = C.LLVMRealORD
	FloatUNO            FloatPredicate = C.LLVMRealUNO
	FloatUEQ            FloatPredicate = C.LLVMRealUEQ
	FloatUGT            FloatPredicate = C.LLVMRealUGT
	FloatUGE            FloatPredicate = C.LLVMRealUGE
	FloatULT            FloatPredicate = C.LLVMRealULT
	FloatULE            FloatPredicate = C.LLVMRealULE
	FloatUNE            FloatPredicate = C.LLVMRealUNE
	FloatPredicateTrue  FloatPredicate = C.LLVMRealPredicateTrue
)

//-------------------------------------------------------------------------
// llvm.LandingPadClause
//-------------------------------------------------------------------------

const (
	LandingPadCatch  LandingPadClause = C.LLVMLandingPadCatch
	LandingPadFilter LandingPadClause = C.LLVMLandingPadFilter
)

//-------------------------------------------------------------------------
// llvm.InlineAsmDialect
//-------------------------------------------------------------------------

const (
	InlineAsmDialectATT   InlineAsmDialect = C.LLVMInlineAsmDialectATT
	InlineAsmDialectIntel InlineAsmDialect = C.LLVMInlineAsmDialectIntel
)

//-------------------------------------------------------------------------
// llvm.Context
//-------------------------------------------------------------------------

func NewContext() Context    { return Context{C.LLVMContextCreate()} }
func GlobalContext() Context { return Context{C.LLVMGetGlobalContext()} }
func (c Context) Dispose()   { C.LLVMContextDispose(c.C) }

func (c Context) MDKindID(name string) (id int) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	id = int(C.LLVMGetMDKindIDInContext(c.C, cname, C.unsigned(len(name))))
	return
}

func MDKindID(name string) (id int) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	id = int(C.LLVMGetMDKindID(cname, C.unsigned(len(name))))
	return
}

//-------------------------------------------------------------------------
// llvm.Attribute
//-------------------------------------------------------------------------

func AttributeKindID(name string) (id uint) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	id = uint(C.LLVMGetEnumAttributeKindForName(cname, C.size_t(len(name))))
	return
}

func (c Context) CreateEnumAttribute(kind uint, val uint64) (a Attribute) {
  a.C = C.LLVMCreateEnumAttribute(c.C, C.unsigned(kind), C.uint64_t(val))
  return
}

func (a Attribute) GetEnumKind() (id int) {
  id = int(C.LLVMGetEnumAttributeKind(a.C))
  return
}

func (a Attribute) GetEnumValue() (val uint64) {
  val = uint64(C.LLVMGetEnumAttributeValue(a.C))
  return
}

func (c Context) CreateStringAttribute(kind string, val string) (a Attribute) {
  ckind := C.CString(kind)
  defer C.free(unsafe.Pointer(ckind))
  cval := C.CString(val)
  defer C.free(unsafe.Pointer(cval))
  a.C = C.LLVMCreateStringAttribute(c.C,
                                    ckind, C.unsigned(len(kind)),
                                    cval, C.unsigned(len(val)))
  return
}

func (a Attribute) GetStringKind() string {
  length := C.unsigned(0)
  ckind := C.LLVMGetStringAttributeKind(a.C, &length)
  return C.GoStringN(ckind, C.int(length))
}

func (a Attribute) GetStringValue() string {
  length := C.unsigned(0)
  ckind := C.LLVMGetStringAttributeValue(a.C, &length)
  return C.GoStringN(ckind, C.int(length))
}

func (a Attribute) IsEnum() bool {
  return C.LLVMIsEnumAttribute(a.C) != 0;
}

func (a Attribute) IsString() bool {
  return C.LLVMIsStringAttribute(a.C) != 0;
}

//-------------------------------------------------------------------------
// llvm.Module
//-------------------------------------------------------------------------

// Create and destroy modules.
// See llvm::Module::Module.
func NewModule(name string) (m Module) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	m.C = C.LLVMModuleCreateWithName(cname)
	return
}

func (c Context) NewModule(name string) (m Module) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	m.C = C.LLVMModuleCreateWithNameInContext(cname, c.C)
	return
}

// See llvm::Module::~Module
func (m Module) Dispose() { C.LLVMDisposeModule(m.C) }

// Data layout. See Module::getDataLayout.
func (m Module) DataLayout() string {
	clayout := C.LLVMGetDataLayout(m.C)
	return C.GoString(clayout)
}

func (m Module) SetDataLayout(layout string) {
	clayout := C.CString(layout)
	defer C.free(unsafe.Pointer(clayout))
	C.LLVMSetDataLayout(m.C, clayout)
}

// Target triple. See Module::getTargetTriple.
func (m Module) Target() string {
	ctarget := C.LLVMGetTarget(m.C)
	return C.GoString(ctarget)
}
func (m Module) SetTarget(target string) {
	ctarget := C.CString(target)
	defer C.free(unsafe.Pointer(ctarget))
	C.LLVMSetTarget(m.C, ctarget)
}

func (m Module) GetTypeByName(name string) (t Type) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	t.C = C.LLVMGetTypeByName(m.C, cname)
	return
}

// See Module::dump.
func (m Module) Dump() {
	C.LLVMDumpModule(m.C)
}

func (m Module) String() string {
	cir := C.LLVMPrintModuleToString(m.C)
	defer C.free(unsafe.Pointer(cir))
	ir := C.GoString(cir)
	return ir
}

// See Module::setModuleInlineAsm.
func (m Module) SetInlineAsm(asm string) {
	casm := C.CString(asm)
	defer C.free(unsafe.Pointer(casm))
	C.LLVMSetModuleInlineAsm(m.C, casm)
}

func (m Module) AddNamedMetadataOperand(name string, operand Metadata) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	C.LLVMAddNamedMetadataOperand2(m.C, cname, operand.C)
}

func (m Module) Context() (c Context) {
	c.C = C.LLVMGetModuleContext(m.C)
	return
}

//-------------------------------------------------------------------------
// llvm.Type
//-------------------------------------------------------------------------

// LLVM types conform to the following hierarchy:
//
//   types:
//     integer type
//     real type
//     function type
//     sequence types:
//       array type
//       pointer type
//       vector type
//     void type
//     label type
//     opaque type

// See llvm::LLVMTypeKind::getTypeID.
func (t Type) TypeKind() TypeKind { return TypeKind(C.LLVMGetTypeKind(t.C)) }

// See llvm::LLVMType::getContext.
func (t Type) Context() (c Context) {
	c.C = C.LLVMGetTypeContext(t.C)
	return
}

// Operations on integer types
func (c Context) Int1Type() (t Type)  { t.C = C.LLVMInt1TypeInContext(c.C); return }
func (c Context) Int8Type() (t Type)  { t.C = C.LLVMInt8TypeInContext(c.C); return }
func (c Context) Int16Type() (t Type) { t.C = C.LLVMInt16TypeInContext(c.C); return }
func (c Context) Int32Type() (t Type) { t.C = C.LLVMInt32TypeInContext(c.C); return }
func (c Context) Int64Type() (t Type) { t.C = C.LLVMInt64TypeInContext(c.C); return }
func (c Context) IntType(numbits int) (t Type) {
	t.C = C.LLVMIntTypeInContext(c.C, C.unsigned(numbits))
	return
}

func Int1Type() (t Type)  { t.C = C.LLVMInt1Type(); return }
func Int8Type() (t Type)  { t.C = C.LLVMInt8Type(); return }
func Int16Type() (t Type) { t.C = C.LLVMInt16Type(); return }
func Int32Type() (t Type) { t.C = C.LLVMInt32Type(); return }
func Int64Type() (t Type) { t.C = C.LLVMInt64Type(); return }

func IntType(numbits int) (t Type) {
	t.C = C.LLVMIntType(C.unsigned(numbits))
	return
}

func (t Type) IntTypeWidth() int {
	return int(C.LLVMGetIntTypeWidth(t.C))
}

// Operations on real types
func (c Context) FloatType() (t Type)    { t.C = C.LLVMFloatTypeInContext(c.C); return }
func (c Context) DoubleType() (t Type)   { t.C = C.LLVMDoubleTypeInContext(c.C); return }
func (c Context) X86FP80Type() (t Type)  { t.C = C.LLVMX86FP80TypeInContext(c.C); return }
func (c Context) FP128Type() (t Type)    { t.C = C.LLVMFP128TypeInContext(c.C); return }
func (c Context) PPCFP128Type() (t Type) { t.C = C.LLVMPPCFP128TypeInContext(c.C); return }

func FloatType() (t Type)    { t.C = C.LLVMFloatType(); return }
func DoubleType() (t Type)   { t.C = C.LLVMDoubleType(); return }
func X86FP80Type() (t Type)  { t.C = C.LLVMX86FP80Type(); return }
func FP128Type() (t Type)    { t.C = C.LLVMFP128Type(); return }
func PPCFP128Type() (t Type) { t.C = C.LLVMPPCFP128Type(); return }

// Operations on function types
func FunctionType(returnType Type, paramTypes []Type, isVarArg bool) (t Type) {
	var pt *C.LLVMTypeRef
	var ptlen C.unsigned
	if len(paramTypes) > 0 {
		pt = llvmTypeRefPtr(&paramTypes[0])
		ptlen = C.unsigned(len(paramTypes))
	}
	t.C = C.LLVMFunctionType(returnType.C,
		pt,
		ptlen,
		boolToLLVMBool(isVarArg))
	return
}

func (t Type) IsFunctionVarArg() bool { return C.LLVMIsFunctionVarArg(t.C) != 0 }
func (t Type) ReturnType() (rt Type)  { rt.C = C.LLVMGetReturnType(t.C); return }
func (t Type) ParamTypesCount() int   { return int(C.LLVMCountParamTypes(t.C)) }
func (t Type) ParamTypes() []Type {
	count := t.ParamTypesCount()
	if count > 0 {
		out := make([]Type, count)
		C.LLVMGetParamTypes(t.C, llvmTypeRefPtr(&out[0]))
		return out
	}
	return nil
}

// Operations on struct types
func (c Context) StructType(elementTypes []Type, packed bool) (t Type) {
	var pt *C.LLVMTypeRef
	var ptlen C.unsigned
	if len(elementTypes) > 0 {
		pt = llvmTypeRefPtr(&elementTypes[0])
		ptlen = C.unsigned(len(elementTypes))
	}
	t.C = C.LLVMStructTypeInContext(c.C,
		pt,
		ptlen,
		boolToLLVMBool(packed))
	return
}

func StructType(elementTypes []Type, packed bool) (t Type) {
	var pt *C.LLVMTypeRef
	var ptlen C.unsigned
	if len(elementTypes) > 0 {
		pt = llvmTypeRefPtr(&elementTypes[0])
		ptlen = C.unsigned(len(elementTypes))
	}
	t.C = C.LLVMStructType(pt, ptlen, boolToLLVMBool(packed))
	return
}

func (c Context) StructCreateNamed(name string) (t Type) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	t.C = C.LLVMStructCreateNamed(c.C, cname)
	return
}

func (t Type) StructName() string {
	return C.GoString(C.LLVMGetStructName(t.C))
}

func (t Type) StructSetBody(elementTypes []Type, packed bool) {
	var pt *C.LLVMTypeRef
	var ptlen C.unsigned
	if len(elementTypes) > 0 {
		pt = llvmTypeRefPtr(&elementTypes[0])
		ptlen = C.unsigned(len(elementTypes))
	}
	C.LLVMStructSetBody(t.C, pt, ptlen, boolToLLVMBool(packed))
}

func (t Type) IsStructPacked() bool         { return C.LLVMIsPackedStruct(t.C) != 0 }
func (t Type) StructElementTypesCount() int { return int(C.LLVMCountStructElementTypes(t.C)) }
func (t Type) StructElementTypes() []Type {
	out := make([]Type, t.StructElementTypesCount())
	if len(out) > 0 {
		C.LLVMGetStructElementTypes(t.C, llvmTypeRefPtr(&out[0]))
	}
	return out
}

// Operations on array, pointer, and vector types (sequence types)
func (t Type) Subtypes() (ret []Type) {
	ret = make([]Type, C.LLVMGetNumContainedTypes(t.C))
	C.LLVMGetSubtypes(t.C, llvmTypeRefPtr(&ret[0]))
	return
}

func ArrayType(elementType Type, elementCount int) (t Type) {
	t.C = C.LLVMArrayType(elementType.C, C.unsigned(elementCount))
	return
}
func PointerType(elementType Type, addressSpace int) (t Type) {
	t.C = C.LLVMPointerType(elementType.C, C.unsigned(addressSpace))
	return
}
func VectorType(elementType Type, elementCount int) (t Type) {
	t.C = C.LLVMVectorType(elementType.C, C.unsigned(elementCount))
	return
}

func (t Type) ElementType() (rt Type)   { rt.C = C.LLVMGetElementType(t.C); return }
func (t Type) ArrayLength() int         { return int(C.LLVMGetArrayLength(t.C)) }
func (t Type) PointerAddressSpace() int { return int(C.LLVMGetPointerAddressSpace(t.C)) }
func (t Type) VectorSize() int          { return int(C.LLVMGetVectorSize(t.C)) }

// Operations on other types
func (c Context) VoidType() (t Type)  { t.C = C.LLVMVoidTypeInContext(c.C); return }
func (c Context) LabelType() (t Type) { t.C = C.LLVMLabelTypeInContext(c.C); return }
func (c Context) TokenType() (t Type) { t.C = C.LLVMTokenTypeInContext(c.C); return }

func VoidType() (t Type)  { t.C = C.LLVMVoidType(); return }
func LabelType() (t Type) { t.C = C.LLVMLabelType(); return }

//-------------------------------------------------------------------------
// llvm.Value
//-------------------------------------------------------------------------

// Operations on all values
func (v Value) Type() (t Type) { t.C = C.LLVMTypeOf(v.C); return }
func (v Value) Name() string   { return C.GoString(C.LLVMGetValueName(v.C)) }
func (v Value) SetName(name string) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	C.LLVMSetValueName(v.C, cname)
}
func (v Value) Dump()                       { C.LLVMDumpValue(v.C) }
func (v Value) ReplaceAllUsesWith(nv Value) { C.LLVMReplaceAllUsesWith(v.C, nv.C) }
func (v Value) HasMetadata() bool           { return C.LLVMHasMetadata(v.C) != 0 }
func (v Value) Metadata(kind int) (rv Value) {
	rv.C = C.LLVMGetMetadata(v.C, C.unsigned(kind))
	return
}
func (v Value) SetMetadata(kind int, node Metadata) {
	C.LLVMSetMetadata2(v.C, C.unsigned(kind), node.C)
}

// Conversion functions.
// Return the input value if it is an instance of the specified class, otherwise NULL.
// See llvm::dyn_cast_or_null<>.
func (v Value) IsAArgument() (rv Value)   { rv.C = C.LLVMIsAArgument(v.C); return }
func (v Value) IsABasicBlock() (rv Value) { rv.C = C.LLVMIsABasicBlock(v.C); return }
func (v Value) IsAInlineAsm() (rv Value)  { rv.C = C.LLVMIsAInlineAsm(v.C); return }
func (v Value) IsAUser() (rv Value)       { rv.C = C.LLVMIsAUser(v.C); return }
func (v Value) IsAConstant() (rv Value)   { rv.C = C.LLVMIsAConstant(v.C); return }
func (v Value) IsAConstantAggregateZero() (rv Value) {
	rv.C = C.LLVMIsAConstantAggregateZero(v.C)
	return
}
func (v Value) IsAConstantArray() (rv Value)       { rv.C = C.LLVMIsAConstantArray(v.C); return }
func (v Value) IsAConstantExpr() (rv Value)        { rv.C = C.LLVMIsAConstantExpr(v.C); return }
func (v Value) IsAConstantFP() (rv Value)          { rv.C = C.LLVMIsAConstantFP(v.C); return }
func (v Value) IsAConstantInt() (rv Value)         { rv.C = C.LLVMIsAConstantInt(v.C); return }
func (v Value) IsAConstantPointerNull() (rv Value) { rv.C = C.LLVMIsAConstantPointerNull(v.C); return }
func (v Value) IsAConstantStruct() (rv Value)      { rv.C = C.LLVMIsAConstantStruct(v.C); return }
func (v Value) IsAConstantVector() (rv Value)      { rv.C = C.LLVMIsAConstantVector(v.C); return }
func (v Value) IsAGlobalValue() (rv Value)         { rv.C = C.LLVMIsAGlobalValue(v.C); return }
func (v Value) IsAFunction() (rv Value)            { rv.C = C.LLVMIsAFunction(v.C); return }
func (v Value) IsAGlobalAlias() (rv Value)         { rv.C = C.LLVMIsAGlobalAlias(v.C); return }
func (v Value) IsAGlobalVariable() (rv Value)      { rv.C = C.LLVMIsAGlobalVariable(v.C); return }
func (v Value) IsAUndefValue() (rv Value)          { rv.C = C.LLVMIsAUndefValue(v.C); return }
func (v Value) IsAInstruction() (rv Value)         { rv.C = C.LLVMIsAInstruction(v.C); return }
func (v Value) IsABinaryOperator() (rv Value)      { rv.C = C.LLVMIsABinaryOperator(v.C); return }
func (v Value) IsACallInst() (rv Value)            { rv.C = C.LLVMIsACallInst(v.C); return }
func (v Value) IsAIntrinsicInst() (rv Value)       { rv.C = C.LLVMIsAIntrinsicInst(v.C); return }
func (v Value) IsADbgInfoIntrinsic() (rv Value)    { rv.C = C.LLVMIsADbgInfoIntrinsic(v.C); return }
func (v Value) IsADbgDeclareInst() (rv Value)      { rv.C = C.LLVMIsADbgDeclareInst(v.C); return }
func (v Value) IsAMemIntrinsic() (rv Value)        { rv.C = C.LLVMIsAMemIntrinsic(v.C); return }
func (v Value) IsAMemCpyInst() (rv Value)          { rv.C = C.LLVMIsAMemCpyInst(v.C); return }
func (v Value) IsAMemMoveInst() (rv Value)         { rv.C = C.LLVMIsAMemMoveInst(v.C); return }
func (v Value) IsAMemSetInst() (rv Value)          { rv.C = C.LLVMIsAMemSetInst(v.C); return }
func (v Value) IsACmpInst() (rv Value)             { rv.C = C.LLVMIsACmpInst(v.C); return }
func (v Value) IsAFCmpInst() (rv Value)            { rv.C = C.LLVMIsAFCmpInst(v.C); return }
func (v Value) IsAICmpInst() (rv Value)            { rv.C = C.LLVMIsAICmpInst(v.C); return }
func (v Value) IsAExtractElementInst() (rv Value)  { rv.C = C.LLVMIsAExtractElementInst(v.C); return }
func (v Value) IsAGetElementPtrInst() (rv Value)   { rv.C = C.LLVMIsAGetElementPtrInst(v.C); return }
func (v Value) IsAInsertElementInst() (rv Value)   { rv.C = C.LLVMIsAInsertElementInst(v.C); return }
func (v Value) IsAInsertValueInst() (rv Value)     { rv.C = C.LLVMIsAInsertValueInst(v.C); return }
func (v Value) IsAPHINode() (rv Value)             { rv.C = C.LLVMIsAPHINode(v.C); return }
func (v Value) IsASelectInst() (rv Value)          { rv.C = C.LLVMIsASelectInst(v.C); return }
func (v Value) IsAShuffleVectorInst() (rv Value)   { rv.C = C.LLVMIsAShuffleVectorInst(v.C); return }
func (v Value) IsAStoreInst() (rv Value)           { rv.C = C.LLVMIsAStoreInst(v.C); return }
func (v Value) IsABranchInst() (rv Value)          { rv.C = C.LLVMIsABranchInst(v.C); return }
func (v Value) IsAInvokeInst() (rv Value)          { rv.C = C.LLVMIsAInvokeInst(v.C); return }
func (v Value) IsAReturnInst() (rv Value)          { rv.C = C.LLVMIsAReturnInst(v.C); return }
func (v Value) IsASwitchInst() (rv Value)          { rv.C = C.LLVMIsASwitchInst(v.C); return }
func (v Value) IsAUnreachableInst() (rv Value)     { rv.C = C.LLVMIsAUnreachableInst(v.C); return }
func (v Value) IsAUnaryInstruction() (rv Value)    { rv.C = C.LLVMIsAUnaryInstruction(v.C); return }
func (v Value) IsAAllocaInst() (rv Value)          { rv.C = C.LLVMIsAAllocaInst(v.C); return }
func (v Value) IsACastInst() (rv Value)            { rv.C = C.LLVMIsACastInst(v.C); return }
func (v Value) IsABitCastInst() (rv Value)         { rv.C = C.LLVMIsABitCastInst(v.C); return }
func (v Value) IsAFPExtInst() (rv Value)           { rv.C = C.LLVMIsAFPExtInst(v.C); return }
func (v Value) IsAFPToSIInst() (rv Value)          { rv.C = C.LLVMIsAFPToSIInst(v.C); return }
func (v Value) IsAFPToUIInst() (rv Value)          { rv.C = C.LLVMIsAFPToUIInst(v.C); return }
func (v Value) IsAFPTruncInst() (rv Value)         { rv.C = C.LLVMIsAFPTruncInst(v.C); return }
func (v Value) IsAIntToPtrInst() (rv Value)        { rv.C = C.LLVMIsAIntToPtrInst(v.C); return }
func (v Value) IsAPtrToIntInst() (rv Value)        { rv.C = C.LLVMIsAPtrToIntInst(v.C); return }
func (v Value) IsASExtInst() (rv Value)            { rv.C = C.LLVMIsASExtInst(v.C); return }
func (v Value) IsASIToFPInst() (rv Value)          { rv.C = C.LLVMIsASIToFPInst(v.C); return }
func (v Value) IsATruncInst() (rv Value)           { rv.C = C.LLVMIsATruncInst(v.C); return }
func (v Value) IsAUIToFPInst() (rv Value)          { rv.C = C.LLVMIsAUIToFPInst(v.C); return }
func (v Value) IsAZExtInst() (rv Value)            { rv.C = C.LLVMIsAZExtInst(v.C); return }
func (v Value) IsAExtractValueInst() (rv Value)    { rv.C = C.LLVMIsAExtractValueInst(v.C); return }
func (v Value) IsALoadInst() (rv Value)            { rv.C = C.LLVMIsALoadInst(v.C); return }
func (v Value) IsAVAArgInst() (rv Value)           { rv.C = C.LLVMIsAVAArgInst(v.C); return }

// Operations on Uses
func (v Value) FirstUse() (u Use)  { u.C = C.LLVMGetFirstUse(v.C); return }
func (u Use) NextUse() (ru Use)    { ru.C = C.LLVMGetNextUse(u.C); return }
func (u Use) User() (v Value)      { v.C = C.LLVMGetUser(u.C); return }
func (u Use) UsedValue() (v Value) { v.C = C.LLVMGetUsedValue(u.C); return }

// Operations on Users
func (v Value) Operand(i int) (rv Value)   { rv.C = C.LLVMGetOperand(v.C, C.unsigned(i)); return }
func (v Value) SetOperand(i int, op Value) { C.LLVMSetOperand(v.C, C.unsigned(i), op.C) }
func (v Value) OperandsCount() int         { return int(C.LLVMGetNumOperands(v.C)) }

// Operations on constants of any type
func ConstNull(t Type) (v Value)        { v.C = C.LLVMConstNull(t.C); return }
func ConstAllOnes(t Type) (v Value)     { v.C = C.LLVMConstAllOnes(t.C); return }
func Undef(t Type) (v Value)            { v.C = C.LLVMGetUndef(t.C); return }
func (v Value) IsConstant() bool        { return C.LLVMIsConstant(v.C) != 0 }
func (v Value) IsNull() bool            { return C.LLVMIsNull(v.C) != 0 }
func (v Value) IsUndef() bool           { return C.LLVMIsUndef(v.C) != 0 }
func ConstPointerNull(t Type) (v Value) { v.C = C.LLVMConstPointerNull(t.C); return }

// Operations on metadata
func (c Context) MDString(str string) (md Metadata) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	md.C = C.LLVMMDString2(c.C, cstr, C.unsigned(len(str)))
	return
}
func (c Context) MDNode(mds []Metadata) (md Metadata) {
	ptr, nvals := llvmMetadataRefs(mds)
	md.C = C.LLVMMDNode2(c.C, ptr, nvals)
	return
}
func (v Value) ConstantAsMetadata() (md Metadata) {
	md.C = C.LLVMConstantAsMetadata(v.C)
	return
}

// Operations on scalar constants
func ConstInt(t Type, n uint64, signExtend bool) (v Value) {
	v.C = C.LLVMConstInt(t.C,
		C.ulonglong(n),
		boolToLLVMBool(signExtend))
	return
}
func ConstIntFromString(t Type, str string, radix int) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	v.C = C.LLVMConstIntOfString(t.C, cstr, C.uint8_t(radix))
	return
}
func ConstFloat(t Type, n float64) (v Value) {
	v.C = C.LLVMConstReal(t.C, C.double(n))
	return
}
func ConstFloatFromString(t Type, str string) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	v.C = C.LLVMConstRealOfString(t.C, cstr)
	return
}

func (v Value) ZExtValue() uint64 { return uint64(C.LLVMConstIntGetZExtValue(v.C)) }
func (v Value) SExtValue() int64  { return int64(C.LLVMConstIntGetSExtValue(v.C)) }

// Operations on composite constants
func (c Context) ConstString(str string, addnull bool) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	v.C = C.LLVMConstStringInContext(c.C, cstr,
		C.unsigned(len(str)), boolToLLVMBool(!addnull))
	return
}
func (c Context) ConstStruct(constVals []Value, packed bool) (v Value) {
	ptr, nvals := llvmValueRefs(constVals)
	v.C = C.LLVMConstStructInContext(c.C, ptr, nvals,
		boolToLLVMBool(packed))
	return
}
func ConstNamedStruct(t Type, constVals []Value) (v Value) {
	ptr, nvals := llvmValueRefs(constVals)
	v.C = C.LLVMConstNamedStruct(t.C, ptr, nvals)
	return
}
func ConstString(str string, addnull bool) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	v.C = C.LLVMConstString(cstr,
		C.unsigned(len(str)), boolToLLVMBool(!addnull))
	return
}
func ConstArray(t Type, constVals []Value) (v Value) {
	ptr, nvals := llvmValueRefs(constVals)
	v.C = C.LLVMConstArray(t.C, ptr, nvals)
	return
}
func ConstStruct(constVals []Value, packed bool) (v Value) {
	ptr, nvals := llvmValueRefs(constVals)
	v.C = C.LLVMConstStruct(ptr, nvals, boolToLLVMBool(packed))
	return
}
func ConstVector(scalarConstVals []Value, packed bool) (v Value) {
	ptr, nvals := llvmValueRefs(scalarConstVals)
	v.C = C.LLVMConstVector(ptr, nvals)
	return
}

// Constant expressions
func (v Value) Opcode() Opcode                { return Opcode(C.LLVMGetConstOpcode(v.C)) }
func (v Value) InstructionOpcode() Opcode     { return Opcode(C.LLVMGetInstructionOpcode(v.C)) }
func AlignOf(t Type) (v Value)                { v.C = C.LLVMAlignOf(t.C); return }
func SizeOf(t Type) (v Value)                 { v.C = C.LLVMSizeOf(t.C); return }
func ConstNeg(v Value) (rv Value)             { rv.C = C.LLVMConstNeg(v.C); return }
func ConstNSWNeg(v Value) (rv Value)          { rv.C = C.LLVMConstNSWNeg(v.C); return }
func ConstNUWNeg(v Value) (rv Value)          { rv.C = C.LLVMConstNUWNeg(v.C); return }
func ConstFNeg(v Value) (rv Value)            { rv.C = C.LLVMConstFNeg(v.C); return }
func ConstNot(v Value) (rv Value)             { rv.C = C.LLVMConstNot(v.C); return }
func ConstAdd(lhs, rhs Value) (v Value)       { v.C = C.LLVMConstAdd(lhs.C, rhs.C); return }
func ConstNSWAdd(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNSWAdd(lhs.C, rhs.C); return }
func ConstNUWAdd(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNUWAdd(lhs.C, rhs.C); return }
func ConstFAdd(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstFAdd(lhs.C, rhs.C); return }
func ConstSub(lhs, rhs Value) (v Value)       { v.C = C.LLVMConstSub(lhs.C, rhs.C); return }
func ConstNSWSub(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNSWSub(lhs.C, rhs.C); return }
func ConstNUWSub(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNUWSub(lhs.C, rhs.C); return }
func ConstFSub(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstFSub(lhs.C, rhs.C); return }
func ConstMul(lhs, rhs Value) (v Value)       { v.C = C.LLVMConstMul(lhs.C, rhs.C); return }
func ConstNSWMul(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNSWMul(lhs.C, rhs.C); return }
func ConstNUWMul(lhs, rhs Value) (v Value)    { v.C = C.LLVMConstNUWMul(lhs.C, rhs.C); return }
func ConstFMul(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstFMul(lhs.C, rhs.C); return }
func ConstUDiv(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstUDiv(lhs.C, rhs.C); return }
func ConstSDiv(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstSDiv(lhs.C, rhs.C); return }
func ConstExactSDiv(lhs, rhs Value) (v Value) { v.C = C.LLVMConstExactSDiv(lhs.C, rhs.C); return }
func ConstFDiv(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstFDiv(lhs.C, rhs.C); return }
func ConstURem(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstURem(lhs.C, rhs.C); return }
func ConstSRem(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstSRem(lhs.C, rhs.C); return }
func ConstFRem(lhs, rhs Value) (v Value)      { v.C = C.LLVMConstFRem(lhs.C, rhs.C); return }
func ConstAnd(lhs, rhs Value) (v Value)       { v.C = C.LLVMConstAnd(lhs.C, rhs.C); return }
func ConstOr(lhs, rhs Value) (v Value)        { v.C = C.LLVMConstOr(lhs.C, rhs.C); return }
func ConstXor(lhs, rhs Value) (v Value)       { v.C = C.LLVMConstXor(lhs.C, rhs.C); return }

func ConstICmp(pred IntPredicate, lhs, rhs Value) (v Value) {
	v.C = C.LLVMConstICmp(C.LLVMIntPredicate(pred), lhs.C, rhs.C)
	return
}
func ConstFCmp(pred FloatPredicate, lhs, rhs Value) (v Value) {
	v.C = C.LLVMConstFCmp(C.LLVMRealPredicate(pred), lhs.C, rhs.C)
	return
}

func ConstShl(lhs, rhs Value) (v Value)  { v.C = C.LLVMConstShl(lhs.C, rhs.C); return }
func ConstLShr(lhs, rhs Value) (v Value) { v.C = C.LLVMConstLShr(lhs.C, rhs.C); return }
func ConstAShr(lhs, rhs Value) (v Value) { v.C = C.LLVMConstAShr(lhs.C, rhs.C); return }

func ConstGEP(v Value, indices []Value) (rv Value) {
	ptr, nvals := llvmValueRefs(indices)
	rv.C = C.LLVMConstGEP(v.C, ptr, nvals)
	return
}
func ConstInBoundsGEP(v Value, indices []Value) (rv Value) {
	ptr, nvals := llvmValueRefs(indices)
	rv.C = C.LLVMConstInBoundsGEP(v.C, ptr, nvals)
	return
}
func ConstTrunc(v Value, t Type) (rv Value)         { rv.C = C.LLVMConstTrunc(v.C, t.C); return }
func ConstSExt(v Value, t Type) (rv Value)          { rv.C = C.LLVMConstSExt(v.C, t.C); return }
func ConstZExt(v Value, t Type) (rv Value)          { rv.C = C.LLVMConstZExt(v.C, t.C); return }
func ConstFPTrunc(v Value, t Type) (rv Value)       { rv.C = C.LLVMConstFPTrunc(v.C, t.C); return }
func ConstFPExt(v Value, t Type) (rv Value)         { rv.C = C.LLVMConstFPExt(v.C, t.C); return }
func ConstUIToFP(v Value, t Type) (rv Value)        { rv.C = C.LLVMConstUIToFP(v.C, t.C); return }
func ConstSIToFP(v Value, t Type) (rv Value)        { rv.C = C.LLVMConstSIToFP(v.C, t.C); return }
func ConstFPToUI(v Value, t Type) (rv Value)        { rv.C = C.LLVMConstFPToUI(v.C, t.C); return }
func ConstFPToSI(v Value, t Type) (rv Value)        { rv.C = C.LLVMConstFPToSI(v.C, t.C); return }
func ConstPtrToInt(v Value, t Type) (rv Value)      { rv.C = C.LLVMConstPtrToInt(v.C, t.C); return }
func ConstIntToPtr(v Value, t Type) (rv Value)      { rv.C = C.LLVMConstIntToPtr(v.C, t.C); return }
func ConstBitCast(v Value, t Type) (rv Value)       { rv.C = C.LLVMConstBitCast(v.C, t.C); return }
func ConstZExtOrBitCast(v Value, t Type) (rv Value) { rv.C = C.LLVMConstZExtOrBitCast(v.C, t.C); return }
func ConstSExtOrBitCast(v Value, t Type) (rv Value) { rv.C = C.LLVMConstSExtOrBitCast(v.C, t.C); return }
func ConstTruncOrBitCast(v Value, t Type) (rv Value) {
	rv.C = C.LLVMConstTruncOrBitCast(v.C, t.C)
	return
}
func ConstPointerCast(v Value, t Type) (rv Value) { rv.C = C.LLVMConstPointerCast(v.C, t.C); return }
func ConstIntCast(v Value, t Type, signed bool) (rv Value) {
	rv.C = C.LLVMConstIntCast(v.C, t.C, boolToLLVMBool(signed))
	return
}
func ConstFPCast(v Value, t Type) (rv Value) { rv.C = C.LLVMConstFPCast(v.C, t.C); return }
func ConstSelect(cond, iftrue, iffalse Value) (rv Value) {
	rv.C = C.LLVMConstSelect(cond.C, iftrue.C, iffalse.C)
	return
}
func ConstExtractElement(vec, i Value) (rv Value) {
	rv.C = C.LLVMConstExtractElement(vec.C, i.C)
	return
}
func ConstInsertElement(vec, elem, i Value) (rv Value) {
	rv.C = C.LLVMConstInsertElement(vec.C, elem.C, i.C)
	return
}
func ConstShuffleVector(veca, vecb, mask Value) (rv Value) {
	rv.C = C.LLVMConstShuffleVector(veca.C, vecb.C, mask.C)
	return
}

//TODO
//LLVMValueRef LLVMConstExtractValue(LLVMValueRef AggConstant, unsigned *IdxList,
//                                   unsigned NumIdx);

func ConstExtractValue(agg Value, indices []uint32) (rv Value) {
	n := len(indices)
	if n == 0 {
		panic("one or more indices are required")
	}
	ptr := (*C.unsigned)(&indices[0])
	rv.C = C.LLVMConstExtractValue(agg.C, ptr, C.unsigned(n))
	return
}

func ConstInsertValue(agg, val Value, indices []uint32) (rv Value) {
	n := len(indices)
	if n == 0 {
		panic("one or more indices are required")
	}
	ptr := (*C.unsigned)(&indices[0])
	rv.C = C.LLVMConstInsertValue(agg.C, val.C, ptr, C.unsigned(n))
	return
}

func BlockAddress(f Value, bb BasicBlock) (v Value) {
	v.C = C.LLVMBlockAddress(f.C, bb.C)
	return
}

// Operations on global variables, functions, and aliases (globals)
func (v Value) GlobalParent() (m Module) { m.C = C.LLVMGetGlobalParent(v.C); return }
func (v Value) IsDeclaration() bool      { return C.LLVMIsDeclaration(v.C) != 0 }
func (v Value) Linkage() Linkage         { return Linkage(C.LLVMGetLinkage(v.C)) }
func (v Value) SetLinkage(l Linkage)     { C.LLVMSetLinkage(v.C, C.LLVMLinkage(l)) }
func (v Value) Section() string          { return C.GoString(C.LLVMGetSection(v.C)) }
func (v Value) SetSection(str string) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	C.LLVMSetSection(v.C, cstr)
}
func (v Value) Visibility() Visibility      { return Visibility(C.LLVMGetVisibility(v.C)) }
func (v Value) SetVisibility(vi Visibility) { C.LLVMSetVisibility(v.C, C.LLVMVisibility(vi)) }
func (v Value) Alignment() int              { return int(C.LLVMGetAlignment(v.C)) }
func (v Value) SetAlignment(a int)          { C.LLVMSetAlignment(v.C, C.unsigned(a)) }
func (v Value) SetUnnamedAddr(ua bool)      { C.LLVMSetUnnamedAddr(v.C, boolToLLVMBool(ua)) }

// Operations on global variables
func AddGlobal(m Module, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMAddGlobal(m.C, t.C, cname)
	return
}
func AddGlobalInAddressSpace(m Module, t Type, name string, addressSpace int) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMAddGlobalInAddressSpace(m.C, t.C, cname, C.unsigned(addressSpace))
	return
}
func (m Module) NamedGlobal(name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMGetNamedGlobal(m.C, cname)
	return
}

func (m Module) FirstGlobal() (v Value)   { v.C = C.LLVMGetFirstGlobal(m.C); return }
func (m Module) LastGlobal() (v Value)    { v.C = C.LLVMGetLastGlobal(m.C); return }
func NextGlobal(v Value) (rv Value)       { rv.C = C.LLVMGetNextGlobal(v.C); return }
func PrevGlobal(v Value) (rv Value)       { rv.C = C.LLVMGetPreviousGlobal(v.C); return }
func (v Value) EraseFromParentAsGlobal()  { C.LLVMDeleteGlobal(v.C) }
func (v Value) Initializer() (rv Value)   { rv.C = C.LLVMGetInitializer(v.C); return }
func (v Value) SetInitializer(cv Value)   { C.LLVMSetInitializer(v.C, cv.C) }
func (v Value) IsThreadLocal() bool       { return C.LLVMIsThreadLocal(v.C) != 0 }
func (v Value) SetThreadLocal(tl bool)    { C.LLVMSetThreadLocal(v.C, boolToLLVMBool(tl)) }
func (v Value) IsGlobalConstant() bool    { return C.LLVMIsGlobalConstant(v.C) != 0 }
func (v Value) SetGlobalConstant(gc bool) { C.LLVMSetGlobalConstant(v.C, boolToLLVMBool(gc)) }
func (v Value) IsVolatile() bool          { return C.LLVMGetVolatile(v.C) != 0 }
func (v Value) SetVolatile(volatile bool) { C.LLVMSetVolatile(v.C, boolToLLVMBool(volatile)) }

// Operations on aliases
func AddAlias(m Module, t Type, aliasee Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMAddAlias(m.C, t.C, aliasee.C, cname)
	return
}

// Operations on comdat
func (m Module) Comdat(name string) (c Comdat) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	c.C = C.LLVMGetOrInsertComdat(m.C, cname)
	return
}

func (v Value) Comdat() (c Comdat) { c.C = C.LLVMGetComdat(v.C); return }
func (v Value) SetComdat(c Comdat) { C.LLVMSetComdat(v.C, c.C) }

func (c Comdat) SelectionKind() ComdatSelectionKind {
	return ComdatSelectionKind(C.LLVMGetComdatSelectionKind(c.C))
}

func (c Comdat) SetSelectionKind(k ComdatSelectionKind) {
	C.LLVMSetComdatSelectionKind(c.C, (C.LLVMComdatSelectionKind)(k))
}

// Operations on functions
func AddFunction(m Module, name string, ft Type) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMAddFunction(m.C, cname, ft.C)
	return
}

func (m Module) NamedFunction(name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMGetNamedFunction(m.C, cname)
	return
}

func (m Module) FirstFunction() (v Value)  { v.C = C.LLVMGetFirstFunction(m.C); return }
func (m Module) LastFunction() (v Value)   { v.C = C.LLVMGetLastFunction(m.C); return }
func NextFunction(v Value) (rv Value)      { rv.C = C.LLVMGetNextFunction(v.C); return }
func PrevFunction(v Value) (rv Value)      { rv.C = C.LLVMGetPreviousFunction(v.C); return }
func (v Value) EraseFromParentAsFunction() { C.LLVMDeleteFunction(v.C) }
func (v Value) IntrinsicID() int           { return int(C.LLVMGetIntrinsicID(v.C)) }
func (v Value) FunctionCallConv() CallConv {
	return CallConv(C.LLVMCallConv(C.LLVMGetFunctionCallConv(v.C)))
}
func (v Value) SetFunctionCallConv(cc CallConv) { C.LLVMSetFunctionCallConv(v.C, C.unsigned(cc)) }
func (v Value) GC() string                      { return C.GoString(C.LLVMGetGC(v.C)) }
func (v Value) SetGC(name string) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	C.LLVMSetGC(v.C, cname)
}
func (v Value) AddAttributeAtIndex(i int, a Attribute) {
  C.LLVMAddAttributeAtIndex(v.C, C.LLVMAttributeIndex(i), a.C)
}
func (v Value) AddFunctionAttr(a Attribute) {
  v.AddAttributeAtIndex(C.LLVMAttributeFunctionIndex, a);
}
func (v Value) GetEnumAttributeAtIndex(i int, kind uint) (a Attribute) {
  a.C = C.LLVMGetEnumAttributeAtIndex(v.C, C.LLVMAttributeIndex(i), C.unsigned(kind))
  return
}
func (v Value) GetEnumFunctionAttribute(kind uint) Attribute {
  return v.GetEnumAttributeAtIndex(C.LLVMAttributeFunctionIndex, kind)
}
func (v Value) GetStringAttributeAtIndex(i int, kind string) (a Attribute) {
  ckind := C.CString(kind)
  defer C.free(unsafe.Pointer(ckind))
  a.C = C.LLVMGetStringAttributeAtIndex(v.C, C.LLVMAttributeIndex(i),
                                        ckind, C.unsigned(len(kind)))
  return
}
func (v Value) RemoveEnumAttributeAtIndex(i int, kind uint) {
  C.LLVMRemoveEnumAttributeAtIndex(v.C, C.LLVMAttributeIndex(i), C.unsigned(kind))
}
func (v Value) RemoveEnumFunctionAttribute(kind uint) {
  v.RemoveEnumAttributeAtIndex(C.LLVMAttributeFunctionIndex, kind);
}
func (v Value) RemoveStringAttributeAtIndex(i int, kind string) {
  ckind := C.CString(kind)
  defer C.free(unsafe.Pointer(ckind))
  C.LLVMRemoveStringAttributeAtIndex(v.C, C.LLVMAttributeIndex(i),
                                     ckind, C.unsigned(len(kind)))
}
func (v Value) AddTargetDependentFunctionAttr(attr, value string) {
	cattr := C.CString(attr)
	defer C.free(unsafe.Pointer(cattr))
	cvalue := C.CString(value)
	defer C.free(unsafe.Pointer(cvalue))
	C.LLVMAddTargetDependentFunctionAttr(v.C, cattr, cvalue)
}
func (v Value) SetPersonality(p Value) {
	C.LLVMSetPersonalityFn(v.C, p.C)
}

// Operations on parameters
func (v Value) ParamsCount() int { return int(C.LLVMCountParams(v.C)) }
func (v Value) Params() []Value {
	out := make([]Value, v.ParamsCount())
	if len(out) > 0 {
		C.LLVMGetParams(v.C, llvmValueRefPtr(&out[0]))
	}
	return out
}
func (v Value) Param(i int) (rv Value)  { rv.C = C.LLVMGetParam(v.C, C.unsigned(i)); return }
func (v Value) ParamParent() (rv Value) { rv.C = C.LLVMGetParamParent(v.C); return }
func (v Value) FirstParam() (rv Value)  { rv.C = C.LLVMGetFirstParam(v.C); return }
func (v Value) LastParam() (rv Value)   { rv.C = C.LLVMGetLastParam(v.C); return }
func NextParam(v Value) (rv Value)      { rv.C = C.LLVMGetNextParam(v.C); return }
func PrevParam(v Value) (rv Value)      { rv.C = C.LLVMGetPreviousParam(v.C); return }
func (v Value) SetParamAlignment(align int) { C.LLVMSetParamAlignment(v.C, C.unsigned(align)) }

// Operations on basic blocks
func (bb BasicBlock) AsValue() (v Value)      { v.C = C.LLVMBasicBlockAsValue(bb.C); return }
func (v Value) IsBasicBlock() bool            { return C.LLVMValueIsBasicBlock(v.C) != 0 }
func (v Value) AsBasicBlock() (bb BasicBlock) { bb.C = C.LLVMValueAsBasicBlock(v.C); return }
func (bb BasicBlock) Parent() (v Value)       { v.C = C.LLVMGetBasicBlockParent(bb.C); return }
func (v Value) BasicBlocksCount() int         { return int(C.LLVMCountBasicBlocks(v.C)) }
func (v Value) BasicBlocks() []BasicBlock {
	out := make([]BasicBlock, v.BasicBlocksCount())
	C.LLVMGetBasicBlocks(v.C, llvmBasicBlockRefPtr(&out[0]))
	return out
}
func (v Value) FirstBasicBlock() (bb BasicBlock)    { bb.C = C.LLVMGetFirstBasicBlock(v.C); return }
func (v Value) LastBasicBlock() (bb BasicBlock)     { bb.C = C.LLVMGetLastBasicBlock(v.C); return }
func NextBasicBlock(bb BasicBlock) (rbb BasicBlock) { rbb.C = C.LLVMGetNextBasicBlock(bb.C); return }
func PrevBasicBlock(bb BasicBlock) (rbb BasicBlock) { rbb.C = C.LLVMGetPreviousBasicBlock(bb.C); return }
func (v Value) EntryBasicBlock() (bb BasicBlock)    { bb.C = C.LLVMGetEntryBasicBlock(v.C); return }
func (c Context) AddBasicBlock(f Value, name string) (bb BasicBlock) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	bb.C = C.LLVMAppendBasicBlockInContext(c.C, f.C, cname)
	return
}
func (c Context) InsertBasicBlock(ref BasicBlock, name string) (bb BasicBlock) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	bb.C = C.LLVMInsertBasicBlockInContext(c.C, ref.C, cname)
	return
}
func AddBasicBlock(f Value, name string) (bb BasicBlock) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	bb.C = C.LLVMAppendBasicBlock(f.C, cname)
	return
}
func InsertBasicBlock(ref BasicBlock, name string) (bb BasicBlock) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	bb.C = C.LLVMInsertBasicBlock(ref.C, cname)
	return
}
func (bb BasicBlock) EraseFromParent()          { C.LLVMDeleteBasicBlock(bb.C) }
func (bb BasicBlock) MoveBefore(pos BasicBlock) { C.LLVMMoveBasicBlockBefore(bb.C, pos.C) }
func (bb BasicBlock) MoveAfter(pos BasicBlock)  { C.LLVMMoveBasicBlockAfter(bb.C, pos.C) }

// Operations on instructions
func (v Value) InstructionParent() (bb BasicBlock) { bb.C = C.LLVMGetInstructionParent(v.C); return }
func (bb BasicBlock) FirstInstruction() (v Value)  { v.C = C.LLVMGetFirstInstruction(bb.C); return }
func (bb BasicBlock) LastInstruction() (v Value)   { v.C = C.LLVMGetLastInstruction(bb.C); return }
func NextInstruction(v Value) (rv Value)           { rv.C = C.LLVMGetNextInstruction(v.C); return }
func PrevInstruction(v Value) (rv Value)           { rv.C = C.LLVMGetPreviousInstruction(v.C); return }

// Operations on call sites
func (v Value) SetInstructionCallConv(cc CallConv) {
	C.LLVMSetInstructionCallConv(v.C, C.unsigned(cc))
}
func (v Value) InstructionCallConv() CallConv {
	return CallConv(C.LLVMCallConv(C.LLVMGetInstructionCallConv(v.C)))
}
func (v Value) AddCallSiteAttribute(i int, a Attribute) {
	C.LLVMAddCallSiteAttribute(v.C, C.LLVMAttributeIndex(i), a.C)
}
func (v Value) SetInstrParamAlignment(i int, align int) {
	C.LLVMSetInstrParamAlignment(v.C, C.unsigned(i), C.unsigned(align))
}

// Operations on call instructions (only)
func (v Value) IsTailCall() bool    { return C.LLVMIsTailCall(v.C) != 0 }
func (v Value) SetTailCall(is bool) { C.LLVMSetTailCall(v.C, boolToLLVMBool(is)) }

// Operations on phi nodes
func (v Value) AddIncoming(vals []Value, blocks []BasicBlock) {
	ptr, nvals := llvmValueRefs(vals)
	C.LLVMAddIncoming(v.C, ptr, llvmBasicBlockRefPtr(&blocks[0]), nvals)
}
func (v Value) IncomingCount() int { return int(C.LLVMCountIncoming(v.C)) }
func (v Value) IncomingValue(i int) (rv Value) {
	rv.C = C.LLVMGetIncomingValue(v.C, C.unsigned(i))
	return
}
func (v Value) IncomingBlock(i int) (bb BasicBlock) {
	bb.C = C.LLVMGetIncomingBlock(v.C, C.unsigned(i))
	return
}

// Operations on inline assembly
func InlineAsm(t Type, asmString, constraints string, hasSideEffects, isAlignStack bool, dialect InlineAsmDialect) (rv Value) {
	casm := C.CString(asmString)
	defer C.free(unsafe.Pointer(casm))
	cconstraints := C.CString(constraints)
	defer C.free(unsafe.Pointer(cconstraints))
	rv.C = C.LLVMGetInlineAsm(t.C, casm, C.size_t(len(asmString)), cconstraints, C.size_t(len(constraints)), boolToLLVMBool(hasSideEffects), boolToLLVMBool(isAlignStack), C.LLVMInlineAsmDialect(dialect))
	return
}

// Operations on aggregates
func (v Value) Indices() []uint32 {
	num := C.LLVMGetNumIndices(v.C)
	indicesPtr := C.LLVMGetIndices(v.C)
	// https://github.com/golang/go/wiki/cgo#turning-c-arrays-into-go-slices
	rawIndices := (*[1 << 30]C.uint)(unsafe.Pointer(indicesPtr))[:num:num]
	indices := make([]uint32, num)
	for i := range indices {
		indices[i] = uint32(rawIndices[i])
	}
	return indices
}

//-------------------------------------------------------------------------
// llvm.Builder
//-------------------------------------------------------------------------

// An instruction builder represents a point within a basic block, and is the
// exclusive means of building instructions using the C interface.

func (c Context) NewBuilder() (b Builder) { b.C = C.LLVMCreateBuilderInContext(c.C); return }
func NewBuilder() (b Builder)             { b.C = C.LLVMCreateBuilder(); return }
func (b Builder) SetInsertPoint(block BasicBlock, instr Value) {
	C.LLVMPositionBuilder(b.C, block.C, instr.C)
}
func (b Builder) SetInsertPointBefore(instr Value)     { C.LLVMPositionBuilderBefore(b.C, instr.C) }
func (b Builder) SetInsertPointAtEnd(block BasicBlock) { C.LLVMPositionBuilderAtEnd(b.C, block.C) }
func (b Builder) GetInsertBlock() (bb BasicBlock)      { bb.C = C.LLVMGetInsertBlock(b.C); return }
func (b Builder) ClearInsertionPoint()                 { C.LLVMClearInsertionPosition(b.C) }
func (b Builder) Insert(instr Value)                   { C.LLVMInsertIntoBuilder(b.C, instr.C) }
func (b Builder) InsertWithName(instr Value, name string) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	C.LLVMInsertIntoBuilderWithName(b.C, instr.C, cname)
}
func (b Builder) Dispose() { C.LLVMDisposeBuilder(b.C) }

// Metadata
type DebugLoc struct {
	Line, Col      uint
	Scope          Metadata
	InlinedAt      Metadata
}
func (b Builder) SetCurrentDebugLocation(line, col uint, scope, inlinedAt Metadata) {
	C.LLVMSetCurrentDebugLocation2(b.C, C.unsigned(line), C.unsigned(col), scope.C, inlinedAt.C)
}
// Get current debug location. Please do not call this function until setting debug location with SetCurrentDebugLocation()
func (b Builder) GetCurrentDebugLocation() (loc DebugLoc) {
	md := C.LLVMGetCurrentDebugLocation2(b.C)
	loc.Line = uint(md.Line)
	loc.Col = uint(md.Col)
	loc.Scope = Metadata{C: md.Scope}
	loc.InlinedAt = Metadata{C: md.InlinedAt}
	return
}
func (b Builder) SetInstDebugLocation(v Value) { C.LLVMSetInstDebugLocation(b.C, v.C) }
func (b Builder) InsertDeclare(module Module, storage Value, md Value) Value {
	f := module.NamedFunction("llvm.dbg.declare")
	if f.IsNil() {
		ftyp := FunctionType(VoidType(), []Type{storage.Type(), md.Type()}, false)
		f = AddFunction(module, "llvm.dbg.declare", ftyp)
	}
	return b.CreateCall(f, []Value{storage, md}, "")
}

// Terminators
func (b Builder) CreateRetVoid() (rv Value)    { rv.C = C.LLVMBuildRetVoid(b.C); return }
func (b Builder) CreateRet(v Value) (rv Value) { rv.C = C.LLVMBuildRet(b.C, v.C); return }
func (b Builder) CreateAggregateRet(vs []Value) (rv Value) {
	ptr, nvals := llvmValueRefs(vs)
	rv.C = C.LLVMBuildAggregateRet(b.C, ptr, nvals)
	return
}
func (b Builder) CreateBr(bb BasicBlock) (rv Value) { rv.C = C.LLVMBuildBr(b.C, bb.C); return }
func (b Builder) CreateCondBr(ifv Value, thenb, elseb BasicBlock) (rv Value) {
	rv.C = C.LLVMBuildCondBr(b.C, ifv.C, thenb.C, elseb.C)
	return
}
func (b Builder) CreateSwitch(v Value, elseb BasicBlock, numCases int) (rv Value) {
	rv.C = C.LLVMBuildSwitch(b.C, v.C, elseb.C, C.unsigned(numCases))
	return
}
func (b Builder) CreateIndirectBr(addr Value, numDests int) (rv Value) {
	rv.C = C.LLVMBuildIndirectBr(b.C, addr.C, C.unsigned(numDests))
	return
}
func (b Builder) CreateInvoke(fn Value, args []Value, then, catch BasicBlock, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	ptr, nvals := llvmValueRefs(args)
	rv.C = C.LLVMBuildInvoke(b.C, fn.C, ptr, nvals, then.C, catch.C, cname)
	return
}
func (b Builder) CreateUnreachable() (rv Value) { rv.C = C.LLVMBuildUnreachable(b.C); return }

// Add a case to the switch instruction
func (v Value) AddCase(on Value, dest BasicBlock) { C.LLVMAddCase(v.C, on.C, dest.C) }

// Add a destination to the indirectbr instruction
func (v Value) AddDest(dest BasicBlock) { C.LLVMAddDestination(v.C, dest.C) }

// Arithmetic
func (b Builder) CreateAdd(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildAdd(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNSWAdd(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNSWAdd(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNUWAdd(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNUWAdd(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFAdd(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFAdd(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateSub(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSub(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNSWSub(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNSWSub(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNUWSub(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNUWSub(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFSub(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	v.C = C.LLVMBuildFSub(b.C, lhs.C, rhs.C, cname)
	C.free(unsafe.Pointer(cname))
	return
}
func (b Builder) CreateMul(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildMul(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNSWMul(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNSWMul(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNUWMul(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildNUWMul(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFMul(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFMul(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateUDiv(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildUDiv(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateSDiv(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSDiv(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateExactSDiv(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildExactSDiv(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFDiv(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFDiv(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateURem(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildURem(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateSRem(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSRem(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFRem(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFRem(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateShl(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildShl(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateLShr(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildLShr(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateAShr(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildAShr(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateAnd(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildAnd(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateOr(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildOr(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateXor(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildXor(b.C, lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateBinOp(op Opcode, lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildBinOp(b.C, C.LLVMOpcode(op), lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateNeg(v Value, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	rv.C = C.LLVMBuildNeg(b.C, v.C, cname)
	return
}
func (b Builder) CreateNSWNeg(v Value, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	rv.C = C.LLVMBuildNSWNeg(b.C, v.C, cname)
	return
}
func (b Builder) CreateNUWNeg(v Value, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	rv.C = C.LLVMBuildNUWNeg(b.C, v.C, cname)
	return
}
func (b Builder) CreateFNeg(v Value, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	rv.C = C.LLVMBuildFNeg(b.C, v.C, cname)
	return
}
func (b Builder) CreateNot(v Value, name string) (rv Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	rv.C = C.LLVMBuildNot(b.C, v.C, cname)
	return
}

// Memory

func (b Builder) CreateMalloc(t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildMalloc(b.C, t.C, cname)
	return
}
func (b Builder) CreateArrayMalloc(t Type, val Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildArrayMalloc(b.C, t.C, val.C, cname)
	return
}
func (b Builder) CreateAlloca(t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildAlloca(b.C, t.C, cname)
	return
}
func (b Builder) CreateArrayAlloca(t Type, val Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildArrayAlloca(b.C, t.C, val.C, cname)
	return
}
func (b Builder) CreateFree(p Value) (v Value) {
	v.C = C.LLVMBuildFree(b.C, p.C)
	return
}
func (b Builder) CreateLoad(p Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildLoad(b.C, p.C, cname)
	return
}
func (b Builder) CreateStore(val Value, p Value) (v Value) {
	v.C = C.LLVMBuildStore(b.C, val.C, p.C)
	return
}
func (b Builder) CreateGEP(p Value, indices []Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	ptr, nvals := llvmValueRefs(indices)
	v.C = C.LLVMBuildGEP(b.C, p.C, ptr, nvals, cname)
	return
}
func (b Builder) CreateInBoundsGEP(p Value, indices []Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	ptr, nvals := llvmValueRefs(indices)
	v.C = C.LLVMBuildInBoundsGEP(b.C, p.C, ptr, nvals, cname)
	return
}
func (b Builder) CreateStructGEP(p Value, i int, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildStructGEP(b.C, p.C, C.unsigned(i), cname)
	return
}
func (b Builder) CreateGlobalString(str, name string) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildGlobalString(b.C, cstr, cname)
	return
}
func (b Builder) CreateGlobalStringPtr(str, name string) (v Value) {
	cstr := C.CString(str)
	defer C.free(unsafe.Pointer(cstr))
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildGlobalStringPtr(b.C, cstr, cname)
	return
}

// Casts
func (b Builder) CreateTrunc(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildTrunc(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateZExt(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildZExt(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateSExt(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSExt(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateFPToUI(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFPToUI(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateFPToSI(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFPToSI(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateUIToFP(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildUIToFP(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateSIToFP(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSIToFP(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateFPTrunc(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFPTrunc(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateFPExt(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFPExt(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreatePtrToInt(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildPtrToInt(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateIntToPtr(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildIntToPtr(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateBitCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildBitCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateZExtOrBitCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildZExtOrBitCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateSExtOrBitCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSExtOrBitCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateTruncOrBitCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildTruncOrBitCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateCast(val Value, op Opcode, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildCast(b.C, C.LLVMOpcode(op), val.C, t.C, cname)
	return
} //
func (b Builder) CreatePointerCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildPointerCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateIntCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildIntCast(b.C, val.C, t.C, cname)
	return
}
func (b Builder) CreateFPCast(val Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFPCast(b.C, val.C, t.C, cname)
	return
}

// Comparisons
func (b Builder) CreateICmp(pred IntPredicate, lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildICmp(b.C, C.LLVMIntPredicate(pred), lhs.C, rhs.C, cname)
	return
}
func (b Builder) CreateFCmp(pred FloatPredicate, lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildFCmp(b.C, C.LLVMRealPredicate(pred), lhs.C, rhs.C, cname)
	return
}

// Miscellaneous instructions
func (b Builder) CreatePHI(t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildPhi(b.C, t.C, cname)
	return
}
func (b Builder) CreateCall(fn Value, args []Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	ptr, nvals := llvmValueRefs(args)
	v.C = C.LLVMBuildCall(b.C, fn.C, ptr, nvals, cname)
	return
}

func (b Builder) CreateSelect(ifv, thenv, elsev Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildSelect(b.C, ifv.C, thenv.C, elsev.C, cname)
	return
}

func (b Builder) CreateVAArg(list Value, t Type, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildVAArg(b.C, list.C, t.C, cname)
	return
}
func (b Builder) CreateExtractElement(vec, i Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildExtractElement(b.C, vec.C, i.C, cname)
	return
}
func (b Builder) CreateInsertElement(vec, elt, i Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildInsertElement(b.C, vec.C, elt.C, i.C, cname)
	return
}
func (b Builder) CreateShuffleVector(v1, v2, mask Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildShuffleVector(b.C, v1.C, v2.C, mask.C, cname)
	return
}
func (b Builder) CreateExtractValue(agg Value, i int, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildExtractValue(b.C, agg.C, C.unsigned(i), cname)
	return
}
func (b Builder) CreateInsertValue(agg, elt Value, i int, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildInsertValue(b.C, agg.C, elt.C, C.unsigned(i), cname)
	return
}

func (b Builder) CreateIsNull(val Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildIsNull(b.C, val.C, cname)
	return
}
func (b Builder) CreateIsNotNull(val Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildIsNotNull(b.C, val.C, cname)
	return
}
func (b Builder) CreatePtrDiff(lhs, rhs Value, name string) (v Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	v.C = C.LLVMBuildPtrDiff(b.C, lhs.C, rhs.C, cname)
	return
}

func (b Builder) CreateLandingPad(t Type, nclauses int, name string) (l Value) {
	cname := C.CString(name)
	defer C.free(unsafe.Pointer(cname))
	l.C = C.LLVMBuildLandingPad(b.C, t.C, nil, C.unsigned(nclauses), cname)
	return l
}

func (l Value) AddClause(v Value) {
	C.LLVMAddClause(l.C, v.C)
}

func (l Value) SetCleanup(cleanup bool) {
	C.LLVMSetCleanup(l.C, boolToLLVMBool(cleanup))
}

func (b Builder) CreateResume(ex Value) (v Value) {
	v.C = C.LLVMBuildResume(b.C, ex.C)
	return
}

//-------------------------------------------------------------------------
// llvm.ModuleProvider
//-------------------------------------------------------------------------

// Changes the type of M so it can be passed to FunctionPassManagers and the
// JIT. They take ModuleProviders for historical reasons.
func NewModuleProviderForModule(m Module) (mp ModuleProvider) {
	mp.C = C.LLVMCreateModuleProviderForExistingModule(m.C)
	return
}

// Destroys the module M.
func (mp ModuleProvider) Dispose() { C.LLVMDisposeModuleProvider(mp.C) }

//-------------------------------------------------------------------------
// llvm.MemoryBuffer
//-------------------------------------------------------------------------

func NewMemoryBufferFromFile(path string) (b MemoryBuffer, err error) {
	var cmsg *C.char
	cpath := C.CString(path)
	defer C.free(unsafe.Pointer(cpath))
	fail := C.LLVMCreateMemoryBufferWithContentsOfFile(cpath, &b.C, &cmsg)
	if fail != 0 {
		b.C = nil
		err = errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
	}
	return
}

func NewMemoryBufferFromStdin() (b MemoryBuffer, err error) {
	var cmsg *C.char
	fail := C.LLVMCreateMemoryBufferWithSTDIN(&b.C, &cmsg)
	if fail != 0 {
		b.C = nil
		err = errors.New(C.GoString(cmsg))
		C.LLVMDisposeMessage(cmsg)
	}
	return
}

func (b MemoryBuffer) Bytes() []byte {
	cstart := C.LLVMGetBufferStart(b.C)
	csize := C.LLVMGetBufferSize(b.C)
	return C.GoBytes(unsafe.Pointer(cstart), C.int(csize))
}

func (b MemoryBuffer) Dispose() { C.LLVMDisposeMemoryBuffer(b.C) }

//-------------------------------------------------------------------------
// llvm.PassManager
//-------------------------------------------------------------------------

// Constructs a new whole-module pass pipeline. This type of pipeline is
// suitable for link-time optimization and whole-module transformations.
// See llvm::PassManager::PassManager.
func NewPassManager() (pm PassManager) { pm.C = C.LLVMCreatePassManager(); return }

// Constructs a new function-by-function pass pipeline over the module
// provider. It does not take ownership of the module provider. This type of
// pipeline is suitable for code generation and JIT compilation tasks.
// See llvm::FunctionPassManager::FunctionPassManager.
func NewFunctionPassManagerForModule(m Module) (pm PassManager) {
	pm.C = C.LLVMCreateFunctionPassManagerForModule(m.C)
	return
}

// Initializes, executes on the provided module, and finalizes all of the
// passes scheduled in the pass manager. Returns 1 if any of the passes
// modified the module, 0 otherwise. See llvm::PassManager::run(Module&).
func (pm PassManager) Run(m Module) bool { return C.LLVMRunPassManager(pm.C, m.C) != 0 }

// Initializes all of the function passes scheduled in the function pass
// manager. Returns 1 if any of the passes modified the module, 0 otherwise.
// See llvm::FunctionPassManager::doInitialization.
func (pm PassManager) InitializeFunc() bool { return C.LLVMInitializeFunctionPassManager(pm.C) != 0 }

// Executes all of the function passes scheduled in the function pass manager
// on the provided function. Returns 1 if any of the passes modified the
// function, false otherwise.
// See llvm::FunctionPassManager::run(Function&).
func (pm PassManager) RunFunc(f Value) bool { return C.LLVMRunFunctionPassManager(pm.C, f.C) != 0 }

// Finalizes all of the function passes scheduled in the function pass
// manager. Returns 1 if any of the passes modified the module, 0 otherwise.
// See llvm::FunctionPassManager::doFinalization.
func (pm PassManager) FinalizeFunc() bool { return C.LLVMFinalizeFunctionPassManager(pm.C) != 0 }

// Frees the memory of a pass pipeline. For function pipelines, does not free
// the module provider.
// See llvm::PassManagerBase::~PassManagerBase.
func (pm PassManager) Dispose() { C.LLVMDisposePassManager(pm.C) }



================================================
FILE: src/bindings/go/llvm/ir_test.go
================================================
//===- ir_test.go - Tests for ir ------------------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file tests bindings for the ir component.
//
//===----------------------------------------------------------------------===//

package llvm

import (
	"strings"
	"testing"
)

func testAttribute(t *testing.T, name string) {
	mod := NewModule("")
	defer mod.Dispose()

	ftyp := FunctionType(VoidType(), nil, false)
	fn := AddFunction(mod, "foo", ftyp)

	kind := AttributeKindID(name)
	attr := mod.Context().CreateEnumAttribute(kind, 0)

	fn.AddFunctionAttr(attr)
	newattr := fn.GetEnumFunctionAttribute(kind)
	if attr != newattr {
		t.Errorf("got attribute %p, want %p", newattr.C, attr.C)
	}

	text := mod.String()
	if !strings.Contains(text, " "+name+" ") {
		t.Errorf("expected attribute '%s', got:\n%s", name, text)
	}

	fn.RemoveEnumFunctionAttribute(kind)
	newattr = fn.GetEnumFunctionAttribute(kind)
	if !newattr.IsNil() {
		t.Errorf("got attribute %p, want 0", newattr.C)
	}
}

func TestAttributes(t *testing.T) {
	// Tests that our attribute constants haven't drifted from LLVM's.
	attrTests := []string{
		"sanitize_address",
		"alwaysinline",
		"builtin",
		"byval",
		"convergent",
		"inalloca",
		"inlinehint",
		"inreg",
		"jumptable",
		"minsize",
		"naked",
		"nest",
		"noalias",
		"nobuiltin",
		"nocapture",
		"noduplicate",
		"noimplicitfloat",
		"noinline",
		"nonlazybind",
		"nonnull",
		"noredzone",
		"noreturn",
		"nounwind",
		"optnone",
		"optsize",
		"readnone",
		"readonly",
		"returned",
		"returns_twice",
		"signext",
		"safestack",
		"ssp",
		"sspreq",
		"sspstrong",
		"sret",
		"sanitize_thread",
		"sanitize_memory",
		"uwtable",
		"zeroext",
		"cold",
		"nocf_check",
	}

	for _, name := range attrTests {
		testAttribute(t, name)
	}
}

func TestDebugLoc(t *testing.T) {
	mod := NewModule("")
	defer mod.Dispose()

	ctx := mod.Context()

	b := ctx.NewBuilder()
	defer b.Dispose()

	d := NewDIBuilder(mod)
	defer func() {
		d.Destroy()
	}()
	file := d.CreateFile("dummy_file", "dummy_dir")
	voidInfo := d.CreateBasicType(DIBasicType{Name: "void"})
	typeInfo := d.CreateSubroutineType(DISubroutineType{
		File:       file,
		Parameters: []Metadata{voidInfo},
		Flags:      0,
	})
	scope := d.CreateFunction(file, DIFunction{
		Name:         "foo",
		LinkageName:  "foo",
		Line:         10,
		ScopeLine:    10,
		Type:         typeInfo,
		File:         file,
		IsDefinition: true,
	})

	b.SetCurrentDebugLocation(10, 20, scope, Metadata{})
	loc := b.GetCurrentDebugLocation()
	if loc.Line != 10 {
		t.Errorf("Got line %d, though wanted 10", loc.Line)
	}
	if loc.Col != 20 {
		t.Errorf("Got column %d, though wanted 20", loc.Col)
	}
	if loc.Scope.C != scope.C {
		t.Errorf("Got metadata %v as scope, though wanted %v", loc.Scope.C, scope.C)
	}
}

func TestSubtypes(t *testing.T) {
	cont := NewContext()
	defer cont.Dispose()

	int_pointer := PointerType(cont.Int32Type(), 0)
	int_inner := int_pointer.Subtypes()
	if len(int_inner) != 1 {
		t.Errorf("Got size %d, though wanted 1", len(int_inner))
	}
	if int_inner[0] != cont.Int32Type() {
		t.Errorf("Expected int32 type")
	}

	st_pointer := cont.StructType([]Type{cont.Int32Type(), cont.Int8Type()}, false)
	st_inner := st_pointer.Subtypes()
	if len(st_inner) != 2 {
		t.Errorf("Got size %d, though wanted 2", len(int_inner))
	}
	if st_inner[0] != cont.Int32Type() {
		t.Errorf("Expected first struct field to be int32")
	}
	if st_inner[1] != cont.Int8Type() {
		t.Errorf("Expected second struct field to be int8")
	}
}



================================================
FILE: src/bindings/go/llvm/IRBindings.cpp
================================================
//===- IRBindings.cpp - Additional bindings for ir ------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines additional C bindings for the ir component.
//
//===----------------------------------------------------------------------===//

#include "IRBindings.h"
#include "llvm/IR/Attributes.h"
#include "llvm/IR/DebugLoc.h"
#include "llvm/IR/DebugInfoMetadata.h"
#include "llvm/IR/Function.h"
#include "llvm/IR/IRBuilder.h"
#include "llvm/IR/LLVMContext.h"
#include "llvm/IR/Module.h"

using namespace llvm;

LLVMMetadataRef LLVMConstantAsMetadata(LLVMValueRef C) {
  return wrap(ConstantAsMetadata::get(unwrap<Constant>(C)));
}

LLVMMetadataRef LLVMMDString2(LLVMContextRef C, const char *Str, unsigned SLen) {
  return wrap(MDString::get(*unwrap(C), StringRef(Str, SLen)));
}

LLVMMetadataRef LLVMMDNode2(LLVMContextRef C, LLVMMetadataRef *MDs,
                            unsigned Count) {
  return wrap(
      MDNode::get(*unwrap(C), ArrayRef<Metadata *>(unwrap(MDs), Count)));
}

void LLVMAddNamedMetadataOperand2(LLVMModuleRef M, const char *name,
                                  LLVMMetadataRef Val) {
  NamedMDNode *N = unwrap(M)->getOrInsertNamedMetadata(name);
  if (!N)
    return;
  if (!Val)
    return;
  N->addOperand(unwrap<MDNode>(Val));
}

void LLVMSetMetadata2(LLVMValueRef Inst, unsigned KindID, LLVMMetadataRef MD) {
  MDNode *N = MD ? unwrap<MDNode>(MD) : nullptr;
  unwrap<Instruction>(Inst)->setMetadata(KindID, N);
}

void LLVMSetCurrentDebugLocation2(LLVMBuilderRef Bref, unsigned Line,
                                  unsigned Col, LLVMMetadataRef Scope,
                                  LLVMMetadataRef InlinedAt) {
  unwrap(Bref)->SetCurrentDebugLocation(
      DebugLoc::get(Line, Col, Scope ? unwrap<MDNode>(Scope) : nullptr,
                    InlinedAt ? unwrap<MDNode>(InlinedAt) : nullptr));
}

LLVMDebugLocMetadata LLVMGetCurrentDebugLocation2(LLVMBuilderRef Bref) {
  const auto& Loc = unwrap(Bref)->getCurrentDebugLocation();
  const auto* InlinedAt = Loc.getInlinedAt();
  const LLVMDebugLocMetadata md{
    Loc.getLine(),
    Loc.getCol(),
    wrap(Loc.getScope()),
    InlinedAt == nullptr ? nullptr : wrap(InlinedAt->getRawInlinedAt()),
  };
  return md;
}




================================================
FILE: src/bindings/go/llvm/IRBindings.h
================================================
//===- IRBindings.h - Additional bindings for IR ----------------*- C++ -*-===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines additional C bindings for the IR component.
//
//===----------------------------------------------------------------------===//

#ifndef LLVM_BINDINGS_GO_LLVM_IRBINDINGS_H
#define LLVM_BINDINGS_GO_LLVM_IRBINDINGS_H

#include "llvm-c/Core.h"
#include "llvm-c/DebugInfo.h"
#ifdef __cplusplus
#include "llvm/IR/Metadata.h"
#include "llvm/Support/CBindingWrapping.h"
#endif

#include <stdint.h>

#ifdef __cplusplus
extern "C" {
#endif

struct LLVMDebugLocMetadata{
    unsigned Line;
    unsigned Col;
    LLVMMetadataRef Scope;
    LLVMMetadataRef InlinedAt;
};

LLVMMetadataRef LLVMConstantAsMetadata(LLVMValueRef Val);

LLVMMetadataRef LLVMMDString2(LLVMContextRef C, const char *Str, unsigned SLen);
LLVMMetadataRef LLVMMDNode2(LLVMContextRef C, LLVMMetadataRef *MDs,
                            unsigned Count);

void LLVMAddNamedMetadataOperand2(LLVMModuleRef M, const char *name,
                                  LLVMMetadataRef Val);
void LLVMSetMetadata2(LLVMValueRef Inst, unsigned KindID, LLVMMetadataRef MD);

void LLVMSetCurrentDebugLocation2(LLVMBuilderRef Bref, unsigned Line,
                                  unsigned Col, LLVMMetadataRef Scope,
                                  LLVMMetadataRef InlinedAt);

struct LLVMDebugLocMetadata LLVMGetCurrentDebugLocation2(LLVMBuilderRef Bref);

#ifdef __cplusplus
}

#endif

#endif



================================================
FILE: src/bindings/go/llvm/linker.go
================================================
//===- linker.go - Bindings for linker ------------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the linker component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Core.h"
#include "llvm-c/Linker.h"
#include <stdlib.h>
*/
import "C"
import "errors"

func LinkModules(Dest, Src Module) error {
	failed := C.LLVMLinkModules2(Dest.C, Src.C)
	if failed != 0 {
		err := errors.New("Linking failed")
		return err
	}
	return nil
}



================================================
FILE: src/bindings/go/llvm/llvm_config.go.in
================================================
// +build !byollvm

package llvm

/*
#cgo CXXFLAGS: -std=c++11
#cgo CPPFLAGS: @LLVM_CFLAGS@
#cgo LDFLAGS: @LLVM_LDFLAGS@
*/
import "C"

type (run_build_sh int)



================================================
FILE: src/bindings/go/llvm/llvm_dep.go
================================================
//===- llvm_dep.go - creates LLVM dependency ------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file ensures that the LLVM libraries are built before using the
// bindings.
//
//===----------------------------------------------------------------------===//

// +build !byollvm

package llvm

var _ run_build_sh



================================================
FILE: src/bindings/go/llvm/string.go
================================================
//===- string.go - Stringer implementation for Type -----------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file implements the Stringer interface for the Type type.
//
//===----------------------------------------------------------------------===//

package llvm

import "fmt"

func (t TypeKind) String() string {
	switch t {
	case VoidTypeKind:
		return "VoidTypeKind"
	case FloatTypeKind:
		return "FloatTypeKind"
	case DoubleTypeKind:
		return "DoubleTypeKind"
	case X86_FP80TypeKind:
		return "X86_FP80TypeKind"
	case FP128TypeKind:
		return "FP128TypeKind"
	case PPC_FP128TypeKind:
		return "PPC_FP128TypeKind"
	case LabelTypeKind:
		return "LabelTypeKind"
	case IntegerTypeKind:
		return "IntegerTypeKind"
	case FunctionTypeKind:
		return "FunctionTypeKind"
	case StructTypeKind:
		return "StructTypeKind"
	case ArrayTypeKind:
		return "ArrayTypeKind"
	case PointerTypeKind:
		return "PointerTypeKind"
	case VectorTypeKind:
		return "VectorTypeKind"
	case MetadataTypeKind:
		return "MetadataTypeKind"
	}
	panic("unreachable")
}

func (t Type) String() string {
	ts := typeStringer{s: make(map[Type]string)}
	return ts.typeString(t)
}

type typeStringer struct {
	s map[Type]string
}

func (ts *typeStringer) typeString(t Type) string {
	if s, ok := ts.s[t]; ok {
		return s
	}

	k := t.TypeKind()
	s := k.String()
	s = s[:len(s)-len("Kind")]

	switch k {
	case ArrayTypeKind:
		s += fmt.Sprintf("(%v[%v])", ts.typeString(t.ElementType()), t.ArrayLength())
	case PointerTypeKind:
		s += fmt.Sprintf("(%v)", ts.typeString(t.ElementType()))
	case FunctionTypeKind:
		params := t.ParamTypes()
		s += "("
		if len(params) > 0 {
			s += fmt.Sprintf("%v", ts.typeString(params[0]))
			for i := 1; i < len(params); i++ {
				s += fmt.Sprintf(", %v", ts.typeString(params[i]))
			}
		}
		s += fmt.Sprintf("):%v", ts.typeString(t.ReturnType()))
	case StructTypeKind:
		if name := t.StructName(); name != "" {
			ts.s[t] = "%" + name
			s = fmt.Sprintf("%%%s: %s", name, s)
		}
		etypes := t.StructElementTypes()
		s += "("
		if n := len(etypes); n > 0 {
			s += ts.typeString(etypes[0])
			for i := 1; i < n; i++ {
				s += fmt.Sprintf(", %v", ts.typeString(etypes[i]))
			}
		}
		s += ")"
	case IntegerTypeKind:
		s += fmt.Sprintf("(%d bits)", t.IntTypeWidth())
	}

	ts.s[t] = s
	return s
}



================================================
FILE: src/bindings/go/llvm/string_test.go
================================================
//===- string_test.go - test Stringer implementation for Type -------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file tests the Stringer interface for the Type type.
//
//===----------------------------------------------------------------------===//

package llvm

import (
	"testing"
)

func TestStringRecursiveType(t *testing.T) {
	ctx := NewContext()
	defer ctx.Dispose()
	s := ctx.StructCreateNamed("recursive")
	s.StructSetBody([]Type{s, s}, false)
	if str := s.String(); str != "%recursive: StructType(%recursive, %recursive)" {
		t.Errorf("incorrect string result %q", str)
	}
}



================================================
FILE: src/bindings/go/llvm/support.go
================================================
//===- support.go - Bindings for support ----------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the support component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Support.h"
#include "SupportBindings.h"
#include <stdlib.h>
*/
import "C"

import (
	"errors"
	"unsafe"
)

// Loads a dynamic library such that it may be used as an LLVM plugin.
// See llvm::sys::DynamicLibrary::LoadLibraryPermanently.
func LoadLibraryPermanently(lib string) error {
	var errstr *C.char
	libstr := C.CString(lib)
	defer C.free(unsafe.Pointer(libstr))
	C.LLVMLoadLibraryPermanently2(libstr, &errstr)
	if errstr != nil {
		err := errors.New(C.GoString(errstr))
		C.free(unsafe.Pointer(errstr))
		return err
	}
	return nil
}

// Parse the given arguments using the LLVM command line parser.
// See llvm::cl::ParseCommandLineOptions.
func ParseCommandLineOptions(args []string, overview string) {
	argstrs := make([]*C.char, len(args))
	for i, arg := range args {
		argstrs[i] = C.CString(arg)
		defer C.free(unsafe.Pointer(argstrs[i]))
	}
	overviewstr := C.CString(overview)
	defer C.free(unsafe.Pointer(overviewstr))
	C.LLVMParseCommandLineOptions(C.int(len(args)), &argstrs[0], overviewstr)
}



================================================
FILE: src/bindings/go/llvm/SupportBindings.cpp
================================================
//===- SupportBindings.cpp - Additional bindings for support --------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines additional C bindings for the support component.
//
//===----------------------------------------------------------------------===//

#include "SupportBindings.h"
#include "llvm/Support/DynamicLibrary.h"
#include <stdlib.h>
#include <string.h>

void LLVMLoadLibraryPermanently2(const char *Filename, char **ErrMsg) {
  std::string ErrMsgStr;
  if (llvm::sys::DynamicLibrary::LoadLibraryPermanently(Filename, &ErrMsgStr)) {
    *ErrMsg = static_cast<char *>(malloc(ErrMsgStr.size() + 1));
    memcpy(static_cast<void *>(*ErrMsg),
           static_cast<const void *>(ErrMsgStr.c_str()), ErrMsgStr.size() + 1);
  }
}



================================================
FILE: src/bindings/go/llvm/SupportBindings.h
================================================
//===- SupportBindings.h - Additional bindings for Support ------*- C++ -*-===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines additional C bindings for the Support component.
//
//===----------------------------------------------------------------------===//

#ifndef LLVM_BINDINGS_GO_LLVM_SUPPORTBINDINGS_H
#define LLVM_BINDINGS_GO_LLVM_SUPPORTBINDINGS_H

#ifdef __cplusplus
extern "C" {
#endif

// This function duplicates the LLVMLoadLibraryPermanently function in the
// stable C API and adds an extra ErrMsg parameter to retrieve the error
// message.
void LLVMLoadLibraryPermanently2(const char *Filename, char **ErrMsg);

#ifdef __cplusplus
}
#endif

#endif



================================================
FILE: src/bindings/go/llvm/target.go
================================================
//===- target.go - Bindings for target ------------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the target component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Core.h"
#include "llvm-c/Target.h"
#include "llvm-c/TargetMachine.h"
#include <stdlib.h>
*/
import "C"
import "unsafe"
import "errors"

type (
	TargetData struct {
		C C.LLVMTargetDataRef
	}
	Target struct {
		C C.LLVMTargetRef
	}
	TargetMachine struct {
		C C.LLVMTargetMachineRef
	}
	ByteOrdering    C.enum_LLVMByteOrdering
	RelocMode       C.LLVMRelocMode
	CodeGenOptLevel C.LLVMCodeGenOptLevel
	CodeGenFileType C.LLVMCodeGenFileType
	CodeModel       C.LLVMCodeModel
)

const (
	BigEndian    ByteOrdering = C.LLVMBigEndian
	LittleEndian ByteOrdering = C.LLVMLittleEndian
)

const (
	RelocDefault      RelocMode = C.LLVMRelocDefault
	RelocStatic       RelocMode = C.LLVMRelocStatic
	RelocPIC          RelocMode = C.LLVMRelocPIC
	RelocDynamicNoPic RelocMode = C.LLVMRelocDynamicNoPic
)

const (
	CodeGenLevelNone       CodeGenOptLevel = C.LLVMCodeGenLevelNone
	CodeGenLevelLess       CodeGenOptLevel = C.LLVMCodeGenLevelLess
	CodeGenLevelDefault    CodeGenOptLevel = C.LLVMCodeGenLevelDefault
	CodeGenLevelAggressive CodeGenOptLevel = C.LLVMCodeGenLevelAggressive
)

const (
	CodeModelDefault    CodeModel = C.LLVMCodeModelDefault
	CodeModelJITDefault CodeModel = C.LLVMCodeModelJITDefault
	CodeModelTiny       CodeModel = C.LLVMCodeModelTiny
	CodeModelSmall      CodeModel = C.LLVMCodeModelSmall
	CodeModelKernel     CodeModel = C.LLVMCodeModelKernel
	CodeModelMedium     CodeModel = C.LLVMCodeModelMedium
	CodeModelLarge      CodeModel = C.LLVMCodeModelLarge
)

const (
	AssemblyFile CodeGenFileType = C.LLVMAssemblyFile
	ObjectFile   CodeGenFileType = C.LLVMObjectFile
)

// InitializeAllTargetInfos - The main program should call this function if it
// wants access to all available targets that LLVM is configured to support.
func InitializeAllTargetInfos() { C.LLVMInitializeAllTargetInfos() }

// InitializeAllTargets - The main program should call this function if it wants
// to link in all available targets that LLVM is configured to support.
func InitializeAllTargets() { C.LLVMInitializeAllTargets() }

func InitializeAllTargetMCs() { C.LLVMInitializeAllTargetMCs() }

func InitializeAllAsmParsers() { C.LLVMInitializeAllAsmParsers() }

func InitializeAllAsmPrinters() { C.LLVMInitializeAllAsmPrinters() }

var initializeNativeTargetError = errors.New("Failed to initialize native target")

// InitializeNativeTarget - The main program should call this function to
// initialize the native target corresponding to the host. This is useful
// for JIT applications to ensure that the target gets linked in correctly.
func InitializeNativeTarget() error {
	fail := C.LLVMInitializeNativeTarget()
	if fail != 0 {
		return initializeNativeTargetError
	}
	return nil
}

func InitializeNativeAsmPrinter() error {
	fail := C.LLVMInitializeNativeAsmPrinter()
	if fail != 0 {
		return initializeNativeTargetError
	}
	return nil
}

//-------------------------------------------------------------------------
// llvm.TargetData
//-------------------------------------------------------------------------

// Creates target data from a target layout string.
// See the constructor llvm::TargetData::TargetData.
func NewTargetData(rep string) (td TargetData) {
	crep := C.CString(rep)
	defer C.free(unsafe.Pointer(crep))
	td.C = C.LLVMCreateTargetData(crep)
	return
}

// Converts target data to a target layout string. The string must be disposed
// with LLVMDisposeMessage.
// See the constructor llvm::TargetData::TargetData.
func (td TargetData) String() (s string) {
	cmsg := C.LLVMCopyStringRepOfTargetData(td.C)
	s = C.GoString(cmsg)
	C.LLVMDisposeMessage(cmsg)
	return
}

// Returns the byte order of a target, either BigEndian or LittleEndian.
// See the method llvm::TargetData::isLittleEndian.
func (td TargetData) ByteOrder() ByteOrdering { return ByteOrdering(C.LLVMByteOrder(td.C)) }

// Returns the pointer size in bytes for a target.
// See the method llvm::TargetData::getPointerSize.
func (td TargetData) PointerSize() int { return int(C.LLVMPointerSize(td.C)) }

// Returns the integer type that is the same size as a pointer on a target.
// See the method llvm::TargetData::getIntPtrType.
func (td TargetData) IntPtrType() (t Type) { t.C = C.LLVMIntPtrType(td.C); return }

// Computes the size of a type in bytes for a target.
// See the method llvm::TargetData::getTypeSizeInBits.
func (td TargetData) TypeSizeInBits(t Type) uint64 {
	return uint64(C.LLVMSizeOfTypeInBits(td.C, t.C))
}

// Computes the storage size of a type in bytes for a target.
// See the method llvm::TargetData::getTypeStoreSize.
func (td TargetData) TypeStoreSize(t Type) uint64 {
	return uint64(C.LLVMStoreSizeOfType(td.C, t.C))
}

// Computes the ABI size of a type in bytes for a target.
// See the method llvm::TargetData::getTypeAllocSize.
func (td TargetData) TypeAllocSize(t Type) uint64 {
	return uint64(C.LLVMABISizeOfType(td.C, t.C))
}

// Computes the ABI alignment of a type in bytes for a target.
// See the method llvm::TargetData::getABITypeAlignment.
func (td TargetData) ABITypeAlignment(t Type) int {
	return int(C.LLVMABIAlignmentOfType(td.C, t.C))
}

// Computes the call frame alignment of a type in bytes for a target.
// See the method llvm::TargetData::getCallFrameTypeAlignment.
func (td TargetData) CallFrameTypeAlignment(t Type) int {
	return int(C.LLVMCallFrameAlignmentOfType(td.C, t.C))
}

// Computes the preferred alignment of a type in bytes for a target.
// See the method llvm::TargetData::getPrefTypeAlignment.
func (td TargetData) PrefTypeAlignment(t Type) int {
	return int(C.LLVMPreferredAlignmentOfType(td.C, t.C))
}

// Computes the preferred alignment of a global variable in bytes for a target.
// See the method llvm::TargetData::getPreferredAlignment.
func (td TargetData) PreferredAlignment(g Value) int {
	return int(C.LLVMPreferredAlignmentOfGlobal(td.C, g.C))
}

// Computes the structure element that contains the byte offset for a target.
// See the method llvm::StructLayout::getElementContainingOffset.
func (td TargetData) ElementContainingOffset(t Type, offset uint64) int {
	return int(C.LLVMElementAtOffset(td.C, t.C, C.ulonglong(offset)))
}

// Computes the byte offset of the indexed struct element for a target.
// See the method llvm::StructLayout::getElementOffset.
func (td TargetData) ElementOffset(t Type, element int) uint64 {
	return uint64(C.LLVMOffsetOfElement(td.C, t.C, C.unsigned(element)))
}

// Deallocates a TargetData.
// See the destructor llvm::TargetData::~TargetData.
func (td TargetData) Dispose() { C.LLVMDisposeTargetData(td.C) }

//-------------------------------------------------------------------------
// llvm.Target
//-------------------------------------------------------------------------

func FirstTarget() Target {
	return Target{C.LLVMGetFirstTarget()}
}

func (t Target) NextTarget() Target {
	return Target{C.LLVMGetNextTarget(t.C)}
}

func GetTargetFromTriple(triple string) (t Target, err error) {
	var errstr *C.char
	ctriple := C.CString(triple)
	defer C.free(unsafe.Pointer(ctriple))
	fail := C.LLVMGetTargetFromTriple(ctriple, &t.C, &errstr)
	if fail != 0 {
		err = errors.New(C.GoString(errstr))
		C.free(unsafe.Pointer(errstr))
	}
	return
}

func (t Target) Name() string {
	return C.GoString(C.LLVMGetTargetName(t.C))
}

func (t Target) Description() string {
	return C.GoString(C.LLVMGetTargetDescription(t.C))
}

//-------------------------------------------------------------------------
// llvm.TargetMachine
//-------------------------------------------------------------------------

// CreateTargetMachine creates a new TargetMachine.
func (t Target) CreateTargetMachine(Triple string, CPU string, Features string,
	Level CodeGenOptLevel, Reloc RelocMode,
	CodeModel CodeModel) (tm TargetMachine) {
	cTriple := C.CString(Triple)
	defer C.free(unsafe.Pointer(cTriple))
	cCPU := C.CString(CPU)
	defer C.free(unsafe.Pointer(cCPU))
	cFeatures := C.CString(Features)
	defer C.free(unsafe.Pointer(cFeatures))
	tm.C = C.LLVMCreateTargetMachine(t.C, cTriple, cCPU, cFeatures,
		C.LLVMCodeGenOptLevel(Level),
		C.LLVMRelocMode(Reloc),
		C.LLVMCodeModel(CodeModel))
	return
}

// CreateTargetData returns a new TargetData describing the TargetMachine's
// data layout. The returned TargetData is owned by the caller, who is
// responsible for disposing of it by calling the TargetData.Dispose method.
func (tm TargetMachine) CreateTargetData() TargetData {
	return TargetData{C.LLVMCreateTargetDataLayout(tm.C)}
}

// Triple returns the triple describing the machine (arch-vendor-os).
func (tm TargetMachine) Triple() string {
	cstr := C.LLVMGetTargetMachineTriple(tm.C)
	return C.GoString(cstr)
}

func (tm TargetMachine) EmitToMemoryBuffer(m Module, ft CodeGenFileType) (MemoryBuffer, error) {
	var errstr *C.char
	var mb MemoryBuffer
	fail := C.LLVMTargetMachineEmitToMemoryBuffer(tm.C, m.C, C.LLVMCodeGenFileType(ft), &errstr, &mb.C)
	if fail != 0 {
		err := errors.New(C.GoString(errstr))
		C.free(unsafe.Pointer(errstr))
		return MemoryBuffer{}, err
	}
	return mb, nil
}

func (tm TargetMachine) AddAnalysisPasses(pm PassManager) {
	C.LLVMAddAnalysisPasses(tm.C, pm.C)
}

// Dispose releases resources related to the TargetMachine.
func (tm TargetMachine) Dispose() {
	C.LLVMDisposeTargetMachine(tm.C)
}

func DefaultTargetTriple() (triple string) {
	cTriple := C.LLVMGetDefaultTargetTriple()
	defer C.free(unsafe.Pointer(cTriple))
	triple = C.GoString(cTriple)
	return
}



================================================
FILE: src/bindings/go/llvm/transforms_coroutines.go
================================================
//===- transforms_coroutines.go - Bindings for coroutines -----------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the coroutines component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Transforms/Coroutines.h"
*/
import "C"

func (pm PassManager) AddCoroEarlyPass()      { C.LLVMAddCoroEarlyPass(pm.C) }
func (pm PassManager) AddCoroSplitPass()      { C.LLVMAddCoroSplitPass(pm.C) }
func (pm PassManager) AddCoroElidePass()      { C.LLVMAddCoroElidePass(pm.C) }
func (pm PassManager) AddCoroCleanupPass()    { C.LLVMAddCoroCleanupPass(pm.C) }



================================================
FILE: src/bindings/go/llvm/transforms_instrumentation.go
================================================
//===- transforms_instrumentation.go - Bindings for instrumentation -------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the instrumentation component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "InstrumentationBindings.h"
#include <stdlib.h>
*/
import "C"
import "unsafe"

func (pm PassManager) AddAddressSanitizerFunctionPass() {
	C.LLVMAddAddressSanitizerFunctionPass(pm.C)
}

func (pm PassManager) AddAddressSanitizerModulePass() {
	C.LLVMAddAddressSanitizerModulePass(pm.C)
}

func (pm PassManager) AddThreadSanitizerPass() {
	C.LLVMAddThreadSanitizerPass(pm.C)
}

func (pm PassManager) AddMemorySanitizerLegacyPassPass() {
	C.LLVMAddMemorySanitizerLegacyPassPass(pm.C)
}

func (pm PassManager) AddDataFlowSanitizerPass(abilist []string) {
	abiliststrs := make([]*C.char, len(abilist))
	for i, arg := range abilist {
		abiliststrs[i] = C.CString(arg)
		defer C.free(unsafe.Pointer(abiliststrs[i]))
	}
	C.LLVMAddDataFlowSanitizerPass(pm.C, C.int(len(abilist)), &abiliststrs[0])
}



================================================
FILE: src/bindings/go/llvm/transforms_ipo.go
================================================
//===- transforms_ipo.go - Bindings for ipo -------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the ipo component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Transforms/IPO.h"
*/
import "C"

// helpers
func boolToUnsigned(b bool) C.unsigned {
	if b {
		return 1
	}
	return 0
}

func (pm PassManager) AddArgumentPromotionPass()     { C.LLVMAddArgumentPromotionPass(pm.C) }
func (pm PassManager) AddConstantMergePass()         { C.LLVMAddConstantMergePass(pm.C) }
func (pm PassManager) AddDeadArgEliminationPass()    { C.LLVMAddDeadArgEliminationPass(pm.C) }
func (pm PassManager) AddFunctionAttrsPass()         { C.LLVMAddFunctionAttrsPass(pm.C) }
func (pm PassManager) AddFunctionInliningPass()      { C.LLVMAddFunctionInliningPass(pm.C) }
func (pm PassManager) AddGlobalDCEPass()             { C.LLVMAddGlobalDCEPass(pm.C) }
func (pm PassManager) AddGlobalOptimizerPass()       { C.LLVMAddGlobalOptimizerPass(pm.C) }
func (pm PassManager) AddIPConstantPropagationPass() { C.LLVMAddIPConstantPropagationPass(pm.C) }
func (pm PassManager) AddPruneEHPass()               { C.LLVMAddPruneEHPass(pm.C) }
func (pm PassManager) AddIPSCCPPass()                { C.LLVMAddIPSCCPPass(pm.C) }
func (pm PassManager) AddInternalizePass(allButMain bool) {
	C.LLVMAddInternalizePass(pm.C, boolToUnsigned(allButMain))
}
func (pm PassManager) AddStripDeadPrototypesPass() { C.LLVMAddStripDeadPrototypesPass(pm.C) }



================================================
FILE: src/bindings/go/llvm/transforms_pmbuilder.go
================================================
//===- transforms_pmbuilder.go - Bindings for PassManagerBuilder ----------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the PassManagerBuilder class.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Transforms/PassManagerBuilder.h"
*/
import "C"

type PassManagerBuilder struct {
	C C.LLVMPassManagerBuilderRef
}

func NewPassManagerBuilder() (pmb PassManagerBuilder) {
	pmb.C = C.LLVMPassManagerBuilderCreate()
	return
}

func (pmb PassManagerBuilder) SetOptLevel(level int) {
	C.LLVMPassManagerBuilderSetOptLevel(pmb.C, C.uint(level))
}

func (pmb PassManagerBuilder) SetSizeLevel(level int) {
	C.LLVMPassManagerBuilderSetSizeLevel(pmb.C, C.uint(level))
}

func (pmb PassManagerBuilder) Populate(pm PassManager) {
	C.LLVMPassManagerBuilderPopulateModulePassManager(pmb.C, pm.C)
}

func (pmb PassManagerBuilder) PopulateFunc(pm PassManager) {
	C.LLVMPassManagerBuilderPopulateFunctionPassManager(pmb.C, pm.C)
}

func (pmb PassManagerBuilder) PopulateLTOPassManager(pm PassManager, internalize bool, runInliner bool) {
	C.LLVMPassManagerBuilderPopulateLTOPassManager(pmb.C, pm.C, boolToLLVMBool(internalize), boolToLLVMBool(runInliner))
}

func (pmb PassManagerBuilder) Dispose() {
	C.LLVMPassManagerBuilderDispose(pmb.C)
}

func (pmb PassManagerBuilder) SetDisableUnitAtATime(val bool) {
	C.LLVMPassManagerBuilderSetDisableUnitAtATime(pmb.C, boolToLLVMBool(val))
}

func (pmb PassManagerBuilder) SetDisableUnrollLoops(val bool) {
	C.LLVMPassManagerBuilderSetDisableUnrollLoops(pmb.C, boolToLLVMBool(val))
}

func (pmb PassManagerBuilder) SetDisableSimplifyLibCalls(val bool) {
	C.LLVMPassManagerBuilderSetDisableSimplifyLibCalls(pmb.C, boolToLLVMBool(val))
}

func (pmb PassManagerBuilder) UseInlinerWithThreshold(threshold uint) {
	C.LLVMPassManagerBuilderUseInlinerWithThreshold(pmb.C, C.uint(threshold))
}



================================================
FILE: src/bindings/go/llvm/transforms_scalar.go
================================================
//===- transforms_scalar.go - Bindings for scalaropts ---------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines bindings for the scalaropts component.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm-c/Transforms/Scalar.h"
#include "llvm-c/Transforms/Utils.h"
*/
import "C"

func (pm PassManager) AddAggressiveDCEPass()           { C.LLVMAddAggressiveDCEPass(pm.C) }
func (pm PassManager) AddCFGSimplificationPass()       { C.LLVMAddCFGSimplificationPass(pm.C) }
func (pm PassManager) AddDeadStoreEliminationPass()    { C.LLVMAddDeadStoreEliminationPass(pm.C) }
func (pm PassManager) AddGVNPass()                     { C.LLVMAddGVNPass(pm.C) }
func (pm PassManager) AddIndVarSimplifyPass()          { C.LLVMAddIndVarSimplifyPass(pm.C) }
func (pm PassManager) AddInstructionCombiningPass()    { C.LLVMAddInstructionCombiningPass(pm.C) }
func (pm PassManager) AddJumpThreadingPass()           { C.LLVMAddJumpThreadingPass(pm.C) }
func (pm PassManager) AddLICMPass()                    { C.LLVMAddLICMPass(pm.C) }
func (pm PassManager) AddLoopDeletionPass()            { C.LLVMAddLoopDeletionPass(pm.C) }
func (pm PassManager) AddLoopRotatePass()              { C.LLVMAddLoopRotatePass(pm.C) }
func (pm PassManager) AddLoopUnrollPass()              { C.LLVMAddLoopUnrollPass(pm.C) }
func (pm PassManager) AddLoopUnswitchPass()            { C.LLVMAddLoopUnswitchPass(pm.C) }
func (pm PassManager) AddMemCpyOptPass()               { C.LLVMAddMemCpyOptPass(pm.C) }
func (pm PassManager) AddPromoteMemoryToRegisterPass() { C.LLVMAddPromoteMemoryToRegisterPass(pm.C) }
func (pm PassManager) AddReassociatePass()             { C.LLVMAddReassociatePass(pm.C) }
func (pm PassManager) AddSCCPPass()                    { C.LLVMAddSCCPPass(pm.C) }
func (pm PassManager) AddScalarReplAggregatesPass()    { C.LLVMAddScalarReplAggregatesPass(pm.C) }
func (pm PassManager) AddScalarReplAggregatesPassWithThreshold(threshold int) {
	C.LLVMAddScalarReplAggregatesPassWithThreshold(pm.C, C.int(threshold))
}
func (pm PassManager) AddSimplifyLibCallsPass()       { C.LLVMAddSimplifyLibCallsPass(pm.C) }
func (pm PassManager) AddTailCallEliminationPass()    { C.LLVMAddTailCallEliminationPass(pm.C) }
func (pm PassManager) AddConstantPropagationPass()    { C.LLVMAddConstantPropagationPass(pm.C) }
func (pm PassManager) AddDemoteMemoryToRegisterPass() { C.LLVMAddDemoteMemoryToRegisterPass(pm.C) }
func (pm PassManager) AddVerifierPass()               { C.LLVMAddVerifierPass(pm.C) }



================================================
FILE: src/bindings/go/llvm/version.go
================================================
//===- version.go - LLVM version info -------------------------------------===//
//
//                     The LLVM Compiler Infrastructure
//
// This file is distributed under the University of Illinois Open Source
// License. See LICENSE.TXT for details.
//
//===----------------------------------------------------------------------===//
//
// This file defines LLVM version information.
//
//===----------------------------------------------------------------------===//

package llvm

/*
#include "llvm/Config/llvm-config.h"
*/
import "C"

const Version = C.LLVM_VERSION_STRING



================================================
FILE: src/bindings/ocaml/CMakeLists.txt
================================================
add_subdirectory(llvm)
add_subdirectory(all_backends)
add_subdirectory(analysis)
add_subdirectory(backends)
add_subdirectory(bitreader)
add_subdirectory(bitwriter)
add_subdirectory(irreader)
add_subdirectory(linker)
add_subdirectory(target)
add_subdirectory(transforms)
add_subdirectory(executionengine)



================================================
FILE: src/bindings/ocaml/README.txt
================================================
This directory contains LLVM bindings for the OCaml programming language
(http://ocaml.org).

Prerequisites
-------------

* OCaml 4.00.0+.
* ctypes 0.4+.
* oUnit 2+ (only required for tests).
* CMake (to build LLVM).

Building the bindings
---------------------

If all dependencies are present, the bindings will be built and installed
as a part of the default CMake configuration, with no further action.
They will only work with the specific OCaml compiler detected during the build.

The bindings can also be built out-of-tree, i.e. targeting a preinstalled
LLVM. To do this, configure the LLVM build tree as follows:

    $ cmake -DLLVM_OCAML_OUT_OF_TREE=TRUE \
            -DCMAKE_INSTALL_PREFIX=[OCaml install prefix] \
            [... any other options]

then build and install it as:

    $ make ocaml_all
    $ cmake -P bindings/ocaml/cmake_install.cmake



================================================
FILE: src/bindings/ocaml/all_backends/all_backends_ocaml.c
================================================
/*===-- all_backends_ocaml.c - LLVM OCaml Glue ------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/Target.h"
#include "caml/alloc.h"
#include "caml/fail.h"
#include "caml/memory.h"
#include "caml/custom.h"

/* unit -> unit */
CAMLprim value llvm_initialize_all(value Unit) {
  LLVMInitializeAllTargetInfos();
  LLVMInitializeAllTargets();
  LLVMInitializeAllTargetMCs();
  LLVMInitializeAllAsmPrinters();
  LLVMInitializeAllAsmParsers();
  return Val_unit;
}



================================================
FILE: src/bindings/ocaml/all_backends/CMakeLists.txt
================================================
add_ocaml_library(llvm_all_backends
  OCAML    llvm_all_backends
  OCAMLDEP llvm
  C        all_backends_ocaml
  LLVM     ${LLVM_TARGETS_TO_BUILD})



================================================
FILE: src/bindings/ocaml/all_backends/llvm_all_backends.ml
================================================
(*===-- llvm_all_backends.ml - LLVM OCaml Interface -----------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

external initialize : unit -> unit = "llvm_initialize_all"



================================================
FILE: src/bindings/ocaml/all_backends/llvm_all_backends.mli
================================================
(*===-- llvm_all_backends.mli - LLVM OCaml Interface ----------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Initialize all the backends targets *)
val initialize : unit -> unit



================================================
FILE: src/bindings/ocaml/analysis/analysis_ocaml.c
================================================
/*===-- analysis_ocaml.c - LLVM OCaml Glue ----------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/Analysis.h"
#include "llvm-c/Core.h"
#include "caml/alloc.h"
#include "caml/mlvalues.h"
#include "caml/memory.h"

/* Llvm.llmodule -> string option */
CAMLprim value llvm_verify_module(LLVMModuleRef M) {
  CAMLparam0();
  CAMLlocal2(String, Option);

  char *Message;
  int Result = LLVMVerifyModule(M, LLVMReturnStatusAction, &Message);

  if (0 == Result) {
    Option = Val_int(0);
  } else {
    Option = alloc(1, 0);
    String = copy_string(Message);
    Store_field(Option, 0, String);
  }

  LLVMDisposeMessage(Message);

  CAMLreturn(Option);
}

/* Llvm.llvalue -> bool */
CAMLprim value llvm_verify_function(LLVMValueRef Fn) {
  return Val_bool(LLVMVerifyFunction(Fn, LLVMReturnStatusAction) == 0);
}

/* Llvm.llmodule -> unit */
CAMLprim value llvm_assert_valid_module(LLVMModuleRef M) {
  LLVMVerifyModule(M, LLVMAbortProcessAction, 0);
  return Val_unit;
}

/* Llvm.llvalue -> unit */
CAMLprim value llvm_assert_valid_function(LLVMValueRef Fn) {
  LLVMVerifyFunction(Fn, LLVMAbortProcessAction);
  return Val_unit;
}

/* Llvm.llvalue -> unit */
CAMLprim value llvm_view_function_cfg(LLVMValueRef Fn) {
  LLVMViewFunctionCFG(Fn);
  return Val_unit;
}

/* Llvm.llvalue -> unit */
CAMLprim value llvm_view_function_cfg_only(LLVMValueRef Fn) {
  LLVMViewFunctionCFGOnly(Fn);
  return Val_unit;
}



================================================
FILE: src/bindings/ocaml/analysis/CMakeLists.txt
================================================
add_ocaml_library(llvm_analysis
  OCAML    llvm_analysis
  OCAMLDEP llvm
  C        analysis_ocaml
  LLVM     analysis)



================================================
FILE: src/bindings/ocaml/analysis/llvm_analysis.ml
================================================
(*===-- llvm_analysis.ml - LLVM OCaml Interface ---------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)


external verify_module : Llvm.llmodule -> string option = "llvm_verify_module"

external verify_function : Llvm.llvalue -> bool = "llvm_verify_function"

external assert_valid_module : Llvm.llmodule -> unit
                             = "llvm_assert_valid_module"

external assert_valid_function : Llvm.llvalue -> unit
                               = "llvm_assert_valid_function"
external view_function_cfg : Llvm.llvalue -> unit = "llvm_view_function_cfg"
external view_function_cfg_only : Llvm.llvalue -> unit
                                = "llvm_view_function_cfg_only"



================================================
FILE: src/bindings/ocaml/analysis/llvm_analysis.mli
================================================
(*===-- llvm_analysis.mli - LLVM OCaml Interface --------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Intermediate representation analysis.

    This interface provides an OCaml API for LLVM IR analyses, the classes in
    the Analysis library. *)

(** [verify_module m] returns [None] if the module [m] is valid, and
    [Some reason] if it is invalid. [reason] is a string containing a
    human-readable validation report. See [llvm::verifyModule]. *)
external verify_module : Llvm.llmodule -> string option = "llvm_verify_module"

(** [verify_function f] returns [None] if the function [f] is valid, and
    [Some reason] if it is invalid. [reason] is a string containing a
    human-readable validation report. See [llvm::verifyFunction]. *)
external verify_function : Llvm.llvalue -> bool = "llvm_verify_function"

(** [verify_module m] returns if the module [m] is valid, but prints a
    validation report to [stderr] and aborts the program if it is invalid. See
    [llvm::verifyModule]. *)
external assert_valid_module : Llvm.llmodule -> unit
                             = "llvm_assert_valid_module"

(** [verify_function f] returns if the function [f] is valid, but prints a
    validation report to [stderr] and aborts the program if it is invalid. See
    [llvm::verifyFunction]. *)
external assert_valid_function : Llvm.llvalue -> unit
                               = "llvm_assert_valid_function"

(** [view_function_cfg f] opens up a ghostscript window displaying the CFG of
    the current function with the code for each basic block inside.
    See [llvm::Function::viewCFG]. *)
external view_function_cfg : Llvm.llvalue -> unit = "llvm_view_function_cfg"

(** [view_function_cfg_only f] works just like [view_function_cfg], but does not
    include the contents of basic blocks into the nodes.
    See [llvm::Function::viewCFGOnly]. *)
external view_function_cfg_only : Llvm.llvalue -> unit
                                = "llvm_view_function_cfg_only"



================================================
FILE: src/bindings/ocaml/backends/backend_ocaml.c
================================================
/*===-- backend_ocaml.c - LLVM OCaml Glue -----------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/Target.h"
#include "caml/alloc.h"
#include "caml/memory.h"

/* TODO: Figure out how to call these only for targets which support them.
 * LLVMInitialize ## target ## AsmPrinter();
 * LLVMInitialize ## target ## AsmParser();
 * LLVMInitialize ## target ## Disassembler();
 */

#define INITIALIZER1(target) \
  CAMLprim value llvm_initialize_ ## target(value Unit) {  \
    LLVMInitialize ## target ## TargetInfo();              \
    LLVMInitialize ## target ## Target();                  \
    LLVMInitialize ## target ## TargetMC();                \
    return Val_unit;                                       \
  }

#define INITIALIZER(target) INITIALIZER1(target)

INITIALIZER(TARGET)



================================================
FILE: src/bindings/ocaml/backends/CMakeLists.txt
================================================
foreach(TARGET ${LLVM_TARGETS_TO_BUILD})
  set(OCAML_LLVM_TARGET ${TARGET})

  foreach( ext ml mli )
    configure_file(
        "${CMAKE_CURRENT_SOURCE_DIR}/llvm_backend.${ext}.in"
        "${CMAKE_CURRENT_BINARY_DIR}/llvm_${TARGET}.${ext}")
  endforeach()

  configure_file(
    "${CMAKE_CURRENT_SOURCE_DIR}/backend_ocaml.c"
    "${CMAKE_CURRENT_BINARY_DIR}/${TARGET}_ocaml.c")

  add_ocaml_library(llvm_${TARGET}
    OCAML    llvm_${TARGET}
    C        ${TARGET}_ocaml
    CFLAGS   -DTARGET=${TARGET}
    LLVM     ${TARGET}
    NOCOPY)

  configure_file(
    "${CMAKE_CURRENT_SOURCE_DIR}/META.llvm_backend.in"
    "${LLVM_LIBRARY_DIR}/ocaml/META.llvm_${TARGET}")

  install(FILES "${LLVM_LIBRARY_DIR}/ocaml/META.llvm_${TARGET}"
          DESTINATION "${LLVM_OCAML_INSTALL_PATH}")
endforeach()



================================================
FILE: src/bindings/ocaml/backends/llvm_backend.ml.in
================================================
(*===-- llvm_backend.ml.in - LLVM OCaml Interface -------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

external initialize : unit -> unit = "llvm_initialize_@TARGET@"



================================================
FILE: src/bindings/ocaml/backends/llvm_backend.mli.in
================================================
(*===-- llvm_backend.mli.in - LLVM OCaml Interface ------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** @TARGET@ Initialization.

    This interface provides an OCaml API for initialization of
    the @TARGET@ LLVM target. By referencing this module, you will cause
    OCaml to load or link in the LLVM libraries corresponding to the target.
    By calling [initialize], you will register components of this target
    in the target registry, which is necessary in order to emit assembly,
    object files, and so on. *)

external initialize : unit -> unit = "llvm_initialize_@TARGET@"


================================================
FILE: src/bindings/ocaml/backends/META.llvm_backend.in
================================================
name = "llvm_@TARGET@"
version = "@PACKAGE_VERSION@"
description = "@TARGET@ Backend for LLVM"
requires = "llvm"
archive(byte) = "llvm_@TARGET@.cma"
archive(native) = "llvm_@TARGET@.cmxa"
directory = "llvm"



================================================
FILE: src/bindings/ocaml/bitreader/bitreader_ocaml.c
================================================
/*===-- bitwriter_ocaml.c - LLVM OCaml Glue ---------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/BitReader.h"
#include "llvm-c/Core.h"
#include "caml/alloc.h"
#include "caml/fail.h"
#include "caml/memory.h"
#include "caml/callback.h"

void llvm_raise(value Prototype, char *Message);

/* Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule */
CAMLprim LLVMModuleRef llvm_get_module(LLVMContextRef C, LLVMMemoryBufferRef MemBuf) {
  LLVMModuleRef M;

  if (LLVMGetBitcodeModuleInContext2(C, MemBuf, &M))
    llvm_raise(*caml_named_value("Llvm_bitreader.Error"), LLVMCreateMessage(""));

  return M;
}

/* Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule */
CAMLprim LLVMModuleRef llvm_parse_bitcode(LLVMContextRef C, LLVMMemoryBufferRef MemBuf) {
  LLVMModuleRef M;

  if (LLVMParseBitcodeInContext2(C, MemBuf, &M))
    llvm_raise(*caml_named_value("Llvm_bitreader.Error"), LLVMCreateMessage(""));

  return M;
}



================================================
FILE: src/bindings/ocaml/bitreader/CMakeLists.txt
================================================
add_ocaml_library(llvm_bitreader
  OCAML    llvm_bitreader
  OCAMLDEP llvm
  C        bitreader_ocaml
  LLVM     bitreader)



================================================
FILE: src/bindings/ocaml/bitreader/llvm_bitreader.ml
================================================
(*===-- llvm_bitreader.ml - LLVM OCaml Interface --------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

exception Error of string

let () = Callback.register_exception "Llvm_bitreader.Error" (Error "")

external get_module
  : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule
  = "llvm_get_module"
external parse_bitcode
  : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule
  = "llvm_parse_bitcode"



================================================
FILE: src/bindings/ocaml/bitreader/llvm_bitreader.mli
================================================
(*===-- llvm_bitreader.mli - LLVM OCaml Interface -------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Bitcode reader.

    This interface provides an OCaml API for the LLVM bitcode reader, the
    classes in the Bitreader library. *)

exception Error of string

(** [get_module context mb] reads the bitcode for a new module [m] from the
    memory buffer [mb] in the context [context].  Returns [m] if successful, or
    raises [Error msg] otherwise, where [msg] is a description of the error
    encountered. See the function [llvm::getBitcodeModule]. *)
val get_module : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule

(** [parse_bitcode context mb] parses the bitcode for a new module [m] from the
    memory buffer [mb] in the context [context]. Returns [m] if successful, or
    raises [Error msg] otherwise, where [msg] is a description of the error
    encountered. See the function [llvm::ParseBitcodeFile]. *)
val parse_bitcode : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule



================================================
FILE: src/bindings/ocaml/bitwriter/bitwriter_ocaml.c
================================================
/*===-- bitwriter_ocaml.c - LLVM OCaml Glue ---------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/BitWriter.h"
#include "llvm-c/Core.h"
#include "caml/alloc.h"
#include "caml/mlvalues.h"
#include "caml/memory.h"

/* Llvm.llmodule -> string -> bool */
CAMLprim value llvm_write_bitcode_file(LLVMModuleRef M, value Path) {
  int Result = LLVMWriteBitcodeToFile(M, String_val(Path));
  return Val_bool(Result == 0);
}

/* ?unbuffered:bool -> Llvm.llmodule -> Unix.file_descr -> bool */
CAMLprim value llvm_write_bitcode_to_fd(value U, LLVMModuleRef M, value FD) {
  int Unbuffered;
  int Result;

  if (U == Val_int(0)) {
    Unbuffered = 0;
  } else {
    Unbuffered = Bool_val(Field(U, 0));
  }

  Result = LLVMWriteBitcodeToFD(M, Int_val(FD), 0, Unbuffered);
  return Val_bool(Result == 0);
}

/* Llvm.llmodule -> Llvm.llmemorybuffer */
CAMLprim LLVMMemoryBufferRef llvm_write_bitcode_to_memory_buffer(LLVMModuleRef M) {
  return LLVMWriteBitcodeToMemoryBuffer(M);
}



================================================
FILE: src/bindings/ocaml/bitwriter/CMakeLists.txt
================================================
add_ocaml_library(llvm_bitwriter
  OCAML    llvm_bitwriter
  OCAMLDEP llvm
  C        bitwriter_ocaml
  LLVM     bitwriter)



================================================
FILE: src/bindings/ocaml/bitwriter/llvm_bitwriter.ml
================================================
(*===-- llvm_bitwriter.ml - LLVM OCaml Interface --------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===
 *
 * This interface provides an OCaml API for the LLVM intermediate
 * representation, the classes in the VMCore library.
 *
 *===----------------------------------------------------------------------===*)

external write_bitcode_file
  : Llvm.llmodule -> string -> bool
  = "llvm_write_bitcode_file"

external write_bitcode_to_fd
  : ?unbuffered:bool -> Llvm.llmodule -> Unix.file_descr -> bool
  = "llvm_write_bitcode_to_fd"

external write_bitcode_to_memory_buffer
  : Llvm.llmodule -> Llvm.llmemorybuffer
  = "llvm_write_bitcode_to_memory_buffer"

let output_bitcode ?unbuffered channel m =
  write_bitcode_to_fd ?unbuffered m (Unix.descr_of_out_channel channel)



================================================
FILE: src/bindings/ocaml/bitwriter/llvm_bitwriter.mli
================================================
(*===-- llvm_bitwriter.mli - LLVM OCaml Interface -------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Bitcode writer.

    This interface provides an OCaml API for the LLVM bitcode writer, the
    classes in the Bitwriter library. *)

(** [write_bitcode_file m path] writes the bitcode for module [m] to the file at
    [path]. Returns [true] if successful, [false] otherwise. *)
external write_bitcode_file
  : Llvm.llmodule -> string -> bool
  = "llvm_write_bitcode_file"

(** [write_bitcode_to_fd ~unbuffered fd m] writes the bitcode for module
    [m] to the channel [c]. If [unbuffered] is [true], after every write the fd
    will be flushed. Returns [true] if successful, [false] otherwise. *)
external write_bitcode_to_fd
  : ?unbuffered:bool -> Llvm.llmodule -> Unix.file_descr -> bool
  = "llvm_write_bitcode_to_fd"

(** [write_bitcode_to_memory_buffer m] returns a memory buffer containing
    the bitcode for module [m]. *)
external write_bitcode_to_memory_buffer
  : Llvm.llmodule -> Llvm.llmemorybuffer
  = "llvm_write_bitcode_to_memory_buffer"

(** [output_bitcode ~unbuffered c m] writes the bitcode for module [m]
    to the channel [c]. If [unbuffered] is [true], after every write the fd
    will be flushed. Returns [true] if successful, [false] otherwise. *)
val output_bitcode : ?unbuffered:bool -> out_channel -> Llvm.llmodule -> bool



================================================
FILE: src/bindings/ocaml/executionengine/CMakeLists.txt
================================================
add_ocaml_library(llvm_executionengine
  OCAML    llvm_executionengine
  OCAMLDEP llvm llvm_target
  C        executionengine_ocaml
  LLVM     executionengine mcjit native
  PKG      ctypes)



================================================
FILE: src/bindings/ocaml/executionengine/executionengine_ocaml.c
================================================
/*===-- executionengine_ocaml.c - LLVM OCaml Glue ---------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include <string.h>
#include <assert.h>
#include "llvm-c/Core.h"
#include "llvm-c/ExecutionEngine.h"
#include "llvm-c/Target.h"
#include "caml/alloc.h"
#include "caml/custom.h"
#include "caml/fail.h"
#include "caml/memory.h"
#include "caml/callback.h"

void llvm_raise(value Prototype, char *Message);

/* unit -> bool */
CAMLprim value llvm_ee_initialize(value Unit) {
  LLVMLinkInMCJIT();

  return Val_bool(!LLVMInitializeNativeTarget() &&
                  !LLVMInitializeNativeAsmParser() &&
                  !LLVMInitializeNativeAsmPrinter());
}

/* llmodule -> llcompileroption -> ExecutionEngine.t */
CAMLprim LLVMExecutionEngineRef llvm_ee_create(value OptRecordOpt, LLVMModuleRef M) {
  value OptRecord;
  LLVMExecutionEngineRef MCJIT;
  char *Error;
  struct LLVMMCJITCompilerOptions Options;

  LLVMInitializeMCJITCompilerOptions(&Options, sizeof(Options));
  if (OptRecordOpt != Val_int(0)) {
    OptRecord = Field(OptRecordOpt, 0);
    Options.OptLevel = Int_val(Field(OptRecord, 0));
    Options.CodeModel = Int_val(Field(OptRecord, 1));
    Options.NoFramePointerElim = Int_val(Field(OptRecord, 2));
    Options.EnableFastISel = Int_val(Field(OptRecord, 3));
    Options.MCJMM = NULL;
  }

  if (LLVMCreateMCJITCompilerForModule(&MCJIT, M, &Options,
                                      sizeof(Options), &Error))
    llvm_raise(*caml_named_value("Llvm_executionengine.Error"), Error);
  return MCJIT;
}

/* ExecutionEngine.t -> unit */
CAMLprim value llvm_ee_dispose(LLVMExecutionEngineRef EE) {
  LLVMDisposeExecutionEngine(EE);
  return Val_unit;
}

/* llmodule -> ExecutionEngine.t -> unit */
CAMLprim value llvm_ee_add_module(LLVMModuleRef M, LLVMExecutionEngineRef EE) {
  LLVMAddModule(EE, M);
  return Val_unit;
}

/* llmodule -> ExecutionEngine.t -> llmodule */
CAMLprim value llvm_ee_remove_module(LLVMModuleRef M, LLVMExecutionEngineRef EE) {
  LLVMModuleRef RemovedModule;
  char *Error;
  if (LLVMRemoveModule(EE, M, &RemovedModule, &Error))
    llvm_raise(*caml_named_value("Llvm_executionengine.Error"), Error);
  return Val_unit;
}

/* ExecutionEngine.t -> unit */
CAMLprim value llvm_ee_run_static_ctors(LLVMExecutionEngineRef EE) {
  LLVMRunStaticConstructors(EE);
  return Val_unit;
}

/* ExecutionEngine.t -> unit */
CAMLprim value llvm_ee_run_static_dtors(LLVMExecutionEngineRef EE) {
  LLVMRunStaticDestructors(EE);
  return Val_unit;
}

extern value llvm_alloc_data_layout(LLVMTargetDataRef TargetData);

/* ExecutionEngine.t -> Llvm_target.DataLayout.t */
CAMLprim value llvm_ee_get_data_layout(LLVMExecutionEngineRef EE) {
  value DataLayout;
  LLVMTargetDataRef OrigDataLayout;
  char* TargetDataCStr;

  OrigDataLayout = LLVMGetExecutionEngineTargetData(EE);
  TargetDataCStr = LLVMCopyStringRepOfTargetData(OrigDataLayout);
  DataLayout = llvm_alloc_data_layout(LLVMCreateTargetData(TargetDataCStr));
  LLVMDisposeMessage(TargetDataCStr);

  return DataLayout;
}

/* Llvm.llvalue -> int64 -> llexecutionengine -> unit */
CAMLprim value llvm_ee_add_global_mapping(LLVMValueRef Global, value Ptr,
                                          LLVMExecutionEngineRef EE) {
  LLVMAddGlobalMapping(EE, Global, (void*) (Int64_val(Ptr)));
  return Val_unit;
}

CAMLprim value llvm_ee_get_global_value_address(value Name,
						LLVMExecutionEngineRef EE) {
  return caml_copy_int64((int64_t) LLVMGetGlobalValueAddress(EE, String_val(Name)));
}

CAMLprim value llvm_ee_get_function_address(value Name,
					    LLVMExecutionEngineRef EE) {
  return caml_copy_int64((int64_t) LLVMGetFunctionAddress(EE, String_val(Name)));
}



================================================
FILE: src/bindings/ocaml/executionengine/llvm_executionengine.ml
================================================
(*===-- llvm_executionengine.ml - LLVM OCaml Interface --------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

exception Error of string

let () = Callback.register_exception "Llvm_executionengine.Error" (Error "")

external initialize : unit -> bool
  = "llvm_ee_initialize"

type llexecutionengine

type llcompileroptions = {
  opt_level: int;
  code_model: Llvm_target.CodeModel.t;
  no_framepointer_elim: bool;
  enable_fast_isel: bool;
}

let default_compiler_options = {
  opt_level = 0;
  code_model = Llvm_target.CodeModel.JITDefault;
  no_framepointer_elim = false;
  enable_fast_isel = false }

external create : ?options:llcompileroptions -> Llvm.llmodule -> llexecutionengine
  = "llvm_ee_create"
external dispose : llexecutionengine -> unit
  = "llvm_ee_dispose"
external add_module : Llvm.llmodule -> llexecutionengine -> unit
  = "llvm_ee_add_module"
external remove_module : Llvm.llmodule -> llexecutionengine -> unit
  = "llvm_ee_remove_module"
external run_static_ctors : llexecutionengine -> unit
  = "llvm_ee_run_static_ctors"
external run_static_dtors : llexecutionengine -> unit
  = "llvm_ee_run_static_dtors"
external data_layout : llexecutionengine -> Llvm_target.DataLayout.t
  = "llvm_ee_get_data_layout"
external add_global_mapping_ : Llvm.llvalue -> nativeint -> llexecutionengine -> unit
  = "llvm_ee_add_global_mapping"
external get_global_value_address_ : string -> llexecutionengine -> nativeint
  = "llvm_ee_get_global_value_address"
external get_function_address_ : string -> llexecutionengine -> nativeint
  = "llvm_ee_get_function_address"

let add_global_mapping llval ptr ee =
  add_global_mapping_ llval (Ctypes.raw_address_of_ptr (Ctypes.to_voidp ptr)) ee

let get_global_value_address name typ ee =
  let vptr = get_global_value_address_ name ee in
  if Nativeint.to_int vptr <> 0 then
    let open Ctypes in !@ (coerce (ptr void) (ptr typ) (ptr_of_raw_address vptr))
  else
    raise (Error ("Value " ^ name ^ " not found"))

let get_function_address name typ ee =
  let fptr = get_function_address_ name ee in
  if Nativeint.to_int fptr <> 0 then
    let open Ctypes in coerce (ptr void) typ (ptr_of_raw_address fptr)
  else
    raise (Error ("Function " ^ name ^ " not found"))

(* The following are not bound. Patches are welcome.
target_machine : llexecutionengine -> Llvm_target.TargetMachine.t
 *)



================================================
FILE: src/bindings/ocaml/executionengine/llvm_executionengine.mli
================================================
(*===-- llvm_executionengine.mli - LLVM OCaml Interface -------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** JIT Interpreter.

    This interface provides an OCaml API for LLVM execution engine (JIT/
    interpreter), the classes in the [ExecutionEngine] library. *)

exception Error of string

(** [initialize ()] initializes the backend corresponding to the host.
    Returns [true] if initialization is successful; [false] indicates
    that there is no such backend or it is unable to emit object code
    via MCJIT. *)
val initialize : unit -> bool

(** An execution engine is either a JIT compiler or an interpreter, capable of
    directly loading an LLVM module and executing its functions without first
    invoking a static compiler and generating a native executable. *)
type llexecutionengine

(** MCJIT compiler options. See [llvm::TargetOptions]. *)
type llcompileroptions = {
  opt_level: int;
  code_model: Llvm_target.CodeModel.t;
  no_framepointer_elim: bool;
  enable_fast_isel: bool;
}

(** Default MCJIT compiler options:
    [{ opt_level = 0; code_model = CodeModel.JIT_default;
       no_framepointer_elim = false; enable_fast_isel = false }] *)
val default_compiler_options : llcompileroptions

(** [create m optlevel] creates a new MCJIT just-in-time compiler, taking
    ownership of the module [m] if successful with the desired optimization
    level [optlevel]. Raises [Error msg] if an error occurrs. The execution
    engine is not garbage collected and must be destroyed with [dispose ee].

    Run {!initialize} before using this function.

    See the function [llvm::EngineBuilder::create]. *)
val create : ?options:llcompileroptions -> Llvm.llmodule -> llexecutionengine

(** [dispose ee] releases the memory used by the execution engine and must be
    invoked to avoid memory leaks. *)
val dispose : llexecutionengine -> unit

(** [add_module m ee] adds the module [m] to the execution engine [ee]. *)
val add_module : Llvm.llmodule -> llexecutionengine -> unit

(** [remove_module m ee] removes the module [m] from the execution engine
    [ee]. Raises [Error msg] if an error occurs. *)
val remove_module : Llvm.llmodule -> llexecutionengine -> unit

(** [run_static_ctors ee] executes the static constructors of each module in
    the execution engine [ee]. *)
val run_static_ctors : llexecutionengine -> unit

(** [run_static_dtors ee] executes the static destructors of each module in
    the execution engine [ee]. *)
val run_static_dtors : llexecutionengine -> unit

(** [data_layout ee] is the data layout of the execution engine [ee]. *)
val data_layout : llexecutionengine -> Llvm_target.DataLayout.t

(** [add_global_mapping gv ptr ee] tells the execution engine [ee] that
    the global [gv] is at the specified location [ptr], which must outlive
    [gv] and [ee].
    All uses of [gv] in the compiled code will refer to [ptr]. *)
val add_global_mapping : Llvm.llvalue -> 'a Ctypes.ptr -> llexecutionengine -> unit

(** [get_global_value_address id typ ee] returns a pointer to the
    identifier [id] as type [typ], which will be a pointer type for a
    value, and which will be live as long as [id] and [ee]
    are. Caution: this function finalizes, i.e. forces code
    generation, all loaded modules.  Further modifications to the
    modules will not have any effect. *)
val get_global_value_address : string -> 'a Ctypes.typ -> llexecutionengine -> 'a

(** [get_function_address fn typ ee] returns a pointer to the function
    [fn] as type [typ], which will be a pointer type for a function
    (e.g. [(int -> int) typ]), and which will be live as long as [fn]
    and [ee] are. Caution: this function finalizes, i.e. forces code
    generation, all loaded modules.  Further modifications to the
    modules will not have any effect. *)
val get_function_address : string -> 'a Ctypes.typ -> llexecutionengine -> 'a



================================================
FILE: src/bindings/ocaml/irreader/CMakeLists.txt
================================================
add_ocaml_library(llvm_irreader
  OCAML    llvm_irreader
  OCAMLDEP llvm
  C        irreader_ocaml
  LLVM     irreader)



================================================
FILE: src/bindings/ocaml/irreader/irreader_ocaml.c
================================================
/*===-- irreader_ocaml.c - LLVM OCaml Glue ----------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/IRReader.h"
#include "caml/alloc.h"
#include "caml/fail.h"
#include "caml/memory.h"
#include "caml/callback.h"

void llvm_raise(value Prototype, char *Message);

/* Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule */
CAMLprim value llvm_parse_ir(LLVMContextRef C,
                             LLVMMemoryBufferRef MemBuf) {
  CAMLparam0();
  CAMLlocal2(Variant, MessageVal);
  LLVMModuleRef M;
  char *Message;

  if (LLVMParseIRInContext(C, MemBuf, &M, &Message))
    llvm_raise(*caml_named_value("Llvm_irreader.Error"), Message);

  CAMLreturn((value) M);
}



================================================
FILE: src/bindings/ocaml/irreader/llvm_irreader.ml
================================================
(*===-- llvm_irreader.ml - LLVM OCaml Interface ---------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)


exception Error of string

let _ = Callback.register_exception "Llvm_irreader.Error" (Error "")

external parse_ir : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule
                  = "llvm_parse_ir"



================================================
FILE: src/bindings/ocaml/irreader/llvm_irreader.mli
================================================
(*===-- llvm_irreader.mli - LLVM OCaml Interface --------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** IR reader.

    This interface provides an OCaml API for the LLVM assembly reader, the
    classes in the IRReader library. *)

exception Error of string

(** [parse_ir context mb] parses the IR for a new module [m] from the
    memory buffer [mb] in the context [context]. Returns [m] if successful, or
    raises [Error msg] otherwise, where [msg] is a description of the error
    encountered. See the function [llvm::ParseIR]. *)
val parse_ir : Llvm.llcontext -> Llvm.llmemorybuffer -> Llvm.llmodule



================================================
FILE: src/bindings/ocaml/linker/CMakeLists.txt
================================================
add_ocaml_library(llvm_linker
  OCAML    llvm_linker
  OCAMLDEP llvm
  C        linker_ocaml
  LLVM     linker)



================================================
FILE: src/bindings/ocaml/linker/linker_ocaml.c
================================================
/*===-- linker_ocaml.c - LLVM OCaml Glue ------------------------*- C++ -*-===*\
|*                                                                            *|
|*                     The LLVM Compiler Infrastructure                       *|
|*                                                                            *|
|* This file is distributed under the University of Illinois Open Source      *|
|* License. See LICENSE.TXT for details.                                      *|
|*                                                                            *|
|*===----------------------------------------------------------------------===*|
|*                                                                            *|
|* This file glues LLVM's OCaml interface to its C interface. These functions *|
|* are by and large transparent wrappers to the corresponding C functions.    *|
|*                                                                            *|
|* Note that these functions intentionally take liberties with the CAMLparamX *|
|* macros, since most of the parameters are not GC heap objects.              *|
|*                                                                            *|
\*===----------------------------------------------------------------------===*/

#include "llvm-c/Core.h"
#include "llvm-c/Linker.h"
#include "caml/alloc.h"
#include "caml/memory.h"
#include "caml/fail.h"
#include "caml/callback.h"

void llvm_raise(value Prototype, char *Message);

/* llmodule -> llmodule -> unit */
CAMLprim value llvm_link_modules(LLVMModuleRef Dst, LLVMModuleRef Src) {
  if (LLVMLinkModules2(Dst, Src))
    llvm_raise(*caml_named_value("Llvm_linker.Error"), LLVMCreateMessage("Linking failed"));

  return Val_unit;
}



================================================
FILE: src/bindings/ocaml/linker/llvm_linker.ml
================================================
(*===-- llvm_linker.ml - LLVM OCaml Interface ------------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

exception Error of string

let () = Callback.register_exception "Llvm_linker.Error" (Error "")

external link_modules' : Llvm.llmodule -> Llvm.llmodule -> unit
                       = "llvm_link_modules"



================================================
FILE: src/bindings/ocaml/linker/llvm_linker.mli
================================================
(*===-- llvm_linker.mli - LLVM OCaml Interface -----------------*- OCaml -*-===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Linker.

    This interface provides an OCaml API for LLVM bitcode linker,
    the classes in the Linker library. *)

exception Error of string

(** [link_modules' dst src] links [src] into [dst], raising [Error]
    if the linking fails. The src module is destroyed. *)
val link_modules' : Llvm.llmodule -> Llvm.llmodule -> unit


================================================
FILE: src/bindings/ocaml/llvm/CMakeLists.txt
================================================
add_ocaml_library(llvm
  OCAML llvm
  C     llvm_ocaml
  LLVM  core support)

configure_file(
  "${CMAKE_CURRENT_SOURCE_DIR}/META.llvm.in"
  "${LLVM_LIBRARY_DIR}/ocaml/META.llvm")

install(FILES "${LLVM_LIBRARY_DIR}/ocaml/META.llvm"
        DESTINATION "${LLVM_OCAML_INSTALL_PATH}")



================================================
FILE: src/bindings/ocaml/llvm/llvm.ml
================================================
(*===-- llvm/llvm.ml - LLVM OCaml Interface -------------------------------===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)


type llcontext
type llmodule
type lltype
type llvalue
type lluse
type llbasicblock
type llbuilder
type llattrkind
type llattribute
type llmemorybuffer
type llmdkind

exception FeatureDisabled of string

let () = Callback.register_exception "Llvm.FeatureDisabled" (FeatureDisabled "")

module TypeKind = struct
  type t =
  | Void
  | Half
  | Float
  | Double
  | X86fp80
  | Fp128
  | Ppc_fp128
  | Label
  | Integer
  | Function
  | Struct
  | Array
  | Pointer
  | Vector
  | Metadata
  | X86_mmx
  | Token
end

module Linkage = struct
  type t =
  | External
  | Available_externally
  | Link_once
  | Link_once_odr
  | Link_once_odr_auto_hide
  | Weak
  | Weak_odr
  | Appending
  | Internal
  | Private
  | Dllimport
  | Dllexport
  | External_weak
  | Ghost
  | Common
  | Linker_private
  | Linker_private_weak
end

module Visibility = struct
  type t =
  | Default
  | Hidden
  | Protected
end

module DLLStorageClass = struct
  type t =
  | Default
  | DLLImport
  | DLLExport
end

module CallConv = struct
  let c = 0
  let fast = 8
  let cold = 9
  let x86_stdcall = 64
  let x86_fastcall = 65
end

module AttrRepr = struct
  type t =
  | Enum of llattrkind * int64
  | String of string * string
end

module AttrIndex = struct
  type t =
  | Function
  | Return
  | Param of int

  let to_int index =
    match index with
    | Function -> -1
    | Return -> 0
    | Param(n) -> 1 + n
end

module Attribute = struct
  type t =
  | Zext
  | Sext
  | Noreturn
  | Inreg
  | Structret
  | Nounwind
  | Noalias
  | Byval
  | Nest
  | Readnone
  | Readonly
  | Noinline
  | Alwaysinline
  | Optsize
  | Ssp
  | Sspreq
  | Alignment of int
  | Nocapture
  | Noredzone
  | Noimplicitfloat
  | Naked
  | Inlinehint
  | Stackalignment of int
  | ReturnsTwice
  | UWTable
  | NonLazyBind
end

module Icmp = struct
  type t =
  | Eq
  | Ne
  | Ugt
  | Uge
  | Ult
  | Ule
  | Sgt
  | Sge
  | Slt
  | Sle
end

module Fcmp = struct
  type t =
  | False
  | Oeq
  | Ogt
  | Oge
  | Olt
  | Ole
  | One
  | Ord
  | Uno
  | Ueq
  | Ugt
  | Uge
  | Ult
  | Ule
  | Une
  | True
end

module Opcode  = struct
  type t =
  | Invalid (* not an instruction *)
  (* Terminator Instructions *)
  | Ret
  | Br
  | Switch
  | IndirectBr
  | Invoke
  | Invalid2
  | Unreachable
  (* Standard Binary Operators *)
  | Add
  | FAdd
  | Sub
  | FSub
  | Mul
  | FMul
  | UDiv
  | SDiv
  | FDiv
  | URem
  | SRem
  | FRem
  (* Logical Operators *)
  | Shl
  | LShr
  | AShr
  | And
  | Or
  | Xor
  (* Memory Operators *)
  | Alloca
  | Load
  | Store
  | GetElementPtr
  (* Cast Operators *)
  | Trunc
  | ZExt
  | SExt
  | FPToUI
  | FPToSI
  | UIToFP
  | SIToFP
  | FPTrunc
  | FPExt
  | PtrToInt
  | IntToPtr
  | BitCast
  (* Other Operators *)
  | ICmp
  | FCmp
  | PHI
  | Call
  | Select
  | UserOp1
  | UserOp2
  | VAArg
  | ExtractElement
  | InsertElement
  | ShuffleVector
  | ExtractValue
  | InsertValue
  | Fence
  | AtomicCmpXchg
  | AtomicRMW
  | Resume
  | LandingPad
  | AddrSpaceCast
  | CleanupRet
  | CatchRet
  | CatchPad
  | CleanupPad
  | CatchSwitch
end

module LandingPadClauseTy = struct
  type t =
  | Catch
  | Filter
end

module ThreadLocalMode = struct
  type t =
  | None
  | GeneralDynamic
  | LocalDynamic
  | InitialExec
  | LocalExec
end

module AtomicOrdering = struct
  type t =
  | NotAtomic
  | Unordered
  | Monotonic
  | Invalid
  | Acquire
  | Release
  | AcqiureRelease
  | SequentiallyConsistent
end

module AtomicRMWBinOp = struct
  type t =
  | Xchg
  | Add
  | Sub
  | And
  | Nand
  | Or
  | Xor
  | Max
  | Min
  | UMax
  | UMin
end

module ValueKind = struct
  type t =
  | NullValue
  | Argument
  | BasicBlock
  | InlineAsm
  | MDNode
  | MDString
  | BlockAddress
  | ConstantAggregateZero
  | ConstantArray
  | ConstantDataArray
  | ConstantDataVector
  | ConstantExpr
  | ConstantFP
  | ConstantInt
  | ConstantPointerNull
  | ConstantStruct
  | ConstantVector
  | Function
  | GlobalAlias
  | GlobalIFunc
  | GlobalVariable
  | UndefValue
  | Instruction of Opcode.t
end

module DiagnosticSeverity = struct
  type t =
  | Error
  | Warning
  | Remark
  | Note
end

exception IoError of string

let () = Callback.register_exception "Llvm.IoError" (IoError "")

external install_fatal_error_handler : (string -> unit) -> unit
                                     = "llvm_install_fatal_error_handler"
external reset_fatal_error_handler : unit -> unit
                                   = "llvm_reset_fatal_error_handler"
external enable_pretty_stacktrace : unit -> unit
                                  = "llvm_enable_pretty_stacktrace"
external parse_command_line_options : ?overview:string -> string array -> unit
                                    = "llvm_parse_command_line_options"

type ('a, 'b) llpos =
| At_end of 'a
| Before of 'b

type ('a, 'b) llrev_pos =
| At_start of 'a
| After of 'b


(*===-- Context error handling --------------------------------------------===*)
module Diagnostic = struct
  type t

  external description : t -> string = "llvm_get_diagnostic_description"
  external severity : t -> DiagnosticSeverity.t
                    = "llvm_get_diagnostic_severity"
end

external set_diagnostic_handler
  : llcontext -> (Diagnostic.t -> unit) option -> unit
  = "llvm_set_diagnostic_handler"

(*===-- Contexts ----------------------------------------------------------===*)
external create_context : unit -> llcontext = "llvm_create_context"
external dispose_context : llcontext -> unit = "llvm_dispose_context"
external global_context : unit -> llcontext = "llvm_global_context"
external mdkind_id : llcontext -> string -> llmdkind = "llvm_mdkind_id"

(*===-- Attributes --------------------------------------------------------===*)
exception UnknownAttribute of string

let () = Callback.register_exception "Llvm.UnknownAttribute"
                                     (UnknownAttribute "")

external enum_attr_kind : string -> llattrkind = "llvm_enum_attr_kind"
external llvm_create_enum_attr : llcontext -> llattrkind -> int64 ->
                                 llattribute
                               = "llvm_create_enum_attr_by_kind"
external is_enum_attr : llattribute -> bool = "llvm_is_enum_attr"
external get_enum_attr_kind : llattribute -> llattrkind
                            = "llvm_get_enum_attr_kind"
external get_enum_attr_value : llattribute -> int64
                             = "llvm_get_enum_attr_value"
external llvm_create_string_attr : llcontext -> string -> string ->
                                   llattribute
                                 = "llvm_create_string_attr"
external is_string_attr : llattribute -> bool = "llvm_is_string_attr"
external get_string_attr_kind : llattribute -> string
                              = "llvm_get_string_attr_kind"
external get_string_attr_value : llattribute -> string
                               = "llvm_get_string_attr_value"

let create_enum_attr context name value =
  llvm_create_enum_attr context (enum_attr_kind name) value
let create_string_attr context kind value =
  llvm_create_string_attr context kind value

let attr_of_repr context repr =
  match repr with
  | AttrRepr.Enum(kind, value) -> llvm_create_enum_attr context kind value
  | AttrRepr.String(key, value) -> llvm_create_string_attr context key value

let repr_of_attr attr =
  if is_enum_attr attr then
    AttrRepr.Enum(get_enum_attr_kind attr, get_enum_attr_value attr)
  else if is_string_attr attr then
    AttrRepr.String(get_string_attr_kind attr, get_string_attr_value attr)
  else assert false

(*===-- Modules -----------------------------------------------------------===*)
external create_module : llcontext -> string -> llmodule = "llvm_create_module"
external dispose_module : llmodule -> unit = "llvm_dispose_module"
external target_triple: llmodule -> string
                      = "llvm_target_triple"
external set_target_triple: string -> llmodule -> unit
                          = "llvm_set_target_triple"
external data_layout: llmodule -> string
                    = "llvm_data_layout"
external set_data_layout: string -> llmodule -> unit
                        = "llvm_set_data_layout"
external dump_module : llmodule -> unit = "llvm_dump_module"
external print_module : string -> llmodule -> unit = "llvm_print_module"
external string_of_llmodule : llmodule -> string = "llvm_string_of_llmodule"
external set_module_inline_asm : llmodule -> string -> unit
                               = "llvm_set_module_inline_asm"
external module_context : llmodule -> llcontext = "LLVMGetModuleContext"

(*===-- Types -------------------------------------------------------------===*)
external classify_type : lltype -> TypeKind.t = "llvm_classify_type"
external type_context : lltype -> llcontext = "llvm_type_context"
external type_is_sized : lltype -> bool = "llvm_type_is_sized"
external dump_type : lltype -> unit = "llvm_dump_type"
external string_of_lltype : lltype -> string = "llvm_string_of_lltype"

(*--... Operations on integer types ........................................--*)
external i1_type : llcontext -> lltype = "llvm_i1_type"
external i8_type : llcontext -> lltype = "llvm_i8_type"
external i16_type : llcontext -> lltype = "llvm_i16_type"
external i32_type : llcontext -> lltype = "llvm_i32_type"
external i64_type : llcontext -> lltype = "llvm_i64_type"

external integer_type : llcontext -> int -> lltype = "llvm_integer_type"
external integer_bitwidth : lltype -> int = "llvm_integer_bitwidth"

(*--... Operations on real types ...........................................--*)
external float_type : llcontext -> lltype = "llvm_float_type"
external double_type : llcontext -> lltype = "llvm_double_type"
external x86fp80_type : llcontext -> lltype = "llvm_x86fp80_type"
external fp128_type : llcontext -> lltype = "llvm_fp128_type"
external ppc_fp128_type : llcontext -> lltype = "llvm_ppc_fp128_type"

(*--... Operations on function types .......................................--*)
external function_type : lltype -> lltype array -> lltype = "llvm_function_type"
external var_arg_function_type : lltype -> lltype array -> lltype
                               = "llvm_var_arg_function_type"
external is_var_arg : lltype -> bool = "llvm_is_var_arg"
external return_type : lltype -> lltype = "LLVMGetReturnType"
external param_types : lltype -> lltype array = "llvm_param_types"

(*--... Operations on struct types .........................................--*)
external struct_type : llcontext -> lltype array -> lltype = "llvm_struct_type"
external packed_struct_type : llcontext -> lltype array -> lltype
                            = "llvm_packed_struct_type"
external struct_name : lltype -> string option = "llvm_struct_name"
external named_struct_type : llcontext -> string -> lltype =
    "llvm_named_struct_type"
external struct_set_body : lltype -> lltype array -> bool -> unit =
    "llvm_struct_set_body"
external struct_element_types : lltype -> lltype array
                              = "llvm_struct_element_types"
external is_packed : lltype -> bool = "llvm_is_packed"
external is_opaque : lltype -> bool = "llvm_is_opaque"
external is_literal : lltype -> bool = "llvm_is_literal"

(*--... Operations on pointer, vector, and array types .....................--*)

external subtypes : lltype -> lltype array = "llvm_subtypes"
external array_type : lltype -> int -> lltype = "llvm_array_type"
external pointer_type : lltype -> lltype = "llvm_pointer_type"
external qualified_pointer_type : lltype -> int -> lltype
                                = "llvm_qualified_pointer_type"
external vector_type : lltype -> int -> lltype = "llvm_vector_type"

external element_type : lltype -> lltype = "LLVMGetElementType"
external array_length : lltype -> int = "llvm_array_length"
external address_space : lltype -> int = "llvm_address_space"
external vector_size : lltype -> int = "llvm_vector_size"

(*--... Operations on other types ..........................................--*)
external void_type : llcontext -> lltype = "llvm_void_type"
external label_type : llcontext -> lltype = "llvm_label_type"
external x86_mmx_type : llcontext -> lltype = "llvm_x86_mmx_type"
external type_by_name : llmodule -> string -> lltype option = "llvm_type_by_name"

external classify_value : llvalue -> ValueKind.t = "llvm_classify_value"
(*===-- Values ------------------------------------------------------------===*)
external type_of : llvalue -> lltype = "llvm_type_of"
external value_name : llvalue -> string = "llvm_value_name"
external set_value_name : string -> llvalue -> unit = "llvm_set_value_name"
external dump_value : llvalue -> unit = "llvm_dump_value"
external string_of_llvalue : llvalue -> string = "llvm_string_of_llvalue"
external replace_all_uses_with : llvalue -> llvalue -> unit
                               = "llvm_replace_all_uses_with"

(*--... Operations on uses .................................................--*)
external use_begin : llvalue -> lluse option = "llvm_use_begin"
external use_succ : lluse -> lluse option = "llvm_use_succ"
external user : lluse -> llvalue = "llvm_user"
external used_value : lluse -> llvalue = "llvm_used_value"

let iter_uses f v =
  let rec aux = function
    | None -> ()
    | Some u ->
        f u;
        aux (use_succ u)
  in
  aux (use_begin v)

let fold_left_uses f init v =
  let rec aux init u =
    match u with
    | None -> init
    | Some u -> aux (f init u) (use_succ u)
  in
  aux init (use_begin v)

let fold_right_uses f v init =
  let rec aux u init =
    match u with
    | None -> init
    | Some u -> f u (aux (use_succ u) init)
  in
  aux (use_begin v) init


(*--... Operations on users ................................................--*)
external operand : llvalue -> int -> llvalue = "llvm_operand"
external operand_use : llvalue -> int -> lluse = "llvm_operand_use"
external set_operand : llvalue -> int -> llvalue -> unit = "llvm_set_operand"
external num_operands : llvalue -> int = "llvm_num_operands"
external indices : llvalue -> int array = "llvm_indices"

(*--... Operations on constants of (mostly) any type .......................--*)
external is_constant : llvalue -> bool = "llvm_is_constant"
external const_null : lltype -> llvalue = "LLVMConstNull"
external const_all_ones : (*int|vec*)lltype -> llvalue = "LLVMConstAllOnes"
external const_pointer_null : lltype -> llvalue = "LLVMConstPointerNull"
external undef : lltype -> llvalue = "LLVMGetUndef"
external is_null : llvalue -> bool = "llvm_is_null"
external is_undef : llvalue -> bool = "llvm_is_undef"
external constexpr_opcode : llvalue -> Opcode.t = "llvm_constexpr_get_opcode"

(*--... Operations on instructions .........................................--*)
external has_metadata : llvalue -> bool = "llvm_has_metadata"
external metadata : llvalue -> llmdkind -> llvalue option = "llvm_metadata"
external set_metadata : llvalue -> llmdkind -> llvalue -> unit = "llvm_set_metadata"
external clear_metadata : llvalue -> llmdkind -> unit = "llvm_clear_metadata"

(*--... Operations on metadata .......,.....................................--*)
external mdstring : llcontext -> string -> llvalue = "llvm_mdstring"
external mdnode : llcontext -> llvalue array -> llvalue = "llvm_mdnode"
external mdnull : llcontext -> llvalue = "llvm_mdnull"
external get_mdstring : llvalue -> string option = "llvm_get_mdstring"
external get_mdnode_operands : llvalue -> llvalue array
                            = "llvm_get_mdnode_operands"
external get_named_metadata : llmodule -> string -> llvalue array
                            = "llvm_get_namedmd"
external add_named_metadata_operand : llmodule -> string -> llvalue -> unit
                                    = "llvm_append_namedmd"

(*--... Operations on scalar constants .....................................--*)
external const_int : lltype -> int -> llvalue = "llvm_const_int"
external const_of_int64 : lltype -> Int64.t -> bool -> llvalue
                        = "llvm_const_of_int64"
external int64_of_const : llvalue -> Int64.t option
                        = "llvm_int64_of_const"
external const_int_of_string : lltype -> string -> int -> llvalue
                             = "llvm_const_int_of_string"
external const_float : lltype -> float -> llvalue = "llvm_const_float"
external float_of_const : llvalue -> float option
                        = "llvm_float_of_const"
external const_float_of_string : lltype -> string -> llvalue
                               = "llvm_const_float_of_string"

(*--... Operations on composite constants ..................................--*)
external const_string : llcontext -> string -> llvalue = "llvm_const_string"
external const_stringz : llcontext -> string -> llvalue = "llvm_const_stringz"
external const_array : lltype -> llvalue array -> llvalue = "llvm_const_array"
external const_struct : llcontext -> llvalue array -> llvalue
                      = "llvm_const_struct"
external const_named_struct : lltype -> llvalue array -> llvalue
                      = "llvm_const_named_struct"
external const_packed_struct : llcontext -> llvalue array -> llvalue
                             = "llvm_const_packed_struct"
external const_vector : llvalue array -> llvalue = "llvm_const_vector"
external string_of_const : llvalue -> string option = "llvm_string_of_const"
external const_element : llvalue -> int -> llvalue = "llvm_const_element"

(*--... Constant expressions ...............................................--*)
external align_of : lltype -> llvalue = "LLVMAlignOf"
external size_of : lltype -> llvalue = "LLVMSizeOf"
external const_neg : llvalue -> llvalue = "LLVMConstNeg"
external const_nsw_neg : llvalue -> llvalue = "LLVMConstNSWNeg"
external const_nuw_neg : llvalue -> llvalue = "LLVMConstNUWNeg"
external const_fneg : llvalue -> llvalue = "LLVMConstFNeg"
external const_not : llvalue -> llvalue = "LLVMConstNot"
external const_add : llvalue -> llvalue -> llvalue = "LLVMConstAdd"
external const_nsw_add : llvalue -> llvalue -> llvalue = "LLVMConstNSWAdd"
external const_nuw_add : llvalue -> llvalue -> llvalue = "LLVMConstNUWAdd"
external const_fadd : llvalue -> llvalue -> llvalue = "LLVMConstFAdd"
external const_sub : llvalue -> llvalue -> llvalue = "LLVMConstSub"
external const_nsw_sub : llvalue -> llvalue -> llvalue = "LLVMConstNSWSub"
external const_nuw_sub : llvalue -> llvalue -> llvalue = "LLVMConstNUWSub"
external const_fsub : llvalue -> llvalue -> llvalue = "LLVMConstFSub"
external const_mul : llvalue -> llvalue -> llvalue = "LLVMConstMul"
external const_nsw_mul : llvalue -> llvalue -> llvalue = "LLVMConstNSWMul"
external const_nuw_mul : llvalue -> llvalue -> llvalue = "LLVMConstNUWMul"
external const_fmul : llvalue -> llvalue -> llvalue = "LLVMConstFMul"
external const_udiv : llvalue -> llvalue -> llvalue = "LLVMConstUDiv"
external const_sdiv : llvalue -> llvalue -> llvalue = "LLVMConstSDiv"
external const_exact_sdiv : llvalue -> llvalue -> llvalue = "LLVMConstExactSDiv"
external const_fdiv : llvalue -> llvalue -> llvalue = "LLVMConstFDiv"
external const_urem : llvalue -> llvalue -> llvalue = "LLVMConstURem"
external const_srem : llvalue -> llvalue -> llvalue = "LLVMConstSRem"
external const_frem : llvalue -> llvalue -> llvalue = "LLVMConstFRem"
external const_and : llvalue -> llvalue -> llvalue = "LLVMConstAnd"
external const_or : llvalue -> llvalue -> llvalue = "LLVMConstOr"
external const_xor : llvalue -> llvalue -> llvalue = "LLVMConstXor"
external const_icmp : Icmp.t -> llvalue -> llvalue -> llvalue
                    = "llvm_const_icmp"
external const_fcmp : Fcmp.t -> llvalue -> llvalue -> llvalue
                    = "llvm_const_fcmp"
external const_shl : llvalue -> llvalue -> llvalue = "LLVMConstShl"
external const_lshr : llvalue -> llvalue -> llvalue = "LLVMConstLShr"
external const_ashr : llvalue -> llvalue -> llvalue = "LLVMConstAShr"
external const_gep : llvalue -> llvalue array -> llvalue = "llvm_const_gep"
external const_in_bounds_gep : llvalue -> llvalue array -> llvalue
                            = "llvm_const_in_bounds_gep"
external const_trunc : llvalue -> lltype -> llvalue = "LLVMConstTrunc"
external const_sext : llvalue -> lltype -> llvalue = "LLVMConstSExt"
external const_zext : llvalue -> lltype -> llvalue = "LLVMConstZExt"
external const_fptrunc : llvalue -> lltype -> llvalue = "LLVMConstFPTrunc"
external const_fpext : llvalue -> lltype -> llvalue = "LLVMConstFPExt"
external const_uitofp : llvalue -> lltype -> llvalue = "LLVMConstUIToFP"
external const_sitofp : llvalue -> lltype -> llvalue = "LLVMConstSIToFP"
external const_fptoui : llvalue -> lltype -> llvalue = "LLVMConstFPToUI"
external const_fptosi : llvalue -> lltype -> llvalue = "LLVMConstFPToSI"
external const_ptrtoint : llvalue -> lltype -> llvalue = "LLVMConstPtrToInt"
external const_inttoptr : llvalue -> lltype -> llvalue = "LLVMConstIntToPtr"
external const_bitcast : llvalue -> lltype -> llvalue = "LLVMConstBitCast"
external const_zext_or_bitcast : llvalue -> lltype -> llvalue
                             = "LLVMConstZExtOrBitCast"
external const_sext_or_bitcast : llvalue -> lltype -> llvalue
                             = "LLVMConstSExtOrBitCast"
external const_trunc_or_bitcast : llvalue -> lltype -> llvalue
                              = "LLVMConstTruncOrBitCast"
external const_pointercast : llvalue -> lltype -> llvalue
                           = "LLVMConstPointerCast"
external const_intcast : llvalue -> lltype -> is_signed:bool -> llvalue
                       = "llvm_const_intcast"
external const_fpcast : llvalue -> lltype -> llvalue = "LLVMConstFPCast"
external const_select : llvalue -> llvalue -> llvalue -> llvalue
                      = "LLVMConstSelect"
external const_extractelement : llvalue -> llvalue -> llvalue
                              = "LLVMConstExtractElement"
external const_insertelement : llvalue -> llvalue -> llvalue -> llvalue
                             = "LLVMConstInsertElement"
external const_shufflevector : llvalue -> llvalue -> llvalue -> llvalue
                             = "LLVMConstShuffleVector"
external const_extractvalue : llvalue -> int array -> llvalue
                            = "llvm_const_extractvalue"
external const_insertvalue : llvalue -> llvalue -> int array -> llvalue
                           = "llvm_const_insertvalue"
external const_inline_asm : lltype -> string -> string -> bool -> bool ->
                            llvalue
                          = "llvm_const_inline_asm"
external block_address : llvalue -> llbasicblock -> llvalue = "LLVMBlockAddress"

(*--... Operations on global variables, functions, and aliases (globals) ...--*)
external global_parent : llvalue -> llmodule = "LLVMGetGlobalParent"
external is_declaration : llvalue -> bool = "llvm_is_declaration"
external linkage : llvalue -> Linkage.t = "llvm_linkage"
external set_linkage : Linkage.t -> llvalue -> unit = "llvm_set_linkage"
external unnamed_addr : llvalue -> bool = "llvm_unnamed_addr"
external set_unnamed_addr : bool -> llvalue -> unit = "llvm_set_unnamed_addr"
external section : llvalue -> string = "llvm_section"
external set_section : string -> llvalue -> unit = "llvm_set_section"
external visibility : llvalue -> Visibility.t = "llvm_visibility"
external set_visibility : Visibility.t -> llvalue -> unit = "llvm_set_visibility"
external dll_storage_class : llvalue -> DLLStorageClass.t = "llvm_dll_storage_class"
external set_dll_storage_class : DLLStorageClass.t -> llvalue -> unit = "llvm_set_dll_storage_class"
external alignment : llvalue -> int = "llvm_alignment"
external set_alignment : int -> llvalue -> unit = "llvm_set_alignment"
external is_global_constant : llvalue -> bool = "llvm_is_global_constant"
external set_global_constant : bool -> llvalue -> unit
                             = "llvm_set_global_constant"

(*--... Operations on global variables .....................................--*)
external declare_global : lltype -> string -> llmodule -> llvalue
                        = "llvm_declare_global"
external declare_qualified_global : lltype -> string -> int -> llmodule ->
                                    llvalue
                                  = "llvm_declare_qualified_global"
external define_global : string -> llvalue -> llmodule -> llvalue
                       = "llvm_define_global"
external define_qualified_global : string -> llvalue -> int -> llmodule ->
                                   llvalue
                                 = "llvm_define_qualified_global"
external lookup_global : string -> llmodule -> llvalue option
                       = "llvm_lookup_global"
external delete_global : llvalue -> unit = "llvm_delete_global"
external global_initializer : llvalue -> llvalue = "LLVMGetInitializer"
external set_initializer : llvalue -> llvalue -> unit = "llvm_set_initializer"
external remove_initializer : llvalue -> unit = "llvm_remove_initializer"
external is_thread_local : llvalue -> bool = "llvm_is_thread_local"
external set_thread_local : bool -> llvalue -> unit = "llvm_set_thread_local"
external thread_local_mode : llvalue -> ThreadLocalMode.t
                           = "llvm_thread_local_mode"
external set_thread_local_mode : ThreadLocalMode.t -> llvalue -> unit
                               = "llvm_set_thread_local_mode"
external is_externally_initialized : llvalue -> bool
                                   = "llvm_is_externally_initialized"
external set_externally_initialized : bool -> llvalue -> unit
                                    = "llvm_set_externally_initialized"
external global_begin : llmodule -> (llmodule, llvalue) llpos
                      = "llvm_global_begin"
external global_succ : llvalue -> (llmodule, llvalue) llpos
                     = "llvm_global_succ"
external global_end : llmodule -> (llmodule, llvalue) llrev_pos
                    = "llvm_global_end"
external global_pred : llvalue -> (llmodule, llvalue) llrev_pos
                     = "llvm_global_pred"

let rec iter_global_range f i e =
  if i = e then () else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid global variable range.")
  | Before bb ->
      f bb;
      iter_global_range f (global_succ bb) e

let iter_globals f m =
  iter_global_range f (global_begin m) (At_end m)

let rec fold_left_global_range f init i e =
  if i = e then init else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid global variable range.")
  | Before bb -> fold_left_global_range f (f init bb) (global_succ bb) e

let fold_left_globals f init m =
  fold_left_global_range f init (global_begin m) (At_end m)

let rec rev_iter_global_range f i e =
  if i = e then () else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid global variable range.")
  | After bb ->
      f bb;
      rev_iter_global_range f (global_pred bb) e

let rev_iter_globals f m =
  rev_iter_global_range f (global_end m) (At_start m)

let rec fold_right_global_range f i e init =
  if i = e then init else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid global variable range.")
  | After bb -> fold_right_global_range f (global_pred bb) e (f bb init)

let fold_right_globals f m init =
  fold_right_global_range f (global_end m) (At_start m) init

(*--... Operations on aliases ..............................................--*)
external add_alias : llmodule -> lltype -> llvalue -> string -> llvalue
                   = "llvm_add_alias"

(*--... Operations on functions ............................................--*)
external declare_function : string -> lltype -> llmodule -> llvalue
                          = "llvm_declare_function"
external define_function : string -> lltype -> llmodule -> llvalue
                         = "llvm_define_function"
external lookup_function : string -> llmodule -> llvalue option
                         = "llvm_lookup_function"
external delete_function : llvalue -> unit = "llvm_delete_function"
external is_intrinsic : llvalue -> bool = "llvm_is_intrinsic"
external function_call_conv : llvalue -> int = "llvm_function_call_conv"
external set_function_call_conv : int -> llvalue -> unit
                                = "llvm_set_function_call_conv"
external gc : llvalue -> string option = "llvm_gc"
external set_gc : string option -> llvalue -> unit = "llvm_set_gc"
external function_begin : llmodule -> (llmodule, llvalue) llpos
                        = "llvm_function_begin"
external function_succ : llvalue -> (llmodule, llvalue) llpos
                       = "llvm_function_succ"
external function_end : llmodule -> (llmodule, llvalue) llrev_pos
                      = "llvm_function_end"
external function_pred : llvalue -> (llmodule, llvalue) llrev_pos
                       = "llvm_function_pred"

let rec iter_function_range f i e =
  if i = e then () else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid function range.")
  | Before fn ->
      f fn;
      iter_function_range f (function_succ fn) e

let iter_functions f m =
  iter_function_range f (function_begin m) (At_end m)

let rec fold_left_function_range f init i e =
  if i = e then init else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid function range.")
  | Before fn -> fold_left_function_range f (f init fn) (function_succ fn) e

let fold_left_functions f init m =
  fold_left_function_range f init (function_begin m) (At_end m)

let rec rev_iter_function_range f i e =
  if i = e then () else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid function range.")
  | After fn ->
      f fn;
      rev_iter_function_range f (function_pred fn) e

let rev_iter_functions f m =
  rev_iter_function_range f (function_end m) (At_start m)

let rec fold_right_function_range f i e init =
  if i = e then init else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid function range.")
  | After fn -> fold_right_function_range f (function_pred fn) e (f fn init)

let fold_right_functions f m init =
  fold_right_function_range f (function_end m) (At_start m) init

external llvm_add_function_attr : llvalue -> llattribute -> int -> unit
                                = "llvm_add_function_attr"
external llvm_function_attrs : llvalue -> int -> llattribute array
                             = "llvm_function_attrs"
external llvm_remove_enum_function_attr : llvalue -> llattrkind -> int -> unit
                                        = "llvm_remove_enum_function_attr"
external llvm_remove_string_function_attr : llvalue -> string -> int -> unit
                                          = "llvm_remove_string_function_attr"

let add_function_attr f a i =
  llvm_add_function_attr f a (AttrIndex.to_int i)
let function_attrs f i =
  llvm_function_attrs f (AttrIndex.to_int i)
let remove_enum_function_attr f k i =
  llvm_remove_enum_function_attr f k (AttrIndex.to_int i)
let remove_string_function_attr f k i =
  llvm_remove_string_function_attr f k (AttrIndex.to_int i)

(*--... Operations on params ...............................................--*)
external params : llvalue -> llvalue array = "llvm_params"
external param : llvalue -> int -> llvalue = "llvm_param"
external param_parent : llvalue -> llvalue = "LLVMGetParamParent"
external param_begin : llvalue -> (llvalue, llvalue) llpos = "llvm_param_begin"
external param_succ : llvalue -> (llvalue, llvalue) llpos = "llvm_param_succ"
external param_end : llvalue -> (llvalue, llvalue) llrev_pos = "llvm_param_end"
external param_pred : llvalue -> (llvalue, llvalue) llrev_pos ="llvm_param_pred"

let rec iter_param_range f i e =
  if i = e then () else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid parameter range.")
  | Before p ->
      f p;
      iter_param_range f (param_succ p) e

let iter_params f fn =
  iter_param_range f (param_begin fn) (At_end fn)

let rec fold_left_param_range f init i e =
  if i = e then init else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid parameter range.")
  | Before p -> fold_left_param_range f (f init p) (param_succ p) e

let fold_left_params f init fn =
  fold_left_param_range f init (param_begin fn) (At_end fn)

let rec rev_iter_param_range f i e =
  if i = e then () else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid parameter range.")
  | After p ->
      f p;
      rev_iter_param_range f (param_pred p) e

let rev_iter_params f fn =
  rev_iter_param_range f (param_end fn) (At_start fn)

let rec fold_right_param_range f init i e =
  if i = e then init else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid parameter range.")
  | After p -> fold_right_param_range f (f p init) (param_pred p) e

let fold_right_params f fn init =
  fold_right_param_range f init (param_end fn) (At_start fn)

(*--... Operations on basic blocks .........................................--*)
external value_of_block : llbasicblock -> llvalue = "LLVMBasicBlockAsValue"
external value_is_block : llvalue -> bool = "llvm_value_is_block"
external block_of_value : llvalue -> llbasicblock = "LLVMValueAsBasicBlock"
external block_parent : llbasicblock -> llvalue = "LLVMGetBasicBlockParent"
external basic_blocks : llvalue -> llbasicblock array = "llvm_basic_blocks"
external entry_block : llvalue -> llbasicblock = "LLVMGetEntryBasicBlock"
external delete_block : llbasicblock -> unit = "llvm_delete_block"
external remove_block : llbasicblock -> unit = "llvm_remove_block"
external move_block_before : llbasicblock -> llbasicblock -> unit
                           = "llvm_move_block_before"
external move_block_after : llbasicblock -> llbasicblock -> unit
                          = "llvm_move_block_after"
external append_block : llcontext -> string -> llvalue -> llbasicblock
                      = "llvm_append_block"
external insert_block : llcontext -> string -> llbasicblock -> llbasicblock
                      = "llvm_insert_block"
external block_begin : llvalue -> (llvalue, llbasicblock) llpos
                     = "llvm_block_begin"
external block_succ : llbasicblock -> (llvalue, llbasicblock) llpos
                    = "llvm_block_succ"
external block_end : llvalue -> (llvalue, llbasicblock) llrev_pos
                   = "llvm_block_end"
external block_pred : llbasicblock -> (llvalue, llbasicblock) llrev_pos
                    = "llvm_block_pred"
external block_terminator : llbasicblock -> llvalue option =
    "llvm_block_terminator"

let rec iter_block_range f i e =
  if i = e then () else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid block range.")
  | Before bb ->
      f bb;
      iter_block_range f (block_succ bb) e

let iter_blocks f fn =
  iter_block_range f (block_begin fn) (At_end fn)

let rec fold_left_block_range f init i e =
  if i = e then init else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid block range.")
  | Before bb -> fold_left_block_range f (f init bb) (block_succ bb) e

let fold_left_blocks f init fn =
  fold_left_block_range f init (block_begin fn) (At_end fn)

let rec rev_iter_block_range f i e =
  if i = e then () else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid block range.")
  | After bb ->
      f bb;
      rev_iter_block_range f (block_pred bb) e

let rev_iter_blocks f fn =
  rev_iter_block_range f (block_end fn) (At_start fn)

let rec fold_right_block_range f init i e =
  if i = e then init else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid block range.")
  | After bb -> fold_right_block_range f (f bb init) (block_pred bb) e

let fold_right_blocks f fn init =
  fold_right_block_range f init (block_end fn) (At_start fn)

(*--... Operations on instructions .........................................--*)
external instr_parent : llvalue -> llbasicblock = "LLVMGetInstructionParent"
external instr_begin : llbasicblock -> (llbasicblock, llvalue) llpos
                     = "llvm_instr_begin"
external instr_succ : llvalue -> (llbasicblock, llvalue) llpos
                     = "llvm_instr_succ"
external instr_end : llbasicblock -> (llbasicblock, llvalue) llrev_pos
                     = "llvm_instr_end"
external instr_pred : llvalue -> (llbasicblock, llvalue) llrev_pos
                     = "llvm_instr_pred"

external instr_opcode : llvalue -> Opcode.t = "llvm_instr_get_opcode"
external icmp_predicate : llvalue -> Icmp.t option = "llvm_instr_icmp_predicate"
external fcmp_predicate : llvalue -> Fcmp.t option = "llvm_instr_fcmp_predicate"
external instr_clone : llvalue -> llvalue = "llvm_instr_clone"

let rec iter_instrs_range f i e =
  if i = e then () else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid instruction range.")
  | Before i ->
      f i;
      iter_instrs_range f (instr_succ i) e

let iter_instrs f bb =
  iter_instrs_range f (instr_begin bb) (At_end bb)

let rec fold_left_instrs_range f init i e =
  if i = e then init else
  match i with
  | At_end _ -> raise (Invalid_argument "Invalid instruction range.")
  | Before i -> fold_left_instrs_range f (f init i) (instr_succ i) e

let fold_left_instrs f init bb =
  fold_left_instrs_range f init (instr_begin bb) (At_end bb)

let rec rev_iter_instrs_range f i e =
  if i = e then () else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid instruction range.")
  | After i ->
      f i;
      rev_iter_instrs_range f (instr_pred i) e

let rev_iter_instrs f bb =
  rev_iter_instrs_range f (instr_end bb) (At_start bb)

let rec fold_right_instr_range f i e init =
  if i = e then init else
  match i with
  | At_start _ -> raise (Invalid_argument "Invalid instruction range.")
  | After i -> fold_right_instr_range f (instr_pred i) e (f i init)

let fold_right_instrs f bb init =
  fold_right_instr_range f (instr_end bb) (At_start bb) init


(*--... Operations on call sites ...........................................--*)
external instruction_call_conv: llvalue -> int
                              = "llvm_instruction_call_conv"
external set_instruction_call_conv: int -> llvalue -> unit
                                  = "llvm_set_instruction_call_conv"

external llvm_add_call_site_attr : llvalue -> llattribute -> int -> unit
                                = "llvm_add_call_site_attr"
external llvm_call_site_attrs : llvalue -> int -> llattribute array
                             = "llvm_call_site_attrs"
external llvm_remove_enum_call_site_attr : llvalue -> llattrkind -> int -> unit
                                        = "llvm_remove_enum_call_site_attr"
external llvm_remove_string_call_site_attr : llvalue -> string -> int -> unit
                                          = "llvm_remove_string_call_site_attr"

let add_call_site_attr f a i =
  llvm_add_call_site_attr f a (AttrIndex.to_int i)
let call_site_attrs f i =
  llvm_call_site_attrs f (AttrIndex.to_int i)
let remove_enum_call_site_attr f k i =
  llvm_remove_enum_call_site_attr f k (AttrIndex.to_int i)
let remove_string_call_site_attr f k i =
  llvm_remove_string_call_site_attr f k (AttrIndex.to_int i)

(*--... Operations on call and invoke instructions (only) ..................--*)
external num_arg_operands : llvalue -> int = "llvm_num_arg_operands"
external is_tail_call : llvalue -> bool = "llvm_is_tail_call"
external set_tail_call : bool -> llvalue -> unit = "llvm_set_tail_call"
external get_normal_dest : llvalue -> llbasicblock = "LLVMGetNormalDest"
external get_unwind_dest : llvalue -> llbasicblock = "LLVMGetUnwindDest"

(*--... Operations on load/store instructions (only) .......................--*)
external is_volatile : llvalue -> bool = "llvm_is_volatile"
external set_volatile : bool -> llvalue -> unit = "llvm_set_volatile"

(*--... Operations on terminators ..........................................--*)

let is_terminator llv =
  let open ValueKind in
  let open Opcode in
  match classify_value llv with
    | Instruction (Br | IndirectBr | Invoke | Resume | Ret | Switch | Unreachable)
      -> true
    | _ -> false

external successor : llvalue -> int -> llbasicblock = "llvm_successor"
external set_successor : llvalue -> int -> llbasicblock -> unit
                       = "llvm_set_successor"
external num_successors : llvalue -> int = "llvm_num_successors"

let successors llv =
  if not (is_terminator llv) then
    raise (Invalid_argument "Llvm.successors can only be used on terminators")
  else
    Array.init (num_successors llv) (successor llv)

let iter_successors f llv =
  if not (is_terminator llv) then
    raise (Invalid_argument "Llvm.iter_successors can only be used on terminators")
  else
    for i = 0 to num_successors llv - 1 do
      f (successor llv i)
    done

let fold_successors f llv z =
  if not (is_terminator llv) then
    raise (Invalid_argument "Llvm.fold_successors can only be used on terminators")
  else
    let n = num_successors llv in
    let rec aux i acc =
      if i >= n then acc
      else begin
        let llb = successor llv i in
        aux (i+1) (f llb acc)
      end
    in aux 0 z


(*--... Operations on branches .............................................--*)
external condition : llvalue -> llvalue = "llvm_condition"
external set_condition : llvalue -> llvalue -> unit
                       = "llvm_set_condition"
external is_conditional : llvalue -> bool = "llvm_is_conditional"

let get_branch llv =
  if classify_value llv <> ValueKind.Instruction Opcode.Br then
    None
  else if is_conditional llv then
    Some (`Conditional (condition llv, successor llv 0, successor llv 1))
  else
    Some (`Unconditional (successor llv 0))

(*--... Operations on phi nodes ............................................--*)
external add_incoming : (llvalue * llbasicblock) -> llvalue -> unit
                      = "llvm_add_incoming"
external incoming : llvalue -> (llvalue * llbasicblock) list = "llvm_incoming"

external delete_instruction : llvalue -> unit = "llvm_delete_instruction"

(*===-- Instruction builders ----------------------------------------------===*)
external builder : llcontext -> llbuilder = "llvm_builder"
external position_builder : (llbasicblock, llvalue) llpos -> llbuilder -> unit
                          = "llvm_position_builder"
external insertion_block : llbuilder -> llbasicblock = "llvm_insertion_block"
external insert_into_builder : llvalue -> string -> llbuilder -> unit
                             = "llvm_insert_into_builder"

let builder_at context ip =
  let b = builder context in
  position_builder ip b;
  b

let builder_before context i = builder_at context (Before i)
let builder_at_end context bb = builder_at context (At_end bb)

let position_before i = position_builder (Before i)
let position_at_end bb = position_builder (At_end bb)


(*--... Metadata ...........................................................--*)
external set_current_debug_location : llbuilder -> llvalue -> unit
                                    = "llvm_set_current_debug_location"
external clear_current_debug_location : llbuilder -> unit
                                      = "llvm_clear_current_debug_location"
external current_debug_location : llbuilder -> llvalue option
                                    = "llvm_current_debug_location"
external set_inst_debug_location : llbuilder -> llvalue -> unit
                                 = "llvm_set_inst_debug_location"


(*--... Terminators ........................................................--*)
external build_ret_void : llbuilder -> llvalue = "llvm_build_ret_void"
external build_ret : llvalue -> llbuilder -> llvalue = "llvm_build_ret"
external build_aggregate_ret : llvalue array -> llbuilder -> llvalue
                             = "llvm_build_aggregate_ret"
external build_br : llbasicblock -> llbuilder -> llvalue = "llvm_build_br"
external build_cond_br : llvalue -> llbasicblock -> llbasicblock -> llbuilder ->
                         llvalue = "llvm_build_cond_br"
external build_switch : llvalue -> llbasicblock -> int -> llbuilder -> llvalue
                      = "llvm_build_switch"
external build_malloc : lltype -> string -> llbuilder -> llvalue =
    "llvm_build_malloc"
external build_array_malloc : lltype -> llvalue -> string -> llbuilder ->
    llvalue = "llvm_build_array_malloc"
external build_free : llvalue -> llbuilder -> llvalue = "llvm_build_free"
external add_case : llvalue -> llvalue -> llbasicblock -> unit
                  = "llvm_add_case"
external switch_default_dest : llvalue -> llbasicblock =
    "LLVMGetSwitchDefaultDest"
external build_indirect_br : llvalue -> int -> llbuilder -> llvalue
                           = "llvm_build_indirect_br"
external add_destination : llvalue -> llbasicblock -> unit
                         = "llvm_add_destination"
external build_invoke : llvalue -> llvalue array -> llbasicblock ->
                        llbasicblock -> string -> llbuilder -> llvalue
                      = "llvm_build_invoke_bc" "llvm_build_invoke_nat"
external build_landingpad : lltype -> llvalue -> int -> string -> llbuilder ->
                            llvalue = "llvm_build_landingpad"
external is_cleanup : llvalue -> bool = "llvm_is_cleanup"
external set_cleanup : llvalue -> bool -> unit = "llvm_set_cleanup"
external add_clause : llvalue -> llvalue -> unit = "llvm_add_clause"
external build_resume : llvalue -> llbuilder -> llvalue = "llvm_build_resume"
external build_unreachable : llbuilder -> llvalue = "llvm_build_unreachable"

(*--... Arithmetic .........................................................--*)
external build_add : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_add"
external build_nsw_add : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nsw_add"
external build_nuw_add : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nuw_add"
external build_fadd : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_fadd"
external build_sub : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_sub"
external build_nsw_sub : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nsw_sub"
external build_nuw_sub : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nuw_sub"
external build_fsub : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_fsub"
external build_mul : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_mul"
external build_nsw_mul : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nsw_mul"
external build_nuw_mul : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nuw_mul"
external build_fmul : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_fmul"
external build_udiv : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_udiv"
external build_sdiv : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_sdiv"
external build_exact_sdiv : llvalue -> llvalue -> string -> llbuilder -> llvalue
                          = "llvm_build_exact_sdiv"
external build_fdiv : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_fdiv"
external build_urem : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_urem"
external build_srem : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_srem"
external build_frem : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_frem"
external build_shl : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_shl"
external build_lshr : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_lshr"
external build_ashr : llvalue -> llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_ashr"
external build_and : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_and"
external build_or : llvalue -> llvalue -> string -> llbuilder -> llvalue
                  = "llvm_build_or"
external build_xor : llvalue -> llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_xor"
external build_neg : llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_neg"
external build_nsw_neg : llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nsw_neg"
external build_nuw_neg : llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_nuw_neg"
external build_fneg : llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_fneg"
external build_not : llvalue -> string -> llbuilder -> llvalue
                   = "llvm_build_not"

(*--... Memory .............................................................--*)
external build_alloca : lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_alloca"
external build_array_alloca : lltype -> llvalue -> string -> llbuilder ->
                              llvalue = "llvm_build_array_alloca"
external build_load : llvalue -> string -> llbuilder -> llvalue
                    = "llvm_build_load"
external build_store : llvalue -> llvalue -> llbuilder -> llvalue
                     = "llvm_build_store"
external build_atomicrmw : AtomicRMWBinOp.t -> llvalue -> llvalue ->
                           AtomicOrdering.t -> bool -> string -> llbuilder ->
                           llvalue
                         = "llvm_build_atomicrmw_bytecode"
                           "llvm_build_atomicrmw_native"
external build_gep : llvalue -> llvalue array -> string -> llbuilder -> llvalue
                   = "llvm_build_gep"
external build_in_bounds_gep : llvalue -> llvalue array -> string ->
                             llbuilder -> llvalue = "llvm_build_in_bounds_gep"
external build_struct_gep : llvalue -> int -> string -> llbuilder -> llvalue
                         = "llvm_build_struct_gep"

external build_global_string : string -> string -> llbuilder -> llvalue
                             = "llvm_build_global_string"
external build_global_stringptr  : string -> string -> llbuilder -> llvalue
                                 = "llvm_build_global_stringptr"

(*--... Casts ..............................................................--*)
external build_trunc : llvalue -> lltype -> string -> llbuilder -> llvalue
                     = "llvm_build_trunc"
external build_zext : llvalue -> lltype -> string -> llbuilder -> llvalue
                    = "llvm_build_zext"
external build_sext : llvalue -> lltype -> string -> llbuilder -> llvalue
                    = "llvm_build_sext"
external build_fptoui : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_fptoui"
external build_fptosi : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_fptosi"
external build_uitofp : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_uitofp"
external build_sitofp : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_sitofp"
external build_fptrunc : llvalue -> lltype -> string -> llbuilder -> llvalue
                       = "llvm_build_fptrunc"
external build_fpext : llvalue -> lltype -> string -> llbuilder -> llvalue
                     = "llvm_build_fpext"
external build_ptrtoint : llvalue -> lltype -> string -> llbuilder -> llvalue
                        = "llvm_build_prttoint"
external build_inttoptr : llvalue -> lltype -> string -> llbuilder -> llvalue
                        = "llvm_build_inttoptr"
external build_bitcast : llvalue -> lltype -> string -> llbuilder -> llvalue
                       = "llvm_build_bitcast"
external build_zext_or_bitcast : llvalue -> lltype -> string -> llbuilder ->
                                 llvalue = "llvm_build_zext_or_bitcast"
external build_sext_or_bitcast : llvalue -> lltype -> string -> llbuilder ->
                                 llvalue = "llvm_build_sext_or_bitcast"
external build_trunc_or_bitcast : llvalue -> lltype -> string -> llbuilder ->
                                  llvalue = "llvm_build_trunc_or_bitcast"
external build_pointercast : llvalue -> lltype -> string -> llbuilder -> llvalue
                           = "llvm_build_pointercast"
external build_intcast : llvalue -> lltype -> string -> llbuilder -> llvalue
                       = "llvm_build_intcast"
external build_fpcast : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_fpcast"

(*--... Comparisons ........................................................--*)
external build_icmp : Icmp.t -> llvalue -> llvalue -> string ->
                      llbuilder -> llvalue = "llvm_build_icmp"
external build_fcmp : Fcmp.t -> llvalue -> llvalue -> string ->
                      llbuilder -> llvalue = "llvm_build_fcmp"

(*--... Miscellaneous instructions .........................................--*)
external build_phi : (llvalue * llbasicblock) list -> string -> llbuilder ->
                     llvalue = "llvm_build_phi"
external build_empty_phi : lltype -> string -> llbuilder -> llvalue
                         = "llvm_build_empty_phi"
external build_call : llvalue -> llvalue array -> string -> llbuilder -> llvalue
                    = "llvm_build_call"
external build_select : llvalue -> llvalue -> llvalue -> string -> llbuilder ->
                        llvalue = "llvm_build_select"
external build_va_arg : llvalue -> lltype -> string -> llbuilder -> llvalue
                      = "llvm_build_va_arg"
external build_extractelement : llvalue -> llvalue -> string -> llbuilder ->
                                llvalue = "llvm_build_extractelement"
external build_insertelement : llvalue -> llvalue -> llvalue -> string ->
                               llbuilder -> llvalue = "llvm_build_insertelement"
external build_shufflevector : llvalue -> llvalue -> llvalue -> string ->
                               llbuilder -> llvalue = "llvm_build_shufflevector"
external build_extractvalue : llvalue -> int -> string -> llbuilder -> llvalue
                            = "llvm_build_extractvalue"
external build_insertvalue : llvalue -> llvalue -> int -> string -> llbuilder ->
                             llvalue = "llvm_build_insertvalue"

external build_is_null : llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_is_null"
external build_is_not_null : llvalue -> string -> llbuilder -> llvalue
                           = "llvm_build_is_not_null"
external build_ptrdiff : llvalue -> llvalue -> string -> llbuilder -> llvalue
                       = "llvm_build_ptrdiff"


(*===-- Memory buffers ----------------------------------------------------===*)

module MemoryBuffer = struct
  external of_file : string -> llmemorybuffer = "llvm_memorybuffer_of_file"
  external of_stdin : unit -> llmemorybuffer = "llvm_memorybuffer_of_stdin"
  external of_string : ?name:string -> string -> llmemorybuffer
                     = "llvm_memorybuffer_of_string"
  external as_string : llmemorybuffer -> string = "llvm_memorybuffer_as_string"
  external dispose : llmemorybuffer -> unit = "llvm_memorybuffer_dispose"
end


(*===-- Pass Manager ------------------------------------------------------===*)

module PassManager = struct
  type 'a t
  type any = [ `Module | `Function ]
  external create : unit -> [ `Module ] t = "llvm_passmanager_create"
  external create_function : llmodule -> [ `Function ] t
                           = "LLVMCreateFunctionPassManager"
  external run_module : llmodule -> [ `Module ] t -> bool
                      = "llvm_passmanager_run_module"
  external initialize : [ `Function ] t -> bool = "llvm_passmanager_initialize"
  external run_function : llvalue -> [ `Function ] t -> bool
                        = "llvm_passmanager_run_function"
  external finalize : [ `Function ] t -> bool = "llvm_passmanager_finalize"
  external dispose : [< any ] t -> unit = "llvm_passmanager_dispose"
end



================================================
FILE: src/bindings/ocaml/llvm/llvm.mli
================================================
(*===-- llvm/llvm.mli - LLVM OCaml Interface ------------------------------===*
 *
 *                     The LLVM Compiler Infrastructure
 *
 * This file is distributed under the University of Illinois Open Source
 * License. See LICENSE.TXT for details.
 *
 *===----------------------------------------------------------------------===*)

(** Core API.

    This interface provides an OCaml API for the LLVM intermediate
    representation, the classes in the VMCore library. *)


(** {6 Abstract types}

    These abstract types correlate directly to the LLVMCore classes. *)

(** The top-level container for all LLVM global data. See the
    [llvm::LLVMContext] class. *)
type llcontext

(** The top-level container for all other LLVM Intermediate Representation (IR)
    objects. See the [llvm::Module] class. *)
type llmodule

(** Each value in the LLVM IR has a type, an instance of [lltype]. See the
    [llvm::Type] class. *)
type lltype

(** Any value in the LLVM IR. Functions, instructions, global variables,
    constants, and much more are all [llvalues]. See the [llvm::Value] class.
    This type covers a wide range of subclasses. *)
type llvalue

(** Used to store users and usees of values. See the [llvm::Use] class. *)
type lluse

(** A basic block in LLVM IR. See the [llvm::BasicBlock] class. *)
type llbasicblock

(** Used to generate instructions in the LLVM IR. See the [llvm::LLVMBuilder]
    class. *)
type llbuilder

(** Used to represent attribute kinds. *)
type llattrkind

(** An attribute in LLVM IR. See the [llvm::Attribute] class. *)
type llattribute

(** Used to efficiently handle large buffers of read-only binary data.
    See the [llvm::MemoryBuffer] class. *)
type llmemorybuffer

(** The kind id of metadata attached to an instruction. *)
type llmdkind

(** The kind of an [lltype], the result of [classify_type ty]. See the
    [llvm::Type::TypeID] enumeration. *)
module TypeKind : sig
  type t =
    Void
  | Half
  | Float
  | Double
  | X86fp80
  | Fp128
  | Ppc_fp128
  | Label
  | Integer
  | Function
  | Struct
  | Array
  | Pointer
  | Vector
  | Metadata
  | X86_mmx
  | Token
end

(** The linkage of a global value, accessed with {!linkage} and
    {!set_linkage}. See [llvm::GlobalValue::LinkageTypes]. *)
module Linkage : sig
  type t =
    External
  | Available_externally
  | Link_once
  | Link_once_odr
  | Link_once_odr_auto_hide
  | Weak
  | Weak_odr
  | Appending
  | Internal
  | Private
  | Dllimport
  | Dllexport
  | External_weak
  | Ghost
  | Common
  | Linker_private
  | Linker_private_weak
end

(** The linker visibility of a global value, accessed with {!visibility} and
    {!set_visibility}. See [llvm::GlobalValue::VisibilityTypes]. *)
module Visibility : sig
  type t =
    Default
  | Hidden
  | Protected
end

(** The DLL storage class of a global value, accessed with {!dll_storage_class} and
    {!set_dll_storage_class}. See [llvm::GlobalValue::DLLStorageClassTypes]. *)
module DLLStorageClass : sig
  type t =
  | Default
  | DLLImport
  | DLLExport
end

(** The following calling convention values may be accessed with
    {!function_call_conv} and {!set_function_call_conv}. Calling
    conventions are open-ended. *)
module CallConv : sig
  val c : int             (** [c] is the C calling convention. *)
  val fast : int          (** [fast] is the calling convention to allow LLVM
                              maximum optimization opportunities. Use only with
                              internal linkage. *)
  val cold : int          (** [cold] is the calling convention for
                              callee-save. *)
  val x86_stdcall : int   (** [x86_stdcall] is the familiar stdcall calling
                              convention from C. *)
  val x86_fastcall : int  (** [x86_fastcall] is the familiar fastcall calling
                              convention from C. *)
end

(** The logical representation of an attribute. *)
module AttrRepr : sig
  type t =
  | Enum of llattrkind * int64
  | String of string * string
end

(** The position of an attribute. See [LLVMAttributeIndex]. *)
module AttrIndex : sig
  type t =
  | Function
  | Return
  | Param of int
end

(** The predicate for an integer comparison ([icmp]) instruction.
    See the [llvm::ICmpInst::Predicate] enumeration. *)
module Icmp : sig
  type t =
  | Eq  (** Equal *)
  | Ne  (** Not equal *)
  | Ugt (** Unsigned greater than *)
  | Uge (** Unsigned greater or equal *)
  | Ult (** Unsigned less than *)
  | Ule (** Unsigned less or equal *)
  | Sgt (** Signed greater than *)
  | Sge (** Signed greater or equal *)
  | Slt (** Signed less than *)
  | Sle (** Signed less or equal *)
end

(** The predicate for a floating-point comparison ([fcmp]) instruction.
    Ordered means that neither operand is a QNAN while unordered means
    that either operand may be a QNAN.
    See the [llvm::FCmpInst::Predicate] enumeration. *)
module Fcmp : sig
  type t =
  | False (** Always false *)
  | Oeq   (** Ordered and equal *)
  | Ogt   (** Ordered and greater than *)
  | Oge   (** Ordered and greater or equal *)
  | Olt   (** Ordered and less than *)
  | Ole   (** Ordered and less or equal *)
  | One   (** Ordered and not equal *)
  | Ord   (** Ordered (no operand is NaN) *)
  | Uno   (** Unordered (one operand at least is NaN) *)
  | Ueq   (** Unordered and equal *)
  | Ugt   (** Unordered and greater than *)
  | Uge   (** Unordered and greater or equal *)
  | Ult   (** Unordered and less than *)
  | Ule   (** Unordered and less or equal *)
  | Une   (** Unordered and not equal *)
  | True  (** Always true *)
end

(** The opcodes for LLVM instructions and constant expressions. *)
module Opcode : sig
  type t =
  | Invalid (** Not an instruction *)

  | Ret (** Terminator Instructions *)
  | Br
  | Switch
  | IndirectBr
  | Invoke
  | Invalid2
  | Unreachable

  | Add (** Standard Binary Operators *)
  | FAdd
  | Sub
  | FSub
  | Mul
  | FMul
  | UDiv
  | SDiv
  | FDiv
  | URem
  | SRem
  | FRem

  | Shl (** Logical Operators *)
  | LShr
  | AShr
  | And
  | Or
  | Xor

  | Alloca (** Memory Operators *)
  | Load
  | Store
  | GetElementPtr

  | Trunc (** Cast Operators *)
  | ZExt
  | SExt
  | FPToUI
  | FPToSI
  | UIToFP
  | SIToFP
  | FPTrunc
  | FPExt
  | PtrToInt
  | IntToPtr
  | BitCast

  | ICmp (** Other Operators *)
  | FCmp
  | PHI
  | Call
  | Select
  | UserOp1
  | UserOp2
  | VAArg
  | ExtractElement
  | InsertElement
  | ShuffleVector
  | ExtractValue
  | InsertValue
  | Fence
  | AtomicCmpXchg
  | AtomicRMW
  | Resume
  | LandingPad
  | AddrSpaceCast
  | CleanupRet
  | CatchRet
  | CatchPad
  | CleanupPad
  | CatchSwitch
end

(** The type of a clause of a [landingpad] instruction.
    See [llvm::LandingPadInst::ClauseType]. *)
module LandingPadClauseTy : sig
  type t =
  | Catch
  | Filter
end

(** The thread local mode of a global value, accessed with {!thread_local_mode}
    and {!set_thread_local_mode}.
    See [llvm::GlobalVariable::ThreadLocalMode]. *)
module ThreadLocalMode : sig
  type t =
  | None
  | GeneralDynamic
  | LocalDynamic
  | InitialExec
  | LocalExec
end

(** The ordering of an atomic [load], [store], [cmpxchg], [atomicrmw] or
    [fence] instruction. See [llvm::AtomicOrdering]. *)
module AtomicOrdering : sig
  type t =
  | NotAtomic
  | Unordered
  | Monotonic
  | Invalid (** removed due to API changes *)
  | Acquire
  | Release
  | AcqiureRelease
  | SequentiallyConsistent
end

(** The opcode of an [atomicrmw] instruction.
    See [llvm::AtomicRMWInst::BinOp]. *)
module AtomicRMWBinOp : sig
  type t =
  | Xchg
  | Add
  | Sub
  | And
  | Nand
  | Or
  | Xor
  | Max
  | Min
  | UMax
  | UMin
end

(** The kind of an [llvalue], the result of [classify_value v].
    See the various [LLVMIsA*] functions. *)
module ValueKind : sig
  type t =
  | NullValue
  | Argument
  | BasicBlock
  | InlineAsm
  | MDNode
  | MDString
  | BlockAddress
  | ConstantAggregateZero
  | ConstantArray
  | ConstantDataArray
  | ConstantDataVector
  | ConstantExpr
  | ConstantFP
  | ConstantInt
  | ConstantPointerNull
  | ConstantStruct
  | ConstantVector
  | Function
  | GlobalAlias
  | GlobalIFunc
  | GlobalVariable
  | UndefValue
  | Instruction of Opcode.t
end

(** The kind of [Diagnostic], the result of [Diagnostic.severity d].
    See [llvm::DiagnosticSeverity]. *)
module DiagnosticSeverity : sig
  type t =
  | Error
  | Warning
  | Remark
  | Note
end


(** {6 Iteration} *)

(** [Before b] and [At_end a] specify positions from the start of the ['b] list
    of [a]. [llpos] is used to specify positions in and for forward iteration
    through the various value lists maintained by the LLVM IR. *)
type ('a, 'b) llpos =
| At_end of 'a
| Before of 'b

(** [After b] and [At_start a] specify positions from the end of the ['b] list
    of [a]. [llrev_pos] is used for reverse iteration through the various value
    lists maintained by the LLVM IR. *)
type ('a, 'b) llrev_pos =
| At_start of 'a
| After of 'b


(** {6 Exceptions} *)

exception FeatureDisabled of string

exception IoError of string


(** {6 Global configuration} *)

(** [enable_pretty_stacktraces ()] enables LLVM's built-in stack trace code.
    This intercepts the OS's crash signals and prints which component of LLVM
    you were in at the time of the crash. *)
val enable_pretty_stacktrace : unit -> unit

(** [install_fatal_error_handler f] installs [f] as LLVM's fatal error handler.
    The handler will receive the reason for termination as a string. After
    the handler has been executed, LLVM calls [exit(1)]. *)
val install_fatal_error_handler : (string -> unit) -> unit

(** [reset_fatal_error_handler ()] resets LLVM's fatal error handler. *)
val reset_fatal_error_handler : unit -> unit

(** [parse_command_line_options ?overview args] parses [args] using
    the LLVM command line parser. Note that the only stable thing about this
    function is its signature; you cannot rely on any particular set of command
    line arguments being interpreted the same way across LLVM versions.

    See the function [llvm::cl::ParseCommandLineOptions()]. *)
val parse_command_line_options : ?overview:string -> string array -> unit

(** {6 Context error handling} *)

module Diagnostic : sig
  type t

  (** [description d] returns a textual description of [d]. *)
  val description : t -> string

  (** [severity d] returns the severity of [d]. *)
  val severity : t -> DiagnosticSeverity.t
end

(** [set_diagnostic_handler c h] set the diagnostic handler of [c] to [h].
    See the method [llvm::LLVMContext::setDiagnosticHandler]. *)
val set_diagnostic_handler : llcontext -> (Diagnostic.t -> unit) option -> unit

(** {6 Contexts} *)

(** [create_context ()] creates a context for storing the "global" state in
    LLVM. See the constructor [llvm::LLVMContext]. *)
val create_context : unit -> llcontext

(** [destroy_context ()] destroys a context. See the destructor
    [llvm::LLVMContext::~LLVMContext]. *)
val dispose_context : llcontext -> unit

(** See the function [LLVMGetGlobalContext]. *)
val global_context : unit -> llcontext

(** [mdkind_id context name] returns the MDKind ID that corresponds to the
    name [name] in the context [context].  See the function
    [llvm::LLVMContext::getMDKindID]. *)
val mdkind_id : llcontext -> string -> llmdkind


(** {6 Attributes} *)

(** [UnknownAttribute attr] is raised when a enum attribute name [name]
    is not recognized by LLVM. *)
exception UnknownAttribute of string

(** [enum_attr_kind name] returns the kind of enum attributes named [name].
    May raise [UnknownAttribute]. *)
val enum_attr_kind : string -> llattrkind

(** [create_enum_attr context value kind] creates an enum attribute
    with the supplied [kind] and [value] in [context]; if the value
    is not required (as for the majority of attributes), use [0L].
    May raise [UnknownAttribute].
    See the constructor [llvm::Attribute::get]. *)
val create_enum_attr : llcontext -> string -> int64 -> llattribute

(** [create_string_attr context kind value] creates a string attribute
    with the supplied [kind] and [value] in [context].
    See the constructor [llvm::Attribute::get]. *)
val create_string_attr : llcontext -> string -> string -> llattribute

(** [attr_of_repr context repr] creates an attribute with the supplied
    representation [repr] in [context]. *)
val attr_of_repr : llcontext -> AttrRepr.t -> llattribute

(** [repr_of_attr attr] describes the representation of attribute [attr]. *)
val repr_of_attr : llattribute -> AttrRepr.t


(** {6 Modules} *)

(** [create_module context id] creates a module with the supplied module ID in
    the context [context].  Modules are not garbage collected; it is mandatory
    to call {!dispose_module} to free memory. See the constructor
    [llvm::Module::Module]. *)
val create_module : llcontext -> string -> llmodule

(** [dispose_module m] destroys a module [m] and all of the IR objects it
    contained. All references to subordinate objects are invalidated;
    referencing them will invoke undefined behavior. See the destructor
    [llvm::Module::~Module]. *)
val dispose_module : llmodule -> unit

(** [target_triple m] is the target specifier for the module [m], something like
    [i686-apple-darwin8]. See the method [llvm::Module::getTargetTriple]. *)
val target_triple: llmodule -> string

(** [target_triple triple m] changes the target specifier for the module [m] to
    the string [triple]. See the method [llvm::Module::setTargetTriple]. *)
val set_target_triple: string -> llmodule -> unit

(** [data_layout m] is the data layout specifier for the module [m], something
    like [e-p:32:32:32-i1:8:8-i8:8:8-i16:16:16-...-a0:0:64-f80:128:128]. See the
    method [llvm::Module::getDataLayout]. *)
val data_layout: llmodule -> string

(** [set_data_layout s m] changes the data layout specifier for the module [m]
    to the string [s]. See the method [llvm::Module::setDataLayout]. *)
val set_data_layout: string -> llmodule -> unit

(** [dump_module m] prints the .ll representation of the module [m] to standard
    error. See the method [llvm::Module::dump]. *)
val dump_module : llmodule -> unit

(** [print_module f m] prints the .ll representation of the module [m]
    to file [f]. See the method [llvm::Module::print]. *)
val print_module : string -> llmodule -> unit

(** [string_of_llmodule m] returns the .ll representation of the module [m]
    as a string. See the method [llvm::Module::print]. *)
val string_of_llmodule : llmodule -> string

(** [set_module_inline_asm m asm] sets the inline assembler for the module. See
    the method [llvm::Module::setModuleInlineAsm]. *)
val set_module_inline_asm : llmodule -> string -> unit

(** [module_context m] returns the context of the specified module.
    See the method [llvm::Module::getContext] *)
val module_context : llmodule -> llcontext


(** {6 Types} *)

(** [classify_type ty] returns the {!TypeKind.t} corresponding to the type [ty].
    See the method [llvm::Type::getTypeID]. *)
val classify_type : lltype -> TypeKind.t

(** [type_is_sized ty] returns whether the type has a size or not.
    If it doesn't then it is not safe to call the [DataLayout::] methods on it.
    *)
val type_is_sized : lltype -> bool

(** [type_context ty] returns the {!llcontext} corresponding to the type [ty].
    See the method [llvm::Type::getContext]. *)
val type_context : lltype -> llcontext

(** [dump_type ty] prints the .ll representation of the type [ty] to standard
    error. See the method [llvm::Type::dump]. *)
val dump_type : lltype -> unit

(** [string_of_lltype ty] returns a string describing the type [ty]. *)
val string_of_lltype : lltype -> string


(** {7 Operations on integer types} *)

(** [i1_type c] returns an integer type of bitwidth 1 in the context [c]. See
    [llvm::Type::Int1Ty]. *)
val i1_type : llcontext -> lltype

(** [i8_type c] returns an integer type of bitwidth 8 in the context [c]. See
    [llvm::Type::Int8Ty]. *)
val i8_type : llcontext -> lltype

(** [i16_type c] returns an integer type of bitwidth 16 in the context [c]. See
    [llvm::Type::Int16Ty]. *)
val i16_type : llcontext -> lltype

(** [i32_type c] returns an integer type of bitwidth 32 in the context [c]. See
    [llvm::Type::Int32Ty]. *)
val i32_type : llcontext -> lltype

(** [i64_type c] returns an integer type of bitwidth 64 in the context [c]. See
    [llvm::Type::Int64Ty]. *)
val i64_type : llcontext -> lltype

(** [integer_type c n] returns an integer type of bitwidth [n] in the context
    [c]. See the method [llvm::IntegerType::get]. *)
val integer_type : llcontext -> int -> lltype

(** [integer_bitwidth c ty] returns the number of bits in the integer type [ty]
    in the context [c].  See the method [llvm::IntegerType::getBitWidth]. *)
val integer_bitwidth : lltype -> int


(** {7 Operations on real types} *)

(** [float_type c] returns the IEEE 32-bit floating point type in the context
    [c]. See [llvm::Type::FloatTy]. *)
val float_type : llcontext -> lltype

(** [double_type c] returns the IEEE 64-bit floating point type in the context
    [c]. See [llvm::Type::DoubleTy]. *)
val double_type : llcontext -> lltype

(** [x86fp80_type c] returns the x87 80-bit floating point type in the context
    [c]. See [llvm::Type::X86_FP80Ty]. *)
val x86fp80_type : llcontext -> lltype

(** [fp128_type c] returns the IEEE 128-bit floating point type in the context
    [c]. See [llvm::Type::FP128Ty]. *)
val fp128_type : llcontext -> lltype

(** [ppc_fp128_type c] returns the PowerPC 128-bit floating point type in the
    context [c]. See [llvm::Type::PPC_FP128Ty]. *)
val ppc_fp128_type : llcontext -> lltype


(** {7 Operations on function types} *)

(** [function_type ret_ty param_tys] returns the function type returning
    [ret_ty] and taking [param_tys] as parameters.
    See the method [llvm::FunctionType::get]. *)
val function_type : lltype -> lltype array -> lltype

(** [var_arg_function_type ret_ty param_tys] is just like
    [function_type ret_ty param_tys] except that it returns the function type
    which also takes a variable number of arguments.
    See the method [llvm::FunctionType::get]. *)
val var_arg_function_type : lltype -> lltype array -> lltype

(** [is_var_arg fty] returns [true] if [fty] is a varargs function type, [false]
    otherwise. See the method [llvm::FunctionType::isVarArg]. *)
val is_var_arg : lltype -> bool

(** [return_type fty] gets the return type of the function type [fty].
    See the method [llvm::FunctionType::getReturnType]. *)
val return_type : lltype -> lltype

(** [param_types fty] gets the parameter types of the function type [fty].
    See the method [llvm::FunctionType::getParamType]. *)
val param_types : lltype -> lltype array


(** {7 Operations on struct types} *)

(** [struct_type context tys] returns the structure type in the context
    [context] containing in the types in the array [tys]. See the method
    [llvm::StructType::get]. *)
val struct_type : llcontext -> lltype array -> lltype

(** [packed_struct_type context ys] returns the packed structure type in the
    context [context] containing in the types in the array [tys]. See the method
    [llvm::StructType::get]. *)
val packed_struct_type : llcontext -> lltype array -> lltype

(** [struct_name ty] returns the name of the named structure type [ty],
    or None if the structure type is not named *)
val struct_name : lltype -> string option

(** [named_struct_type context name] returns the named structure type [name]
    in the context [context].
    See the method [llvm::StructType::get]. *)
val named_struct_type : llcontext -> string -> lltype

(** [struct_set_body ty elts ispacked] sets the body of the named struct [ty]
    to the [elts] elements.
    See the moethd [llvm::StructType::setBody]. *)
val struct_set_body : lltype -> lltype array -> bool -> unit

(** [struct_element_types sty] returns the constituent types of the struct type
    [sty]. See the method [llvm::StructType::getElementType]. *)
val struct_element_types : lltype -> lltype array

(** [is_packed sty] returns [true] if the structure type [sty] is packed,
    [false] otherwise. See the method [llvm::StructType::isPacked]. *)
val is_packed : lltype -> bool

(** [is_opaque sty] returns [true] if the structure type [sty] is opaque.
    [false] otherwise. See the method [llvm::StructType::isOpaque]. *)
val is_opaque : lltype -> bool

(** [is_literal sty] returns [true] if the structure type [sty] is literal.
    [false] otherwise. See the method [llvm::StructType::isLiteral]. *)
val is_literal : lltype -> bool


(** {7 Operations on pointer, vector, and array types} *)

(** [subtypes ty] returns [ty]'s subtypes *)
val subtypes : lltype -> lltype array

(** [array_type ty n] returns the array type containing [n] elements of type
    [ty]. See the method [llvm::ArrayType::get]. *)
val array_type : lltype -> int -> lltype

(** [pointer_type ty] returns the pointer type referencing objects of type
    [ty] in the default address space (0).
    See the method [llvm::PointerType::getUnqual]. *)
val pointer_type : lltype -> lltype

(** [qualified_pointer_type ty as] returns the pointer type referencing objects
    of type [ty] in address space [as].
    See the method [llvm::PointerType::get]. *)
val qualified_pointer_type : lltype -> int -> lltype

(** [vector_type ty n] returns the array type containing [n] elements of the
    primitive type [ty]. See the method [llvm::ArrayType::get]. *)
val vector_type : lltype -> int -> lltype

(** [element_type ty] returns the element type of the pointer, vector, or array
    type [ty]. See the method [llvm::SequentialType::get]. *)
val element_type : lltype -> lltype

(** [element_type aty] returns the element count of the array type [aty].
    See the method [llvm::ArrayType::getNumElements]. *)
val array_length : lltype -> int

(** [address_space pty] returns the address space qualifier of the pointer type
    [pty]. See the method [llvm::PointerType::getAddressSpace]. *)
val address_space : lltype -> int

(** [element_type ty] returns the element count of the vector type [ty].
    See the method [llvm::VectorType::getNumElements]. *)
val vector_size : lltype -> int


(** {7 Operations on other types} *)

(** [void_type c] creates a type of a function which does not return any
    value in the context [c]. See [llvm::Type::VoidTy]. *)
val void_type : llcontext -> lltype

(** [label_type c] creates a type of a basic block in the context [c]. See
    [llvm::Type::LabelTy]. *)
val label_type : llcontext -> lltype

(** [x86_mmx_type c] returns the x86 64-bit MMX register type in the
    context [c]. See [llvm::Type::X86_MMXTy]. *)
val x86_mmx_type : llcontext -> lltype

(** [type_by_name m name] returns the specified type from the current module
    if it exists.
    See the method [llvm::Module::getTypeByName] *)
val type_by_name : llmodule -> string -> lltype option


(** {6 Values} *)

(** [type_of v] returns the type of the value [v].
    See the method [llvm::Value::getType]. *)
val type_of : llvalue -> lltype

(** [classify_value v] returns the kind of the value [v]. *)
val classify_value : llvalue -> ValueKind.t

(** [value_name v] returns the name of the value [v]. For global values, this is
    the symbol name. For instructions and basic blocks, it is the SSA register
    name. It is meaningless for constants.
    See the method [llvm::Value::getName]. *)
val value_name : llvalue -> string

(** [set_value_name n v] sets the name of the value [v] to [n]. See the method
    [llvm::Value::setName]. *)
val set_value_name : string -> llvalue -> unit

(** [dump_value v] prints the .ll representation of the value [v] to standard
    error. See the method [llvm::Value::dump]. *)
val dump_value : llvalue -> unit

(** [string_of_llvalue v] returns a string describing the value [v]. *)
val string_of_llvalue : llvalue -> string

(** [replace_all_uses_with old new] replaces all uses of the value [old]
    with the value [new]. See the method [llvm::Value::replaceAllUsesWith]. *)
val replace_all_uses_with : llvalue -> llvalue -> unit


(** {6 Uses} *)

(** [use_begin v] returns the first position in the use list for the value [v].
    [use_begin] and [use_succ] can e used to iterate over the use list in order.
    See the method [llvm::Value::use_begin]. *)
val use_begin : llvalue -> lluse option

(** [use_succ u] returns the use list position succeeding [u].
    See the method [llvm::use_value_iterator::operator++]. *)
val use_succ : lluse -> lluse option

(** [user u] returns the user of the use [u].
    See the method [llvm::Use::getUser]. *)
val user : lluse -> llvalue

(** [used_value u] returns the usee of the use [u].
    See the method [llvm::Use::getUsedValue]. *)
val used_value : lluse -> llvalue

(** [iter_uses f v] applies function [f] to each of the users of the value [v]
    in order. Tail recursive. *)
val iter_uses : (lluse -> unit) -> llvalue -> unit

(** [fold_left_uses f init v] is [f (... (f init u1) ...) uN] where
    [u1,...,uN] are the users of the value [v]. Tail recursive. *)
val fold_left_uses : ('a -> lluse -> 'a) -> 'a -> llvalue -> 'a

(** [fold_right_uses f v init] is [f u1 (... (f uN init) ...)