Directory structure:
└── microsoft-microsoft-ui-xaml/
    ├── README.md
    ├── CODE_OF_CONDUCT.md
    ├── CONTRIBUTING.md
    ├── CONTRIBUTING_feedback_and_requests.md
    ├── LICENSE
    ├── privacy.md
    ├── SECURITY.md
    ├── docs/
    │   ├── contribution_handling.md
    │   ├── contribution_workflow.md
    │   ├── debugging_buildfailures.md
    │   ├── debugging_crashes.md
    │   ├── feature_proposal_process.md
    │   ├── roadmap.md
    │   ├── SECURITY.md
    │   ├── triage.md
    │   ├── winrt-apis-for-desktop.md
    │   ├── winui3_migration.md
    │   └── images/
    │       └── BrowseInformation.PNG
    ├── specs/
    │   ├── AnimatedVisualPlayer Spec.md
    │   ├── api_spec_template.md
    │   ├── appwindow-spec.md
    │   ├── custom-iresourcemanager-spec.md
    │   ├── DateTimePicker-Visual-Updates-Spec.md
    │   ├── FooterMenuItemTemplate-spec.md
    │   ├── NavigationViewTemplateSettings-OpenPaneLength.md
    │   ├── Popup-AdditionalLayoutProperties-Spec.md
    │   ├── public-api-review-process.md
    │   ├── xaml-backdrop-api.md
    │   ├── xaml-resource-references-tracing-spec.md
    │   ├── CalendarView/
    │   │   └── CalendarViewSpec1.md
    │   ├── ColorPicker/
    │   │   └── ColorPicker.Orientation.md
    │   ├── images/
    │   │   ├── datepicker-evolution.PNG
    │   │   ├── DPTP-other-states.PNG
    │   │   └── timepicker-evolution.PNG
    │   ├── InfoBadge/
    │   │   ├── InfoBadge-spec.md
    │   │   └── images/
    │   │       └── color-breakdown.PNG
    │   ├── ScrollingControls/
    │   │   ├── ScrollPresenter.md
    │   │   └── ScrollView.md
    │   └── TitleBar/
    │       ├── titleBar-dev-spec.md
    │       └── titlebar-functional-spec.md
    ├── src/
    │   ├── CODE_OF_CONDUCT.md
    │   ├── Directory.Build.props
    │   ├── Directory.Build.targets
    │   ├── dirs.targets
    │   ├── global.json
    │   ├── nuget.config
    │   ├── packages.arm64ec.config
    │   ├── packages.config
    │   ├── Packages.props
    │   ├── UpdateMockWinAppSDKPackage.csproj
    │   ├── UpdateMockWinAppSDKPackageBeforeBuilding.props
    │   ├── XamlCompilerPrerequisites.sln
    │   ├── .vsconfig
    │   ├── .vsconfig_buildtools
    │   ├── controls/
    │   │   ├── app.config
    │   │   ├── Build.cmd
    │   │   ├── CleanupMSBuildProcesses.csproj
    │   │   ├── CppWinRT.props
    │   │   ├── CustomInlineTasks.targets
    │   │   ├── CustomTasks.sln
    │   │   ├── DevCmd.cmd
    │   │   ├── Directory.Build.props
    │   │   ├── Directory.Build.targets
    │   │   ├── environment.props
    │   │   ├── FeatureAreas.props
    │   │   ├── HybridCRT.props
    │   │   ├── MidlShared.props
    │   │   ├── MidlShared.targets
    │   │   ├── mux.controls.props
    │   │   ├── MUXControls.sln
    │   │   ├── MUXControlsInnerLoop.sln
    │   │   ├── nuget.props
    │   │   ├── privacy.md
    │   │   ├── ProjectConfigurations.props
    │   │   ├── ProjectImports.targets
    │   │   ├── SdkVersion.props
    │   │   ├── version.props
    │   │   ├── .editorconfig
    │   │   ├── .GitHubCommitSyncedTo
    │   │   ├── dev/
    │   │   │   ├── dirs.proj
    │   │   │   ├── AnimatedIcon/
    │   │   │   │   ├── AnimatedIcon.cpp
    │   │   │   │   ├── AnimatedIcon.h
    │   │   │   │   ├── AnimatedIcon.idl
    │   │   │   │   ├── AnimatedIcon.vcxitems
    │   │   │   │   ├── AnimatedIcon.vcxitems.filters
    │   │   │   │   ├── AnimatedIconTestHooks.cpp
    │   │   │   │   ├── AnimatedIconTestHooks.h
    │   │   │   │   ├── AnimatedIconTestHooks.idl
    │   │   │   │   ├── AnimatedVisuals/
    │   │   │   │   │   ├── AnimatedAcceptVisualSource.cpp
    │   │   │   │   │   ├── AnimatedAcceptVisualSource.h
    │   │   │   │   │   ├── AnimatedAcceptVisualSource.idl
    │   │   │   │   │   ├── AnimatedBackVisualSource.cpp
    │   │   │   │   │   ├── AnimatedBackVisualSource.h
    │   │   │   │   │   ├── AnimatedBackVisualSource.idl
    │   │   │   │   │   ├── AnimatedChevronDownSmallVisualSource.cpp
    │   │   │   │   │   ├── AnimatedChevronDownSmallVisualSource.h
    │   │   │   │   │   ├── AnimatedChevronDownSmallVisualSource.idl
    │   │   │   │   │   ├── AnimatedChevronRightDownSmallVisualSource.cpp
    │   │   │   │   │   ├── AnimatedChevronRightDownSmallVisualSource.h
    │   │   │   │   │   ├── AnimatedChevronRightDownSmallVisualSource.idl
    │   │   │   │   │   ├── AnimatedChevronUpDownSmallVisualSource.cpp
    │   │   │   │   │   ├── AnimatedChevronUpDownSmallVisualSource.h
    │   │   │   │   │   ├── AnimatedChevronUpDownSmallVisualSource.idl
    │   │   │   │   │   ├── AnimatedFindVisualSource.cpp
    │   │   │   │   │   ├── AnimatedFindVisualSource.h
    │   │   │   │   │   ├── AnimatedFindVisualSource.idl
    │   │   │   │   │   ├── AnimatedGlobalNavigationButtonVisualSource.cpp
    │   │   │   │   │   ├── AnimatedGlobalNavigationButtonVisualSource.h
    │   │   │   │   │   ├── AnimatedGlobalNavigationButtonVisualSource.idl
    │   │   │   │   │   ├── AnimatedSettingsVisualSource.cpp
    │   │   │   │   │   ├── AnimatedSettingsVisualSource.h
    │   │   │   │   │   └── AnimatedSettingsVisualSource.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── AnimatedIcon_APITests.projitems
    │   │   │   │   │   ├── AnimatedIcon_APITests.shproj
    │   │   │   │   │   ├── AnimatedIconTests.cs
    │   │   │   │   │   └── MockAnimatedIconSource.cs
    │   │   │   │   ├── Docs/
    │   │   │   │   │   ├── AnimatedIconDevDesign.md
    │   │   │   │   │   ├── MultiStateSegmentLookupProposal.md
    │   │   │   │   │   └── SingleStateSegmentLookup.md
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── AnimatedIcon_TestUI.projitems
    │   │   │   │       ├── AnimatedIcon_TestUI.shproj
    │   │   │   │       ├── AnimatedIconHost.cs
    │   │   │   │       ├── AnimatedIconPage.xaml
    │   │   │   │       ├── AnimatedIconPage.xaml.cs
    │   │   │   │       ├── BrightnessSun.cs
    │   │   │   │       ├── ColorToSolidColorBrushConverter.cs
    │   │   │   │       ├── DoubleToStringConverter.cs
    │   │   │   │       ├── MockIRichAnimatedIconSource.cs
    │   │   │   │       └── ToggleAnimatedIconHost.cs
    │   │   │   ├── AnimatedVisualPlayer/
    │   │   │   │   ├── AnimatedVisualPlayer.cpp
    │   │   │   │   ├── AnimatedVisualPlayer.h
    │   │   │   │   ├── AnimatedVisualPlayer.idl
    │   │   │   │   ├── AnimatedVisualPlayer.vcxitems
    │   │   │   │   ├── AnimatedVisualPlayerAutomationPeer.cpp
    │   │   │   │   ├── AnimatedVisualPlayerAutomationPeer.h
    │   │   │   │   ├── AnimatedVisualPlayerAutomationPeer.idl
    │   │   │   │   ├── inc/
    │   │   │   │   │   └── Constants.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── AnimatedVisualPlayer_InteractionTests.projitems
    │   │   │   │   │   ├── AnimatedVisualPlayer_InteractionTests.shproj
    │   │   │   │   │   └── AnimatedVisualPlayerTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── AnimatedVisualPlayer_TestUI.projitems
    │   │   │   │       ├── AnimatedVisualPlayer_TestUI.shproj
    │   │   │   │       ├── AnimatedVisualPlayerPage.xaml
    │   │   │   │       ├── AnimatedVisualPlayerPage.xaml.cs
    │   │   │   │       ├── LottieLogo.cs
    │   │   │   │       └── nullsource.cs
    │   │   │   ├── AnnotatedScrollBar/
    │   │   │   │   ├── AnnotatedScrollBar.cpp
    │   │   │   │   ├── AnnotatedScrollBar.h
    │   │   │   │   ├── AnnotatedScrollBar.idl
    │   │   │   │   ├── AnnotatedScrollBar.vcxitems
    │   │   │   │   ├── AnnotatedScrollBar.xaml
    │   │   │   │   ├── AnnotatedScrollBar_themeresources.xaml
    │   │   │   │   ├── AnnotatedScrollBarDetailLabelRequestedEventArgs.cpp
    │   │   │   │   ├── AnnotatedScrollBarDetailLabelRequestedEventArgs.h
    │   │   │   │   ├── AnnotatedScrollBarLabel.cpp
    │   │   │   │   ├── AnnotatedScrollBarLabel.h
    │   │   │   │   ├── AnnotatedScrollBarPanningInfo.cpp
    │   │   │   │   ├── AnnotatedScrollBarPanningInfo.h
    │   │   │   │   ├── AnnotatedScrollBarScrollingEventArgs.cpp
    │   │   │   │   ├── AnnotatedScrollBarScrollingEventArgs.h
    │   │   │   │   ├── AnnotatedScrollBarTrace.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── AnnotatedScrollBar_APITests.projitems
    │   │   │   │   │   ├── AnnotatedScrollBar_APITests.shproj
    │   │   │   │   │   └── AnnotatedScrollBarTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── AnnotatedScrollBar_InteractionTests.projitems
    │   │   │   │   │   ├── AnnotatedScrollBar_InteractionTests.shproj
    │   │   │   │   │   └── AnnotatedScrollBarInteractionTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── AnnotatedScrollBar_TestUI.projitems
    │   │   │   │       ├── AnnotatedScrollBar_TestUI.shproj
    │   │   │   │       ├── AnnotatedScrollBarIScrollControllerPage.xaml
    │   │   │   │       ├── AnnotatedScrollBarIScrollControllerPage.xaml.cs
    │   │   │   │       ├── AnnotatedScrollBarPage.xaml
    │   │   │   │       ├── AnnotatedScrollBarPage.xaml.cs
    │   │   │   │       ├── AnnotatedScrollBarRangeBasePage.xaml
    │   │   │   │       ├── AnnotatedScrollBarRangeBasePage.xaml.cs
    │   │   │   │       ├── AnnotatedScrollBarSummaryPage.xaml
    │   │   │   │       └── AnnotatedScrollBarSummaryPage.xaml.cs
    │   │   │   ├── AutoSuggestBox/
    │   │   │   │   ├── AutoSuggestBox.vcxitems
    │   │   │   │   ├── AutoSuggestBox_themeresources.xaml
    │   │   │   │   ├── AutoSuggestBoxHelper.cpp
    │   │   │   │   ├── AutoSuggestBoxHelper.h
    │   │   │   │   ├── AutoSuggestBoxHelper.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── AutoSuggestBox_APITests.projitems
    │   │   │   │   │   ├── AutoSuggestBox_APITests.shproj
    │   │   │   │   │   └── AutoSuggestBoxTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── AutoSuggestBox_InteractionTests.projitems
    │   │   │   │   │   ├── AutoSuggestBox_InteractionTests.shproj
    │   │   │   │   │   └── AutoSuggestBoxTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── AutoSuggestBox_TestUI.projitems
    │   │   │   │       ├── AutoSuggestBox_TestUI.shproj
    │   │   │   │       ├── AutoSuggestBoxPage.xaml
    │   │   │   │       └── AutoSuggestBoxPage.xaml.cs
    │   │   │   ├── Breadcrumb/
    │   │   │   │   ├── Breadcrumb.vcxitems
    │   │   │   │   ├── BreadcrumbBar.cpp
    │   │   │   │   ├── BreadcrumbBar.h
    │   │   │   │   ├── BreadcrumbBar.idl
    │   │   │   │   ├── BreadcrumbBar.xaml
    │   │   │   │   ├── BreadcrumbBar_themeresources.xaml
    │   │   │   │   ├── BreadcrumbBarAutomationPeer.idl
    │   │   │   │   ├── BreadcrumbBarElementFactory.cpp
    │   │   │   │   ├── BreadcrumbBarElementFactory.h
    │   │   │   │   ├── BreadcrumbBarItem.cpp
    │   │   │   │   ├── BreadcrumbBarItem.h
    │   │   │   │   ├── BreadcrumbBarItemAutomationPeer.cpp
    │   │   │   │   ├── BreadcrumbBarItemAutomationPeer.h
    │   │   │   │   ├── BreadcrumbBarItemClickedEventArgs.cpp
    │   │   │   │   ├── BreadcrumbBarItemClickedEventArgs.h
    │   │   │   │   ├── BreadcrumbItem.properties.cpp
    │   │   │   │   ├── BreadcrumbItem.properties.h
    │   │   │   │   ├── BreadcrumbIterable.cpp
    │   │   │   │   ├── BreadcrumbIterable.h
    │   │   │   │   ├── BreadcrumbIterator.cpp
    │   │   │   │   ├── BreadcrumbIterator.h
    │   │   │   │   ├── BreadcrumbLayout.cpp
    │   │   │   │   ├── BreadcrumbLayout.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── Breadcrumb_APITests.projitems
    │   │   │   │   │   ├── BreadcrumbBar_APITests.shproj
    │   │   │   │   │   └── BreadcrumbTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── Breadcrumb_InteractionTests.projitems
    │   │   │   │   │   ├── BreadcrumbBar_InteractionTests.shproj
    │   │   │   │   │   └── BreadcrumbBarTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-gb/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── Breadcrumb_TestUI.projitems
    │   │   │   │       ├── BreadcrumbBar_TestUI.shproj
    │   │   │   │       ├── BreadcrumbBarAxeTestPage.xaml
    │   │   │   │       ├── BreadcrumbBarAxeTestPage.xaml.cs
    │   │   │   │       ├── BreadcrumbBarPage.xaml
    │   │   │   │       ├── BreadcrumbBarPage.xaml.cs
    │   │   │   │       └── TreeStructure.cs
    │   │   │   ├── Collections/
    │   │   │   │   ├── BindableVector.h
    │   │   │   │   ├── Collections.vcxitems
    │   │   │   │   ├── HashMap.h
    │   │   │   │   ├── Vector.h
    │   │   │   │   ├── VectorChangedEventArgs.h
    │   │   │   │   └── VectorIterator.h
    │   │   │   ├── ColorPicker/
    │   │   │   │   ├── readme.md
    │   │   │   │   ├── ColorChangedEventArgs.cpp
    │   │   │   │   ├── ColorChangedEventArgs.h
    │   │   │   │   ├── ColorHelpers.cpp
    │   │   │   │   ├── ColorHelpers.h
    │   │   │   │   ├── ColorPicker.cpp
    │   │   │   │   ├── ColorPicker.h
    │   │   │   │   ├── ColorPicker.idl
    │   │   │   │   ├── ColorPicker.vcxitems
    │   │   │   │   ├── ColorPicker.xaml
    │   │   │   │   ├── ColorPicker_themeresources.xaml
    │   │   │   │   ├── ColorPickerSlider.cpp
    │   │   │   │   ├── ColorPickerSlider.h
    │   │   │   │   ├── ColorPickerSlider.idl
    │   │   │   │   ├── ColorPickerSliderAutomationPeer.cpp
    │   │   │   │   ├── ColorPickerSliderAutomationPeer.h
    │   │   │   │   ├── ColorPickerSliderAutomationPeer.idl
    │   │   │   │   ├── ColorSpectrum.cpp
    │   │   │   │   ├── ColorSpectrum.h
    │   │   │   │   ├── ColorSpectrum.idl
    │   │   │   │   ├── ColorSpectrum.xaml
    │   │   │   │   ├── ColorSpectrumAutomationPeer.cpp
    │   │   │   │   ├── ColorSpectrumAutomationPeer.h
    │   │   │   │   ├── ColorSpectrumAutomationPeer.idl
    │   │   │   │   ├── Common.idl
    │   │   │   │   ├── improvements.md
    │   │   │   │   ├── SpectrumBrush.cpp
    │   │   │   │   ├── SpectrumBrush.h
    │   │   │   │   ├── SpectrumBrush.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ColorPicker_APITests.projitems
    │   │   │   │   │   ├── ColorPicker_APITests.shproj
    │   │   │   │   │   └── ColorPickerTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ColorPicker_InteractionTests.projitems
    │   │   │   │   │   ├── ColorPicker_InteractionTests.shproj
    │   │   │   │   │   └── ColorPickerTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ColorPicker_TestUI.projitems
    │   │   │   │       ├── ColorPicker_TestUI.shproj
    │   │   │   │       ├── ColorPickerPage.xaml
    │   │   │   │       └── ColorPickerPage.xaml.cs
    │   │   │   ├── ComboBox/
    │   │   │   │   ├── ComboBox.vcxitems
    │   │   │   │   ├── ComboBox_themeresources.xaml
    │   │   │   │   ├── ComboBoxHelper.cpp
    │   │   │   │   ├── ComboBoxHelper.h
    │   │   │   │   ├── ComboBoxHelper.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ComboBox_APITests.projitems
    │   │   │   │   │   ├── ComboBox_APITests.shproj
    │   │   │   │   │   └── ComboBoxTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ComboBox_TestUI.projitems
    │   │   │   │       ├── ComboBox_TestUI.shproj
    │   │   │   │       ├── ComboBoxPage.xaml
    │   │   │   │       └── ComboBoxPage.xaml.cs
    │   │   │   ├── CommandBarFlyout/
    │   │   │   │   ├── CommandBarFlyout.cpp
    │   │   │   │   ├── CommandBarFlyout.h
    │   │   │   │   ├── CommandBarFlyout.idl
    │   │   │   │   ├── CommandBarFlyout.vcxitems
    │   │   │   │   ├── CommandBarFlyout.xaml
    │   │   │   │   ├── CommandBarFlyout_themeresources.xaml
    │   │   │   │   ├── CommandBarFlyoutCommandBar.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBar.h
    │   │   │   │   ├── CommandBarFlyoutCommandBar.idl
    │   │   │   │   ├── CommandBarFlyoutCommandBarAutomationProperties.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBarAutomationProperties.h
    │   │   │   │   ├── CommandBarFlyoutCommandBarTemplateSettings.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBarTemplateSettings.h
    │   │   │   │   ├── CommandBarFlyoutTrace.h
    │   │   │   │   ├── TextCommandBarFlyout.cpp
    │   │   │   │   ├── TextCommandBarFlyout.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── CommandBarFlyout_APITests.projitems
    │   │   │   │   │   ├── CommandBarFlyout_APITests.shproj
    │   │   │   │   │   └── CommandBarFlyoutTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── CommandBarFlyout_InteractionTests.projitems
    │   │   │   │   │   ├── CommandBarFlyout_InteractionTests.shproj
    │   │   │   │   │   ├── CommandBarFlyoutTests.cs
    │   │   │   │   │   └── TextCommandBarFlyoutTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── CommandBarFlyout_TestUI.projitems
    │   │   │   │       ├── CommandBarFlyout_TestUI.shproj
    │   │   │   │       ├── CommandBarFlyoutMainPage.xaml
    │   │   │   │       ├── CommandBarFlyoutMainPage.xaml.cs
    │   │   │   │       ├── CommandBarFlyoutPage.xaml
    │   │   │   │       ├── CommandBarFlyoutPage.xaml.cs
    │   │   │   │       ├── ExtraCommandBarFlyoutPage.xaml
    │   │   │   │       ├── ExtraCommandBarFlyoutPage.xaml.cs
    │   │   │   │       ├── TextCommandBarFlyoutPage.xaml
    │   │   │   │       └── TextCommandBarFlyoutPage.xaml.cs
    │   │   │   ├── Common/
    │   │   │   │   ├── AutoHandle.h
    │   │   │   │   ├── ColorConversion.cpp
    │   │   │   │   ├── ColorConversion.h
    │   │   │   │   ├── Common.vcxitems
    │   │   │   │   ├── CornerRadiusFilterConverter.cpp
    │   │   │   │   ├── CornerRadiusFilterConverter.h
    │   │   │   │   ├── CornerRadiusFilterConverters.idl
    │   │   │   │   ├── CornerRadiusToThicknessConverter.cpp
    │   │   │   │   ├── CornerRadiusToThicknessConverter.h
    │   │   │   │   ├── CornerRadiusToThicknessConverter.idl
    │   │   │   │   ├── Flags_Enum.h
    │   │   │   │   ├── LifetimeHandler.cpp
    │   │   │   │   ├── LifetimeHandler.h
    │   │   │   │   ├── PointerInfo.h
    │   │   │   │   ├── PointerInfoRevokers.h
    │   │   │   │   └── WinEventLogLevels.h
    │   │   │   ├── CommonManaged/
    │   │   │   │   ├── CommonManaged.projitems
    │   │   │   │   ├── CommonManaged.shproj
    │   │   │   │   └── PlatformConfiguration.cs
    │   │   │   ├── CommonStyles/
    │   │   │   │   ├── AppBarButton_themeresources.xaml
    │   │   │   │   ├── AppBarSeparator_themeresources.xaml
    │   │   │   │   ├── AppBarToggleButton_themeresources.xaml
    │   │   │   │   ├── Button_themeresources.xaml
    │   │   │   │   ├── CalendarDatePicker_themeresources.xaml
    │   │   │   │   ├── CalendarView_themeresources.xaml
    │   │   │   │   ├── CheckBox_themeresources.xaml
    │   │   │   │   ├── CommandBar_themeresources.xaml
    │   │   │   │   ├── Common_themeresources.xaml
    │   │   │   │   ├── Common_themeresources_any.xaml
    │   │   │   │   ├── CommonStyles.vcxitems
    │   │   │   │   ├── ContentDialog_themeresources.xaml
    │   │   │   │   ├── CornerRadius_themeresources.xaml
    │   │   │   │   ├── DatePicker_themeresources.xaml
    │   │   │   │   ├── DateTimePickerFlyout_themeresources.xaml
    │   │   │   │   ├── Deprecated_themeresources.xaml
    │   │   │   │   ├── Deprecated_themeresources_any.xaml
    │   │   │   │   ├── FlipView_themeresources.xaml
    │   │   │   │   ├── FlipViewItem_themeresources.xaml
    │   │   │   │   ├── FlyoutPresenter_themeresources.xaml
    │   │   │   │   ├── GridViewItem_themeresources.xaml
    │   │   │   │   ├── Hyperlink_themeresources.xaml
    │   │   │   │   ├── HyperlinkButton_themeresources.xaml
    │   │   │   │   ├── InkToolbar_themeresources.xaml
    │   │   │   │   ├── ListBox_themeresources.xaml
    │   │   │   │   ├── ListViewItem_themeresources.xaml
    │   │   │   │   ├── MediaTransportControls_themeresources.xaml
    │   │   │   │   ├── MenuFlyout_themeresources.xaml
    │   │   │   │   ├── PasswordBox_themeresources.xaml
    │   │   │   │   ├── Pivot_themeresources.xaml
    │   │   │   │   ├── RadioButton_themeresources.xaml
    │   │   │   │   ├── RepeatButton_themeresources.xaml
    │   │   │   │   ├── RichEditBox_themeresources.xaml
    │   │   │   │   ├── ScrollBar_themeresources.xaml
    │   │   │   │   ├── ScrollViewer_themeresources.xaml
    │   │   │   │   ├── Slider_themeresources.xaml
    │   │   │   │   ├── TextBlock_themeresources.xaml
    │   │   │   │   ├── TextBlock_themeresources_v2.5.xaml
    │   │   │   │   ├── TextBox_themeresources.xaml
    │   │   │   │   ├── TextControlsCommon_themeresources.xaml
    │   │   │   │   ├── TimePicker_themeresources.xaml
    │   │   │   │   ├── ToggleButton_themeresources.xaml
    │   │   │   │   ├── ToggleSwitch_themeresources.xaml
    │   │   │   │   ├── ToolTip_themeresources.xaml
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── BaselineResources2dot5stable.cs
    │   │   │   │   │   ├── CalendarViewTests.cs
    │   │   │   │   │   ├── CommonStyles_APITests.projitems
    │   │   │   │   │   ├── CommonStyles_APITests.shproj
    │   │   │   │   │   └── CommonStylesTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── CommonStyles_InteractionTests.projitems
    │   │   │   │   │   ├── CommonStyles_InteractionTests.shproj
    │   │   │   │   │   └── CommonStylesTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── AppBarPage.xaml
    │   │   │   │       ├── AppBarPage.xaml.cs
    │   │   │   │       ├── BlankPage.xaml
    │   │   │   │       ├── BlankPage.xaml.cs
    │   │   │   │       ├── BorderThicknessPage.xaml
    │   │   │   │       ├── BorderThicknessPage.xaml.cs
    │   │   │   │       ├── CalendarDatePickerPage.xaml
    │   │   │   │       ├── CalendarDatePickerPage.xaml.cs
    │   │   │   │       ├── CalendarViewPage.xaml
    │   │   │   │       ├── CalendarViewPage.xaml.cs
    │   │   │   │       ├── CheckBoxPage.xaml
    │   │   │   │       ├── CheckBoxPage.xaml.cs
    │   │   │   │       ├── CommandBarCenterPage.xaml
    │   │   │   │       ├── CommandBarCenterPage.xaml.cs
    │   │   │   │       ├── CommandBarPage.xaml
    │   │   │   │       ├── CommandBarPage.xaml.cs
    │   │   │   │       ├── CommandBarSummaryPage.xaml
    │   │   │   │       ├── CommandBarSummaryPage.xaml.cs
    │   │   │   │       ├── CommonStyles_TestUI.projitems
    │   │   │   │       ├── CommonStyles_TestUI.shproj
    │   │   │   │       ├── CommonStylesPage.xaml
    │   │   │   │       ├── CommonStylesPage.xaml.cs
    │   │   │   │       ├── CompactPage.xaml
    │   │   │   │       ├── CompactPage.xaml.cs
    │   │   │   │       ├── ContentDialogPage.xaml
    │   │   │   │       ├── ContentDialogPage.xaml.cs
    │   │   │   │       ├── CornerRadiusPage.xaml
    │   │   │   │       ├── CornerRadiusPage.xaml.cs
    │   │   │   │       ├── DatePickerPage.xaml
    │   │   │   │       ├── DatePickerPage.xaml.cs
    │   │   │   │       ├── FlatItemsControlPage.xaml
    │   │   │   │       ├── FlatItemsControlPage.xaml.cs
    │   │   │   │       ├── FlipViewPage.xaml
    │   │   │   │       ├── FlipViewPage.xaml.cs
    │   │   │   │       ├── GridViewPage.xaml
    │   │   │   │       ├── GridViewPage.xaml.cs
    │   │   │   │       ├── GroupedItemsControlPage.xaml
    │   │   │   │       ├── GroupedItemsControlPage.xaml.cs
    │   │   │   │       ├── GroupedListViewBasePage.xaml
    │   │   │   │       ├── GroupedListViewBasePage.xaml.cs
    │   │   │   │       ├── ImagePage.xaml
    │   │   │   │       ├── ImagePage.xaml.cs
    │   │   │   │       ├── InkToolbarPage.xaml
    │   │   │   │       ├── InkToolbarPage.xaml.cs
    │   │   │   │       ├── ItemsControlPage.xaml
    │   │   │   │       ├── ItemsControlPage.xaml.cs
    │   │   │   │       ├── ListViewAnchoringPage.xaml
    │   │   │   │       ├── ListViewAnchoringPage.xaml.cs
    │   │   │   │       ├── ListViewBasePage.xaml
    │   │   │   │       ├── ListViewBasePage.xaml.cs
    │   │   │   │       ├── ListViewElementNameBindingPage.xaml
    │   │   │   │       ├── ListViewElementNameBindingPage.xaml.cs
    │   │   │   │       ├── ListViewPage.xaml
    │   │   │   │       ├── ListViewPage.xaml.cs
    │   │   │   │       ├── MediaTransportControlsPage.xaml
    │   │   │   │       ├── MediaTransportControlsPage.xaml.cs
    │   │   │   │       ├── MenuFlyoutPage.xaml
    │   │   │   │       ├── MenuFlyoutPage.xaml.cs
    │   │   │   │       ├── NestedGridViewsPage.xaml
    │   │   │   │       ├── NestedGridViewsPage.xaml.cs
    │   │   │   │       ├── NestedItemsControlsPage.xaml
    │   │   │   │       ├── NestedItemsControlsPage.xaml.cs
    │   │   │   │       ├── NestedListViewsPage.xaml
    │   │   │   │       ├── NestedListViewsPage.xaml.cs
    │   │   │   │       ├── NewWindowRootPage.xaml
    │   │   │   │       ├── NewWindowRootPage.xaml.cs
    │   │   │   │       ├── PivotPage.xaml
    │   │   │   │       ├── PivotPage.xaml.cs
    │   │   │   │       ├── ScrollBarPage.xaml
    │   │   │   │       ├── ScrollBarPage.xaml.cs
    │   │   │   │       ├── ScrollViewerPage.xaml
    │   │   │   │       ├── ScrollViewerPage.xaml.cs
    │   │   │   │       ├── SliderPage.xaml
    │   │   │   │       ├── SliderPage.xaml.cs
    │   │   │   │       ├── TextControlsPage.xaml
    │   │   │   │       ├── TextControlsPage.xaml.cs
    │   │   │   │       ├── TimePickerPage.xaml
    │   │   │   │       ├── TimePickerPage.xaml.cs
    │   │   │   │       ├── ToolTipPage.xaml
    │   │   │   │       ├── ToolTipPage.xaml.cs
    │   │   │   │       ├── VisualPropertiesPage.xaml
    │   │   │   │       ├── VisualPropertiesPage.xaml.cs
    │   │   │   │       ├── VisualStatesPage.xaml
    │   │   │   │       ├── VisualStatesPage.xaml.cs
    │   │   │   │       ├── WindowPage.xaml
    │   │   │   │       └── WindowPage.xaml.cs
    │   │   │   ├── dll/
    │   │   │   │   ├── CommandingHelpers.cpp
    │   │   │   │   ├── CommonHelpers.tt
    │   │   │   │   ├── CppWinRTFilterTypes.tt
    │   │   │   │   ├── Directory.Build.props
    │   │   │   │   ├── dllmain.cpp
    │   │   │   │   ├── DoubleUtil.cpp
    │   │   │   │   ├── FloatUtil.cpp
    │   │   │   │   ├── Microsoft.UI.Xaml.Common.props
    │   │   │   │   ├── Microsoft.UI.Xaml.Common.targets
    │   │   │   │   ├── Microsoft.UI.Xaml.Controls.def
    │   │   │   │   ├── Microsoft.UI.Xaml.Controls.rc
    │   │   │   │   ├── Microsoft.UI.Xaml.Controls.vcxproj
    │   │   │   │   ├── Microsoft.UI.Xaml.Controls.vcxproj.filters
    │   │   │   │   ├── MUXControlsFactory.cpp
    │   │   │   │   ├── MUXControlsFactory.h
    │   │   │   │   ├── packages.config
    │   │   │   │   ├── pch.cpp
    │   │   │   │   ├── pch.h
    │   │   │   │   ├── RegUtil.cpp
    │   │   │   │   ├── SharedHelpers.cpp
    │   │   │   │   ├── targetver.h
    │   │   │   │   ├── WinRtType.tt
    │   │   │   │   ├── XamlControlsResources.cpp
    │   │   │   │   ├── XamlControlsResources.h
    │   │   │   │   ├── XamlMember.cpp
    │   │   │   │   ├── XamlMember.h
    │   │   │   │   ├── XamlMetadataDependencyLocator.cpp
    │   │   │   │   ├── XamlMetadataProvider.cpp
    │   │   │   │   ├── XamlMetadataProvider.h
    │   │   │   │   ├── XamlMetadataProviderGenerated.h
    │   │   │   │   ├── XamlMetadataProviderGenerated.tt
    │   │   │   │   ├── XamlMetadataProviderWindowsCodeGen.tt
    │   │   │   │   ├── XamlType.cpp
    │   │   │   │   ├── XamlType.h
    │   │   │   │   └── DensityStyles/
    │   │   │   │       ├── Compact.xaml
    │   │   │   │       └── CompactDatePickerTimePickerFlyout.xaml
    │   │   │   ├── DropDownButton/
    │   │   │   │   ├── DropDownButton.cpp
    │   │   │   │   ├── DropDownButton.h
    │   │   │   │   ├── DropDownButton.idl
    │   │   │   │   ├── DropDownButton.vcxitems
    │   │   │   │   ├── DropDownButton.xaml
    │   │   │   │   ├── DropDownButton_themeresources.xaml
    │   │   │   │   ├── DropDownButtonAutomationPeer.cpp
    │   │   │   │   ├── DropDownButtonAutomationPeer.h
    │   │   │   │   ├── DropDownButtonAutomationPeer.idl
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── DropDownButton_InteractionTests.projitems
    │   │   │   │   │   ├── DropDownButton_InteractionTests.shproj
    │   │   │   │   │   └── DropDownButtonTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── DropDownButton_TestUI.projitems
    │   │   │   │       ├── DropDownButton_TestUI.shproj
    │   │   │   │       ├── DropDownButtonPage.xaml
    │   │   │   │       └── DropDownButtonPage.xaml.cs
    │   │   │   ├── Effects/
    │   │   │   │   ├── microsoft.ui.private.composition.effects.idl
    │   │   │   │   ├── Microsoft.UI.Private.Composition.Effects.vcxitems
    │   │   │   │   └── microsoft.ui.private.composition.effects_impl.h
    │   │   │   ├── Expander/
    │   │   │   │   ├── Expander.cpp
    │   │   │   │   ├── Expander.h
    │   │   │   │   ├── Expander.idl
    │   │   │   │   ├── Expander.vcxitems
    │   │   │   │   ├── Expander.xaml
    │   │   │   │   ├── Expander_themeresources.xaml
    │   │   │   │   ├── ExpanderAutomationPeer.cpp
    │   │   │   │   ├── ExpanderAutomationPeer.h
    │   │   │   │   ├── ExpanderAutomationPeer.idl
    │   │   │   │   ├── ExpanderTemplateSettings.cpp
    │   │   │   │   ├── ExpanderTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── Expander_APITests.projitems
    │   │   │   │   │   ├── Expander_APITests.shproj
    │   │   │   │   │   ├── Expander_APITests.testsettings
    │   │   │   │   │   └── ExpanderTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── Expander_InteractionTests.projitems
    │   │   │   │   │   ├── Expander_InteractionTests.shproj
    │   │   │   │   │   └── ExpanderTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── Expander_TestUI.projitems
    │   │   │   │       ├── Expander_TestUI.shproj
    │   │   │   │       ├── ExpanderPage.xaml
    │   │   │   │       └── ExpanderPage.xaml.cs
    │   │   │   ├── Generated/
    │   │   │   │   ├── AcrylicBrush.properties.cpp
    │   │   │   │   ├── AcrylicBrush.properties.h
    │   │   │   │   ├── AcrylicTestApi.properties.cpp
    │   │   │   │   ├── AnimatedAcceptVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedBackVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedChevronDownSmallVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedChevronRightDownSmallVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedChevronUpDownSmallVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedFindVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedGlobalNavigationButtonVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedIcon.properties.cpp
    │   │   │   │   ├── AnimatedIcon.properties.h
    │   │   │   │   ├── AnimatedIconSource.properties.cpp
    │   │   │   │   ├── AnimatedIconSource.properties.h
    │   │   │   │   ├── AnimatedIconTestHooks.properties.cpp
    │   │   │   │   ├── AnimatedSettingsVisualSource.properties.cpp
    │   │   │   │   ├── AnimatedVisualPlayer.properties.cpp
    │   │   │   │   ├── AnimatedVisualPlayer.properties.h
    │   │   │   │   ├── AnimatedVisualPlayerAutomationPeer.properties.cpp
    │   │   │   │   ├── AnnotatedScrollBar.properties.cpp
    │   │   │   │   ├── AnnotatedScrollBar.properties.h
    │   │   │   │   ├── AnnotatedScrollBarLabel.properties.cpp
    │   │   │   │   ├── AutoSuggestBoxHelper.properties.cpp
    │   │   │   │   ├── AutoSuggestBoxHelper.properties.h
    │   │   │   │   ├── BreadcrumbBar.properties.cpp
    │   │   │   │   ├── BreadcrumbBar.properties.h
    │   │   │   │   ├── BreadcrumbBarItem.properties.cpp
    │   │   │   │   ├── BreadcrumbBarItemAutomationPeer.properties.cpp
    │   │   │   │   ├── ButtonInteraction.properties.cpp
    │   │   │   │   ├── ButtonInteraction.properties.h
    │   │   │   │   ├── ColorPicker.properties.cpp
    │   │   │   │   ├── ColorPicker.properties.h
    │   │   │   │   ├── ColorPickerSlider.properties.cpp
    │   │   │   │   ├── ColorPickerSlider.properties.h
    │   │   │   │   ├── ColorPickerSliderAutomationPeer.properties.cpp
    │   │   │   │   ├── ColorSpectrum.properties.cpp
    │   │   │   │   ├── ColorSpectrum.properties.h
    │   │   │   │   ├── ColorSpectrumAutomationPeer.properties.cpp
    │   │   │   │   ├── ColumnMajorUniformToLargestGridLayout.properties.cpp
    │   │   │   │   ├── ColumnMajorUniformToLargestGridLayout.properties.h
    │   │   │   │   ├── ComboBoxHelper.properties.cpp
    │   │   │   │   ├── ComboBoxHelper.properties.h
    │   │   │   │   ├── CommandBarFlyout.properties.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBar.properties.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBar.properties.h
    │   │   │   │   ├── CommandBarFlyoutCommandBarAutomationProperties.properties.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBarAutomationProperties.properties.h
    │   │   │   │   ├── CommandBarFlyoutCommandBarTemplateSettings.properties.cpp
    │   │   │   │   ├── CommandBarFlyoutCommandBarTemplateSettings.properties.h
    │   │   │   │   ├── CornerRadiusFilterConverter.properties.cpp
    │   │   │   │   ├── CornerRadiusFilterConverter.properties.h
    │   │   │   │   ├── CornerRadiusToThicknessConverter.properties.cpp
    │   │   │   │   ├── CornerRadiusToThicknessConverter.properties.h
    │   │   │   │   ├── DesktopAcrylicBackdrop.properties.cpp
    │   │   │   │   ├── DisplayRegionHelperTestApi.properties.cpp
    │   │   │   │   ├── DropDownButton.properties.cpp
    │   │   │   │   ├── DropDownButtonAutomationPeer.properties.cpp
    │   │   │   │   ├── ElementFactory.properties.cpp
    │   │   │   │   ├── Expander.properties.cpp
    │   │   │   │   ├── Expander.properties.h
    │   │   │   │   ├── ExpanderAutomationPeer.properties.cpp
    │   │   │   │   ├── ExpanderTemplateSettings.properties.cpp
    │   │   │   │   ├── ExpanderTemplateSettings.properties.h
    │   │   │   │   ├── FlowLayout.properties.cpp
    │   │   │   │   ├── FlowLayout.properties.h
    │   │   │   │   ├── FlowLayoutState.properties.cpp
    │   │   │   │   ├── ImageIcon.properties.cpp
    │   │   │   │   ├── ImageIcon.properties.h
    │   │   │   │   ├── ImageIconSource.properties.cpp
    │   │   │   │   ├── ImageIconSource.properties.h
    │   │   │   │   ├── IndexPath.properties.cpp
    │   │   │   │   ├── InfoBadge.properties.cpp
    │   │   │   │   ├── InfoBadge.properties.h
    │   │   │   │   ├── InfoBadgeTemplateSettings.properties.cpp
    │   │   │   │   ├── InfoBadgeTemplateSettings.properties.h
    │   │   │   │   ├── InfoBar.properties.cpp
    │   │   │   │   ├── InfoBar.properties.h
    │   │   │   │   ├── InfoBarAutomationPeer.properties.cpp
    │   │   │   │   ├── InfoBarClosedEventArgs.properties.cpp
    │   │   │   │   ├── InfoBarClosingEventArgs.properties.cpp
    │   │   │   │   ├── InfoBarPanel.properties.cpp
    │   │   │   │   ├── InfoBarPanel.properties.h
    │   │   │   │   ├── InfoBarTemplateSettings.properties.cpp
    │   │   │   │   ├── InfoBarTemplateSettings.properties.h
    │   │   │   │   ├── InkCanvas.properties.cpp
    │   │   │   │   ├── InkCanvas.properties.h
    │   │   │   │   ├── InkCanvasAutomationPeer.properties.cpp
    │   │   │   │   ├── InkToolBar.properties.cpp
    │   │   │   │   ├── InkToolBar.properties.h
    │   │   │   │   ├── InkToolBarAutomationPeer.properties.cpp
    │   │   │   │   ├── InkToolBarBallpointPenButton.properties.cpp
    │   │   │   │   ├── InkToolBarCustomPen.properties.cpp
    │   │   │   │   ├── InkToolBarCustomPenButton.properties.cpp
    │   │   │   │   ├── InkToolBarCustomPenButton.properties.h
    │   │   │   │   ├── InkToolBarCustomToggleButton.properties.cpp
    │   │   │   │   ├── InkToolBarCustomToolButton.properties.cpp
    │   │   │   │   ├── InkToolBarCustomToolButton.properties.h
    │   │   │   │   ├── InkToolBarEraserButton.properties.cpp
    │   │   │   │   ├── InkToolBarEraserButton.properties.h
    │   │   │   │   ├── InkToolBarFlyoutItem.properties.cpp
    │   │   │   │   ├── InkToolBarFlyoutItem.properties.h
    │   │   │   │   ├── InkToolBarFlyoutItemAutomationPeer.properties.cpp
    │   │   │   │   ├── InkToolBarHighlighterButton.properties.cpp
    │   │   │   │   ├── InkToolBarMenuButton.properties.cpp
    │   │   │   │   ├── InkToolBarMenuButton.properties.h
    │   │   │   │   ├── InkToolBarMenuButtonAutomationPeer.properties.cpp
    │   │   │   │   ├── InkToolBarPenButton.properties.cpp
    │   │   │   │   ├── InkToolBarPenButton.properties.h
    │   │   │   │   ├── InkToolBarPencilButton.properties.cpp
    │   │   │   │   ├── InkToolBarPenConfigurationControl.properties.cpp
    │   │   │   │   ├── InkToolBarPenConfigurationControl.properties.h
    │   │   │   │   ├── InkToolBarStencilButton.properties.cpp
    │   │   │   │   ├── InkToolBarStencilButton.properties.h
    │   │   │   │   ├── InkToolBarToggleButton.properties.cpp
    │   │   │   │   ├── InkToolBarToolButton.properties.cpp
    │   │   │   │   ├── InkToolBarToolButton.properties.h
    │   │   │   │   ├── InkToolBarToolButtonAutomationPeer.properties.cpp
    │   │   │   │   ├── ItemCollectionTransitionProvider.properties.cpp
    │   │   │   │   ├── ItemCollectionTransitionProvider.properties.h
    │   │   │   │   ├── ItemContainer.properties.cpp
    │   │   │   │   ├── ItemContainer.properties.h
    │   │   │   │   ├── ItemContainerAutomationPeer.properties.cpp
    │   │   │   │   ├── ItemsRepeater.properties.cpp
    │   │   │   │   ├── ItemsRepeater.properties.h
    │   │   │   │   ├── ItemsRepeaterScrollHost.properties.cpp
    │   │   │   │   ├── ItemsSourceView.properties.cpp
    │   │   │   │   ├── ItemsSourceView.properties.h
    │   │   │   │   ├── ItemsView.properties.cpp
    │   │   │   │   ├── ItemsView.properties.h
    │   │   │   │   ├── ItemsViewAutomationPeer.properties.cpp
    │   │   │   │   ├── ItemsViewTestHooks.properties.cpp
    │   │   │   │   ├── Layout.properties.cpp
    │   │   │   │   ├── Layout.properties.h
    │   │   │   │   ├── LayoutContext.properties.cpp
    │   │   │   │   ├── LayoutPanel.properties.cpp
    │   │   │   │   ├── LayoutPanel.properties.h
    │   │   │   │   ├── LayoutsTestHooks.properties.cpp
    │   │   │   │   ├── LinedFlowLayout.properties.cpp
    │   │   │   │   ├── LinedFlowLayout.properties.h
    │   │   │   │   ├── LinedFlowLayoutItemCollectionTransitionProvider.properties.cpp
    │   │   │   │   ├── MapControl.properties.cpp
    │   │   │   │   ├── MapControl.properties.h
    │   │   │   │   ├── MapElement.properties.cpp
    │   │   │   │   ├── MapElementClickEventArgs.properties.cpp
    │   │   │   │   ├── MapElementsLayer.properties.cpp
    │   │   │   │   ├── MapElementsLayer.properties.h
    │   │   │   │   ├── MapIcon.properties.cpp
    │   │   │   │   ├── MapIcon.properties.h
    │   │   │   │   ├── MapLayer.properties.cpp
    │   │   │   │   ├── MaterialHelperTestApi.properties.cpp
    │   │   │   │   ├── MenuBar.properties.cpp
    │   │   │   │   ├── MenuBar.properties.h
    │   │   │   │   ├── MenuBarAutomationPeer.properties.cpp
    │   │   │   │   ├── MenuBarItem.properties.cpp
    │   │   │   │   ├── MenuBarItem.properties.h
    │   │   │   │   ├── MenuBarItemAutomationPeer.properties.cpp
    │   │   │   │   ├── MenuBarItemFlyout.properties.cpp
    │   │   │   │   ├── MicaBackdrop.properties.cpp
    │   │   │   │   ├── MicaBackdrop.properties.h
    │   │   │   │   ├── MonochromaticOverlayPresenter.properties.cpp
    │   │   │   │   ├── MonochromaticOverlayPresenter.properties.h
    │   │   │   │   ├── MUXControlsTestHooks.properties.cpp
    │   │   │   │   ├── NavigationView.properties.cpp
    │   │   │   │   ├── NavigationView.properties.h
    │   │   │   │   ├── NavigationViewAutomationPeer.properties.cpp
    │   │   │   │   ├── NavigationViewItem.properties.cpp
    │   │   │   │   ├── NavigationViewItem.properties.h
    │   │   │   │   ├── NavigationViewItemAutomationPeer.properties.cpp
    │   │   │   │   ├── NavigationViewItemBase.properties.cpp
    │   │   │   │   ├── NavigationViewItemBase.properties.h
    │   │   │   │   ├── NavigationViewItemHeader.properties.cpp
    │   │   │   │   ├── NavigationViewItemInvokedEventArgs.properties.cpp
    │   │   │   │   ├── NavigationViewItemPresenter.properties.cpp
    │   │   │   │   ├── NavigationViewItemPresenter.properties.h
    │   │   │   │   ├── NavigationViewItemPresenterTemplateSettings.properties.cpp
    │   │   │   │   ├── NavigationViewItemPresenterTemplateSettings.properties.h
    │   │   │   │   ├── NavigationViewItemSeparator.properties.cpp
    │   │   │   │   ├── NavigationViewTemplateSettings.properties.cpp
    │   │   │   │   ├── NavigationViewTemplateSettings.properties.h
    │   │   │   │   ├── NonVirtualizingLayout.properties.cpp
    │   │   │   │   ├── NonVirtualizingLayoutContext.properties.cpp
    │   │   │   │   ├── NumberBox.properties.cpp
    │   │   │   │   ├── NumberBox.properties.h
    │   │   │   │   ├── NumberBoxAutomationPeer.properties.cpp
    │   │   │   │   ├── PagerControl.properties.cpp
    │   │   │   │   ├── PagerControl.properties.h
    │   │   │   │   ├── PagerControlAutomationPeer.properties.cpp
    │   │   │   │   ├── PagerControlTemplateSettings.properties.cpp
    │   │   │   │   ├── PagerControlTemplateSettings.properties.h
    │   │   │   │   ├── ParallaxView.properties.cpp
    │   │   │   │   ├── ParallaxView.properties.h
    │   │   │   │   ├── PersonPicture.properties.cpp
    │   │   │   │   ├── PersonPicture.properties.h
    │   │   │   │   ├── PersonPictureAutomationPeer.properties.cpp
    │   │   │   │   ├── PersonPictureTemplateSettings.properties.cpp
    │   │   │   │   ├── PersonPictureTemplateSettings.properties.h
    │   │   │   │   ├── PipsPager.properties.cpp
    │   │   │   │   ├── PipsPager.properties.h
    │   │   │   │   ├── PipsPagerAutomationPeer.properties.cpp
    │   │   │   │   ├── PipsPagerTemplateSettings.properties.cpp
    │   │   │   │   ├── PipsPagerTemplateSettings.properties.h
    │   │   │   │   ├── ProgressBar.properties.cpp
    │   │   │   │   ├── ProgressBar.properties.h
    │   │   │   │   ├── ProgressBarAutomationPeer.properties.cpp
    │   │   │   │   ├── ProgressBarTemplateSettings.properties.cpp
    │   │   │   │   ├── ProgressBarTemplateSettings.properties.h
    │   │   │   │   ├── ProgressRing.properties.cpp
    │   │   │   │   ├── ProgressRing.properties.h
    │   │   │   │   ├── ProgressRingAutomationPeer.properties.cpp
    │   │   │   │   ├── ProgressRingTemplateSettings.properties.cpp
    │   │   │   │   ├── ProgressRingTemplateSettings.properties.h
    │   │   │   │   ├── PullToRefreshHelperTestApi.properties.cpp
    │   │   │   │   ├── RadialGradientBrush.properties.cpp
    │   │   │   │   ├── RadialGradientBrush.properties.h
    │   │   │   │   ├── RadioButtons.properties.cpp
    │   │   │   │   ├── RadioButtons.properties.h
    │   │   │   │   ├── RadioButtonsAutomationPeer.properties.cpp
    │   │   │   │   ├── RadioButtonsTestHooks.properties.cpp
    │   │   │   │   ├── RadioMenuFlyoutItem.properties.cpp
    │   │   │   │   ├── RadioMenuFlyoutItem.properties.h
    │   │   │   │   ├── RatingControl.properties.cpp
    │   │   │   │   ├── RatingControl.properties.h
    │   │   │   │   ├── RatingControlAutomationPeer.properties.cpp
    │   │   │   │   ├── RatingItemFontInfo.properties.cpp
    │   │   │   │   ├── RatingItemFontInfo.properties.h
    │   │   │   │   ├── RatingItemImageInfo.properties.cpp
    │   │   │   │   ├── RatingItemImageInfo.properties.h
    │   │   │   │   ├── RatingItemInfo.properties.cpp
    │   │   │   │   ├── RecyclePool.properties.cpp
    │   │   │   │   ├── RecyclePool.properties.h
    │   │   │   │   ├── RecyclingElementFactory.properties.cpp
    │   │   │   │   ├── RecyclingElementFactory.properties.h
    │   │   │   │   ├── RefreshContainer.properties.cpp
    │   │   │   │   ├── RefreshContainer.properties.h
    │   │   │   │   ├── RefreshVisualizer.properties.cpp
    │   │   │   │   ├── RefreshVisualizer.properties.h
    │   │   │   │   ├── RepeatedScrollSnapPoint.properties.cpp
    │   │   │   │   ├── RepeatedZoomSnapPoint.properties.cpp
    │   │   │   │   ├── RepeaterAutomationPeer.properties.cpp
    │   │   │   │   ├── RepeaterTestHooks.properties.cpp
    │   │   │   │   ├── RevealBackgroundBrush.properties.cpp
    │   │   │   │   ├── RevealBorderBrush.properties.cpp
    │   │   │   │   ├── RevealBorderLight.properties.cpp
    │   │   │   │   ├── RevealBrush.properties.cpp
    │   │   │   │   ├── RevealBrush.properties.h
    │   │   │   │   ├── RevealBrushTestApi.properties.cpp
    │   │   │   │   ├── RevealHoverLight.properties.cpp
    │   │   │   │   ├── RevealListViewItemPresenter.properties.cpp
    │   │   │   │   ├── RevealTestApi.properties.cpp
    │   │   │   │   ├── ScrollControllerAddScrollVelocityRequestedEventArgs.properties.cpp
    │   │   │   │   ├── ScrollControllerPanRequestedEventArgs.properties.cpp
    │   │   │   │   ├── ScrollControllerScrollByRequestedEventArgs.properties.cpp
    │   │   │   │   ├── ScrollControllerScrollToRequestedEventArgs.properties.cpp
    │   │   │   │   ├── ScrollingScrollOptions.properties.cpp
    │   │   │   │   ├── ScrollingZoomOptions.properties.cpp
    │   │   │   │   ├── ScrollPresenter.properties.cpp
    │   │   │   │   ├── ScrollPresenter.properties.h
    │   │   │   │   ├── ScrollPresenterAutomationPeer.properties.cpp
    │   │   │   │   ├── ScrollPresenterTestHooks.properties.cpp
    │   │   │   │   ├── ScrollSnapPoint.properties.cpp
    │   │   │   │   ├── ScrollSnapPointBase.properties.cpp
    │   │   │   │   ├── ScrollView.properties.cpp
    │   │   │   │   ├── ScrollView.properties.h
    │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter.properties.cpp
    │   │   │   │   ├── ScrollViewTestHooks.properties.cpp
    │   │   │   │   ├── SelectionModel.properties.cpp
    │   │   │   │   ├── SelectionModel.properties.h
    │   │   │   │   ├── SelectorBar.properties.cpp
    │   │   │   │   ├── SelectorBar.properties.h
    │   │   │   │   ├── SelectorBarItem.properties.cpp
    │   │   │   │   ├── SelectorBarItem.properties.h
    │   │   │   │   ├── SelectorBarItemAutomationPeer.properties.cpp
    │   │   │   │   ├── SelectorBarTestHooks.properties.cpp
    │   │   │   │   ├── SliderInteraction.properties.cpp
    │   │   │   │   ├── SliderInteraction.properties.h
    │   │   │   │   ├── SnapPointBase.properties.cpp
    │   │   │   │   ├── SpectrumBrush.properties.cpp
    │   │   │   │   ├── SpectrumBrush.properties.h
    │   │   │   │   ├── SplitButton.properties.cpp
    │   │   │   │   ├── SplitButton.properties.h
    │   │   │   │   ├── SplitButtonAutomationPeer.properties.cpp
    │   │   │   │   ├── SplitButtonTestApi.properties.cpp
    │   │   │   │   ├── StackLayout.properties.cpp
    │   │   │   │   ├── StackLayout.properties.h
    │   │   │   │   ├── StackLayoutState.properties.cpp
    │   │   │   │   ├── SwipeControl.properties.cpp
    │   │   │   │   ├── SwipeControl.properties.h
    │   │   │   │   ├── SwipeItem.properties.cpp
    │   │   │   │   ├── SwipeItem.properties.h
    │   │   │   │   ├── SwipeItems.properties.cpp
    │   │   │   │   ├── SwipeItems.properties.h
    │   │   │   │   ├── SwipeTestHooks.properties.cpp
    │   │   │   │   ├── TabView.properties.cpp
    │   │   │   │   ├── TabView.properties.h
    │   │   │   │   ├── TabViewAutomationPeer.properties.cpp
    │   │   │   │   ├── TabViewItem.properties.cpp
    │   │   │   │   ├── TabViewItem.properties.h
    │   │   │   │   ├── TabViewItemAutomationPeer.properties.cpp
    │   │   │   │   ├── TabViewItemTemplateSettings.properties.cpp
    │   │   │   │   ├── TabViewItemTemplateSettings.properties.h
    │   │   │   │   ├── TabViewListView.properties.cpp
    │   │   │   │   ├── TeachingTip.properties.cpp
    │   │   │   │   ├── TeachingTip.properties.h
    │   │   │   │   ├── TeachingTipAutomationPeer.properties.cpp
    │   │   │   │   ├── TeachingTipTemplateSettings.properties.cpp
    │   │   │   │   ├── TeachingTipTemplateSettings.properties.h
    │   │   │   │   ├── TeachingTipTestHooks.properties.cpp
    │   │   │   │   ├── TextCommandBarFlyout.properties.cpp
    │   │   │   │   ├── TitleBar.properties.cpp
    │   │   │   │   ├── TitleBar.properties.h
    │   │   │   │   ├── TitleBarAutomationPeer.properties.cpp
    │   │   │   │   ├── TitleBarTemplateSettings.properties.cpp
    │   │   │   │   ├── TitleBarTemplateSettings.properties.h
    │   │   │   │   ├── ToggleSplitButton.properties.cpp
    │   │   │   │   ├── ToggleSplitButton.properties.h
    │   │   │   │   ├── ToggleSplitButtonAutomationPeer.properties.cpp
    │   │   │   │   ├── TreeView.properties.cpp
    │   │   │   │   ├── TreeView.properties.h
    │   │   │   │   ├── TreeViewItem.properties.cpp
    │   │   │   │   ├── TreeViewItem.properties.h
    │   │   │   │   ├── TreeViewItemAutomationPeer.properties.cpp
    │   │   │   │   ├── TreeViewItemDataAutomationPeer.properties.cpp
    │   │   │   │   ├── TreeViewItemTemplateSettings.properties.cpp
    │   │   │   │   ├── TreeViewItemTemplateSettings.properties.h
    │   │   │   │   ├── TreeViewList.properties.cpp
    │   │   │   │   ├── TreeViewListAutomationPeer.properties.cpp
    │   │   │   │   ├── TreeViewNode.properties.cpp
    │   │   │   │   ├── TreeViewNode.properties.h
    │   │   │   │   ├── TwoPaneView.properties.cpp
    │   │   │   │   ├── TwoPaneView.properties.h
    │   │   │   │   ├── UniformGridLayout.properties.cpp
    │   │   │   │   ├── UniformGridLayout.properties.h
    │   │   │   │   ├── UniformGridLayoutState.properties.cpp
    │   │   │   │   ├── VirtualizingLayout.properties.cpp
    │   │   │   │   ├── VirtualizingLayoutContext.properties.cpp
    │   │   │   │   ├── WebView2.properties.cpp
    │   │   │   │   ├── WebView2.properties.h
    │   │   │   │   ├── WebView2AutomationPeer.properties.cpp
    │   │   │   │   ├── XamlAmbientLight.properties.cpp
    │   │   │   │   ├── XamlAmbientLight.properties.h
    │   │   │   │   ├── XamlControlsResources.properties.cpp
    │   │   │   │   ├── XamlControlsResources.properties.h
    │   │   │   │   ├── XamlControlsXamlMetaDataProvider.properties.cpp
    │   │   │   │   ├── ZoomSnapPoint.properties.cpp
    │   │   │   │   └── ZoomSnapPointBase.properties.cpp
    │   │   │   ├── IconSource/
    │   │   │   │   ├── AnimatedIconSource.cpp
    │   │   │   │   ├── AnimatedIconSource.h
    │   │   │   │   ├── IconSource.idl
    │   │   │   │   ├── IconSource.vcxitems
    │   │   │   │   ├── ImageIconSource.cpp
    │   │   │   │   ├── ImageIconSource.h
    │   │   │   │   └── APITests/
    │   │   │   │       ├── IconSource_APITests.projitems
    │   │   │   │       ├── IconSource_APITests.shproj
    │   │   │   │       └── IconSourceApiTests.cs
    │   │   │   ├── ImageIcon/
    │   │   │   │   ├── ImageIcon.cpp
    │   │   │   │   ├── ImageIcon.h
    │   │   │   │   ├── ImageIcon.idl
    │   │   │   │   ├── ImageIcon.vcxitems
    │   │   │   │   ├── ImageIcon.xaml
    │   │   │   │   ├── ImageIcon_themeresources.xaml
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ImageIcon_APITests.projitems
    │   │   │   │   │   ├── ImageIcon_APITests.shproj
    │   │   │   │   │   └── ImageIconTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ImageIcon_InteractionTests.projitems
    │   │   │   │   │   ├── ImageIcon_InteractionTests.shproj
    │   │   │   │   │   └── ImageIconTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ImageIcon_TestUI.projitems
    │   │   │   │       ├── ImageIcon_TestUI.shproj
    │   │   │   │       ├── ImageIconPage.xaml
    │   │   │   │       └── ImageIconPage.xaml.cs
    │   │   │   ├── inc/
    │   │   │   │   ├── AutoHandle.h
    │   │   │   │   ├── BoxHelpers.h
    │   │   │   │   ├── BuildMacros.h
    │   │   │   │   ├── CastHelpers.h
    │   │   │   │   ├── CollectionHelper.h
    │   │   │   │   ├── CommandingHelpers.h
    │   │   │   │   ├── common.h
    │   │   │   │   ├── CppWinRTHelpers.h
    │   │   │   │   ├── CppWinRTIncludes.h
    │   │   │   │   ├── DispatcherHelper.h
    │   │   │   │   ├── DoubleUtil.h
    │   │   │   │   ├── enum_array.h
    │   │   │   │   ├── enum_vector.h
    │   │   │   │   ├── ErrorHandling.h
    │   │   │   │   ├── event.h
    │   │   │   │   ├── FloatUtil.h
    │   │   │   │   ├── FocusHelper.h
    │   │   │   │   ├── GlobalDependencyProperty.h
    │   │   │   │   ├── RegUtil.h
    │   │   │   │   ├── RoutedEventHelpers.h
    │   │   │   │   ├── RuntimeClassHelpers.h
    │   │   │   │   ├── SharedHelpers.h
    │   │   │   │   ├── StaticAssertFalse.h
    │   │   │   │   ├── tracker_ref.h
    │   │   │   │   ├── velocity.h
    │   │   │   │   ├── WinEventLogLevels.h
    │   │   │   │   └── gsl/
    │   │   │   │       ├── ReadMe.md
    │   │   │   │       ├── gsl
    │   │   │   │       ├── gsl_algorithm
    │   │   │   │       ├── gsl_assert
    │   │   │   │       ├── gsl_byte
    │   │   │   │       ├── gsl_util
    │   │   │   │       ├── multi_span
    │   │   │   │       ├── pointers
    │   │   │   │       ├── span
    │   │   │   │       └── string_span
    │   │   │   ├── InfoBadge/
    │   │   │   │   ├── InfoBadge.cpp
    │   │   │   │   ├── InfoBadge.h
    │   │   │   │   ├── InfoBadge.idl
    │   │   │   │   ├── InfoBadge.vcxitems
    │   │   │   │   ├── InfoBadge.xaml
    │   │   │   │   ├── InfoBadge_themeresources.xaml
    │   │   │   │   ├── InfoBadgeTemplateSettings.cpp
    │   │   │   │   ├── InfoBadgeTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── InfoBadge_APITests.projitems
    │   │   │   │   │   ├── InfoBadge_APITests.shproj
    │   │   │   │   │   └── InfoBadgeTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── InfoBadge_InteractionTests.projitems
    │   │   │   │   │   └── InfoBadge_InteractionTests.shproj
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── InfoBadge_TestUI.projitems
    │   │   │   │       ├── InfoBadge_TestUI.shproj
    │   │   │   │       ├── InfoBadgePage.xaml
    │   │   │   │       └── InfoBadgePage.xaml.cs
    │   │   │   ├── InfoBar/
    │   │   │   │   ├── InfoBar.cpp
    │   │   │   │   ├── InfoBar.h
    │   │   │   │   ├── InfoBar.idl
    │   │   │   │   ├── InfoBar.vcxitems
    │   │   │   │   ├── InfoBar.xaml
    │   │   │   │   ├── InfoBar_themeresources.xaml
    │   │   │   │   ├── InfoBarAutomationPeer.cpp
    │   │   │   │   ├── InfoBarAutomationPeer.h
    │   │   │   │   ├── InfoBarClosedEventArgs.cpp
    │   │   │   │   ├── InfoBarClosedEventArgs.h
    │   │   │   │   ├── InfoBarClosingEventArgs.cpp
    │   │   │   │   ├── InfoBarClosingEventArgs.h
    │   │   │   │   ├── InfoBarPanel.cpp
    │   │   │   │   ├── InfoBarPanel.h
    │   │   │   │   ├── InfoBarTemplateSettings.cpp
    │   │   │   │   ├── InfoBarTemplateSettings.h
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── InfoBar_InteractionTests.projitems
    │   │   │   │   │   ├── InfoBar_InteractionTests.shproj
    │   │   │   │   │   └── InfoBarTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── InfoBar_TestUI.projitems
    │   │   │   │       ├── InfoBar_TestUI.shproj
    │   │   │   │       ├── InfobarAxeTestage.xaml
    │   │   │   │       ├── InfobarAxeTestage.xaml.cs
    │   │   │   │       ├── InfoBarPage.xaml
    │   │   │   │       └── InfoBarPage.xaml.cs
    │   │   │   ├── InkCanvas/
    │   │   │   │   ├── InkCanvas.cpp
    │   │   │   │   ├── InkCanvas.h
    │   │   │   │   ├── InkCanvas.idl
    │   │   │   │   ├── InkCanvas.vcxitems
    │   │   │   │   ├── InkCanvasAutomationPeer.cpp
    │   │   │   │   ├── InkCanvasAutomationPeer.h
    │   │   │   │   └── InkCanvasAutomationPeer.idl
    │   │   │   ├── InkToolBar/
    │   │   │   │   ├── InkToolBar.h
    │   │   │   │   ├── InkToolBar.idl
    │   │   │   │   ├── InkToolBar.vcxitems
    │   │   │   │   ├── InkToolBar_themeresources.xaml
    │   │   │   │   ├── InkToolbarAutomationPeer.h
    │   │   │   │   ├── InkToolBarAutomationPeer.idl
    │   │   │   │   ├── InkToolBarBallpointPenButton.h
    │   │   │   │   ├── InkToolBarCustomPen.h
    │   │   │   │   ├── InkToolBarCustomPenButton.h
    │   │   │   │   ├── InkToolBarCustomToggleButton.h
    │   │   │   │   ├── InkToolBarCustomToolButton.h
    │   │   │   │   ├── InkToolBarEraserButton.h
    │   │   │   │   ├── InkToolBarEraserButtonInternal.h
    │   │   │   │   ├── InkToolBarEraserFlyoutItemClickedEventArgs.h
    │   │   │   │   ├── InkToolBarFlyoutItem.h
    │   │   │   │   ├── InkToolBarFlyoutItemAutomationPeer.h
    │   │   │   │   ├── InkToolBarHighlighterButton.h
    │   │   │   │   ├── InkToolBarIsStencilButtonCheckedChangedEventArgs.h
    │   │   │   │   ├── InkToolBarMenuButton.h
    │   │   │   │   ├── InkToolBarMenuButtonAutomationPeer.h
    │   │   │   │   ├── InkToolBarPenButton.h
    │   │   │   │   ├── InktoolBarPencilButton.h
    │   │   │   │   ├── InkToolBarPenConfigurationControl.h
    │   │   │   │   ├── InkToolBarStencilButton.h
    │   │   │   │   ├── InkToolBarToggleButton.h
    │   │   │   │   ├── InkToolBarToolButton.h
    │   │   │   │   ├── InkToolBarToolButtonAutomationPeer.h
    │   │   │   │   └── InkToolBarTrace.h
    │   │   │   ├── Interactions/
    │   │   │   │   ├── ButtonInteraction/
    │   │   │   │   │   ├── ButtonInteraction.cpp
    │   │   │   │   │   ├── ButtonInteraction.h
    │   │   │   │   │   ├── ButtonInteraction.idl
    │   │   │   │   │   ├── ButtonInteraction.vcxitems
    │   │   │   │   │   ├── ButtonInteractionInvokedEventArgs.cpp
    │   │   │   │   │   ├── ButtonInteractionInvokedEventArgs.h
    │   │   │   │   │   ├── APITests/
    │   │   │   │   │   │   ├── ButtonInteraction_APITests.projitems
    │   │   │   │   │   │   ├── ButtonInteraction_APITests.shproj
    │   │   │   │   │   │   └── ButtonInteractionTests.cs
    │   │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   │   ├── ButtonInteraction_InteractionTests.projitems
    │   │   │   │   │   │   ├── ButtonInteraction_InteractionTests.shproj
    │   │   │   │   │   │   └── ButtonInteractionTests.cs
    │   │   │   │   │   └── TestUI/
    │   │   │   │   │       ├── ButtonInteraction_TestUI.projitems
    │   │   │   │   │       ├── ButtonInteraction_TestUI.shproj
    │   │   │   │   │       ├── ButtonInteractionPage.xaml
    │   │   │   │   │       ├── ButtonInteractionPage.xaml.cs
    │   │   │   │   │       ├── TargetElement.xaml
    │   │   │   │   │       └── TargetElement.xaml.cs
    │   │   │   │   └── SliderInteraction/
    │   │   │   │       ├── SliderInteraction.cpp
    │   │   │   │       ├── SliderInteraction.h
    │   │   │   │       ├── SliderInteraction.idl
    │   │   │   │       ├── SliderInteraction.vcxitems
    │   │   │   │       ├── APITests/
    │   │   │   │       │   ├── SliderInteraction_APITests.projitems
    │   │   │   │       │   ├── SliderInteraction_APITests.shproj
    │   │   │   │       │   └── SliderInteractionTests.cs
    │   │   │   │       ├── InteractionTests/
    │   │   │   │       │   ├── SliderInteraction_InteractionTests.projitems
    │   │   │   │       │   ├── SliderInteraction_InteractionTests.shproj
    │   │   │   │       │   └── SliderInteractionTests.cs
    │   │   │   │       └── TestUI/
    │   │   │   │           ├── SliderInteraction_TestUI.projitems
    │   │   │   │           ├── SliderInteraction_TestUI.shproj
    │   │   │   │           ├── SliderInteractionPage.xaml
    │   │   │   │           └── SliderInteractionPage.xaml.cs
    │   │   │   ├── ItemContainer/
    │   │   │   │   ├── ItemContainer.cpp
    │   │   │   │   ├── ItemContainer.h
    │   │   │   │   ├── ItemContainer.idl
    │   │   │   │   ├── ItemContainer.vcxitems
    │   │   │   │   ├── ItemContainer.xaml
    │   │   │   │   ├── ItemContainer_themeresources.xaml
    │   │   │   │   ├── ItemContainerAutomationPeer.cpp
    │   │   │   │   ├── ItemContainerAutomationPeer.h
    │   │   │   │   ├── ItemContainerInvokedEventArgs.cpp
    │   │   │   │   ├── ItemContainerInvokedEventArgs.h
    │   │   │   │   ├── ItemContainerRevokers.h
    │   │   │   │   ├── ItemContainerTrace.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ItemContainer_APITests.projitems
    │   │   │   │   │   ├── ItemContainer_APITests.shproj
    │   │   │   │   │   └── ItemContainerTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ItemContainer_InteractionTests.projitems
    │   │   │   │   │   ├── ItemContainer_InteractionTests.shproj
    │   │   │   │   │   └── ItemContainerTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ItemContainer_TestUI.projitems
    │   │   │   │       ├── ItemContainer_TestUI.shproj
    │   │   │   │       ├── ItemContainerLayoutPage.xaml
    │   │   │   │       ├── ItemContainerLayoutPage.xaml.cs
    │   │   │   │       ├── ItemContainerPage.xaml
    │   │   │   │       ├── ItemContainerPage.xaml.cs
    │   │   │   │       ├── ItemContainerSummaryPage.xaml
    │   │   │   │       └── ItemContainerSummaryPage.xaml.cs
    │   │   │   ├── ItemsView/
    │   │   │   │   ├── ExtendedSelector.cpp
    │   │   │   │   ├── ExtendedSelector.h
    │   │   │   │   ├── ItemsView.cpp
    │   │   │   │   ├── ItemsView.h
    │   │   │   │   ├── ItemsView.idl
    │   │   │   │   ├── ItemsView.vcxitems
    │   │   │   │   ├── ItemsView.xaml
    │   │   │   │   ├── ItemsView_themeresources.xaml
    │   │   │   │   ├── ItemsViewAutomationPeer.cpp
    │   │   │   │   ├── ItemsViewAutomationPeer.h
    │   │   │   │   ├── ItemsViewInteractions.cpp
    │   │   │   │   ├── ItemsViewItemInvokedEventArgs.cpp
    │   │   │   │   ├── ItemsViewItemInvokedEventArgs.h
    │   │   │   │   ├── ItemsViewSelectionChangedEventArgs.cpp
    │   │   │   │   ├── ItemsViewSelectionChangedEventArgs.h
    │   │   │   │   ├── ItemsViewTestHooks.cpp
    │   │   │   │   ├── ItemsViewTestHooks.h
    │   │   │   │   ├── ItemsViewTestHooks.idl
    │   │   │   │   ├── ItemsViewTestHooksFactory.cpp
    │   │   │   │   ├── ItemsViewTestHooksFactory.h
    │   │   │   │   ├── ItemsViewTrace.h
    │   │   │   │   ├── MultipleSelector.cpp
    │   │   │   │   ├── MultipleSelector.h
    │   │   │   │   ├── NullSelector.cpp
    │   │   │   │   ├── NullSelector.h
    │   │   │   │   ├── SelectorBase.cpp
    │   │   │   │   ├── SelectorBase.h
    │   │   │   │   ├── SingleSelector.cpp
    │   │   │   │   ├── SingleSelector.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ItemsView_APITests.projitems
    │   │   │   │   │   ├── ItemsView_APITests.shproj
    │   │   │   │   │   └── ItemsViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ItemsView_InteractionTests.projitems
    │   │   │   │   │   ├── ItemsView_InteractionTests.shproj
    │   │   │   │   │   └── ItemsViewTestsWithInputHelper.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ItemsView_TestUI.projitems
    │   │   │   │       ├── ItemsView_TestUI.shproj
    │   │   │   │       ├── ItemsViewBlankPage.xaml
    │   │   │   │       ├── ItemsViewBlankPage.xaml.cs
    │   │   │   │       ├── ItemsViewIntegrationPage.xaml
    │   │   │   │       ├── ItemsViewIntegrationPage.xaml.cs
    │   │   │   │       ├── ItemsViewInteractiveTestsPage.xaml
    │   │   │   │       ├── ItemsViewInteractiveTestsPage.xaml.cs
    │   │   │   │       ├── ItemsViewPage.xaml
    │   │   │   │       ├── ItemsViewPage.xaml.cs
    │   │   │   │       ├── ItemsViewPictureLibraryPage.xaml
    │   │   │   │       ├── ItemsViewPictureLibraryPage.xaml.cs
    │   │   │   │       ├── ItemsViewSummaryPage.xaml
    │   │   │   │       ├── ItemsViewSummaryPage.xaml.cs
    │   │   │   │       ├── ItemsViewTransitionPage.xaml
    │   │   │   │       └── ItemsViewTransitionPage.xaml.cs
    │   │   │   ├── LayoutPanel/
    │   │   │   │   ├── LayoutPanel.cpp
    │   │   │   │   ├── LayoutPanel.h
    │   │   │   │   ├── LayoutPanel.idl
    │   │   │   │   ├── LayoutPanel.vcxitems
    │   │   │   │   ├── LayoutPanelLayoutContext.cpp
    │   │   │   │   ├── LayoutPanelLayoutContext.h
    │   │   │   │   └── APITests/
    │   │   │   │       ├── LayoutPanel_APITests.projitems
    │   │   │   │       ├── LayoutPanel_APITests.shproj
    │   │   │   │       └── LayoutPanelTests.cs
    │   │   │   ├── Lights/
    │   │   │   │   ├── AnimationUtility.cpp
    │   │   │   │   ├── AnimationUtility.h
    │   │   │   │   ├── IsTargetDPHelper.h
    │   │   │   │   ├── Lights.vcxitems
    │   │   │   │   ├── MaterialHelper.cpp
    │   │   │   │   ├── MaterialHelper.h
    │   │   │   │   ├── MaterialHelperTestApi.cpp
    │   │   │   │   ├── MaterialHelperTestApi.h
    │   │   │   │   ├── MaterialHelperTestApi.idl
    │   │   │   │   ├── MaterialHelperTestApiFactory.cpp
    │   │   │   │   ├── MaterialHelperTestApiFactory.h
    │   │   │   │   ├── RevealBorderLight.cpp
    │   │   │   │   ├── RevealBorderLight.h
    │   │   │   │   ├── RevealBorderLight.idl
    │   │   │   │   ├── RevealHoverLight.cpp
    │   │   │   │   ├── RevealHoverLight.h
    │   │   │   │   ├── RevealHoverLight.idl
    │   │   │   │   ├── RevealTestApi.cpp
    │   │   │   │   ├── RevealTestApi.h
    │   │   │   │   ├── RevealTestApi.idl
    │   │   │   │   ├── SpotLightStateHelper.cpp
    │   │   │   │   ├── SpotLightStateHelper.h
    │   │   │   │   ├── XamlAmbientLight.cpp
    │   │   │   │   ├── XamlAmbientLight.h
    │   │   │   │   ├── XamlAmbientLight.idl
    │   │   │   │   └── ApiTests/
    │   │   │   │       └── Lights_ApiTests/
    │   │   │   │           ├── LightConfigurationTests.cs
    │   │   │   │           ├── Lights_ApiTests.projitems
    │   │   │   │           └── Lights_ApiTests.shproj
    │   │   │   ├── Lightup/
    │   │   │   │   └── Microsoft.UI.Xaml.Controls.Lightup.vcxproj
    │   │   │   ├── MapControl/
    │   │   │   │   ├── map.html
    │   │   │   │   ├── MapControl.cpp
    │   │   │   │   ├── MapControl.h
    │   │   │   │   ├── MapControl.idl
    │   │   │   │   ├── MapControl.vcxitems
    │   │   │   │   ├── MapControl.xaml
    │   │   │   │   ├── MapControlMapServiceErrorOccurredEventArgs.cpp
    │   │   │   │   ├── MapControlMapServiceErrorOccurredEventArgs.h
    │   │   │   │   ├── MapElement.cpp
    │   │   │   │   ├── MapElement.h
    │   │   │   │   ├── MapElementClickEventArgs.cpp
    │   │   │   │   ├── MapElementClickEventArgs.h
    │   │   │   │   ├── MapElementsLayer.cpp
    │   │   │   │   ├── MapElementsLayer.h
    │   │   │   │   ├── MapIcon.cpp
    │   │   │   │   ├── MapIcon.h
    │   │   │   │   ├── MapLayer.cpp
    │   │   │   │   ├── MapLayer.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── MapControl_APITests.projitems
    │   │   │   │   │   ├── MapControl_APITests.shproj
    │   │   │   │   │   └── MapControlTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── MapControl_InteractionTests.projitems
    │   │   │   │   │   ├── MapControl_InteractionTests.shproj
    │   │   │   │   │   └── MapControlTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── MapControl_TestUI.projitems
    │   │   │   │       ├── MapControl_TestUI.shproj
    │   │   │   │       ├── MapControlApiKey.cs
    │   │   │   │       ├── MapControlPage.xaml
    │   │   │   │       └── MapControlPage.xaml.cs
    │   │   │   ├── Materials/
    │   │   │   │   ├── Acrylic/
    │   │   │   │   │   ├── AcrylicBrush.cpp
    │   │   │   │   │   ├── AcrylicBrush.h
    │   │   │   │   │   ├── AcrylicBrush.idl
    │   │   │   │   │   ├── AcrylicBrush.vcxitems
    │   │   │   │   │   ├── AcrylicBrush_themeresources.xaml
    │   │   │   │   │   ├── AcrylicBrushFactory.cpp
    │   │   │   │   │   ├── AcrylicBrushFactory.h
    │   │   │   │   │   ├── AcrylicTestApi.cpp
    │   │   │   │   │   ├── AcrylicTestApi.h
    │   │   │   │   │   ├── AcrylicTestApi.idl
    │   │   │   │   │   ├── APITests/
    │   │   │   │   │   │   ├── AcrylicBrush_ApiTests.projitems
    │   │   │   │   │   │   ├── AcrylicBrush_ApiTests.shproj
    │   │   │   │   │   │   └── AcrylicBrushTests.cs
    │   │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   │   ├── AcrylicBrush_InteractionTests.projitems
    │   │   │   │   │   │   ├── AcrylicBrush_InteractionTests.shproj
    │   │   │   │   │   │   └── AcrylicBrushTests.cs
    │   │   │   │   │   └── TestUI/
    │   │   │   │   │       ├── AcrylicBrush_TestUI.projitems
    │   │   │   │   │       ├── AcrylicBrush_TestUI.shproj
    │   │   │   │   │       ├── AcrylicBrushBasicPage.xaml
    │   │   │   │   │       ├── AcrylicBrushBasicPage.xaml.cs
    │   │   │   │   │       ├── AcrylicBrushLuminosityTestPage.xaml
    │   │   │   │   │       ├── AcrylicBrushLuminosityTestPage.xaml.cs
    │   │   │   │   │       ├── AcrylicBrushPage.xaml
    │   │   │   │   │       ├── AcrylicBrushPage.xaml.cs
    │   │   │   │   │       ├── AcrylicColorPage.xaml
    │   │   │   │   │       ├── AcrylicColorPage.xaml.cs
    │   │   │   │   │       ├── AcrylicMarkupPage.xaml
    │   │   │   │   │       ├── AcrylicMarkupPage.xaml.cs
    │   │   │   │   │       ├── AcrylicPage.xaml
    │   │   │   │   │       ├── AcrylicPage.xaml.cs
    │   │   │   │   │       ├── AcrylicRenderingPage.xaml
    │   │   │   │   │       ├── AcrylicRenderingPage.xaml.cs
    │   │   │   │   │       └── AcrylicBrush_TestUI/
    │   │   │   │   │           ├── AcrylicBrush_TestUI.projitems
    │   │   │   │   │           └── AcrylicBrush_TestUI.shproj
    │   │   │   │   ├── DesktopAcrylicBackdrop/
    │   │   │   │   │   ├── DesktopAcrylicBackdrop.cpp
    │   │   │   │   │   ├── DesktopAcrylicBackdrop.h
    │   │   │   │   │   ├── DesktopAcrylicBackdrop.idl
    │   │   │   │   │   └── DesktopAcrylicBackdrop.vcxitems
    │   │   │   │   ├── MicaBackdrop/
    │   │   │   │   │   ├── MicaBackdrop.cpp
    │   │   │   │   │   ├── MicaBackdrop.h
    │   │   │   │   │   ├── MicaBackdrop.idl
    │   │   │   │   │   └── MicaBackdrop.vcxitems
    │   │   │   │   └── Reveal/
    │   │   │   │       ├── RevealBackgroundBrush.h
    │   │   │   │       ├── RevealBorderBrush.h
    │   │   │   │       ├── RevealBrush.cpp
    │   │   │   │       ├── RevealBrush.h
    │   │   │   │       ├── RevealBrush.idl
    │   │   │   │       ├── RevealBrush.vcxitems
    │   │   │   │       ├── RevealBrush_themeresources.xaml
    │   │   │   │       ├── RevealBrushTestApi.cpp
    │   │   │   │       ├── RevealBrushTestApi.h
    │   │   │   │       ├── RevealBrushTestApi.idl
    │   │   │   │       ├── RevealControls.idl
    │   │   │   │       ├── RevealListViewItemPresenter.cpp
    │   │   │   │       ├── RevealListViewItemPresenter.h
    │   │   │   │       ├── APITests/
    │   │   │   │       │   ├── Reveal_APITests.projitems
    │   │   │   │       │   ├── Reveal_APITests.shproj
    │   │   │   │       │   └── RevealTests.cs
    │   │   │   │       ├── InteractionTests/
    │   │   │   │       │   └── Reveal_InteractionTests/
    │   │   │   │       │       ├── Reveal_InteractionTests.projitems
    │   │   │   │       │       ├── Reveal_InteractionTests.shproj
    │   │   │   │       │       └── RevealBrushTests.cs
    │   │   │   │       └── TestUI/
    │   │   │   │           ├── CoreWindowEventsPage.xaml
    │   │   │   │           ├── CoreWindowEventsPage.xaml.cs
    │   │   │   │           ├── Reveal_TestUI.projitems
    │   │   │   │           ├── Reveal_TestUI.shproj
    │   │   │   │           ├── RevealBasicPage.xaml
    │   │   │   │           ├── RevealBasicPage.xaml.cs
    │   │   │   │           ├── RevealColorPage.xaml
    │   │   │   │           ├── RevealColorPage.xaml.cs
    │   │   │   │           ├── RevealFallbackPage.xaml
    │   │   │   │           ├── RevealFallbackPage.xaml.cs
    │   │   │   │           ├── RevealListPage.xaml
    │   │   │   │           ├── RevealListPage.xaml.cs
    │   │   │   │           ├── RevealMarkupPage.xaml
    │   │   │   │           ├── RevealMarkupPage.xaml.cs
    │   │   │   │           ├── RevealPage.xaml
    │   │   │   │           ├── RevealPage.xaml.cs
    │   │   │   │           ├── RevealRegressionTestsPage.xaml
    │   │   │   │           ├── RevealRegressionTestsPage.xaml.cs
    │   │   │   │           ├── RevealScenarioColors.xaml
    │   │   │   │           ├── RevealScenarioColors.xaml.cs
    │   │   │   │           ├── RevealScenarioGrid.xaml
    │   │   │   │           ├── RevealScenarioGrid.xaml.cs
    │   │   │   │           ├── RevealScenarioLights.xaml
    │   │   │   │           ├── RevealScenarioLights.xaml.cs
    │   │   │   │           ├── RevealScenarioList.xaml
    │   │   │   │           ├── RevealScenarioList.xaml.cs
    │   │   │   │           ├── RevealScenarios.xaml
    │   │   │   │           ├── RevealScenarios.xaml.cs
    │   │   │   │           ├── RevealScenarioSecondaryView.xaml
    │   │   │   │           ├── RevealScenarioSecondaryView.xaml.cs
    │   │   │   │           ├── RevealSimpleListPage.xaml
    │   │   │   │           ├── RevealSimpleListPage.xaml.cs
    │   │   │   │           ├── RevealStatesPage.xaml
    │   │   │   │           └── RevealStatesPage.xaml.cs
    │   │   │   ├── MenuBar/
    │   │   │   │   ├── MenuBar.cpp
    │   │   │   │   ├── MenuBar.h
    │   │   │   │   ├── MenuBar.idl
    │   │   │   │   ├── MenuBar.vcxitems
    │   │   │   │   ├── MenuBar.xaml
    │   │   │   │   ├── MenuBar_themeresources.xaml
    │   │   │   │   ├── MenuBarAutomationPeer.cpp
    │   │   │   │   ├── MenuBarAutomationPeer.h
    │   │   │   │   ├── MenuBarAutomationPeer.idl
    │   │   │   │   ├── MenuBarItem.cpp
    │   │   │   │   ├── MenuBarItem.h
    │   │   │   │   ├── MenuBarItem.xaml
    │   │   │   │   ├── MenuBarItemAutomationPeer.cpp
    │   │   │   │   ├── MenuBarItemAutomationPeer.h
    │   │   │   │   ├── MenuBarItemFlyout.cpp
    │   │   │   │   ├── MenuBarItemFlyout.h
    │   │   │   │   ├── MenuBar_InteractionTests/
    │   │   │   │   │   ├── MenuBar_InteractionTests.projitems
    │   │   │   │   │   ├── MenuBar_InteractionTests.shproj
    │   │   │   │   │   └── MenuBarTests.cs
    │   │   │   │   └── MenuBar_TestUI/
    │   │   │   │       ├── MenuBar_TestUI.projitems
    │   │   │   │       ├── MenuBar_TestUI.shproj
    │   │   │   │       ├── MenuBarPage.xaml
    │   │   │   │       └── MenuBarPage.xaml.cs
    │   │   │   ├── Microsoft.UI.Xaml.Design/
    │   │   │   │   ├── Microsoft.UI.Xaml.Design.csproj
    │   │   │   │   ├── RegisterMetadata.cs
    │   │   │   │   ├── Icons/
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.ColorPicker.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.CommandBarFlyout.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.DropDownButton.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.MenuBar.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.NavigationView.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.ParallaxView.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.PersonPicture.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.RatingControl.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.RefreshContainer.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.SplitButton.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.SwipeControl.bmp
    │   │   │   │   │   ├── Microsoft.UI.Xaml.Controls.ToggleSplitButton.bmp
    │   │   │   │   │   └── Microsoft.UI.Xaml.Controls.TreeView.bmp
    │   │   │   │   └── Properties/
    │   │   │   │       └── AssemblyInfo.cs
    │   │   │   ├── Microsoft.UI.Xaml.FrameworkPackagePRI/
    │   │   │   │   ├── README.md
    │   │   │   │   ├── Microsoft.UI.Xaml.FrameworkPackagePRI.csproj
    │   │   │   │   └── Properties/
    │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │       └── Microsoft.UI.Xaml.rd.xml
    │   │   │   ├── MonochromaticOverlayPresenter/
    │   │   │   │   ├── MonochromaticOverlayPresenter.cpp
    │   │   │   │   ├── MonochromaticOverlayPresenter.h
    │   │   │   │   ├── MonochromaticOverlayPresenter.idl
    │   │   │   │   ├── MonochromaticOverlayPresenter.vcxitems
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── MonochromaticOverlayPresenter_TestUI.projitems
    │   │   │   │       ├── MonochromaticOverlayPresenter_TestUI.shproj
    │   │   │   │       ├── MonochromaticOverlayPresenterPage.xaml
    │   │   │   │       └── MonochromaticOverlayPresenterPage.xaml.cs
    │   │   │   ├── NavigationView/
    │   │   │   │   ├── readme.md
    │   │   │   │   ├── NavigationBackButton.xaml
    │   │   │   │   ├── NavigationBackButton_themeresources.xaml
    │   │   │   │   ├── NavigationView.cpp
    │   │   │   │   ├── NavigationView.h
    │   │   │   │   ├── NavigationView.idl
    │   │   │   │   ├── NavigationView.vcxitems
    │   │   │   │   ├── NavigationView.xaml
    │   │   │   │   ├── NavigationView_themeresources.xaml
    │   │   │   │   ├── NavigationViewAutomationPeer.cpp
    │   │   │   │   ├── NavigationViewAutomationPeer.h
    │   │   │   │   ├── NavigationViewBackRequestedEventArgs.cpp
    │   │   │   │   ├── NavigationViewBackRequestedEventArgs.h
    │   │   │   │   ├── NavigationViewDisplayModeChangedEventArgs.cpp
    │   │   │   │   ├── NavigationViewDisplayModeChangedEventArgs.h
    │   │   │   │   ├── NavigationViewHelper.h
    │   │   │   │   ├── NavigationViewItem.cpp
    │   │   │   │   ├── NavigationViewItem.h
    │   │   │   │   ├── NavigationViewItemAutomationPeer.cpp
    │   │   │   │   ├── NavigationViewItemAutomationPeer.h
    │   │   │   │   ├── NavigationViewItemAutomationPeer.idl
    │   │   │   │   ├── NavigationViewItemBase.cpp
    │   │   │   │   ├── NavigationViewItemBase.h
    │   │   │   │   ├── NavigationViewItemBaseRevokers.h
    │   │   │   │   ├── NavigationViewItemCollapsedEventArgs.cpp
    │   │   │   │   ├── NavigationViewItemCollapsedEventArgs.h
    │   │   │   │   ├── NavigationViewItemExpandingEventArgs.cpp
    │   │   │   │   ├── NavigationViewItemExpandingEventArgs.h
    │   │   │   │   ├── NavigationViewItemHeader.cpp
    │   │   │   │   ├── NavigationViewItemHeader.h
    │   │   │   │   ├── NavigationViewItemInvokedEventArgs.cpp
    │   │   │   │   ├── NavigationViewItemInvokedEventArgs.h
    │   │   │   │   ├── NavigationViewItemPresenter.cpp
    │   │   │   │   ├── NavigationViewItemPresenter.h
    │   │   │   │   ├── NavigationViewItemPresenter.idl
    │   │   │   │   ├── NavigationViewItemPresenterTemplateSettings.cpp
    │   │   │   │   ├── NavigationViewItemPresenterTemplateSettings.h
    │   │   │   │   ├── NavigationViewItemSeparator.cpp
    │   │   │   │   ├── NavigationViewItemSeparator.h
    │   │   │   │   ├── NavigationViewItemsFactory.cpp
    │   │   │   │   ├── NavigationViewItemsFactory.h
    │   │   │   │   ├── NavigationViewPaneClosingEventArgs.cpp
    │   │   │   │   ├── NavigationViewPaneClosingEventArgs.h
    │   │   │   │   ├── NavigationViewSelectionChangedEventArgs.cpp
    │   │   │   │   ├── NavigationViewSelectionChangedEventArgs.h
    │   │   │   │   ├── NavigationViewTemplateSettings.cpp
    │   │   │   │   ├── NavigationViewTemplateSettings.h
    │   │   │   │   ├── NavigationViewTrace.h
    │   │   │   │   ├── SplitDataSourceBase.h
    │   │   │   │   ├── TopNavigationViewDataProvider.cpp
    │   │   │   │   ├── TopNavigationViewDataProvider.h
    │   │   │   │   ├── docs/
    │   │   │   │   │   ├── NavigationViewItem.md
    │   │   │   │   │   └── rendering.md
    │   │   │   │   ├── NavigationView_ApiTests/
    │   │   │   │   │   ├── NavigationView_ApiTests.projitems
    │   │   │   │   │   ├── NavigationView_ApiTests.shproj
    │   │   │   │   │   └── NavigationViewTests.cs
    │   │   │   │   ├── NavigationView_InteractionTests/
    │   │   │   │   │   ├── CommonTests.cs
    │   │   │   │   │   ├── EventTests.cs
    │   │   │   │   │   ├── FocusBehaviorTests.cs
    │   │   │   │   │   ├── NavigationView_InteractionTests.projitems
    │   │   │   │   │   ├── NavigationView_InteractionTests.shproj
    │   │   │   │   │   ├── NavigationViewTestsBase.cs
    │   │   │   │   │   ├── PaneBehaviorTests.cs
    │   │   │   │   │   ├── SelectionTests.cs
    │   │   │   │   │   └── TopModeTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── DialogWithNavView.xaml
    │   │   │   │       ├── DialogWithNavView.xaml.cs
    │   │   │   │       ├── NavigationView_TestUI.projitems
    │   │   │   │       ├── NavigationView_TestUI.shproj
    │   │   │   │       ├── NavigationViewAxeTestPage.xaml
    │   │   │   │       ├── NavigationViewAxeTestPage.xaml.cs
    │   │   │   │       ├── NavigationViewCaseBundle.xaml
    │   │   │   │       ├── NavigationViewCaseBundle.xaml.cs
    │   │   │   │       ├── Common/
    │   │   │   │       │   ├── NavigationViewAnimationPage.xaml
    │   │   │   │       │   ├── NavigationViewAnimationPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewBlankPage1.xaml
    │   │   │   │       │   ├── NavigationViewBlankPage1.xaml.cs
    │   │   │   │       │   ├── NavigationViewCompactPaneLengthTestPage.xaml
    │   │   │   │       │   ├── NavigationViewCompactPaneLengthTestPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewInfoBadge.xaml
    │   │   │   │       │   ├── NavigationViewInfoBadge.xaml.cs
    │   │   │   │       │   ├── NavigationViewInitPage.xaml
    │   │   │   │       │   ├── NavigationViewInitPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewIsPaneOpenPage.xaml
    │   │   │   │       │   ├── NavigationViewIsPaneOpenPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewMenuItemsSourcePage.xaml
    │   │   │   │       │   ├── NavigationViewMenuItemsSourcePage.xaml.cs
    │   │   │   │       │   ├── NavigationViewMenuItemStretchPage.xaml
    │   │   │   │       │   ├── NavigationViewMenuItemStretchPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewMinimalPage.xaml
    │   │   │   │       │   ├── NavigationViewMinimalPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewPage.xaml
    │   │   │   │       │   ├── NavigationViewPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewPageDataContext.xaml
    │   │   │   │       │   ├── NavigationViewPageDataContext.xaml.cs
    │   │   │   │       │   ├── NavigationViewSelectedItemEdgeCasePage.xaml
    │   │   │   │       │   ├── NavigationViewSelectedItemEdgeCasePage.xaml.cs
    │   │   │   │       │   ├── NavigationViewStretchPage.xaml
    │   │   │   │       │   └── NavigationViewStretchPage.xaml.cs
    │   │   │   │       ├── CustomResources/
    │   │   │   │       │   ├── CustomNavigationViewItem.xaml
    │   │   │   │       │   ├── CustomNavigationViewItem.xaml.cs
    │   │   │   │       │   ├── NavigationViewCustomMenuItemPage.xaml
    │   │   │   │       │   ├── NavigationViewCustomMenuItemPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewCustomThemeResourcesPage.xaml
    │   │   │   │       │   ├── NavigationViewCustomThemeResourcesPage.xaml.cs
    │   │   │   │       │   ├── NavigationViewItemTemplatePage.xaml
    │   │   │   │       │   └── NavigationViewItemTemplatePage.xaml.cs
    │   │   │   │       ├── Footer/
    │   │   │   │       │   ├── PaneFooterTestPage.xaml
    │   │   │   │       │   ├── PaneFooterTestPage.xaml.cs
    │   │   │   │       │   ├── PaneLayoutTestPage.xaml
    │   │   │   │       │   └── PaneLayoutTestPage.xaml.cs
    │   │   │   │       ├── Hierarchical/
    │   │   │   │       │   ├── HierarchicalNavigationViewDataBinding.xaml
    │   │   │   │       │   ├── HierarchicalNavigationViewDataBinding.xaml.cs
    │   │   │   │       │   ├── HierarchicalNavigationViewMarkup.xaml
    │   │   │   │       │   └── HierarchicalNavigationViewMarkup.xaml.cs
    │   │   │   │       ├── Regression/
    │   │   │   │       │   ├── NavigationViewRS3Page.xaml
    │   │   │   │       │   ├── NavigationViewRS3Page.xaml.cs
    │   │   │   │       │   ├── NavigationViewRS4Page.xaml
    │   │   │   │       │   └── NavigationViewRS4Page.xaml.cs
    │   │   │   │       └── TopMode/
    │   │   │   │           ├── NavigationViewTopNavOnlyPage.xaml
    │   │   │   │           ├── NavigationViewTopNavOnlyPage.xaml.cs
    │   │   │   │           ├── NavigationViewTopNavOverflowButtonPage.xaml
    │   │   │   │           ├── NavigationViewTopNavOverflowButtonPage.xaml.cs
    │   │   │   │           ├── NavigationViewTopNavPage.xaml
    │   │   │   │           ├── NavigationViewTopNavPage.xaml.cs
    │   │   │   │           ├── NavigationViewTopNavStorePage.xaml
    │   │   │   │           └── NavigationViewTopNavStorePage.xaml.cs
    │   │   │   ├── NumberBox/
    │   │   │   │   ├── NumberBox.cpp
    │   │   │   │   ├── NumberBox.h
    │   │   │   │   ├── NumberBox.idl
    │   │   │   │   ├── NumberBox.vcxitems
    │   │   │   │   ├── NumberBox.vcxitems.filters
    │   │   │   │   ├── NumberBox.xaml
    │   │   │   │   ├── NumberBox_themeresources.xaml
    │   │   │   │   ├── NumberBoxAutomationPeer.cpp
    │   │   │   │   ├── NumberBoxAutomationPeer.h
    │   │   │   │   ├── NumberBoxParser.cpp
    │   │   │   │   ├── NumberBoxParser.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── NumberBox_APITests.projitems
    │   │   │   │   │   ├── NumberBox_APITests.shproj
    │   │   │   │   │   └── NumberBoxTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── NumberBox_InteractionTests.projitems
    │   │   │   │   │   ├── NumberBox_InteractionTests.shproj
    │   │   │   │   │   └── NumberBoxTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-US/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── NumberBox_TestUI.projitems
    │   │   │   │       ├── NumberBox_TestUI.shproj
    │   │   │   │       ├── NumberBoxAxeTestPage.xaml
    │   │   │   │       ├── NumberBoxAxeTestPage.xaml.cs
    │   │   │   │       ├── NumberBoxPage.xaml
    │   │   │   │       └── NumberBoxPage.xaml.cs
    │   │   │   ├── PagerControl/
    │   │   │   │   ├── readme.md
    │   │   │   │   ├── PagerControl.cpp
    │   │   │   │   ├── PagerControl.h
    │   │   │   │   ├── PagerControl.idl
    │   │   │   │   ├── PagerControl.vcxitems
    │   │   │   │   ├── PagerControl.xaml
    │   │   │   │   ├── PagerControl_themeresources.xaml
    │   │   │   │   ├── PagerControlAutomationPeer.cpp
    │   │   │   │   ├── PagerControlAutomationPeer.h
    │   │   │   │   ├── PagerControlAutomationPeer.idl
    │   │   │   │   ├── PagerControlSelectedIndexChangedEventArgs.h
    │   │   │   │   ├── PagerControlTemplateSettings.cpp
    │   │   │   │   ├── PagerControlTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── PagerControl_APITests.projitems
    │   │   │   │   │   ├── PagerControl_APITests.shproj
    │   │   │   │   │   └── PagerControlTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── PagerControl_InteractionTests.projitems
    │   │   │   │   │   ├── PagerControl_InteractionTests.shproj
    │   │   │   │   │   ├── PagerControlTestBase.cs
    │   │   │   │   │   ├── PagerControlTestPageElements.cs
    │   │   │   │   │   └── PagerControlTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── PagerControl_TestUI.projitems
    │   │   │   │       ├── PagerControl_TestUI.shproj
    │   │   │   │       ├── PagerControlAxeTestPage.xaml
    │   │   │   │       ├── PagerControlAxeTestPage.xaml.cs
    │   │   │   │       ├── PagerControlPage.xaml
    │   │   │   │       └── PagerControlPage.xaml.cs
    │   │   │   ├── ParallaxView/
    │   │   │   │   ├── ParallaxView.cpp
    │   │   │   │   ├── ParallaxView.h
    │   │   │   │   ├── ParallaxView.idl
    │   │   │   │   ├── ParallaxView.vcxitems
    │   │   │   │   ├── ScrollInputHelper.cpp
    │   │   │   │   ├── ScrollInputHelper.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ParallaxView_APITests.projitems
    │   │   │   │   │   ├── ParallaxView_APITests.shproj
    │   │   │   │   │   └── ParallaxViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ParallaxView_InteractionTests.projitems
    │   │   │   │   │   ├── ParallaxView_InteractionTests.shproj
    │   │   │   │   │   └── ParallaxViewTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── DynamicPage.xaml
    │   │   │   │       ├── DynamicPage.xaml.cs
    │   │   │   │       ├── Ingredient.cs
    │   │   │   │       ├── ListViewBackgroundPage.xaml
    │   │   │   │       ├── ListViewBackgroundPage.xaml.cs
    │   │   │   │       ├── ListViewHeaderPage.xaml
    │   │   │   │       ├── ListViewHeaderPage.xaml.cs
    │   │   │   │       ├── ListViewItemPage.xaml
    │   │   │   │       ├── ListViewItemPage.xaml.cs
    │   │   │   │       ├── ParallaxView_TestUI.projitems
    │   │   │   │       ├── ParallaxView_TestUI.shproj
    │   │   │   │       ├── ParallaxViewPage.xaml
    │   │   │   │       ├── ParallaxViewPage.xaml.cs
    │   │   │   │       ├── ParallaxViewStackPanelPage.xaml
    │   │   │   │       ├── ParallaxViewStackPanelPage.xaml.cs
    │   │   │   │       ├── SimpleRectanglePage.xaml
    │   │   │   │       ├── SimpleRectanglePage.xaml.cs
    │   │   │   │       ├── TextPage.xaml
    │   │   │   │       ├── TextPage.xaml.cs
    │   │   │   │       ├── VirtualizingStackPanelPage.xaml
    │   │   │   │       └── VirtualizingStackPanelPage.xaml.cs
    │   │   │   ├── PersonPicture/
    │   │   │   │   ├── InitialsGenerator.cpp
    │   │   │   │   ├── InitialsGenerator.h
    │   │   │   │   ├── PersonPicture.cpp
    │   │   │   │   ├── PersonPicture.h
    │   │   │   │   ├── PersonPicture.idl
    │   │   │   │   ├── PersonPicture.vcxitems
    │   │   │   │   ├── PersonPicture.xaml
    │   │   │   │   ├── PersonPicture_themeresources.xaml
    │   │   │   │   ├── PersonPictureAutomationPeer.cpp
    │   │   │   │   ├── PersonPictureAutomationPeer.h
    │   │   │   │   ├── PersonPictureAutomationPeer.idl
    │   │   │   │   ├── PersonPictureTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── PersonPicture_APITests.projitems
    │   │   │   │   │   ├── PersonPicture_APITests.shproj
    │   │   │   │   │   └── PersonPictureTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── PersonPicture_InteractionTests.projitems
    │   │   │   │   │   ├── PersonPicture_InteractionTests.shproj
    │   │   │   │   │   └── PersonPictureTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── PersonPicture_TestUI.projitems
    │   │   │   │       ├── PersonPicture_TestUI.shproj
    │   │   │   │       ├── PersonPicturePage.xaml
    │   │   │   │       └── PersonPicturePage.xaml.cs
    │   │   │   ├── PipsPager/
    │   │   │   │   ├── PipsPager.cpp
    │   │   │   │   ├── PipsPager.h
    │   │   │   │   ├── PipsPager.idl
    │   │   │   │   ├── PipsPager.vcxitems
    │   │   │   │   ├── PipsPager.xaml
    │   │   │   │   ├── PipsPager_themeresources.xaml
    │   │   │   │   ├── PipsPagerAutomationPeer.cpp
    │   │   │   │   ├── PipsPagerAutomationPeer.h
    │   │   │   │   ├── PipsPagerAutomationPeer.idl
    │   │   │   │   ├── PipsPagerSelectedIndexChangedEventArgs.h
    │   │   │   │   ├── PipsPagerTemplateSettings.cpp
    │   │   │   │   ├── PipsPagerTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── PipsPager_APITests.projitems
    │   │   │   │   │   ├── PipsPager_APITests.shproj
    │   │   │   │   │   └── PipsPagerTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── PipsPager_InteractionTests.projitems
    │   │   │   │   │   ├── PipsPager_InteractionTests.shproj
    │   │   │   │   │   ├── PipsPagerElements.cs
    │   │   │   │   │   ├── PipsPagerTestBase.cs
    │   │   │   │   │   └── PipsPagerTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── PipsPager_TestUI.projitems
    │   │   │   │       ├── PipsPager_TestUI.shproj
    │   │   │   │       ├── PipsPagerAxeTestPage.xaml
    │   │   │   │       ├── PipsPagerAxeTestPage.xaml.cs
    │   │   │   │       ├── PipsPagerExamples.xaml
    │   │   │   │       ├── PipsPagerExamples.xaml.cs
    │   │   │   │       ├── PipsPagerPage.xaml
    │   │   │   │       └── PipsPagerPage.xaml.cs
    │   │   │   ├── ProgressBar/
    │   │   │   │   ├── ProgressBar.cpp
    │   │   │   │   ├── ProgressBar.h
    │   │   │   │   ├── ProgressBar.idl
    │   │   │   │   ├── ProgressBar.vcxitems
    │   │   │   │   ├── ProgressBar.xaml
    │   │   │   │   ├── ProgressBar_themeresources.xaml
    │   │   │   │   ├── ProgressBarAutomationPeer.cpp
    │   │   │   │   ├── ProgressBarAutomationPeer.h
    │   │   │   │   ├── ProgressBarTemplateSettings.cpp
    │   │   │   │   ├── ProgressBarTemplateSettings.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ProgressBar_APITests.projitems
    │   │   │   │   │   ├── ProgressBar_APITests.shproj
    │   │   │   │   │   └── ProgressBarTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ProgressBar_InteractionTests.projitems
    │   │   │   │   │   ├── ProgressBar_InteractionTests.shproj
    │   │   │   │   │   └── ProgressBarTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ProgressBar_TestUI.projitems
    │   │   │   │       ├── ProgressBar_TestUI.shproj
    │   │   │   │       ├── ProgressBarAxeTestPage.xaml
    │   │   │   │       ├── ProgressBarAxeTestPage.xaml.cs
    │   │   │   │       ├── ProgressBarPage.xaml
    │   │   │   │       ├── ProgressBarPage.xaml.cs
    │   │   │   │       ├── ProgressBarReTemplatePage.xaml
    │   │   │   │       └── ProgressBarReTemplatePage.xaml.cs
    │   │   │   ├── ProgressRing/
    │   │   │   │   ├── ProgressRing.cpp
    │   │   │   │   ├── ProgressRing.h
    │   │   │   │   ├── ProgressRing.idl
    │   │   │   │   ├── ProgressRing.vcxitems
    │   │   │   │   ├── ProgressRing.vcxitems.filters
    │   │   │   │   ├── ProgressRing.xaml
    │   │   │   │   ├── ProgressRing_themeresources.xaml
    │   │   │   │   ├── ProgressRingAutomationPeer.cpp
    │   │   │   │   ├── ProgressRingAutomationPeer.h
    │   │   │   │   ├── ProgressRingTemplateSettings.cpp
    │   │   │   │   ├── ProgressRingTemplateSettings.h
    │   │   │   │   ├── AnimatedVisuals/
    │   │   │   │   │   ├── ProgressRingDeterminate.cpp
    │   │   │   │   │   ├── ProgressRingDeterminate.h
    │   │   │   │   │   ├── ProgressRingIndeterminate.cpp
    │   │   │   │   │   └── ProgressRingIndeterminate.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ProgressRing_APITests.projitems
    │   │   │   │   │   ├── ProgressRing_APITests.shproj
    │   │   │   │   │   └── ProgressRingTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ProgressRing_InteractionTests.projitems
    │   │   │   │   │   ├── ProgressRing_InteractionTests.shproj
    │   │   │   │   │   └── ProgressRingTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ProgressRing_TestUI.projitems
    │   │   │   │       ├── ProgressRing_TestUI.shproj
    │   │   │   │       ├── ProgressRingAxeTestPage.xaml
    │   │   │   │       ├── ProgressRingAxeTestPage.xaml.cs
    │   │   │   │       ├── ProgressRingCustomLottieSourcePage.xaml
    │   │   │   │       ├── ProgressRingCustomLottieSourcePage.xaml.cs
    │   │   │   │       ├── ProgressRingDeterminate.cs
    │   │   │   │       ├── ProgressRingPage.xaml
    │   │   │   │       ├── ProgressRingPage.xaml.cs
    │   │   │   │       ├── ProgressRingStoryboardAnimationPage.xaml
    │   │   │   │       └── ProgressRingStoryboardAnimationPage.xaml.cs
    │   │   │   ├── PullToRefresh/
    │   │   │   │   ├── PTRTracing/
    │   │   │   │   │   ├── PTRTracing.h
    │   │   │   │   │   └── PTRTracing.vcxitems
    │   │   │   │   ├── RefreshContainer/
    │   │   │   │   │   ├── RefreshContainer.cpp
    │   │   │   │   │   ├── RefreshContainer.h
    │   │   │   │   │   ├── RefreshContainer.idl
    │   │   │   │   │   ├── RefreshContainer.vcxitems
    │   │   │   │   │   ├── RefreshContainer.xaml
    │   │   │   │   │   ├── RefreshContainer_themeresources.xaml
    │   │   │   │   │   ├── RefreshContainerPrivate.idl
    │   │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   │   ├── RefreshContainer_InteractionTests.projitems
    │   │   │   │   │   │   ├── RefreshContainer_InteractionTests.shproj
    │   │   │   │   │   │   └── RefreshContainerTests.cs
    │   │   │   │   │   └── TestUI/
    │   │   │   │   │       ├── AnimationHandler.cs
    │   │   │   │   │       ├── ImageIRefreshInfoProviderAdapter.cs
    │   │   │   │   │       ├── RefreshContainer_TestUI.projitems
    │   │   │   │   │       ├── RefreshContainer_TestUI.shproj
    │   │   │   │   │       ├── RefreshContainerOnImagePage.xaml
    │   │   │   │   │       ├── RefreshContainerOnImagePage.xaml.cs
    │   │   │   │   │       ├── RefreshContainerPage.xaml
    │   │   │   │   │       └── RefreshContainerPage.xaml.cs
    │   │   │   │   ├── RefreshVisualizer/
    │   │   │   │   │   ├── PullToRefreshHelperTestApi.cpp
    │   │   │   │   │   ├── PullToRefreshHelperTestApi.h
    │   │   │   │   │   ├── PullToRefreshHelperTestAPI.idl
    │   │   │   │   │   ├── PullToRefreshHelperTestApiFactory.cpp
    │   │   │   │   │   ├── PullToRefreshHelperTestApiFactory.h
    │   │   │   │   │   ├── RefreshInteractionRatioChangedEventArgs.cpp
    │   │   │   │   │   ├── RefreshInteractionRatioChangedEventArgs.h
    │   │   │   │   │   ├── RefreshVisualizer.cpp
    │   │   │   │   │   ├── RefreshVisualizer.h
    │   │   │   │   │   ├── RefreshVisualizer.idl
    │   │   │   │   │   ├── RefreshVisualizer.vcxitems
    │   │   │   │   │   ├── RefreshVisualizer.xaml
    │   │   │   │   │   ├── RefreshVisualizer_themeresources.xaml
    │   │   │   │   │   ├── RefreshVisualizerEventArgs.cpp
    │   │   │   │   │   ├── RefreshVisualizerEventArgs.h
    │   │   │   │   │   ├── RefreshVisualizerPrivate.idl
    │   │   │   │   │   ├── APITests/
    │   │   │   │   │   │   ├── RefreshVisualizer_APITests.projitems
    │   │   │   │   │   │   ├── RefreshVisualizer_APITests.shproj
    │   │   │   │   │   │   └── RefreshVisualizerTests.cs
    │   │   │   │   │   └── TestUI/
    │   │   │   │   │       ├── RefreshVisualizer_TestUI.projitems
    │   │   │   │   │       ├── RefreshVisualizer_TestUI.shproj
    │   │   │   │   │       ├── RefreshVisualizerPage.xaml
    │   │   │   │   │       ├── RefreshVisualizerPage.xaml.cs
    │   │   │   │   │       └── SliderAsRefreshInfoProvider.cs
    │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter/
    │   │   │   │   │   ├── RefreshInfoProviderImpl.cpp
    │   │   │   │   │   ├── RefreshInfoProviderImpl.h
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter.cpp
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter.h
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter.idl
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapter.vcxitems
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapterFactory.cpp
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderAdapterFactory.h
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderDefaultAnimationHandler.cpp
    │   │   │   │   │   ├── ScrollViewerIRefreshInfoProviderDefaultAnimationHandler.h
    │   │   │   │   │   ├── APITests/
    │   │   │   │   │   │   ├── APITests.projitems
    │   │   │   │   │   │   ├── ScrollViewerAdapter_APITests.shproj
    │   │   │   │   │   │   └── ScrollViewerAdapterTests.cs
    │   │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   │   ├── ScrollViewerAdapter_InteractionTests.projitems
    │   │   │   │   │   │   ├── ScrollViewerAdapter_InteractionTests.shproj
    │   │   │   │   │   │   └── ScrollViewerAdapterTests.cs
    │   │   │   │   │   └── TestUI/
    │   │   │   │   │       ├── ScrollViewerAdapter_TestUI.projitems
    │   │   │   │   │       ├── ScrollViewerAdapter_TestUI.shproj
    │   │   │   │   │       ├── ScrollViewerAdapterPage.xaml
    │   │   │   │   │       └── ScrollViewerAdapterPage.xaml.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── PTR_TestUI.projitems
    │   │   │   │       ├── PTR_TestUI.shproj
    │   │   │   │       ├── PTRPage.xaml
    │   │   │   │       ├── PTRPage.xaml.cs
    │   │   │   │       ├── PullToRefreshPage.xaml
    │   │   │   │       └── PullToRefreshPage.xaml.cs
    │   │   │   ├── RadialGradientBrush/
    │   │   │   │   ├── RadialGradientBrush.cpp
    │   │   │   │   ├── RadialGradientBrush.h
    │   │   │   │   ├── RadialGradientBrush.idl
    │   │   │   │   ├── RadialGradientBrush.vcxitems
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── RadialGradientBrush_InteractionTests.projitems
    │   │   │   │   │   ├── RadialGradientBrush_InteractionTests.shproj
    │   │   │   │   │   └── RadialGradientBrushTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── RadialGradientBrush_TestUI.projitems
    │   │   │   │       ├── RadialGradientBrush_TestUI.shproj
    │   │   │   │       ├── RadialGradientBrushPage.xaml
    │   │   │   │       └── RadialGradientBrushPage.xaml.cs
    │   │   │   ├── RadioButtons/
    │   │   │   │   ├── ColumnMajorUniformToLargestGridLayout.cpp
    │   │   │   │   ├── ColumnMajorUniformToLargestGridLayout.h
    │   │   │   │   ├── RadioButton.xaml
    │   │   │   │   ├── RadioButtons.cpp
    │   │   │   │   ├── RadioButtons.h
    │   │   │   │   ├── RadioButtons.idl
    │   │   │   │   ├── RadioButtons.vcxitems
    │   │   │   │   ├── RadioButtons.vcxitems.filters
    │   │   │   │   ├── RadioButtons.xaml
    │   │   │   │   ├── RadioButtons_themeresources.xaml
    │   │   │   │   ├── RadioButtonsAutomationPeer.cpp
    │   │   │   │   ├── RadioButtonsAutomationPeer.h
    │   │   │   │   ├── RadioButtonsElementFactory.cpp
    │   │   │   │   ├── RadioButtonsElementFactory.h
    │   │   │   │   ├── RadioButtonsPrimitives.idl
    │   │   │   │   ├── RadioButtonsTestHooks.cpp
    │   │   │   │   ├── RadioButtonsTestHooks.h
    │   │   │   │   ├── RadioButtonsTestHooks.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── RadioButtons_APITests.projitems
    │   │   │   │   │   ├── RadioButtons_APITests.shproj
    │   │   │   │   │   └── RadioButtonsTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── RadioButtons_InteractionTests.projitems
    │   │   │   │   │   ├── RadioButtons_InteractionTests.shproj
    │   │   │   │   │   ├── RadioButtonsFocusTestPageElements.cs
    │   │   │   │   │   ├── RadioButtonsTestPageElements.cs
    │   │   │   │   │   └── RadioButtonsTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── RadioButtons_TestUI.projitems
    │   │   │   │       ├── RadioButtons_TestUI.shproj
    │   │   │   │       ├── RadioButtonsCaseBundle.xaml
    │   │   │   │       ├── RadioButtonsCaseBundle.xaml.cs
    │   │   │   │       ├── RadioButtonsFocusPage.xaml
    │   │   │   │       ├── RadioButtonsFocusPage.xaml.cs
    │   │   │   │       ├── RadioButtonsPage.xaml
    │   │   │   │       └── RadioButtonsPage.xaml.cs
    │   │   │   ├── RadioMenuFlyoutItem/
    │   │   │   │   ├── RadioMenuFlyoutItem.cpp
    │   │   │   │   ├── RadioMenuFlyoutItem.h
    │   │   │   │   ├── RadioMenuFlyoutItem.idl
    │   │   │   │   ├── RadioMenuFlyoutItem.vcxitems
    │   │   │   │   ├── RadioMenuFlyoutItem_themeresources.xaml
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── RadioMenuFlyoutItem_InteractionTests.projitems
    │   │   │   │   │   ├── RadioMenuFlyoutItem_InteractionTests.shproj
    │   │   │   │   │   └── RadioMenuFlyoutItemTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── RadioMenuFlyoutItem_TestUI.projitems
    │   │   │   │       ├── RadioMenuFlyoutItem_TestUI.shproj
    │   │   │   │       ├── RadioMenuFlyoutItemPage.xaml
    │   │   │   │       └── RadioMenuFlyoutItemPage.xaml.cs
    │   │   │   ├── RatingControl/
    │   │   │   │   ├── RatingControl.cpp
    │   │   │   │   ├── RatingControl.h
    │   │   │   │   ├── RatingControl.idl
    │   │   │   │   ├── RatingControl.vcxitems
    │   │   │   │   ├── RatingControl.xaml
    │   │   │   │   ├── RatingControl_themeresources.xaml
    │   │   │   │   ├── RatingControlAutomationPeer.cpp
    │   │   │   │   ├── RatingControlAutomationPeer.h
    │   │   │   │   ├── RatingControlAutomationPeer.idl
    │   │   │   │   ├── RatingItemFontInfo.cpp
    │   │   │   │   ├── RatingItemFontInfo.h
    │   │   │   │   ├── RatingItemImageInfo.cpp
    │   │   │   │   ├── RatingItemImageInfo.h
    │   │   │   │   ├── RatingItemInfo.cpp
    │   │   │   │   ├── RatingItemInfo.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── RatingControl_APITests.projitems
    │   │   │   │   │   ├── RatingControl_APITests.shproj
    │   │   │   │   │   └── RatingControlTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── RatingControl_InteractionTests.projitems
    │   │   │   │   │   ├── RatingControl_InteractionTests.shproj
    │   │   │   │   │   └── RatingControlTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── RatingControl_TestUI.projitems
    │   │   │   │       ├── RatingControl_TestUI.shproj
    │   │   │   │       ├── RatingControlPage.xaml
    │   │   │   │       └── RatingControlPage.xaml.cs
    │   │   │   ├── Repeater/
    │   │   │   │   ├── BuildTreeScheduler.cpp
    │   │   │   │   ├── BuildTreeScheduler.h
    │   │   │   │   ├── ChildrenInTabFocusOrderIterable.cpp
    │   │   │   │   ├── ChildrenInTabFocusOrderIterable.h
    │   │   │   │   ├── CustomProperty.cpp
    │   │   │   │   ├── CustomProperty.h
    │   │   │   │   ├── ElementFactory.cpp
    │   │   │   │   ├── ElementFactory.h
    │   │   │   │   ├── ElementFactoryGetArgsDownlevel.cpp
    │   │   │   │   ├── ElementFactoryGetArgsDownlevel.h
    │   │   │   │   ├── ElementFactoryRecycleArgsDownlevel.cpp
    │   │   │   │   ├── ElementFactoryRecycleArgsDownlevel.h
    │   │   │   │   ├── ElementManager.cpp
    │   │   │   │   ├── ElementManager.h
    │   │   │   │   ├── FlowLayout.cpp
    │   │   │   │   ├── FlowLayout.h
    │   │   │   │   ├── FlowLayoutAlgorithm.cpp
    │   │   │   │   ├── FlowLayoutAlgorithm.h
    │   │   │   │   ├── FlowLayoutState.cpp
    │   │   │   │   ├── FlowLayoutState.h
    │   │   │   │   ├── IFlowLayoutAlgorithmDelegates.h
    │   │   │   │   ├── IndexPath.cpp
    │   │   │   │   ├── IndexPath.h
    │   │   │   │   ├── IndexRange.cpp
    │   │   │   │   ├── IndexRange.h
    │   │   │   │   ├── InspectingDataSource.cpp
    │   │   │   │   ├── InspectingDataSource.h
    │   │   │   │   ├── ItemCollectionTransition.cpp
    │   │   │   │   ├── ItemCollectionTransition.h
    │   │   │   │   ├── ItemCollectionTransitionCompletedEventArgs.cpp
    │   │   │   │   ├── ItemCollectionTransitionCompletedEventArgs.h
    │   │   │   │   ├── ItemCollectionTransitionProgress.cpp
    │   │   │   │   ├── ItemCollectionTransitionProgress.h
    │   │   │   │   ├── ItemCollectionTransitionProvider.cpp
    │   │   │   │   ├── ItemCollectionTransitionProvider.h
    │   │   │   │   ├── ItemsRepeater.common.cpp
    │   │   │   │   ├── ItemsRepeater.common.h
    │   │   │   │   ├── ItemsRepeater.cpp
    │   │   │   │   ├── ItemsRepeater.h
    │   │   │   │   ├── ItemsRepeater.idl
    │   │   │   │   ├── ItemsRepeaterElementClearingEventArgs.cpp
    │   │   │   │   ├── ItemsRepeaterElementClearingEventArgs.h
    │   │   │   │   ├── ItemsRepeaterElementIndexChangedEventArgs.cpp
    │   │   │   │   ├── ItemsRepeaterElementIndexChangedEventArgs.h
    │   │   │   │   ├── ItemsRepeaterElementPreparedEventArgs.cpp
    │   │   │   │   ├── ItemsRepeaterElementPreparedEventArgs.h
    │   │   │   │   ├── ItemsRepeaterScrollHost.cpp
    │   │   │   │   ├── ItemsRepeaterScrollHost.h
    │   │   │   │   ├── ItemsRepeaterTrace.h
    │   │   │   │   ├── ItemsSourceView.cpp
    │   │   │   │   ├── ItemsSourceView.h
    │   │   │   │   ├── ItemsSourceViewFactory.cpp
    │   │   │   │   ├── ItemsSourceViewFactory.h
    │   │   │   │   ├── ItemTemplateWrapper.cpp
    │   │   │   │   ├── ItemTemplateWrapper.h
    │   │   │   │   ├── Layout.cpp
    │   │   │   │   ├── Layout.h
    │   │   │   │   ├── LayoutContext.cpp
    │   │   │   │   ├── LayoutContext.h
    │   │   │   │   ├── LayoutContextAdapter.cpp
    │   │   │   │   ├── LayoutContextAdapter.h
    │   │   │   │   ├── LayoutsTestHooks.cpp
    │   │   │   │   ├── LayoutsTestHooks.h
    │   │   │   │   ├── LayoutsTestHooks.idl
    │   │   │   │   ├── LayoutsTestHooksFactory.cpp
    │   │   │   │   ├── LayoutsTestHooksFactory.h
    │   │   │   │   ├── LayoutsTestHooksLinedFlowLayoutInvalidatedEventArgs.cpp
    │   │   │   │   ├── LayoutsTestHooksLinedFlowLayoutInvalidatedEventArgs.h
    │   │   │   │   ├── LayoutsTestHooksLinedFlowLayoutItemLockedEventArgs.cpp
    │   │   │   │   ├── LayoutsTestHooksLinedFlowLayoutItemLockedEventArgs.h
    │   │   │   │   ├── LinedFlowLayout.cpp
    │   │   │   │   ├── LinedFlowLayout.h
    │   │   │   │   ├── LinedFlowLayoutItemAspectRatios.cpp
    │   │   │   │   ├── LinedFlowLayoutItemAspectRatios.h
    │   │   │   │   ├── LinedFlowLayoutItemCollectionTransitionProvider.cpp
    │   │   │   │   ├── LinedFlowLayoutItemCollectionTransitionProvider.h
    │   │   │   │   ├── LinedFlowLayoutItemsInfoRequestedEventArgs.cpp
    │   │   │   │   ├── LinedFlowLayoutItemsInfoRequestedEventArgs.h
    │   │   │   │   ├── LinedFlowLayoutTrace.h
    │   │   │   │   ├── NonVirtualizingLayout.cpp
    │   │   │   │   ├── NonVirtualizingLayout.h
    │   │   │   │   ├── NonvirtualizingLayoutContext.cpp
    │   │   │   │   ├── NonvirtualizingLayoutContext.h
    │   │   │   │   ├── OrientationBasedMeasures.cpp
    │   │   │   │   ├── OrientationBasedMeasures.h
    │   │   │   │   ├── Phaser.cpp
    │   │   │   │   ├── Phaser.h
    │   │   │   │   ├── QPCTimer.cpp
    │   │   │   │   ├── QPCTimer.h
    │   │   │   │   ├── RecyclePool.cpp
    │   │   │   │   ├── RecyclePool.h
    │   │   │   │   ├── RecyclePoolFactory.cpp
    │   │   │   │   ├── RecyclePoolFactory.h
    │   │   │   │   ├── RecyclingElementFactory.cpp
    │   │   │   │   ├── RecyclingElementFactory.h
    │   │   │   │   ├── Repeater.vcxitems
    │   │   │   │   ├── Repeater.vcxitems.filters
    │   │   │   │   ├── RepeaterAutomationPeer.cpp
    │   │   │   │   ├── RepeaterAutomationPeer.h
    │   │   │   │   ├── RepeaterAutomationPeer.idl
    │   │   │   │   ├── RepeaterLayoutContext.cpp
    │   │   │   │   ├── RepeaterLayoutContext.h
    │   │   │   │   ├── RepeaterPrivate.idl
    │   │   │   │   ├── RepeaterTestHooks.cpp
    │   │   │   │   ├── RepeaterTestHooks.h
    │   │   │   │   ├── RepeaterTestHooks.idl
    │   │   │   │   ├── RepeaterTestHooksFactory.cpp
    │   │   │   │   ├── RepeaterTestHooksFactory.h
    │   │   │   │   ├── SelectedItems.h
    │   │   │   │   ├── SelectionModel.cpp
    │   │   │   │   ├── SelectionModel.h
    │   │   │   │   ├── SelectionModelChildrenRequestedEventArgs.cpp
    │   │   │   │   ├── SelectionModelChildrenRequestedEventArgs.h
    │   │   │   │   ├── SelectionModelSelectionChangedEventArgs.cpp
    │   │   │   │   ├── SelectionModelSelectionChangedEventArgs.h
    │   │   │   │   ├── SelectionNode.cpp
    │   │   │   │   ├── SelectionNode.h
    │   │   │   │   ├── SelectionTreeHelper.cpp
    │   │   │   │   ├── SelectionTreeHelper.h
    │   │   │   │   ├── SelectTemplateEventArgs.cpp
    │   │   │   │   ├── SelectTemplateEventArgs.h
    │   │   │   │   ├── StackLayout.cpp
    │   │   │   │   ├── StackLayout.h
    │   │   │   │   ├── StackLayoutState.cpp
    │   │   │   │   ├── StackLayoutState.h
    │   │   │   │   ├── TransitionManager.cpp
    │   │   │   │   ├── TransitionManager.h
    │   │   │   │   ├── UniformGridLayout.cpp
    │   │   │   │   ├── UniformGridLayout.h
    │   │   │   │   ├── UniformGridLayoutState.cpp
    │   │   │   │   ├── UniformGridLayoutState.h
    │   │   │   │   ├── UniqueIdElementPool.cpp
    │   │   │   │   ├── UniqueIdElementPool.h
    │   │   │   │   ├── ViewManager.cpp
    │   │   │   │   ├── ViewManager.h
    │   │   │   │   ├── ViewportManager.h
    │   │   │   │   ├── ViewportManagerDownlevel.cpp
    │   │   │   │   ├── ViewportManagerDownlevel.h
    │   │   │   │   ├── ViewportManagerWithPlatformFeatures.cpp
    │   │   │   │   ├── ViewportManagerWithPlatformFeatures.h
    │   │   │   │   ├── VirtualizationInfo.cpp
    │   │   │   │   ├── VirtualizationInfo.h
    │   │   │   │   ├── VirtualizingLayout.cpp
    │   │   │   │   ├── VirtualizingLayout.h
    │   │   │   │   ├── VirtualizingLayoutContext.cpp
    │   │   │   │   ├── VirtualizingLayoutContext.h
    │   │   │   │   ├── VirtualLayoutContextAdapter.cpp
    │   │   │   │   ├── VirtualLayoutContextAdapter.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── AccessibilityTests.cs
    │   │   │   │   │   ├── EffectiveViewportScrollPresenterTests.cs
    │   │   │   │   │   ├── EffectiveViewportScrollViewerTests.cs
    │   │   │   │   │   ├── FlowLayoutCollectionChangeTests.cs
    │   │   │   │   │   ├── FlowLayoutTests.cs
    │   │   │   │   │   ├── IndexPathTests.cs
    │   │   │   │   │   ├── InspectingDataSourceTests.cs
    │   │   │   │   │   ├── ItemCollectionTransitionProviderTests.cs
    │   │   │   │   │   ├── ItemTemplateTests.cs
    │   │   │   │   │   ├── LayoutTests.cs
    │   │   │   │   │   ├── LinedFlowLayoutTests.cs
    │   │   │   │   │   ├── PhasingTests.cs
    │   │   │   │   │   ├── RecyclePoolTests.cs
    │   │   │   │   │   ├── Repeater_APITests.projitems
    │   │   │   │   │   ├── Repeater_APITests.shproj
    │   │   │   │   │   ├── RepeaterFocusTests.cs
    │   │   │   │   │   ├── RepeaterTests.cs
    │   │   │   │   │   ├── SelectionModelTests.cs
    │   │   │   │   │   ├── ViewManagerTests.cs
    │   │   │   │   │   ├── ViewportTests.cs
    │   │   │   │   │   └── Common/
    │   │   │   │   │       ├── AspectRatioRespectingControl.cs
    │   │   │   │   │       ├── CollectionChangeEventArgsConverters.cs
    │   │   │   │   │       ├── CustomItemsSource.cs
    │   │   │   │   │       ├── CustomItemsSourceView.cs
    │   │   │   │   │       ├── DataAsElementElementFactory.cs
    │   │   │   │   │       ├── ElementFromElementElementFactory.cs
    │   │   │   │   │       ├── FlowLayoutDerived.cs
    │   │   │   │   │       ├── ItemCollectionTransitionProviderDerived.cs
    │   │   │   │   │       ├── LayoutExtensions.cs
    │   │   │   │   │       ├── NamedGroup.cs
    │   │   │   │   │       ├── NonVirtualStackLayout.cs
    │   │   │   │   │       ├── OrientationBasedMeasures.cs
    │   │   │   │   │       ├── ReadOnlyNotifyPropertyChangedCollection.cs
    │   │   │   │   │       ├── RecyclingViewGeneratorDerived.cs
    │   │   │   │   │       ├── SharedHelpers.cs
    │   │   │   │   │       ├── WinRTCollection.cs
    │   │   │   │   │       └── Mocks/
    │   │   │   │   │           ├── MockItemsSource.cs
    │   │   │   │   │           ├── MockNonVirtualizingLayout.cs
    │   │   │   │   │           ├── MockStackLayout.cs
    │   │   │   │   │           ├── MockViewGenerator.cs
    │   │   │   │   │           └── MockVirtualizingLayout.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── Repeater_InteractionTests.projitems
    │   │   │   │   │   ├── Repeater_InteractionTests.shproj
    │   │   │   │   │   └── RepeaterTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── Repeater_TestUI.projitems
    │   │   │   │       ├── Repeater_TestUI.shproj
    │   │   │   │       ├── RepeaterTestUIPage.xaml
    │   │   │   │       ├── RepeaterTestUIPage.xaml.cs
    │   │   │   │       └── Samples/
    │   │   │   │           ├── BasicDemo.xaml
    │   │   │   │           ├── BasicDemo.xaml.cs
    │   │   │   │           ├── Defaults.xaml
    │   │   │   │           ├── Defaults.xaml.cs
    │   │   │   │           ├── KeyboardNavigationSample.cs
    │   │   │   │           ├── KeyboardNavigationSample.xaml
    │   │   │   │           ├── LinedFlowLayoutDemo.cs
    │   │   │   │           ├── LinedFlowLayoutDemo.xaml
    │   │   │   │           ├── ObjectModelTestPage.xaml
    │   │   │   │           ├── ObjectModelTestPage.xaml.cs
    │   │   │   │           ├── UniformGridLayoutDemo.cs
    │   │   │   │           ├── UniformGridLayoutDemo.xaml
    │   │   │   │           ├── AnimationSamples/
    │   │   │   │           │   ├── AnimationsDemoPage.xaml
    │   │   │   │           │   ├── AnimationsDemoPage.xaml.cs
    │   │   │   │           │   ├── DefaultElementAnimator.cs
    │   │   │   │           │   ├── RadialElementAnimator.cs
    │   │   │   │           │   ├── ScaleAnimatedVerticalListDemo.xaml
    │   │   │   │           │   └── ScaleAnimatedVerticalListDemo.xaml.cs
    │   │   │   │           ├── DataModel/
    │   │   │   │           │   ├── Recipe.cs
    │   │   │   │           │   ├── RecipeGroup.cs
    │   │   │   │           │   └── Year.cs
    │   │   │   │           ├── ItemsSourceSamples/
    │   │   │   │           │   ├── CollectionChangeDemo.xaml
    │   │   │   │           │   ├── CollectionChangeDemo.xaml.cs
    │   │   │   │           │   ├── DelegatingItemsSource.cs
    │   │   │   │           │   ├── ElementsInItemsSourcePage.xaml
    │   │   │   │           │   ├── ElementsInItemsSourcePage.xaml.cs
    │   │   │   │           │   ├── RecipeViewGenerator.cs
    │   │   │   │           │   ├── ResetableCollection.cs
    │   │   │   │           │   ├── SortingAndFilteringPage.xaml
    │   │   │   │           │   ├── SortingAndFilteringPage.xaml.cs
    │   │   │   │           │   ├── VariableSizedItemsPage.xaml
    │   │   │   │           │   └── VariableSizedItemsPage.xaml.cs
    │   │   │   │           ├── ItemTemplateSamples/
    │   │   │   │           │   ├── DisposableUserControl.xaml
    │   │   │   │           │   ├── DisposableUserControl.xaml.cs
    │   │   │   │           │   ├── ItemTemplateDemo.xaml
    │   │   │   │           │   └── ItemTemplateDemo.xaml.cs
    │   │   │   │           ├── LayoutSamplePages/
    │   │   │   │           │   ├── NonVirtual/
    │   │   │   │           │   │   ├── NonVirtualStackLayoutSamplePage.xaml
    │   │   │   │           │   │   └── NonVirtualStackLayoutSamplePage.xaml.cs
    │   │   │   │           │   └── Virtual/
    │   │   │   │           │       ├── PinterestLayoutSamplePage.xaml
    │   │   │   │           │       ├── PinterestLayoutSamplePage.xaml.cs
    │   │   │   │           │       ├── VirtualizingStackLayoutSamplePage.xaml
    │   │   │   │           │       ├── VirtualizingStackLayoutSamplePage.xaml.cs
    │   │   │   │           │       ├── VirtualizingUniformStackLayoutSamplePage.xaml
    │   │   │   │           │       └── VirtualizingUniformStackLayoutSamplePage.xaml.cs
    │   │   │   │           ├── LayoutSamples/
    │   │   │   │           │   ├── NestedLayoutSamples/
    │   │   │   │           │   │   ├── ItemsViewWithDataPage.xaml
    │   │   │   │           │   │   ├── ItemsViewWithDataPage.xaml.cs
    │   │   │   │           │   │   ├── LayoutHelper.cs
    │   │   │   │           │   │   ├── StoreDemoPage.xaml
    │   │   │   │           │   │   ├── StoreDemoPage.xaml.cs
    │   │   │   │           │   │   └── StoreMockData.cs
    │   │   │   │           │   ├── NonVirtualLayoutPages/
    │   │   │   │           │   │   ├── CircleLayout.cs
    │   │   │   │           │   │   ├── CircleLayoutSamplePage.xaml
    │   │   │   │           │   │   ├── CircleLayoutSamplePage.xaml.cs
    │   │   │   │           │   │   ├── Flex.cs
    │   │   │   │           │   │   ├── NonVirtualStackLayout.cs
    │   │   │   │           │   │   ├── NonVirtualStackLayoutSamplePage.xaml
    │   │   │   │           │   │   └── NonVirtualStackLayoutSamplePage.xaml.cs
    │   │   │   │           │   └── VirtualLayoutPages/
    │   │   │   │           │       ├── ActivityFeedLayout.cs
    │   │   │   │           │       ├── ActivityFeedSamplePage.xaml
    │   │   │   │           │       ├── ActivityFeedSamplePage.xaml.cs
    │   │   │   │           │       ├── FlowLayoutDemoPage.xaml
    │   │   │   │           │       ├── FlowLayoutDemoPage.xaml.cs
    │   │   │   │           │       ├── PinterestLayout.cs
    │   │   │   │           │       ├── PinterestLayoutSamplePage.xaml
    │   │   │   │           │       ├── PinterestLayoutSamplePage.xaml.cs
    │   │   │   │           │       ├── StackLayoutDemoPage.xaml
    │   │   │   │           │       ├── StackLayoutDemoPage.xaml.cs
    │   │   │   │           │       ├── UniformGrid2DLayout.cs
    │   │   │   │           │       ├── VirtualizingStackLayout.cs
    │   │   │   │           │       ├── VirtualizingStackLayoutSamplePage.xaml
    │   │   │   │           │       ├── VirtualizingStackLayoutSamplePage.xaml.cs
    │   │   │   │           │       ├── VirtualizingUniformCarouselStackLayout.cs
    │   │   │   │           │       ├── VirtualizingUniformStackLayout.cs
    │   │   │   │           │       ├── VirtualizingUniformStackLayoutSamplePage.xaml
    │   │   │   │           │       └── VirtualizingUniformStackLayoutSamplePage.xaml.cs
    │   │   │   │           ├── NestedLayoutSamples/
    │   │   │   │           │   ├── ItemsViewWithDataPage.xaml
    │   │   │   │           │   ├── ItemsViewWithDataPage.xaml.cs
    │   │   │   │           │   ├── LayoutHelper.cs
    │   │   │   │           │   ├── StoreDemoPage.xaml
    │   │   │   │           │   ├── StoreDemoPage.xaml.cs
    │   │   │   │           │   └── StoreMockData.cs
    │   │   │   │           └── SelectionSample/
    │   │   │   │               ├── Common/
    │   │   │   │               │   ├── BoolToBrushConverter.cs
    │   │   │   │               │   ├── BoolToVisibilityConverter.cs
    │   │   │   │               │   ├── Data.cs
    │   │   │   │               │   ├── SelectionContainer.cs
    │   │   │   │               │   └── SelectionContainerAutomationPeer.cs
    │   │   │   │               ├── Flat/
    │   │   │   │               │   ├── FlatSample.xaml
    │   │   │   │               │   ├── FlatSample.xaml.cs
    │   │   │   │               │   ├── RepeaterItem.cs
    │   │   │   │               │   └── RepeaterItemAutomationPeer.cs
    │   │   │   │               ├── Grouped/
    │   │   │   │               │   ├── GroupedRepeaterItem.cs
    │   │   │   │               │   ├── GroupedRepeaterItemAutomationPeer.cs
    │   │   │   │               │   ├── GroupedSample.xaml
    │   │   │   │               │   └── GroupedSample.xaml.cs
    │   │   │   │               └── TreeView/
    │   │   │   │                   ├── TreeViewItem.cs
    │   │   │   │                   ├── TreeViewItemAutomationPeer.cs
    │   │   │   │                   ├── TreeViewSample.xaml
    │   │   │   │                   └── TreeViewSample.xaml.cs
    │   │   │   ├── ResourceHelper/
    │   │   │   │   ├── ResourceAccessor.cpp
    │   │   │   │   ├── ResourceAccessor.h
    │   │   │   │   ├── ResourceHelper.vcxitems
    │   │   │   │   ├── Utils.cpp
    │   │   │   │   └── Utils.h
    │   │   │   ├── ScrollPresenter/
    │   │   │   │   ├── BringIntoViewOffsetsChange.cpp
    │   │   │   │   ├── BringIntoViewOffsetsChange.h
    │   │   │   │   ├── InteractionTrackerAsyncOperation.cpp
    │   │   │   │   ├── InteractionTrackerAsyncOperation.h
    │   │   │   │   ├── InteractionTrackerOwner.cpp
    │   │   │   │   ├── InteractionTrackerOwner.h
    │   │   │   │   ├── OffsetsChange.cpp
    │   │   │   │   ├── OffsetsChange.h
    │   │   │   │   ├── OffsetsChangeWithAdditionalVelocity.cpp
    │   │   │   │   ├── OffsetsChangeWithAdditionalVelocity.h
    │   │   │   │   ├── RepeatedScrollSnapPoint.h
    │   │   │   │   ├── RepeatedZoomSnapPoint.h
    │   │   │   │   ├── ScrollControllerAddScrollVelocityRequestedEventArgs.cpp
    │   │   │   │   ├── ScrollControllerAddScrollVelocityRequestedEventArgs.h
    │   │   │   │   ├── ScrollControllerPanRequestedEventArgs.cpp
    │   │   │   │   ├── ScrollControllerPanRequestedEventArgs.h
    │   │   │   │   ├── ScrollControllerScrollByRequestedEventArgs.cpp
    │   │   │   │   ├── ScrollControllerScrollByRequestedEventArgs.h
    │   │   │   │   ├── ScrollControllerScrollToRequestedEventArgs.cpp
    │   │   │   │   ├── ScrollControllerScrollToRequestedEventArgs.h
    │   │   │   │   ├── ScrollingAnchorRequestedEventArgs.cpp
    │   │   │   │   ├── ScrollingAnchorRequestedEventArgs.h
    │   │   │   │   ├── ScrollingBringingIntoViewEventArgs.cpp
    │   │   │   │   ├── ScrollingBringingIntoViewEventArgs.h
    │   │   │   │   ├── ScrollingScrollAnimationStartingEventArgs.cpp
    │   │   │   │   ├── ScrollingScrollAnimationStartingEventArgs.h
    │   │   │   │   ├── ScrollingScrollCompletedEventArgs.cpp
    │   │   │   │   ├── ScrollingScrollCompletedEventArgs.h
    │   │   │   │   ├── ScrollingScrollOptions.cpp
    │   │   │   │   ├── ScrollingScrollOptions.h
    │   │   │   │   ├── ScrollingScrollStartingEventArgs.cpp
    │   │   │   │   ├── ScrollingScrollStartingEventArgs.h
    │   │   │   │   ├── ScrollingZoomAnimationStartingEventArgs.cpp
    │   │   │   │   ├── ScrollingZoomAnimationStartingEventArgs.h
    │   │   │   │   ├── ScrollingZoomCompletedEventArgs.cpp
    │   │   │   │   ├── ScrollingZoomCompletedEventArgs.h
    │   │   │   │   ├── ScrollingZoomOptions.cpp
    │   │   │   │   ├── ScrollingZoomOptions.h
    │   │   │   │   ├── ScrollingZoomStartingEventArgs.cpp
    │   │   │   │   ├── ScrollingZoomStartingEventArgs.h
    │   │   │   │   ├── ScrollPresenter.cpp
    │   │   │   │   ├── ScrollPresenter.h
    │   │   │   │   ├── ScrollPresenter.idl
    │   │   │   │   ├── ScrollPresenter.vcxitems
    │   │   │   │   ├── ScrollPresenterAnchoring.cpp
    │   │   │   │   ├── ScrollPresenterAutomationPeer.cpp
    │   │   │   │   ├── ScrollPresenterAutomationPeer.h
    │   │   │   │   ├── ScrollPresenterAutomationPeer.idl
    │   │   │   │   ├── ScrollPresenterPrimitives.idl
    │   │   │   │   ├── ScrollPresenterPrivate.cpp
    │   │   │   │   ├── ScrollPresenterTestHooks.cpp
    │   │   │   │   ├── ScrollPresenterTestHooks.h
    │   │   │   │   ├── ScrollPresenterTestHooks.idl
    │   │   │   │   ├── ScrollPresenterTestHooksAnchorEvaluatedEventArgs.cpp
    │   │   │   │   ├── ScrollPresenterTestHooksAnchorEvaluatedEventArgs.h
    │   │   │   │   ├── ScrollPresenterTestHooksExpressionAnimationStatusChangedEventArgs.cpp
    │   │   │   │   ├── ScrollPresenterTestHooksExpressionAnimationStatusChangedEventArgs.h
    │   │   │   │   ├── ScrollPresenterTestHooksFactory.cpp
    │   │   │   │   ├── ScrollPresenterTestHooksFactory.h
    │   │   │   │   ├── ScrollPresenterTestHooksInteractionSourcesChangedEventArgs.cpp
    │   │   │   │   ├── ScrollPresenterTestHooksInteractionSourcesChangedEventArgs.h
    │   │   │   │   ├── ScrollPresenterTrace.h
    │   │   │   │   ├── ScrollPresenterTypeLogging.cpp
    │   │   │   │   ├── ScrollPresenterTypeLogging.h
    │   │   │   │   ├── ScrollSnapPoint.h
    │   │   │   │   ├── SnapPoint.cpp
    │   │   │   │   ├── SnapPoint.h
    │   │   │   │   ├── SnapPointWrapper.cpp
    │   │   │   │   ├── SnapPointWrapper.h
    │   │   │   │   ├── ViewChange.cpp
    │   │   │   │   ├── ViewChange.h
    │   │   │   │   ├── ViewChangeBase.h
    │   │   │   │   ├── ZoomFactorChange.cpp
    │   │   │   │   ├── ZoomFactorChange.h
    │   │   │   │   ├── ZoomFactorChangeWithAdditionalVelocity.cpp
    │   │   │   │   ├── ZoomFactorChangeWithAdditionalVelocity.h
    │   │   │   │   ├── ZoomSnapPoint.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ScrollControllerTests.cs
    │   │   │   │   │   ├── ScrollPresenter_APITests.projitems
    │   │   │   │   │   ├── ScrollPresenter_APITests.shproj
    │   │   │   │   │   ├── ScrollPresenterAnchoringTests.cs
    │   │   │   │   │   ├── ScrollPresenterBringIntoViewTests.cs
    │   │   │   │   │   ├── ScrollPresenterLayoutTests.cs
    │   │   │   │   │   ├── ScrollPresenterSnapPointTests.cs
    │   │   │   │   │   ├── ScrollPresenterTests.cs
    │   │   │   │   │   └── ScrollPresenterViewChangeTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ScrollPresenter_InteractionTests.projitems
    │   │   │   │   │   ├── ScrollPresenter_InteractionTests.shproj
    │   │   │   │   │   ├── ScrollPresenterTestsBase.cs
    │   │   │   │   │   ├── ScrollPresenterTestsWithAutomationPeer.cs
    │   │   │   │   │   └── ScrollPresenterTestsWithInputHelper.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── BiDirectionalScrollController.cs
    │   │   │   │       ├── CompositionScrollController.cs
    │   │   │   │       ├── ScrollPresenter_TestUI.projitems
    │   │   │   │       ├── ScrollPresenter_TestUI.shproj
    │   │   │   │       ├── ScrollPresenterAccessibilityPage.xaml
    │   │   │   │       ├── ScrollPresenterAccessibilityPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterBringIntoViewPage.xaml
    │   │   │   │       ├── ScrollPresenterBringIntoViewPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterChainingAndRailingPage.xaml
    │   │   │   │       ├── ScrollPresenterChainingAndRailingPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterDynamicPage.xaml
    │   │   │   │       ├── ScrollPresenterDynamicPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterExpressionAnimationSourcesPage.xaml
    │   │   │   │       ├── ScrollPresenterExpressionAnimationSourcesPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterLeakDetectionPage.xaml
    │   │   │   │       ├── ScrollPresenterLeakDetectionPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterManipulationModePage.xaml
    │   │   │   │       ├── ScrollPresenterManipulationModePage.xaml.cs
    │   │   │   │       ├── ScrollPresenterMousePanningPage.xaml
    │   │   │   │       ├── ScrollPresenterMousePanningPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterPage.xaml
    │   │   │   │       ├── ScrollPresenterPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterRepeaterAnchoringPage.xaml
    │   │   │   │       ├── ScrollPresenterRepeaterAnchoringPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterScrollSnapPointsPage.xaml
    │   │   │   │       ├── ScrollPresenterScrollSnapPointsPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterStackPanelAnchoringPage.xaml
    │   │   │   │       ├── ScrollPresenterStackPanelAnchoringPage.xaml.cs
    │   │   │   │       ├── ScrollPresentersWithSimpleContentsPage.xaml
    │   │   │   │       ├── ScrollPresentersWithSimpleContentsPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterTestHooksHelper.cs
    │   │   │   │       ├── ScrollPresenterWithBiDirectionalScrollControllerPage.xaml
    │   │   │   │       ├── ScrollPresenterWithBiDirectionalScrollControllerPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterWithCompositionScrollControllersPage.xaml
    │   │   │   │       ├── ScrollPresenterWithCompositionScrollControllersPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterWithSimpleScrollControllersPage.xaml
    │   │   │   │       ├── ScrollPresenterWithSimpleScrollControllersPage.xaml.cs
    │   │   │   │       ├── ScrollPresenterZoomSnapPointsPage.xaml
    │   │   │   │       ├── ScrollPresenterZoomSnapPointsPage.xaml.cs
    │   │   │   │       └── Themes/
    │   │   │   │           └── AdditionalStyles.xaml
    │   │   │   ├── ScrollView/
    │   │   │   │   ├── ScrollBarController.cpp
    │   │   │   │   ├── ScrollBarController.h
    │   │   │   │   ├── ScrollView.cpp
    │   │   │   │   ├── ScrollView.h
    │   │   │   │   ├── ScrollView.idl
    │   │   │   │   ├── ScrollView.vcxitems
    │   │   │   │   ├── ScrollView.xaml
    │   │   │   │   ├── ScrollView_themeresources.xaml
    │   │   │   │   ├── ScrollViewBringIntoViewOperation.cpp
    │   │   │   │   ├── ScrollViewBringIntoViewOperation.h
    │   │   │   │   ├── ScrollViewLightup.cpp
    │   │   │   │   ├── ScrollViewTestHooks.cpp
    │   │   │   │   ├── ScrollViewTestHooks.h
    │   │   │   │   ├── ScrollViewTestHooks.idl
    │   │   │   │   ├── ScrollViewTestHooksFactory.cpp
    │   │   │   │   ├── ScrollViewTestHooksFactory.h
    │   │   │   │   ├── ScrollViewTrace.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── ScrollView_APITests.projitems
    │   │   │   │   │   ├── ScrollView_APITests.shproj
    │   │   │   │   │   └── ScrollViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── ScrollView_InteractionTests.projitems
    │   │   │   │   │   ├── ScrollView_InteractionTests.shproj
    │   │   │   │   │   └── ScrollViewTestsWithInputHelper.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── ScrollView_TestUI.projitems
    │   │   │   │       ├── ScrollView_TestUI.shproj
    │   │   │   │       ├── ScrollViewBlankPage.xaml
    │   │   │   │       ├── ScrollViewBlankPage.xaml.cs
    │   │   │   │       ├── ScrollViewBringIntoViewPage.xaml
    │   │   │   │       ├── ScrollViewBringIntoViewPage.xaml.cs
    │   │   │   │       ├── ScrollViewDynamicPage.xaml
    │   │   │   │       ├── ScrollViewDynamicPage.xaml.cs
    │   │   │   │       ├── ScrollViewKeyboardAndGamepadNavigationPage.xaml
    │   │   │   │       ├── ScrollViewKeyboardAndGamepadNavigationPage.xaml.cs
    │   │   │   │       ├── ScrollViewPage.xaml
    │   │   │   │       ├── ScrollViewPage.xaml.cs
    │   │   │   │       ├── ScrollViewsWithSimpleContentsPage.xaml
    │   │   │   │       ├── ScrollViewsWithSimpleContentsPage.xaml.cs
    │   │   │   │       ├── ScrollViewTestHooksHelper.cs
    │   │   │   │       ├── ScrollViewWithRTLFlowDirectionPage.xaml
    │   │   │   │       ├── ScrollViewWithRTLFlowDirectionPage.xaml.cs
    │   │   │   │       ├── ScrollViewWithScrollControllersPage.xaml
    │   │   │   │       └── ScrollViewWithScrollControllersPage.xaml.cs
    │   │   │   ├── SelectorBar/
    │   │   │   │   ├── SelectorBar.cpp
    │   │   │   │   ├── SelectorBar.h
    │   │   │   │   ├── SelectorBar.idl
    │   │   │   │   ├── SelectorBar.vcxitems
    │   │   │   │   ├── SelectorBar.xaml
    │   │   │   │   ├── SelectorBar_themeresources.xaml
    │   │   │   │   ├── SelectorBarItem.cpp
    │   │   │   │   ├── SelectorBarItem.h
    │   │   │   │   ├── SelectorBarItemAutomationPeer.cpp
    │   │   │   │   ├── SelectorBarItemAutomationPeer.h
    │   │   │   │   ├── SelectorBarSelectionChangedEventArgs.cpp
    │   │   │   │   ├── SelectorBarSelectionChangedEventArgs.h
    │   │   │   │   ├── SelectorBarTestHooks.cpp
    │   │   │   │   ├── SelectorBarTestHooks.h
    │   │   │   │   ├── SelectorBarTestHooks.idl
    │   │   │   │   ├── SelectorBarTestHooksFactory.cpp
    │   │   │   │   ├── SelectorBarTestHooksFactory.h
    │   │   │   │   ├── SelectorBarTrace.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── SelectorBar_APITests.projitems
    │   │   │   │   │   ├── SelectorBar_APITests.shproj
    │   │   │   │   │   └── SelectorBarTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── SelectorBar_InteractionTests.projitems
    │   │   │   │   │   ├── SelectorBar_InteractionTests.shproj
    │   │   │   │   │   └── SelectorBarTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── SelectorBar_TestUI.projitems
    │   │   │   │       ├── SelectorBar_TestUI.shproj
    │   │   │   │       ├── SelectorBarPage.xaml
    │   │   │   │       ├── SelectorBarPage.xaml.cs
    │   │   │   │       ├── SelectorBarSamplePage.xaml
    │   │   │   │       ├── SelectorBarSamplePage.xaml.cs
    │   │   │   │       ├── SelectorBarSummaryPage.xaml
    │   │   │   │       └── SelectorBarSummaryPage.xaml.cs
    │   │   │   ├── SplitButton/
    │   │   │   │   ├── SplitButton.cpp
    │   │   │   │   ├── SplitButton.h
    │   │   │   │   ├── SplitButton.idl
    │   │   │   │   ├── SplitButton.vcxitems
    │   │   │   │   ├── SplitButton.xaml
    │   │   │   │   ├── SplitButton_themeresources.xaml
    │   │   │   │   ├── SplitButtonAutomationPeer.cpp
    │   │   │   │   ├── SplitButtonAutomationPeer.h
    │   │   │   │   ├── SplitButtonAutomationPeer.idl
    │   │   │   │   ├── SplitButtonEventArgs.h
    │   │   │   │   ├── SplitButtonTestApi.cpp
    │   │   │   │   ├── SplitButtonTestApi.h
    │   │   │   │   ├── SplitButtonTestApi.idl
    │   │   │   │   ├── SplitButtonTestApiFactory.cpp
    │   │   │   │   ├── SplitButtonTestHelper.cpp
    │   │   │   │   ├── SplitButtonTestHelper.h
    │   │   │   │   ├── ToggleSplitButton.cpp
    │   │   │   │   ├── ToggleSplitButton.h
    │   │   │   │   ├── ToggleSplitButtonAutomationPeer.cpp
    │   │   │   │   ├── ToggleSplitButtonAutomationPeer.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── SplitButton_APITests.projitems
    │   │   │   │   │   ├── SplitButton_APITests.shproj
    │   │   │   │   │   └── SplitButtonTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── SplitButton_InteractionTests.projitems
    │   │   │   │   │   ├── SplitButton_InteractionTests.shproj
    │   │   │   │   │   └── SplitButtonTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── SplitButton_TestUI.projitems
    │   │   │   │       ├── SplitButton_TestUI.shproj
    │   │   │   │       ├── SplitButtonPage.xaml
    │   │   │   │       └── SplitButtonPage.xaml.cs
    │   │   │   ├── SplitView/
    │   │   │   │   ├── SplitView.vcxitems
    │   │   │   │   ├── SplitView_themeresources.xaml
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── SplitView_TestUI.projitems
    │   │   │   │       ├── SplitView_TestUI.shproj
    │   │   │   │       ├── SplitViewPage.xaml
    │   │   │   │       └── SplitViewPage.xaml.cs
    │   │   │   ├── SwipeControl/
    │   │   │   │   ├── SwipeControl.cpp
    │   │   │   │   ├── SwipeControl.h
    │   │   │   │   ├── SwipeControl.idl
    │   │   │   │   ├── SwipeControl.vcxitems
    │   │   │   │   ├── SwipeControl.xaml
    │   │   │   │   ├── SwipeControl_themeresources.xaml
    │   │   │   │   ├── SwipeControlInteractionTrackerOwner.cpp
    │   │   │   │   ├── SwipeControlInteractionTrackerOwner.h
    │   │   │   │   ├── SwipeControlTrace.h
    │   │   │   │   ├── SwipeItem.cpp
    │   │   │   │   ├── SwipeItem.h
    │   │   │   │   ├── SwipeItemInvokedEventArgs.cpp
    │   │   │   │   ├── SwipeItemInvokedEventArgs.h
    │   │   │   │   ├── SwipeItems.cpp
    │   │   │   │   ├── SwipeItems.h
    │   │   │   │   ├── SwipeTestHooks.cpp
    │   │   │   │   ├── SwipeTestHooks.h
    │   │   │   │   ├── SwipeTestHooks.idl
    │   │   │   │   ├── SwipeTestHooksFactory.cpp
    │   │   │   │   ├── SwipeTestHooksFactory.h
    │   │   │   │   ├── SwipeControl_APITests/
    │   │   │   │   │   ├── SwipeControl_APITests.projitems
    │   │   │   │   │   ├── SwipeControl_APITests.shproj
    │   │   │   │   │   └── SwipeControlTests.cs
    │   │   │   │   ├── SwipeControl_InteractionTests/
    │   │   │   │   │   ├── SwipeControl_InteractionTests.projitems
    │   │   │   │   │   ├── SwipeControl_InteractionTests.shproj
    │   │   │   │   │   └── SwipeControlTests.cs
    │   │   │   │   └── SwipeControl_TestUI/
    │   │   │   │       ├── SwipeControl_TestUI.projitems
    │   │   │   │       ├── SwipeControl_TestUI.shproj
    │   │   │   │       ├── SwipeControlClearPage.xaml
    │   │   │   │       ├── SwipeControlClearPage.xaml.cs
    │   │   │   │       ├── SwipeControlPage.xaml
    │   │   │   │       ├── SwipeControlPage.xaml.cs
    │   │   │   │       ├── SwipeControlPage2.xaml
    │   │   │   │       ├── SwipeControlPage2.xaml.cs
    │   │   │   │       ├── SwipePage.xaml
    │   │   │   │       ├── SwipePage.xaml.cs
    │   │   │   │       └── TestCommand.cs
    │   │   │   ├── TabView/
    │   │   │   │   ├── TabView.cpp
    │   │   │   │   ├── TabView.h
    │   │   │   │   ├── TabView.idl
    │   │   │   │   ├── TabView.vcxitems
    │   │   │   │   ├── TabView.xaml
    │   │   │   │   ├── TabView_themeresources.xaml
    │   │   │   │   ├── TabViewAutomationPeer.cpp
    │   │   │   │   ├── TabViewAutomationPeer.h
    │   │   │   │   ├── TabViewItem.cpp
    │   │   │   │   ├── TabViewItem.h
    │   │   │   │   ├── TabViewItemAutomationPeer.cpp
    │   │   │   │   ├── TabViewItemAutomationPeer.h
    │   │   │   │   ├── TabViewItemTemplateSettings.h
    │   │   │   │   ├── TabViewListView.cpp
    │   │   │   │   ├── TabViewListView.h
    │   │   │   │   ├── TabViewTrace.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── TabView_APITests.projitems
    │   │   │   │   │   ├── TabView_APITests.shproj
    │   │   │   │   │   └── TabViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── TabView_InteractionTests.projitems
    │   │   │   │   │   ├── TabView_InteractionTests.shproj
    │   │   │   │   │   ├── TabViewTearOutTests.cs
    │   │   │   │   │   └── TabViewTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── MultipleTabViewPage.xaml
    │   │   │   │       ├── MultipleTabViewPage.xaml.cs
    │   │   │   │       ├── TabView_TestUI.projitems
    │   │   │   │       ├── TabView_TestUI.shproj
    │   │   │   │       ├── TabViewAxeTestPage.xaml
    │   │   │   │       ├── TabViewAxeTestPage.xaml.cs
    │   │   │   │       ├── TabViewPage.xaml
    │   │   │   │       ├── TabViewPage.xaml.cs
    │   │   │   │       ├── TabViewSizingPage.xaml
    │   │   │   │       ├── TabViewSizingPage.xaml.cs
    │   │   │   │       ├── TabViewTabClosingBehaviorPage.xaml
    │   │   │   │       ├── TabViewTabClosingBehaviorPage.xaml.cs
    │   │   │   │       ├── TabViewTabItemsSourcePage.xaml
    │   │   │   │       ├── TabViewTabItemsSourcePage.xaml.cs
    │   │   │   │       ├── TabViewTearOutWindowWithDataItems.xaml
    │   │   │   │       ├── TabViewTearOutWindowWithDataItems.xaml.cs
    │   │   │   │       ├── TabViewTearOutWindowWithoutDataItems.xaml
    │   │   │   │       └── TabViewTearOutWindowWithoutDataItems.xaml.cs
    │   │   │   ├── TeachingTip/
    │   │   │   │   ├── TeachingTip.cpp
    │   │   │   │   ├── TeachingTip.h
    │   │   │   │   ├── TeachingTip.idl
    │   │   │   │   ├── TeachingTip.vcxitems
    │   │   │   │   ├── TeachingTip.xaml
    │   │   │   │   ├── TeachingTip_themeresources.xaml
    │   │   │   │   ├── TeachingTipAutomationPeer.cpp
    │   │   │   │   ├── TeachingTipAutomationPeer.h
    │   │   │   │   ├── TeachingTipAutomationPeer.idl
    │   │   │   │   ├── TeachingTipClosedEventArgs.cpp
    │   │   │   │   ├── TeachingTipClosedEventArgs.h
    │   │   │   │   ├── TeachingTipClosingEventArgs.cpp
    │   │   │   │   ├── TeachingTipClosingEventArgs.h
    │   │   │   │   ├── TeachingTipTemplateSettings.cpp
    │   │   │   │   ├── TeachingTipTemplateSettings.h
    │   │   │   │   ├── TeachingTipTestHooks.cpp
    │   │   │   │   ├── TeachingTipTestHooks.h
    │   │   │   │   ├── TeachingTipTestHooks.idl
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── TeachingTip_APITests.projitems
    │   │   │   │   │   ├── TeachingTip_APITests.shproj
    │   │   │   │   │   └── TeachingTipTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── TeachingTip_InteractionTests.projitems
    │   │   │   │   │   ├── TeachingTip_InteractionTests.shproj
    │   │   │   │   │   ├── TeachingTipFocusTestPageElements.cs
    │   │   │   │   │   ├── TeachingTipTestPageElements.cs
    │   │   │   │   │   └── TeachingTipTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── TeachingTip-FocusBehavior.md
    │   │   │   │       ├── TeachingTip_TestUI.projitems
    │   │   │   │       ├── TeachingTip_TestUI.shproj
    │   │   │   │       ├── TeachingTipCaseBundle.xaml
    │   │   │   │       ├── TeachingTipCaseBundle.xaml.cs
    │   │   │   │       ├── TeachingTipFocusPage.xaml
    │   │   │   │       ├── TeachingTipFocusPage.xaml.cs
    │   │   │   │       ├── TeachingTipInXamlPage.xaml
    │   │   │   │       ├── TeachingTipInXamlPage.xaml.cs
    │   │   │   │       ├── TeachingTipPage.xaml
    │   │   │   │       └── TeachingTipPage.xaml.cs
    │   │   │   ├── Telemetry/
    │   │   │   │   ├── MicrosoftTelemetry.h
    │   │   │   │   ├── MuxcTraceLogging.cpp
    │   │   │   │   ├── MuxcTraceLogging.h
    │   │   │   │   ├── RuntimeProfiler.cpp
    │   │   │   │   ├── RuntimeProfiler.h
    │   │   │   │   ├── Telemetry.vcxitems
    │   │   │   │   ├── TypeLogging.cpp
    │   │   │   │   └── TypeLogging.h
    │   │   │   ├── TestHooks/
    │   │   │   │   ├── MUXControlsTestHooks.cpp
    │   │   │   │   ├── MUXControlsTestHooks.h
    │   │   │   │   ├── MUXControlsTestHooks.idl
    │   │   │   │   ├── MUXControlsTestHooksFactory.cpp
    │   │   │   │   ├── MUXControlsTestHooksFactory.h
    │   │   │   │   ├── MUXControlsTestHooksLoggingMessageEventArgs.cpp
    │   │   │   │   ├── MUXControlsTestHooksLoggingMessageEventArgs.h
    │   │   │   │   └── TestHooks.vcxitems
    │   │   │   ├── TitleBar/
    │   │   │   │   ├── TitleBar.cpp
    │   │   │   │   ├── TitleBar.h
    │   │   │   │   ├── TitleBar.idl
    │   │   │   │   ├── TitleBar.vcxitems
    │   │   │   │   ├── TitleBar.xaml
    │   │   │   │   ├── TitleBar_themeresources.xaml
    │   │   │   │   ├── TitleBarAutomationPeer.cpp
    │   │   │   │   ├── TitleBarAutomationPeer.h
    │   │   │   │   ├── TitleBarTemplateSettings.cpp
    │   │   │   │   ├── TitleBarTemplateSettings.h
    │   │   │   │   ├── TitleBarTrace.h
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── TitleBar_InteractionTests.projitems
    │   │   │   │   │   ├── TitleBar_InteractionTests.shproj
    │   │   │   │   │   └── TitleBarTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-ET/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-us/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-PH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-KH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-LA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-MK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ml-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── te-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-Latn-UZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── TitleBar_TestUI.projitems
    │   │   │   │       ├── TitleBar_TestUI.shproj
    │   │   │   │       ├── TitleBarPage.xaml
    │   │   │   │       ├── TitleBarPage.xaml.cs
    │   │   │   │       ├── TitleBarPageWindow.xaml
    │   │   │   │       └── TitleBarPageWindow.xaml.cs
    │   │   │   ├── TreeView/
    │   │   │   │   ├── TreeView.cpp
    │   │   │   │   ├── TreeView.h
    │   │   │   │   ├── TreeView.idl
    │   │   │   │   ├── TreeView.vcxitems
    │   │   │   │   ├── TreeView.xaml
    │   │   │   │   ├── TreeView_themeresources.xaml
    │   │   │   │   ├── TreeViewAutomationPeers.idl
    │   │   │   │   ├── TreeViewCollapsedEventArgs.cpp
    │   │   │   │   ├── TreeViewCollapsedEventArgs.h
    │   │   │   │   ├── TreeViewDragItemsCompletedEventArgs.cpp
    │   │   │   │   ├── TreeViewDragItemsCompletedEventArgs.h
    │   │   │   │   ├── TreeViewDragItemsStartingEventArgs.cpp
    │   │   │   │   ├── TreeViewDragItemsStartingEventArgs.h
    │   │   │   │   ├── TreeViewExpandingEventArgs.cpp
    │   │   │   │   ├── TreeViewExpandingEventArgs.h
    │   │   │   │   ├── TreeViewItem.cpp
    │   │   │   │   ├── TreeViewItem.h
    │   │   │   │   ├── TreeViewItem.xaml
    │   │   │   │   ├── TreeViewItemAutomationPeer.cpp
    │   │   │   │   ├── TreeViewItemAutomationPeer.h
    │   │   │   │   ├── TreeViewItemDataAutomationPeer.cpp
    │   │   │   │   ├── TreeViewItemDataAutomationPeer.h
    │   │   │   │   ├── TreeViewItemInvokedEventArgs.cpp
    │   │   │   │   ├── TreeViewItemInvokedEventArgs.h
    │   │   │   │   ├── TreeViewItemTemplateSettings.cpp
    │   │   │   │   ├── TreeViewItemTemplateSettings.h
    │   │   │   │   ├── TreeViewList.cpp
    │   │   │   │   ├── TreeViewList.h
    │   │   │   │   ├── TreeViewListAutomationPeer.cpp
    │   │   │   │   ├── TreeViewListAutomationPeer.h
    │   │   │   │   ├── TreeViewNode.cpp
    │   │   │   │   ├── TreeViewNode.h
    │   │   │   │   ├── TreeViewSelectionChangedEventArgs.cpp
    │   │   │   │   ├── TreeViewSelectionChangedEventArgs.h
    │   │   │   │   ├── ViewModel.cpp
    │   │   │   │   ├── ViewModel.h
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── TreeView_APITests.projitems
    │   │   │   │   │   ├── TreeView_APITests.shproj
    │   │   │   │   │   └── TreeViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── TreeView_InteractionTests.projitems
    │   │   │   │   │   ├── TreeView_InteractionTests.shproj
    │   │   │   │   │   └── TreeViewTests.cs
    │   │   │   │   ├── Strings/
    │   │   │   │   │   ├── af-ZA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── am-et/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ar-SA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── as-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── az-Latn-AZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bg-BG/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bn-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── bs-Latn-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ca-Es-VALENCIA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cs-CZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── cy-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── da-DK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── de-DE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── el-GR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-GB/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── en-US/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── es-MX/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── et-EE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── eu-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fa-IR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fi-FI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fil-ph/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── fr-CA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── fr-FR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ga-IE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gd-gb/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gl-ES/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── gu-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── he-IL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hi-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hr-HR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hu-HU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── hy-AM/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── id-ID/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── is-IS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── it-IT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ja-JP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ka-GE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kk-KZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── km-kh/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── kn-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ko-KR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── kok-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lb-LU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lo-la/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── lt-LT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── lv-LV/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mi-NZ/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mk-mk/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── ml-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── mr-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ms-MY/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── mt-MT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nb-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ne-NP/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nl-NL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── nn-NO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── or-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pa-IN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pl-PL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-BR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── pt-PT/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── quz-PE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ro-RO/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ru-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sk-SK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sl-SI/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sq-AL/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-BA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Cyrl-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sr-Latn-RS/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── sv-SE/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ta-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── te-in/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── th-TH/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tr-TR/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── tt-RU/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ug-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uk-UA/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── ur-PK/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── uz-latn-uz/
    │   │   │   │   │   │   └── resources.resw
    │   │   │   │   │   ├── vi-VN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   ├── zh-CN/
    │   │   │   │   │   │   └── Resources.resw
    │   │   │   │   │   └── zh-TW/
    │   │   │   │   │       └── Resources.resw
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── TreeView_TestUI.projitems
    │   │   │   │       ├── TreeView_TestUI.shproj
    │   │   │   │       ├── TreeViewItemSource.cs
    │   │   │   │       ├── TreeViewItemsSourceTestPage.xaml
    │   │   │   │       ├── TreeViewItemsSourceTestPage.xaml.cs
    │   │   │   │       ├── TreeViewItemTemplateSelectorTestPage.xaml
    │   │   │   │       ├── TreeViewItemTemplateSelectorTestPage.xaml.cs
    │   │   │   │       ├── TreeViewLateDataInitTestPage.xaml
    │   │   │   │       ├── TreeViewLateDataInitTestPage.xaml.cs
    │   │   │   │       ├── TreeViewNode2.cs
    │   │   │   │       ├── TreeViewNodeInMarkupTestPage.xaml
    │   │   │   │       ├── TreeViewNodeInMarkupTestPage.xaml.cs
    │   │   │   │       ├── TreeViewPage.xaml
    │   │   │   │       ├── TreeViewPage.xaml.cs
    │   │   │   │       ├── TreeViewUnrealizedChildrenTestPage.xaml
    │   │   │   │       ├── TreeViewUnrealizedChildrenTestPage.xaml.cs
    │   │   │   │       ├── TreeViewViewModel.cs
    │   │   │   │       └── VirtualizingDataSource.cs
    │   │   │   ├── TwoPaneView/
    │   │   │   │   ├── DisplayRegionHelper.cpp
    │   │   │   │   ├── DisplayRegionHelper.h
    │   │   │   │   ├── DisplayRegionHelperTestApi.cpp
    │   │   │   │   ├── DisplayRegionHelperTestApi.h
    │   │   │   │   ├── DisplayRegionHelperTestApi.idl
    │   │   │   │   ├── DisplayRegionHelperTestApiFactory.cpp
    │   │   │   │   ├── DisplayRegionHelperTestApiFactory.h
    │   │   │   │   ├── TwoPaneView.cpp
    │   │   │   │   ├── TwoPaneView.h
    │   │   │   │   ├── TwoPaneView.idl
    │   │   │   │   ├── TwoPaneView.vcxitems
    │   │   │   │   ├── TwoPaneView.xaml
    │   │   │   │   ├── APITests/
    │   │   │   │   │   ├── TwoPaneView_APITests.projitems
    │   │   │   │   │   ├── TwoPaneView_APITests.shproj
    │   │   │   │   │   └── TwoPaneViewTests.cs
    │   │   │   │   ├── InteractionTests/
    │   │   │   │   │   ├── TwoPaneView_InteractionTests.projitems
    │   │   │   │   │   ├── TwoPaneView_InteractionTests.shproj
    │   │   │   │   │   └── TwoPaneViewTests.cs
    │   │   │   │   └── TestUI/
    │   │   │   │       ├── TwoPaneView_TestUI.projitems
    │   │   │   │       ├── TwoPaneView_TestUI.shproj
    │   │   │   │       ├── TwoPaneViewPage.xaml
    │   │   │   │       └── TwoPaneViewPage.xaml.cs
    │   │   │   └── WebView2/
    │   │   │       ├── InvokableCallbackHelper.h
    │   │   │       ├── WebView2-Accessibility.md
    │   │   │       ├── WebView2-update.md
    │   │   │       ├── WebView2-versions.md
    │   │   │       ├── WebView2.cpp
    │   │   │       ├── WebView2.h
    │   │   │       ├── WebView2.idl
    │   │   │       ├── WebView2.md
    │   │   │       ├── WebView2.vcxitems
    │   │   │       ├── WebView2AutomationPeer.cpp
    │   │   │       ├── WebView2AutomationPeer.h
    │   │   │       ├── WebView2AutomationPeer.idl
    │   │   │       ├── WebView2Utility.h
    │   │   │       ├── InteractionTests/
    │   │   │       │   ├── WebView2_InteractionTests.projitems
    │   │   │       │   ├── WebView2_InteractionTests.shproj
    │   │   │       │   └── WebView2Tests.cs
    │   │   │       ├── Strings/
    │   │   │       │   ├── af-ZA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── am-ET/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ar-SA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── as-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── az-Latn-AZ/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── bg-BG/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── bn-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── bs-Latn-BA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ca-ES/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ca-Es-VALENCIA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── cs-CZ/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── cy-GB/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── da-DK/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── de-DE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── el-GR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── en-GB/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── en-us/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── es-ES/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── es-MX/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── et-EE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── eu-ES/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── fa-IR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── fi-FI/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── fil-PH/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── fr-CA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── fr-FR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ga-IE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── gd-gb/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── gl-ES/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── gu-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── he-IL/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── hi-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── hr-HR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── hu-HU/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── hy-AM/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── id-ID/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── is-IS/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── it-IT/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ja-JP/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ka-GE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── kk-KZ/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── km-KH/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── kn-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ko-KR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── kok-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── lb-LU/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── lo-LA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── lt-LT/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── lv-LV/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── mi-NZ/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── mk-MK/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ml-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── mr-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ms-MY/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── mt-MT/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── nb-NO/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ne-NP/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── nl-NL/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── nn-NO/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── or-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── pa-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── pl-PL/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── pt-BR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── pt-PT/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── quz-PE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ro-RO/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ru-RU/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sk-SK/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sl-SI/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sq-AL/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sr-Cyrl-BA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sr-Cyrl-RS/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sr-Latn-RS/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── sv-SE/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ta-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── te-IN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── th-TH/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── tr-TR/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── tt-RU/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ug-CN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── uk-UA/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── ur-PK/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── uz-Latn-UZ/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── vi-VN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   ├── zh-CN/
    │   │   │       │   │   └── Resources.resw
    │   │   │       │   └── zh-TW/
    │   │   │       │       └── Resources.resw
    │   │   │       └── TestUI/
    │   │   │           ├── WebView2_TestUI.projitems
    │   │   │           ├── WebView2_TestUI.shproj
    │   │   │           ├── WebView2BasicPage.xaml
    │   │   │           ├── WebView2BasicPage.xaml.cs
    │   │   │           ├── WebView2Common.cs
    │   │   │           ├── WebView2CoreObjectsPage.xaml
    │   │   │           ├── WebView2CoreObjectsPage.xaml.cs
    │   │   │           ├── WebView2Page.xaml
    │   │   │           └── WebView2Page.xaml.cs
    │   │   ├── idl/
    │   │   │   ├── DPCodeGenAttributes.idl
    │   │   │   ├── Effects.idl
    │   │   │   ├── Microsoft.UI.Xaml.Controls.idl
    │   │   │   └── Microsoft.UI.Xaml.Controls.idl.vcxproj
    │   │   ├── test/
    │   │   │   ├── Directory.Build.props
    │   │   │   ├── Directory.Build.targets
    │   │   │   ├── dirs.proj
    │   │   │   ├── RetargetCopyLocalFiles.targets
    │   │   │   ├── TestApp.targets
    │   │   │   ├── IXMPTestApp/
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── App.xaml.cs
    │   │   │   │   ├── IXMPTestApp.csproj
    │   │   │   │   ├── IXMPTestApp.sln
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   ├── WaitForDebugger.cs
    │   │   │   │   ├── Properties/
    │   │   │   │   │   ├── App.rd.xml
    │   │   │   │   │   └── AssemblyInfo.cs
    │   │   │   │   └── Tests/
    │   │   │   │       └── MetadataProviderTests.cs
    │   │   │   ├── MUXControls.Test/
    │   │   │   │   ├── AxeTestHelper.cs
    │   │   │   │   ├── DebugHelper.cs
    │   │   │   │   ├── Directory.Build.props
    │   │   │   │   ├── MUXControls.Test.csproj
    │   │   │   │   ├── PreRunTests.cs
    │   │   │   │   ├── TestAssembly.cs
    │   │   │   │   ├── PrivateAPITests/
    │   │   │   │   │   └── PrivateMetaDataTests.cs
    │   │   │   │   └── ScenarioAppTests/
    │   │   │   │       ├── GenerateWinUIGalleryTestData.ps1
    │   │   │   │       ├── WinUICppDesktopSampleAppTests.cs
    │   │   │   │       ├── WinUICsDesktopSampleAppTests.cs
    │   │   │   │       ├── WinUIGalleryDesktopTests.cs
    │   │   │   │       └── WinUISampleAppTestsUtils.cs
    │   │   │   ├── MUXControlsTestApp/
    │   │   │   │   ├── ApiTestAssemblyHandling.cs
    │   │   │   │   ├── app.manifest
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── App.xaml.cs
    │   │   │   │   ├── AppxManifest.xml
    │   │   │   │   ├── Common.props
    │   │   │   │   ├── Common.targets
    │   │   │   │   ├── ContentIncludes.props
    │   │   │   │   ├── Directory.Build.props
    │   │   │   │   ├── LeakTestPage.xaml
    │   │   │   │   ├── LeakTestPage.xaml.cs
    │   │   │   │   ├── LeakTests.cs
    │   │   │   │   ├── LocalizationTests.cs
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   ├── MUXControlsTestApp.csproj
    │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   ├── TestInventory.cs
    │   │   │   │   ├── ThemeResourcesTests.cs
    │   │   │   │   ├── VisualTreeTestHelper.cs
    │   │   │   │   ├── Assets/
    │   │   │   │   │   ├── ladybug.wmv
    │   │   │   │   │   ├── SimpleInputPage.html
    │   │   │   │   │   ├── SimplePage.html
    │   │   │   │   │   ├── SimplePageForFocus.html
    │   │   │   │   │   ├── SimplePageWithButton.html
    │   │   │   │   │   ├── SimplePageWithImage.html
    │   │   │   │   │   ├── SimplePageWithManyButtons.html
    │   │   │   │   │   ├── SimplePageWithNonÅscií.html
    │   │   │   │   │   ├── SimplePageWithScrollableColoredBlocks.html
    │   │   │   │   │   └── SimplePageWithText.html
    │   │   │   │   ├── DataModel/
    │   │   │   │   │   ├── Entity.cs
    │   │   │   │   │   ├── EntityGroup.cs
    │   │   │   │   │   └── EntityObservableCollection.cs
    │   │   │   │   ├── MiscTests/
    │   │   │   │   │   └── FocusTests.cs
    │   │   │   │   ├── Properties/
    │   │   │   │   │   ├── App.rd.xml
    │   │   │   │   │   ├── AssemblyInfo.cs
    │   │   │   │   │   └── PublishProfiles/
    │   │   │   │   │       ├── win10-arm64.pubxml
    │   │   │   │   │       ├── win10-x64.pubxml
    │   │   │   │   │       └── win10-x86.pubxml
    │   │   │   │   ├── Themes/
    │   │   │   │   │   └── DisableAnimationsStyles.xaml
    │   │   │   │   ├── Utilities/
    │   │   │   │   │   ├── APITestBase.cs
    │   │   │   │   │   ├── AxeScanTestPageAttribute.cs
    │   │   │   │   │   ├── CompositionPropertyLogger.cs
    │   │   │   │   │   ├── CompositionPropertySpy.cs
    │   │   │   │   │   ├── ExtendedObservableCollection.cs
    │   │   │   │   │   ├── IdleSynchronizer.cs
    │   │   │   │   │   ├── MaterialHelper.cs
    │   │   │   │   │   ├── PrivateLoggingHelper.cs
    │   │   │   │   │   ├── RunOnUIThread.cs
    │   │   │   │   │   ├── SemanticZoomTemplateItem.cs
    │   │   │   │   │   ├── SemanticZoomTemplateSelector.cs
    │   │   │   │   │   ├── TestHelpers.cs
    │   │   │   │   │   ├── TopLevelTestPageAttribute.cs
    │   │   │   │   │   ├── ViewHelper.cs
    │   │   │   │   │   ├── VisualTreeUtils.cs
    │   │   │   │   │   ├── ControlStateViewer/
    │   │   │   │   │   │   ├── ControlStateViewer.xaml
    │   │   │   │   │   │   └── ControlStateViewer.xaml.cs
    │   │   │   │   │   ├── EntityPropertiesControl/
    │   │   │   │   │   │   ├── EntityPropertiesControl.xaml
    │   │   │   │   │   │   ├── EntityPropertiesControl.xaml.cs
    │   │   │   │   │   │   ├── EntityPropertyControlDiscardedEventArgs.cs
    │   │   │   │   │   │   ├── EntityPropertyControlGeneratedEventArgs.cs
    │   │   │   │   │   │   ├── EntityPropertyControlNeededEventArgs.cs
    │   │   │   │   │   │   └── TypeConverters.cs
    │   │   │   │   │   ├── LoggingContentControl/
    │   │   │   │   │   │   └── LoggingContentControl.cs
    │   │   │   │   │   └── TilePanel/
    │   │   │   │   │       └── TilePanel.cs
    │   │   │   │   └── verification/
    │   │   │   │       ├── AppBarButton.xml
    │   │   │   │       ├── AppBarToggleButton.xml
    │   │   │   │       ├── AutoSuggestBox.xml
    │   │   │   │       ├── Button.xml
    │   │   │   │       ├── CalendarView.xml
    │   │   │   │       ├── CheckBox.xml
    │   │   │   │       ├── ColorPicker.xml
    │   │   │   │       ├── ComboBox.xml
    │   │   │   │       ├── CommandBar.xml
    │   │   │   │       ├── CommandBarOverflowMenu.xml
    │   │   │   │       ├── ContentDialog.xml
    │   │   │   │       ├── DatePicker.xml
    │   │   │   │       ├── FlipView.xml
    │   │   │   │       ├── ListViewItem.xml
    │   │   │   │       ├── NavigationViewAuto.xml
    │   │   │   │       ├── NavigationViewHierarchy.xml
    │   │   │   │       ├── NavigationViewLeftCompact.xml
    │   │   │   │       ├── NavigationViewLeftMinimal.xml
    │   │   │   │       ├── NavigationViewLeftPaneContent.xml
    │   │   │   │       ├── NavigationViewScrolling.xml
    │   │   │   │       ├── NavigationViewTop.xml
    │   │   │   │       ├── NavigationViewTopPaneContent.xml
    │   │   │   │       ├── PasswordBox.xml
    │   │   │   │       ├── PersonPicture.xml
    │   │   │   │       ├── Pivot.xml
    │   │   │   │       ├── PivotItem.xml
    │   │   │   │       ├── RichEditBox.xml
    │   │   │   │       ├── Slider.xml
    │   │   │   │       ├── SplitView.xml
    │   │   │   │       ├── TextBox.xml
    │   │   │   │       ├── TimePicker.xml
    │   │   │   │       ├── ToggleButton.xml
    │   │   │   │       ├── ToggleSwitch.xml
    │   │   │   │       ├── ToolTip.xml
    │   │   │   │       ├── TreeView.xml
    │   │   │   │       ├── VerifyVerifyHeaderContentMarginOnMinimalNav.xml
    │   │   │   │       ├── VerifyVerifyHeaderContentMarginOnTopNav.xml
    │   │   │   │       ├── VerifyVisualTreeExampleForLightTheme_Light.xml
    │   │   │   │       ├── VerifyVisualTreeExampleLoadAndVerifyForAllThemes_Dark.xml
    │   │   │   │       ├── VerifyVisualTreeExampleLoadAndVerifyForAllThemes_Light.xml
    │   │   │   │       ├── VerifyVisualTreeExampleLoadAndVerifyForDarkThemeWithCustomName.xml
    │   │   │   │       ├── VerifyVisualTreeExampleWithCustomerFilter.xml
    │   │   │   │       ├── VerifyVisualTreeExampleWithCustomerPropertyValueTranslator.xml
    │   │   │   │       ├── VerifyVisualTreeForAppBarAndAppBarToggleButton.xml
    │   │   │   │       └── VerifyVisualTreeForCommandBarCornerRadius.xml
    │   │   │   ├── TabViewTearOutApp/
    │   │   │   │   ├── README.md
    │   │   │   │   ├── App.cpp
    │   │   │   │   ├── App.h
    │   │   │   │   ├── App.idl
    │   │   │   │   ├── app.manifest
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── DesktopWindow.cpp
    │   │   │   │   ├── DesktopWindow.h
    │   │   │   │   ├── DocumentInfo.cpp
    │   │   │   │   ├── DocumentInfo.h
    │   │   │   │   ├── DocumentInfo.idl
    │   │   │   │   ├── MainPage.idl
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cpp
    │   │   │   │   ├── MainPage.xaml.h
    │   │   │   │   ├── MainWindow.cpp
    │   │   │   │   ├── MainWindow.h
    │   │   │   │   ├── pch.cpp
    │   │   │   │   ├── pch.h
    │   │   │   │   ├── resource.h
    │   │   │   │   ├── TabViewTearOutApp.rc
    │   │   │   │   ├── TabViewTearOutApp.vcxproj
    │   │   │   │   ├── TabViewTearOutApp.vcxproj.filters
    │   │   │   │   ├── targetver.h
    │   │   │   │   ├── WinMain.cpp
    │   │   │   │   └── XamlUtil.h
    │   │   │   ├── TestAppCX/
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── App.xaml.cpp
    │   │   │   │   ├── App.xaml.h
    │   │   │   │   ├── BackdropMaterialTestPage.xaml
    │   │   │   │   ├── BackdropMaterialTestPage.xaml.cpp
    │   │   │   │   ├── BackdropMaterialTestPage.xaml.h
    │   │   │   │   ├── CornerRadiusTestPage.xaml
    │   │   │   │   ├── CornerRadiusTestPage.xaml.cpp
    │   │   │   │   ├── CornerRadiusTestPage.xaml.h
    │   │   │   │   ├── LeakCycleTestCX.xaml
    │   │   │   │   ├── LeakCycleTestCX.xaml.cpp
    │   │   │   │   ├── LeakCycleTestCX.xaml.h
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cpp
    │   │   │   │   ├── MainPage.xaml.h
    │   │   │   │   ├── MenuBarTestPage.xaml
    │   │   │   │   ├── MenuBarTestPage.xaml.cpp
    │   │   │   │   ├── MenuBarTestPage.xaml.h
    │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   ├── packages.config
    │   │   │   │   ├── pch.cpp
    │   │   │   │   ├── pch.h
    │   │   │   │   ├── TestAppCX.vcxproj
    │   │   │   │   ├── TestAppCX.vcxproj.filters
    │   │   │   │   ├── TreeViewTestPage.xaml
    │   │   │   │   ├── TreeViewTestPage.xaml.cpp
    │   │   │   │   ├── TreeViewTestPage.xaml.h
    │   │   │   │   ├── WebView2TestPage.xaml
    │   │   │   │   ├── WebView2TestPage.xaml.cpp
    │   │   │   │   └── WebView2TestPage.xaml.h
    │   │   │   ├── TestAppUtils/
    │   │   │   │   ├── DesignModeHelpers.cs
    │   │   │   │   ├── NavigateToTestCommand.cs
    │   │   │   │   ├── PlatformConfiguration.cs
    │   │   │   │   ├── TestAppUtils.projitems
    │   │   │   │   ├── TestAppUtils.shproj
    │   │   │   │   ├── TestDeclaration.cs
    │   │   │   │   ├── TestFrame.cs
    │   │   │   │   ├── TestPage.cs
    │   │   │   │   ├── VisualTreeDumper.cs
    │   │   │   │   └── Themes/
    │   │   │   │       └── Generic.xaml
    │   │   │   └── testinfra/
    │   │   │       ├── Directory.Build.props
    │   │   │       └── MUXTestInfra/
    │   │   │           ├── build-nupkg.cmd
    │   │   │           ├── build-nupkg.ps1
    │   │   │           ├── Microsoft.Internal.MUXTestInfra.Native.targets
    │   │   │           ├── Microsoft.Internal.MUXTestInfra.nuspec
    │   │   │           ├── Microsoft.Internal.MUXTestInfra.targets
    │   │   │           ├── MUXTestInfra.csproj
    │   │   │           ├── TestAppInstallHelper.cs
    │   │   │           ├── Common/
    │   │   │           │   ├── AppsTestExtensions.cs
    │   │   │           │   ├── FindElement.cs
    │   │   │           │   ├── FocusHelper.cs
    │   │   │           │   ├── GamepadHelper.cs
    │   │   │           │   ├── InputHelper.cs
    │   │   │           │   ├── KeyboardHelper.cs
    │   │   │           │   ├── ScrollChangedEventWaiter.cs
    │   │   │           │   ├── ScrollHelper.cs
    │   │   │           │   ├── ScrollPresenterUIObject.cs
    │   │   │           │   ├── TestHelpers.cs
    │   │   │           │   ├── ValueChangedEventWaiter.cs
    │   │   │           │   └── WaitHelper.cs
    │   │   │           ├── CommonManaged/
    │   │   │           │   └── PlatformConfiguration.cs
    │   │   │           └── Infra/
    │   │   │               ├── Application.cs
    │   │   │               ├── TestEnvironment.cs
    │   │   │               └── TestHelpers.cs
    │   │   └── tools/
    │   │       ├── AdalAuth.ps1
    │   │       ├── addaliases.cmd
    │   │       ├── BuildMachineUtils.psm1
    │   │       ├── CreateAppxDirectory.msbuildproj
    │   │       ├── CreateUnreliableTestReport.ps1
    │   │       ├── Directory.Build.props
    │   │       ├── Directory.Build.targets
    │   │       ├── EnableMUXControlsTestAppManagedDebugging.cmd
    │   │       ├── EnableMUXControlsTestAppManagedDebugging.ps1
    │   │       ├── ExtractControls.ps1
    │   │       ├── ExtractPackageDependencies.ps1
    │   │       ├── GenerateAppxDependenciesXML.cmd
    │   │       ├── GenerateAppxDependenciesXML.ps1
    │   │       ├── GenerateMergedXaml.cmd
    │   │       ├── GenerateMergedXaml.ps1
    │   │       ├── GenerateNewControlInProject.cmd
    │   │       ├── GenerateNewControlInProject.ps1
    │   │       ├── GenerateNewControlProject.cmd
    │   │       ├── GenerateNewControlProject.ps1
    │   │       ├── GenerateNewProperty.ps1
    │   │       ├── GenerateSystemDllImageResources.ps1
    │   │       ├── GenerateSystemDllStringResources.ps1
    │   │       ├── GenerateVisualVerificationUpdates.ps1
    │   │       ├── InstallAppFromLayout.ps1
    │   │       ├── InstallTestApp.Desktop.cmd
    │   │       ├── MakeAppxHelper.cmd
    │   │       ├── MergeWinUI2XamlFiles.msbuildproj
    │   │       ├── MergeWinUI2XamlFiles.ps1
    │   │       ├── NugetWrapper.cmd
    │   │       ├── OutputUnreliableTestReport.ps1
    │   │       ├── packages.pkggen.config
    │   │       ├── PerformFullOSBuilds.ps1
    │   │       ├── PortWinUI2ReswFiles.ps1
    │   │       ├── PostBuild.cmd
    │   │       ├── PostBuildWrapper.cmd
    │   │       ├── PostTestsWrapper.cmd
    │   │       ├── PowershellWrapper.cmd
    │   │       ├── ProcessTextTemplate.ps1
    │   │       ├── ps.bat
    │   │       ├── PSProfile.ps1
    │   │       ├── PublishChunk.cmd
    │   │       ├── PublishPostBuild.cmd
    │   │       ├── PublishPostBuildWrapper.cmd
    │   │       ├── RebootBuildMachine.ps1
    │   │       ├── ReleaseHelper.ps1
    │   │       ├── RemoveV1XamlFiles.cmd
    │   │       ├── RemoveV1XamlFiles.ps1
    │   │       ├── sign.cmd
    │   │       ├── UpdateBuildMachineGitInstalls.ps1
    │   │       ├── UpdateBuildMachineSDKs.ps1
    │   │       ├── UpdateBuildMachineVSInstalls.ps1
    │   │       ├── UpdateNamespaces.ps1
    │   │       ├── UpdateThemeResources.ps1
    │   │       ├── UpdateVcxitemsPageReferences.ps1
    │   │       ├── Utils.psm1
    │   │       ├── CustomTasks/
    │   │       │   ├── readme.md
    │   │       │   ├── BatchMergeXaml.cs
    │   │       │   ├── CustomTask.cs
    │   │       │   ├── CustomTasks.csproj
    │   │       │   ├── DependencyPropertyCodeGen.cs
    │   │       │   ├── GenerateWinRTClassRegistrations.cs
    │   │       │   ├── GenerateWinRTClassRegistrationsUnpackaged.cs
    │   │       │   ├── GetAppxManifestExtensionsFromWinMDs.cs
    │   │       │   ├── IsolatedTask.cs
    │   │       │   ├── KillMSBuild.cs
    │   │       │   ├── MergedDictionary.cs
    │   │       │   ├── packages.config
    │   │       │   ├── RunPowershellScript.cs
    │   │       │   ├── StripNamespaces.cs
    │   │       │   ├── TransformTemplate.cs
    │   │       │   ├── Utils.cs
    │   │       │   ├── NuSpecs/
    │   │       │   │   ├── BuildNupkg.cmd
    │   │       │   │   ├── CreateUpdatedNupkg.cmd
    │   │       │   │   ├── IncrementVersionNumber.cmd
    │   │       │   │   ├── IncrementVersionNumber.ps1
    │   │       │   │   ├── license.txt
    │   │       │   │   ├── MUXCustomBuildTasks.nuspec
    │   │       │   │   ├── MUXCustomBuildTasks.targets
    │   │       │   │   ├── PublishNupkg.cmd
    │   │       │   │   ├── UpdateReferences.cmd
    │   │       │   │   └── UpdateReferences.ps1
    │   │       │   └── Properties/
    │   │       │       └── AssemblyInfo.cs
    │   │       ├── CustomTasksTool/
    │   │       │   ├── App.config
    │   │       │   ├── CustomTasksTool.csproj
    │   │       │   ├── packages.config
    │   │       │   ├── Program.cs
    │   │       │   └── Properties/
    │   │       │       └── AssemblyInfo.cs
    │   │       ├── GenerateNewControlProjectFiles/
    │   │       │   ├── NEWCONTROL.cpp
    │   │       │   ├── NEWCONTROL.h
    │   │       │   ├── NEWCONTROL.idl
    │   │       │   ├── NEWCONTROL.vcxitems
    │   │       │   ├── NEWCONTROL.xaml
    │   │       │   ├── NEWCONTROL_themeresources.xaml
    │   │       │   ├── APITests/
    │   │       │   │   ├── NEWCONTROL_APITests.projitems
    │   │       │   │   ├── NEWCONTROL_APITests.shproj
    │   │       │   │   └── NEWCONTROLTests.cs
    │   │       │   ├── InteractionTests/
    │   │       │   │   ├── NEWCONTROL_InteractionTests.projitems
    │   │       │   │   ├── NEWCONTROL_InteractionTests.shproj
    │   │       │   │   └── NEWCONTROLTests.cs
    │   │       │   └── TestUI/
    │   │       │       ├── NEWCONTROL_TestUI.projitems
    │   │       │       ├── NEWCONTROL_TestUI.shproj
    │   │       │       ├── NEWCONTROLPage.xaml
    │   │       │       └── NEWCONTROLPage.xaml.cs
    │   │       └── MUXBaselineResourcesGenerator/
    │   │           ├── readme.md
    │   │           ├── MUXBaselineResourcesGenerator.sln
    │   │           └── MUXBaselineResourcesGenerator/
    │   │               ├── App.xaml
    │   │               ├── App.xaml.cs
    │   │               ├── MainPage.xaml
    │   │               ├── MainPage.xaml.cs
    │   │               ├── MUXBaselineResourcesGenerator.csproj
    │   │               ├── Package.appxmanifest
    │   │               └── Properties/
    │   │                   ├── AssemblyInfo.cs
    │   │                   └── Default.rd.xml
    │   ├── dxaml/
    │   │   ├── atl.props
    │   │   ├── common.props
    │   │   ├── cspell.json
    │   │   ├── experimental-clang.props
    │   │   ├── Microsoft.UI.Xaml.sln
    │   │   ├── use-public-sdk.props
    │   │   ├── Xaml.Cpp.Props
    │   │   ├── Xaml.Cpp.Targets
    │   │   ├── Xaml.NTLegacy.Cpp.props
    │   │   ├── Xaml.NTLegacy.Cpp.targets
    │   │   ├── Xaml.NTLegacy.props
    │   │   └── xcp/
    │   │       ├── common.props
    │   │       ├── hostpalplatmisc.vcxproj
    │   │       ├── project-lift.props
    │   │       ├── projectbase.props
    │   │       ├── runcodegen.cmd
    │   │       ├── components/
    │   │       │   ├── base.props
    │   │       │   ├── common.except.props
    │   │       │   ├── common.props
    │   │       │   ├── includes.props
    │   │       │   ├── unittest-do.props
    │   │       │   ├── unittest-parser.props
    │   │       │   ├── unittest-stubs.props
    │   │       │   ├── unittest-uielement.props
    │   │       │   ├── unittest.props
    │   │       │   ├── unittest_BaseCompstubs.vcxitems
    │   │       │   ├── AccessKeys/
    │   │       │   │   ├── AccessKey/
    │   │       │   │   │   ├── AccessKey.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── AccessKeys.AKAccessKey.vcxproj
    │   │       │   │   ├── Export/
    │   │       │   │   │   ├── AccessKeysEvents.Specializations.h
    │   │       │   │   │   ├── AKExport.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── AccessKeys.AKExport.vcxproj
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AccessKey.h
    │   │       │   │   │   ├── AccessKeysEvents.h
    │   │       │   │   │   ├── AccessKeysOwner.h
    │   │       │   │   │   ├── AccessKeysParser.h
    │   │       │   │   │   ├── AKCommon.h
    │   │       │   │   │   ├── AKExport.h
    │   │       │   │   │   ├── InputInterceptor.h
    │   │       │   │   │   ├── KeyTip.h
    │   │       │   │   │   ├── KeytipAutomaticPlacementAlgorithm.h
    │   │       │   │   │   ├── ModeContainer.h
    │   │       │   │   │   ├── Scope.h
    │   │       │   │   │   ├── ScopeBuilder.h
    │   │       │   │   │   ├── ScopeTree.h
    │   │       │   │   │   ├── TreeAnalyzer.h
    │   │       │   │   │   └── VisualTreeAdapter.h
    │   │       │   │   ├── KeyTips/
    │   │       │   │   │   ├── KeyTip.cpp
    │   │       │   │   │   ├── KeytipAutomaticPlacementAlgorithm.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── AccessKeys.KeyTips.vcxproj
    │   │       │   │   ├── ModeContainer/
    │   │       │   │   │   ├── ModeContainer.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── AccessKeys.AKModeContainer.vcxproj
    │   │       │   │   └── Parser/
    │   │       │   │       ├── AccessKeysParser.cpp
    │   │       │   │       └── lib/
    │   │       │   │           └── AccessKeys.AKParser.vcxproj
    │   │       │   ├── allocation/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── XcpAllocation.h
    │   │       │   │   │   └── XcpAllocationDebug.h
    │   │       │   │   ├── lib/
    │   │       │   │   │   ├── Microsoft.UI.Xaml.Allocation.vcxproj
    │   │       │   │   │   ├── XcpAllocation.cpp
    │   │       │   │   │   ├── XcpAllocationDebug.cpp
    │   │       │   │   │   └── XcpNewDelete.cpp
    │   │       │   │   └── stubs/
    │   │       │   │       ├── Microsoft.UI.Xaml.Allocation.Stubs.vcxproj
    │   │       │   │       └── stubs.cpp
    │   │       │   ├── animation/
    │   │       │   │   ├── Animation.cpp
    │   │       │   │   ├── ColorAnimation.cpp
    │   │       │   │   ├── ColorAnimationUsingKeyFrames.cpp
    │   │       │   │   ├── ColorKeyFrames.cpp
    │   │       │   │   ├── ConnectedAnimation.cpp
    │   │       │   │   ├── ConnectedAnimationService.cpp
    │   │       │   │   ├── DCompAnimationConversionContext.cpp
    │   │       │   │   ├── DCompAnimationConversionContextWUC.cpp
    │   │       │   │   ├── DoubleAnimation.cpp
    │   │       │   │   ├── DoubleAnimationUsingKeyFrames.cpp
    │   │       │   │   ├── DoubleKeyFrames.cpp
    │   │       │   │   ├── EasingFunctions.cpp
    │   │       │   │   ├── KeyFrame.cpp
    │   │       │   │   ├── KeyFrameCollection.cpp
    │   │       │   │   ├── KeySpline.cpp
    │   │       │   │   ├── ParallelTimeline.cpp
    │   │       │   │   ├── PointerKeyFrameCollection.cpp
    │   │       │   │   ├── Storyboard.cpp
    │   │       │   │   ├── Timeline.cpp
    │   │       │   │   ├── TimelineGroup.cpp
    │   │       │   │   ├── TimeManager.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ComputeStateParams.h
    │   │       │   │   │   ├── ConnectedAnimation.h
    │   │       │   │   │   ├── ConnectedAnimationCoreConfiguration.h
    │   │       │   │   │   ├── ConnectedAnimationService.h
    │   │       │   │   │   ├── DCompAnimationConversionContext.h
    │   │       │   │   │   └── IATarget.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Animation.vcxproj
    │   │       │   ├── associative/
    │   │       │   │   └── inc/
    │   │       │   │       ├── AssociativeStorage.h
    │   │       │   │       └── RelaxedAlignmentData.h
    │   │       │   ├── base/
    │   │       │   │   ├── bit_vector.cpp
    │   │       │   │   ├── Clock.cpp
    │   │       │   │   ├── DebugWriter.cpp
    │   │       │   │   ├── DesignMode.cpp
    │   │       │   │   ├── DoubleUtil.cpp
    │   │       │   │   ├── ErrorHandlerSettings.cpp
    │   │       │   │   ├── FloatUtil.cpp
    │   │       │   │   ├── MinMath.cpp
    │   │       │   │   ├── RectUtil.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AssertMacros.h
    │   │       │   │   │   ├── bit_vector.h
    │   │       │   │   │   ├── Clock.h
    │   │       │   │   │   ├── DebugWriter.h
    │   │       │   │   │   ├── DesignMode.h
    │   │       │   │   │   ├── DoubleUtil.h
    │   │       │   │   │   ├── errorcontext.h
    │   │       │   │   │   ├── ErrorContextStructure.h
    │   │       │   │   │   ├── ErrorHandlerSettings.h
    │   │       │   │   │   ├── flags_enum.h
    │   │       │   │   │   ├── FloatUtil.h
    │   │       │   │   │   ├── Handle.h
    │   │       │   │   │   ├── minerror.h
    │   │       │   │   │   ├── MinMath.h
    │   │       │   │   │   ├── NamespaceAliases.h
    │   │       │   │   │   ├── RectUtil.h
    │   │       │   │   │   ├── stack_allocator.h
    │   │       │   │   │   ├── stack_vector.h
    │   │       │   │   │   ├── StaticAssertFalse.h
    │   │       │   │   │   ├── vector_map.h
    │   │       │   │   │   ├── vector_set.h
    │   │       │   │   │   ├── vector_tree.h
    │   │       │   │   │   ├── weakref_count.h
    │   │       │   │   │   ├── weakref_ptr.h
    │   │       │   │   │   ├── wilhelper.h
    │   │       │   │   │   ├── windowscollections.h
    │   │       │   │   │   ├── wrlhelper.h
    │   │       │   │   │   ├── XamlBehaviorMode.h
    │   │       │   │   │   ├── XamlStructCollectionDeclarations.h
    │   │       │   │   │   ├── XamlTelemetry.h
    │   │       │   │   │   ├── XamlTraceLogging.h
    │   │       │   │   │   ├── xhashmap.h
    │   │       │   │   │   ├── xref_ptr.h
    │   │       │   │   │   ├── xtable.h
    │   │       │   │   │   └── abi/
    │   │       │   │   │       └── xaml_abi.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Base.vcxproj
    │   │       │   ├── brushes/
    │   │       │   │   ├── Brush.cpp
    │   │       │   │   ├── BrushTypeUtils.cpp
    │   │       │   │   ├── LinearGradientBrush.cpp
    │   │       │   │   ├── LinearGradientBrushMap.cpp
    │   │       │   │   ├── SolidColorBrush.cpp
    │   │       │   │   ├── WUCBrushManager.cpp
    │   │       │   │   ├── XamlCompositionBrush.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── BrushParams.h
    │   │       │   │   │   ├── BrushTypeUtils.h
    │   │       │   │   │   ├── LinearGradientBrush.h
    │   │       │   │   │   ├── LinearGradientBrushMap.h
    │   │       │   │   │   └── WUCBrushManager.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Brushes.vcxproj
    │   │       │   ├── Collection/
    │   │       │   │   ├── BrushCollection.cpp
    │   │       │   │   ├── collect.cpp
    │   │       │   │   ├── DOCollection.cpp
    │   │       │   │   ├── DoubleCollection.cpp
    │   │       │   │   ├── GridDefinitionCollections.cpp
    │   │       │   │   ├── ItemCollection.cpp
    │   │       │   │   ├── PointCollection.cpp
    │   │       │   │   ├── ResourceDictionaryCollection.cpp
    │   │       │   │   ├── SetterBaseCollection.cpp
    │   │       │   │   ├── StateTriggerCollection.cpp
    │   │       │   │   ├── UIElementCollection.cpp
    │   │       │   │   ├── UIElementWeakCollection.cpp
    │   │       │   │   ├── ValidationErrorsCollection.cpp
    │   │       │   │   ├── VisualStateCollection.cpp
    │   │       │   │   ├── VisualStateGroupCollection.cpp
    │   │       │   │   ├── XamlLightCollection.cpp
    │   │       │   │   ├── Inc/
    │   │       │   │   │   ├── brushcollection.h
    │   │       │   │   │   ├── collectionbase.h
    │   │       │   │   │   ├── definitioncollection.h
    │   │       │   │   │   ├── docollection.h
    │   │       │   │   │   ├── doublecollection.h
    │   │       │   │   │   ├── ICollectionChangeCallback.h
    │   │       │   │   │   ├── pointcollection.h
    │   │       │   │   │   ├── setterbasecollection.h
    │   │       │   │   │   ├── StateTriggerCollection.h
    │   │       │   │   │   ├── uielementcollection.h
    │   │       │   │   │   ├── UIElementWeakCollection.h
    │   │       │   │   │   ├── ValidationErrorsCollection.h
    │   │       │   │   │   ├── VisualStateGroupCollection.h
    │   │       │   │   │   ├── xamlitemcollection.h
    │   │       │   │   │   └── XamlLightCollection.h
    │   │       │   │   └── Lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Collection.vcxproj
    │   │       │   ├── colors/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CColor.h
    │   │       │   │   │   ├── ColorUtil.h
    │   │       │   │   │   ├── GammaLUTs.h
    │   │       │   │   │   ├── KnownColors.h
    │   │       │   │   │   └── pixelformatutils.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── ColorConversions.cpp
    │   │       │   │       ├── GammaLUTs.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.Colors.vcxproj
    │   │       │   │       └── pixelformatutils.cpp
    │   │       │   ├── com/
    │   │       │   │   ├── ComBase.cpp
    │   │       │   │   ├── ComObjectBase.cpp
    │   │       │   │   ├── ComUtils.cpp
    │   │       │   │   ├── WeakReference.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ComBase.h
    │   │       │   │   │   ├── ComEventHandler.h
    │   │       │   │   │   ├── ComEventHandlerTraits.h
    │   │       │   │   │   ├── ComMacros.h
    │   │       │   │   │   ├── ComObject.h
    │   │       │   │   │   ├── ComObjectBase.h
    │   │       │   │   │   ├── ComPtr.h
    │   │       │   │   │   ├── ComTemplates.h
    │   │       │   │   │   ├── ComUtils.h
    │   │       │   │   │   ├── InterfaceForwarder.h
    │   │       │   │   │   └── WeakReferenceImpl.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Com.vcxproj
    │   │       │   ├── common/
    │   │       │   │   └── inc/
    │   │       │   │       └── CommonUtilities.h
    │   │       │   ├── comptree/
    │   │       │   │   ├── CoreWindowIslandAdapter.cpp
    │   │       │   │   ├── DCompPropertyChangedListener.cpp
    │   │       │   │   ├── DCompTreeHost.cpp
    │   │       │   │   ├── HWCompNode.cpp
    │   │       │   │   ├── HWCompNodeWinRT.cpp
    │   │       │   │   ├── HWRedirectedCompTreeNodeWinRT.cpp
    │   │       │   │   ├── HWWindowedPopupCompTreeNodeWinRT.cpp
    │   │       │   │   ├── OfferTracker.cpp
    │   │       │   │   ├── PropertyTransitions.cpp
    │   │       │   │   ├── SharedTransitionAnimations.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CoreWindowIslandAdapter.h
    │   │       │   │   │   ├── DCompPropertyChangedListener.h
    │   │       │   │   │   ├── DCompTreeHost.h
    │   │       │   │   │   ├── HandOffVisualData.h
    │   │       │   │   │   ├── HWCompNodeWinRT.h
    │   │       │   │   │   ├── HWRedirectedCompTreeNodeWinRT.h
    │   │       │   │   │   ├── HWWindowedPopupCompTreeNodeWinRT.h
    │   │       │   │   │   ├── ImplicitAnimations.h
    │   │       │   │   │   ├── OfferTracker.h
    │   │       │   │   │   ├── PropertyTransitions.h
    │   │       │   │   │   └── SharedTransitionAnimations.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.CompTree.vcxproj
    │   │       │   ├── ContentRoot/
    │   │       │   │   ├── ActivationManager.cpp
    │   │       │   │   ├── ContentRoot.cpp
    │   │       │   │   ├── ContentRootCoordinator.cpp
    │   │       │   │   ├── ContentRootEventListener.cpp
    │   │       │   │   ├── ContextMenuProcessor.cpp
    │   │       │   │   ├── DragDropProcessor.cpp
    │   │       │   │   ├── FocusAdapter.cpp
    │   │       │   │   ├── FocusManagerCoreWindowAdapter.cpp
    │   │       │   │   ├── FocusManagerXamlIslandAdapter.cpp
    │   │       │   │   ├── InputDeviceCache.cpp
    │   │       │   │   ├── InputManager.cpp
    │   │       │   │   ├── InputPaneProcessor.cpp
    │   │       │   │   ├── KeyboardInputProcessor.cpp
    │   │       │   │   ├── PointerInputProcessor.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ActivationManager.h
    │   │       │   │   │   ├── ContentRoot.h
    │   │       │   │   │   ├── ContentRootCoordinator.h
    │   │       │   │   │   ├── ContentRootEventListener.h
    │   │       │   │   │   ├── ContextMenuProcessor.h
    │   │       │   │   │   ├── DragDropProcessor.h
    │   │       │   │   │   ├── FocusAdapter.h
    │   │       │   │   │   ├── FocusManagerCoreWindowAdapter.h
    │   │       │   │   │   ├── FocusManagerXamlIslandAdapter.h
    │   │       │   │   │   ├── InputDeviceCache.h
    │   │       │   │   │   ├── InputManager.h
    │   │       │   │   │   ├── InputPaneProcessor.h
    │   │       │   │   │   ├── KeyboardInputProcessor.h
    │   │       │   │   │   ├── PointerInputProcessor.h
    │   │       │   │   │   └── PointerInputTelemetry.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.ContentRoot.vcxproj
    │   │       │   ├── controls/
    │   │       │   │   ├── InputValidation/
    │   │       │   │   │   ├── ValidationCommand.cpp
    │   │       │   │   │   ├── inc/
    │   │       │   │   │   │   └── ValidationCommand.h
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Controls.InputValidation.vcxproj
    │   │       │   │   ├── KeyDownUp/
    │   │       │   │   │   ├── FocusPressState.cpp
    │   │       │   │   │   ├── inc/
    │   │       │   │   │   │   ├── ButtonBaseKeyProcess.h
    │   │       │   │   │   │   ├── FocusPressState.h
    │   │       │   │   │   │   ├── MenuFlyoutKeyPressProcess.h
    │   │       │   │   │   │   ├── SliderKeyProcess.h
    │   │       │   │   │   │   └── ToggleSwitchKeyProcess.h
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Controls.KeyDownUp.vcxproj
    │   │       │   │   └── LightDismissOverlay/
    │   │       │   │       └── inc/
    │   │       │   │           └── LightDismissOverlayHelper.h
    │   │       │   ├── criticalsection/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── CStaticLock.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── CStaticLock.cpp
    │   │       │   │       └── Microsoft.UI.Xaml.CriticalSection.vcxproj
    │   │       │   ├── CValue/
    │   │       │   │   ├── AutomationCValue.cpp
    │   │       │   │   ├── CValue.cpp
    │   │       │   │   ├── CValueConvert.cpp
    │   │       │   │   ├── CValueStores.cpp
    │   │       │   │   ├── CValueTypeInfo.cpp
    │   │       │   │   ├── CValueUtil.cpp
    │   │       │   │   ├── FactoryMethods.cpp
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.CValue.vcxproj
    │   │       │   ├── deferral/
    │   │       │   │   ├── CustomRuntimeDataSerializer.cpp
    │   │       │   │   ├── CustomWriterManager.cpp
    │   │       │   │   ├── CustomWriterRuntimeData.cpp
    │   │       │   │   ├── CustomWriterRuntimeObjectCreator.cpp
    │   │       │   │   ├── DeferredElementCustomRuntimeData.cpp
    │   │       │   │   ├── DeferredElementCustomRuntimeDataSerializer.cpp
    │   │       │   │   ├── DeferredElementCustomWriter.cpp
    │   │       │   │   ├── DeferredElementCustomWriter.h
    │   │       │   │   ├── icustomwriter.h
    │   │       │   │   ├── NameDirectiveCapturingWriter.cpp
    │   │       │   │   ├── NameDirectiveCapturingWriter.h
    │   │       │   │   ├── ResourceDictionaryCustomRuntimeData.cpp
    │   │       │   │   ├── ResourceDictionaryCustomRuntimeDataSerializer.cpp
    │   │       │   │   ├── ResourceDictionaryCustomWriter.cpp
    │   │       │   │   ├── ResourceDictionaryCustomWriter.h
    │   │       │   │   ├── StyleCustomRuntimeData.cpp
    │   │       │   │   ├── StyleCustomRuntimeDataSerializer.cpp
    │   │       │   │   ├── StyleCustomWriter.cpp
    │   │       │   │   ├── StyleCustomWriter.h
    │   │       │   │   ├── VisualStateGroupCollectionCustomRuntimeData.cpp
    │   │       │   │   ├── VisualStateGroupCollectionCustomRuntimeDataSerializer.cpp
    │   │       │   │   ├── VisualStateGroupCollectionCustomWriter.cpp
    │   │       │   │   ├── VisualStateGroupCollectionCustomWriter.h
    │   │       │   │   ├── VisualTransitionTableOptimizedLookup.cpp
    │   │       │   │   ├── VisualTransitionTableOptimizedLookup.h
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CustomRuntimeDataSerializer.h
    │   │       │   │   │   ├── CustomWriterManager.h
    │   │       │   │   │   ├── CustomWriterRuntimeContext.h
    │   │       │   │   │   ├── CustomWriterRuntimeData.h
    │   │       │   │   │   ├── CustomWriterRuntimeDataTypeIndex.h
    │   │       │   │   │   ├── CustomWriterRuntimeObjectCreator.h
    │   │       │   │   │   ├── DeferredElementCustomRuntimeData.h
    │   │       │   │   │   ├── DeferredElementCustomRuntimeDataSerializer.h
    │   │       │   │   │   ├── ICustomWriterActivator.h
    │   │       │   │   │   ├── icustomwritercallbacks.h
    │   │       │   │   │   ├── ICustomWriterRuntimeDataReceiver.h
    │   │       │   │   │   ├── ResourceDictionaryCustomRuntimeData.h
    │   │       │   │   │   ├── ResourceDictionaryCustomRuntimeDataSerializer.h
    │   │       │   │   │   ├── StyleCustomRuntimeData.h
    │   │       │   │   │   ├── StyleCustomRuntimeDataSerializer.h
    │   │       │   │   │   ├── VisualStateGroupCollectionCustomRuntimeData.h
    │   │       │   │   │   └── VisualStateGroupCollectionCustomRuntimeDataSerializer.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Deferral.vcxproj
    │   │       │   ├── dependencyLocator/
    │   │       │   │   ├── DependencyLocator.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── DependencyLocator.h
    │   │       │   │   │   ├── ExternalDependency.h
    │   │       │   │   │   └── PhoneImports.h
    │   │       │   │   ├── lib/
    │   │       │   │   │   └── Microsoft.UI.Xaml.DependencyLocator.vcxproj
    │   │       │   │   └── mockExternalDependency/
    │   │       │   │       ├── MockExternalDependency.cpp
    │   │       │   │       └── MockExternalDependency.h
    │   │       │   ├── DependencyObject/
    │   │       │   │   ├── CMultiParentShareableDependencyObject.cpp
    │   │       │   │   ├── CNoParentShareableDependencyObject.cpp
    │   │       │   │   ├── Collection.cpp
    │   │       │   │   ├── dependencyobject.cpp
    │   │       │   │   ├── DependencyObjectCollection.cpp
    │   │       │   │   ├── DependencyObjectDCompRegistry.cpp
    │   │       │   │   ├── DependencyObjectMin.cpp
    │   │       │   │   ├── DependencyProperty.cpp
    │   │       │   │   ├── ModifiedValue.cpp
    │   │       │   │   ├── PropertySystem.cpp
    │   │       │   │   ├── Theming.cpp
    │   │       │   │   ├── ValueBuffer.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── DependencyObjectDCompRegistry.h
    │   │       │   │   │   └── ValueBuffer.h
    │   │       │   │   ├── lib/
    │   │       │   │   │   └── Microsoft.UI.Xaml.DependencyObject.vcxproj
    │   │       │   │   └── minlib/
    │   │       │   │       └── Microsoft.UI.Xaml.DependencyObjectMin.vcxproj
    │   │       │   ├── DesktopUtility/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── DesktopUtility.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.DesktopUtility.vcxproj
    │   │       │   ├── diagnosticsInterop/
    │   │       │   │   ├── DiagnosticsInterop.cpp
    │   │       │   │   ├── MetadataIterator.cpp
    │   │       │   │   ├── PropertyChainEvaluator.cpp
    │   │       │   │   ├── PropertyChainIterator.cpp
    │   │       │   │   ├── ResourceDependency.cpp
    │   │       │   │   ├── ResourceGraph.cpp
    │   │       │   │   ├── StyleContext.cpp
    │   │       │   │   ├── Unsealer.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── MetadataIterator.h
    │   │       │   │   │   ├── PropertyChainEvaluator.h
    │   │       │   │   │   ├── PropertyChainIterator.h
    │   │       │   │   │   ├── ResourceDependency.h
    │   │       │   │   │   ├── ResourceGraph.h
    │   │       │   │   │   ├── StyleContext.h
    │   │       │   │   │   └── Unsealer.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.DiagnosticsInterop.vcxproj
    │   │       │   ├── elements/
    │   │       │   │   ├── FacadeAnimationHelper.cpp
    │   │       │   │   ├── FacadeReferenceWrapper.cpp
    │   │       │   │   ├── FacadeStorage.cpp
    │   │       │   │   ├── FrameworkElement.cpp
    │   │       │   │   ├── LayoutTransitionElement.cpp
    │   │       │   │   ├── Popup.cpp
    │   │       │   │   ├── PopupRoot.cpp
    │   │       │   │   ├── PropertySetListener.cpp
    │   │       │   │   ├── TransitionTarget.cpp
    │   │       │   │   ├── UIElement.cpp
    │   │       │   │   ├── UIElementHitTesting.cpp
    │   │       │   │   ├── UIElementLayout.cpp
    │   │       │   │   ├── UIElementRenderWalk.cpp
    │   │       │   │   ├── UIElementSimplePropertiesCallbacks.g.cpp
    │   │       │   │   ├── lib/
    │   │       │   │   │   └── Microsoft.UI.Xaml.Elements.vcxproj
    │   │       │   │   └── sharedstubs/
    │   │       │   │       ├── Microsoft.UI.Xaml.Elements.SharedStubs.vcxproj
    │   │       │   │       └── SharedStubs.cpp
    │   │       │   ├── eventArgs/
    │   │       │   │   ├── HasValidationErrorsChangedEventArgs.cpp
    │   │       │   │   ├── ValidationErrorEventArgs.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── HasValidationErrorsChangedEventArgs.h
    │   │       │   │   │   └── ValidationErrorEventArgs.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.EventArgs.vcxproj
    │   │       │   ├── experimental/
    │   │       │   │   ├── experimental.cpp
    │   │       │   │   ├── Microsoft.UI.Xaml.Experimental.vcxproj
    │   │       │   │   └── inc/
    │   │       │   │       └── experimental.h
    │   │       │   ├── ExtMetadataProvider/
    │   │       │   │   ├── XamlLibMetadataProvider.cpp
    │   │       │   │   ├── XamlMember.cpp
    │   │       │   │   ├── XamlMember.h
    │   │       │   │   ├── XamlType.cpp
    │   │       │   │   ├── XamlType.h
    │   │       │   │   ├── XamlTypeInfoProvider.h
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── XamlLibMetadataProvider.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.ExtMetadataProvider.vcxproj
    │   │       │   ├── flyweight/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── FlyweightCoreAdapter.h
    │   │       │   │   │   ├── FlyweightCoreState.h
    │   │       │   │   │   ├── FlyweightFactory.h
    │   │       │   │   │   └── ValueObjectBase.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── DurationVO.cpp
    │   │       │   │       ├── FlyweightCoreAdapter.cpp
    │   │       │   │       ├── KeyTimeVO.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.Flyweight.vcxproj
    │   │       │   │       └── RepeatBehaviorVO.cpp
    │   │       │   ├── focus/
    │   │       │   │   ├── export/
    │   │       │   │   │   ├── Export.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Focus.Export.vcxproj
    │   │       │   │   ├── FocusObserver/
    │   │       │   │   │   ├── ConversionFunctions.cpp
    │   │       │   │   │   ├── CoreWindowFocusObserver.cpp
    │   │       │   │   │   ├── FocusObserver.cpp
    │   │       │   │   │   └── Microsoft.UI.Xaml.Focus.FocusObserver.vcxproj
    │   │       │   │   ├── FocusProperties/
    │   │       │   │   │   ├── DefaultFocusChildrenIterable.cpp
    │   │       │   │   │   ├── DefaultFocusChildrenIterator.cpp
    │   │       │   │   │   ├── FocusChildrenIteratorWrapper.cpp
    │   │       │   │   │   ├── FocusProperties.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Focus.FocusProperties.vcxproj
    │   │       │   │   ├── FocusSelection/
    │   │       │   │   │   ├── FocusSelection.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Focus.FocusSelection.vcxproj
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ConversionFunctions.h
    │   │       │   │   │   ├── CoreWindowFocusObserver.h
    │   │       │   │   │   ├── DefaultFocusChildrenIterable.h
    │   │       │   │   │   ├── DefaultFocusChildrenIterator.h
    │   │       │   │   │   ├── FocusChildrenIteratorWrapper.h
    │   │       │   │   │   ├── FocusLockOverrideGuard.h
    │   │       │   │   │   ├── FocusMovement.h
    │   │       │   │   │   ├── FocusObserver.h
    │   │       │   │   │   ├── FocusProperties.h
    │   │       │   │   │   ├── FocusSelection.h
    │   │       │   │   │   ├── InitialFocusSIPSuspender.h
    │   │       │   │   │   ├── OcclusivityTester.h
    │   │       │   │   │   └── XYFocus.h
    │   │       │   │   ├── Movement/
    │   │       │   │   │   ├── FocusMovement.cpp
    │   │       │   │   │   └── lib/
    │   │       │   │   │       └── Microsoft.UI.Xaml.Focus.FocusMovement.vcxproj
    │   │       │   │   └── XYFocus/
    │   │       │   │       ├── AlgorithmHelper.cpp
    │   │       │   │       ├── Bubbling.cpp
    │   │       │   │       ├── ProximityStrategy.cpp
    │   │       │   │       ├── TreeWalker.cpp
    │   │       │   │       ├── XYFocus.cpp
    │   │       │   │       ├── XYFocusAlgorithms.cpp
    │   │       │   │       ├── inc/
    │   │       │   │       │   ├── AlgorithmHelper.h
    │   │       │   │       │   ├── Bubbling.h
    │   │       │   │       │   ├── Focusability.h
    │   │       │   │       │   ├── ProximityStrategy.h
    │   │       │   │       │   ├── TreeWalker.h
    │   │       │   │       │   └── XYFocusAlgorithms.h
    │   │       │   │       └── lib/
    │   │       │   │           └── Microsoft.UI.Xaml.Focus.XYFocus.vcxproj
    │   │       │   ├── FocusRect/
    │   │       │   │   ├── Focusable.cpp
    │   │       │   │   ├── FocusRectHost.cpp
    │   │       │   │   ├── FocusRectManager.cpp
    │   │       │   │   ├── RevealFocusAnimator.cpp
    │   │       │   │   ├── RevealFocusDefaultValue.cpp
    │   │       │   │   ├── RevealFocusSource.cpp
    │   │       │   │   ├── RevealMotion.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── Focusable.h
    │   │       │   │   │   ├── FocusRectHelper.h
    │   │       │   │   │   ├── FocusRectHost.h
    │   │       │   │   │   ├── FocusRectManager.h
    │   │       │   │   │   ├── FocusRectNudging.h
    │   │       │   │   │   ├── focusrectoptions.h
    │   │       │   │   │   ├── RevealFocusAnimator.h
    │   │       │   │   │   ├── RevealFocusDefaultValue.h
    │   │       │   │   │   ├── RevealFocusSource.h
    │   │       │   │   │   └── RevealMotion.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.FocusRect.vcxproj
    │   │       │   ├── gestures/
    │   │       │   │   ├── export/
    │   │       │   │   │   ├── ElementGestureTracker.cpp
    │   │       │   │   │   ├── GestureRecognizerAdapter.cpp
    │   │       │   │   │   └── Microsoft.UI.Xaml.Gestures.Export.vcxproj
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ElementGestureTracker.h
    │   │       │   │   │   ├── GestureOutputMapper.h
    │   │       │   │   │   └── GestureRecognizerAdapter.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── GestureConfigurationBuilder.cpp
    │   │       │   │       ├── GestureConfigurationBuilder.h
    │   │       │   │       ├── GestureOutputMapper.cpp
    │   │       │   │       └── Microsoft.UI.Xaml.Gestures.vcxproj
    │   │       │   ├── graphics/
    │   │       │   │   ├── AlphaMask.cpp
    │   │       │   │   ├── EffectPolicyHelper.cpp
    │   │       │   │   ├── ExpressionHelper.cpp
    │   │       │   │   ├── HWTexture.cpp
    │   │       │   │   ├── ProjectedShadowManager.cpp
    │   │       │   │   ├── RectangleGeometry.cpp
    │   │       │   │   ├── Scheduler.cpp
    │   │       │   │   ├── SystemBackdrop.cpp
    │   │       │   │   ├── ThemeShadow.cpp
    │   │       │   │   ├── WindowsGraphicsDeviceManager.cpp
    │   │       │   │   ├── XamlLight.cpp
    │   │       │   │   ├── XamlLightTargetIdMap.cpp
    │   │       │   │   ├── XamlLightTargetMap.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AAEdgeFlags.h
    │   │       │   │   │   ├── AlphaMask.h
    │   │       │   │   │   ├── DropShadowRecipe.h
    │   │       │   │   │   ├── EffectPolicyHelper.h
    │   │       │   │   │   ├── ExpressionHelper.h
    │   │       │   │   │   ├── GraphicsTelemetry.h
    │   │       │   │   │   ├── GraphicsUtility.h
    │   │       │   │   │   ├── ProjectedShadowManager.h
    │   │       │   │   │   ├── RectangleGeometry.h
    │   │       │   │   │   ├── Scheduler.h
    │   │       │   │   │   ├── SystemBackdrop.h
    │   │       │   │   │   ├── XamlLight.h
    │   │       │   │   │   ├── XamlLightTargetIdMap.h
    │   │       │   │   │   └── XamlLightTargetMap.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.GraphicsUtility.vcxproj
    │   │       │   ├── imaging/
    │   │       │   │   ├── AsyncCopyToSurfaceTask.cpp
    │   │       │   │   ├── AsyncDecodeResponse.cpp
    │   │       │   │   ├── AsyncImageDecoder.cpp
    │   │       │   │   ├── AsyncImageFactory.cpp
    │   │       │   │   ├── DecodedImageCache.cpp
    │   │       │   │   ├── EncodedImageData.cpp
    │   │       │   │   ├── ImageCache.cpp
    │   │       │   │   ├── ImageCacheDecodeHandlerTask.cpp
    │   │       │   │   ├── ImageCacheDownloadCallbackMarshaller.cpp
    │   │       │   │   ├── ImageCacheDownloadProgressTask.cpp
    │   │       │   │   ├── ImageCacheDownloadResponseTask.cpp
    │   │       │   │   ├── ImageDecodeRequest.cpp
    │   │       │   │   ├── ImageDecoderFactory.cpp
    │   │       │   │   ├── ImageMetadataViewImpl.cpp
    │   │       │   │   ├── ImageMetadataViewImpl.h
    │   │       │   │   ├── ImageProvider.cpp
    │   │       │   │   ├── ImageTaskDispatcher.cpp
    │   │       │   │   ├── ImageViewBase.cpp
    │   │       │   │   ├── ImagingUtility.cpp
    │   │       │   │   ├── OfferableSoftwareBitmap.cpp
    │   │       │   │   ├── PixelFormat.cpp
    │   │       │   │   ├── RenderTargetBitmapImplBase.cpp
    │   │       │   │   ├── RenderTargetBitmapImplUsingSpriteVisuals.cpp
    │   │       │   │   ├── SoftwareBitmapSource.cpp
    │   │       │   │   ├── SoftwareBitmapUtility.cpp
    │   │       │   │   ├── SvgImageDecoder.cpp
    │   │       │   │   ├── SvgImageSource.cpp
    │   │       │   │   ├── TinyRGB.h
    │   │       │   │   ├── WicAnimatedGifDecoder.cpp
    │   │       │   │   ├── WicBitmapLock.cpp
    │   │       │   │   ├── WicService.cpp
    │   │       │   │   ├── WicSingleImageDecoder.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AsyncCopyToSurfaceTask.h
    │   │       │   │   │   ├── AsyncDecodeResponse.h
    │   │       │   │   │   ├── AsyncImageDecoder.h
    │   │       │   │   │   ├── AsyncImageWorkData.h
    │   │       │   │   │   ├── BufferMemoryProxy.h
    │   │       │   │   │   ├── DecodedImageCache.h
    │   │       │   │   │   ├── EncodedImageData.h
    │   │       │   │   │   ├── ImageAsyncCallback.h
    │   │       │   │   │   ├── ImageAvailableCallback.h
    │   │       │   │   │   ├── ImageCache.h
    │   │       │   │   │   ├── ImageCacheDecodeHandlerTask.h
    │   │       │   │   │   ├── ImageCacheDownloadCallbackMarshaller.h
    │   │       │   │   │   ├── ImageCacheDownloadProgressTask.h
    │   │       │   │   │   ├── ImageCacheDownloadResponseTask.h
    │   │       │   │   │   ├── ImageCopyParams.h
    │   │       │   │   │   ├── ImageDecodeParams.h
    │   │       │   │   │   ├── ImageDecodeRequest.h
    │   │       │   │   │   ├── ImageDecoderFactory.h
    │   │       │   │   │   ├── ImageMetadata.h
    │   │       │   │   │   ├── ImageMetadataView.h
    │   │       │   │   │   ├── ImageProviderInterfaces.h
    │   │       │   │   │   ├── ImageTaskDispatcher.h
    │   │       │   │   │   ├── ImageViewBase.h
    │   │       │   │   │   ├── ImageViewListener.h
    │   │       │   │   │   ├── imaginginterfaces.h
    │   │       │   │   │   ├── ImagingTelemetry.h
    │   │       │   │   │   ├── ImagingUtility.h
    │   │       │   │   │   ├── OfferableSoftwareBitmap.h
    │   │       │   │   │   ├── PALMemoryProxy.h
    │   │       │   │   │   ├── PixelFormat.h
    │   │       │   │   │   ├── RawData.h
    │   │       │   │   │   ├── RenderTargetBitmapImplBase.h
    │   │       │   │   │   ├── RenderTargetBitmapImplUsingSpriteVisuals.h
    │   │       │   │   │   ├── RenderTargetBitmapTypes.h
    │   │       │   │   │   ├── SoftwareBitmapSource.h
    │   │       │   │   │   ├── SoftwareBitmapUtility.h
    │   │       │   │   │   ├── SurfaceDecodeParams.h
    │   │       │   │   │   ├── SvgImageDecoder.h
    │   │       │   │   │   ├── SvgImageSource.h
    │   │       │   │   │   ├── SynchronousImageAvailableCallback.h
    │   │       │   │   │   ├── WicAnimatedGifDecoder.h
    │   │       │   │   │   ├── WicBitmapLock.h
    │   │       │   │   │   ├── WicService.h
    │   │       │   │   │   └── WicSingleImageDecoder.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── cgmanifest.json
    │   │       │   │       └── Microsoft.UI.Xaml.Media.Imaging.vcxproj
    │   │       │   ├── input/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── KeyboardAutomationInvoker.h
    │   │       │   │   │   ├── KeyboardUtility.h
    │   │       │   │   │   └── RemapVirtualKey.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── KeyboardUtility.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.Input.vcxproj
    │   │       │   │       └── RemapVirtualKey.cpp
    │   │       │   ├── inputpane/
    │   │       │   │   ├── FrameworkInputPaneOneCore.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── FrameworkInputPaneOneCore.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.InputPane.vcxproj
    │   │       │   ├── ItemIndexRangeHelper/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── ItemIndexRangeHelper.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── ItemIndexRangeHelper.cpp
    │   │       │   │       └── Microsoft.UI.Xaml.ItemIndexRangeHelper.vcxproj
    │   │       │   ├── KeyboardAccelerator/
    │   │       │   │   ├── KeyboardAcceleratorUtility.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── KeyboardAcceleratorUtility.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.KeyboardAcceleratorUtility.vcxproj
    │   │       │   ├── legacy/
    │   │       │   │   ├── README.md
    │   │       │   │   ├── ImageCacheIdentifier.cpp
    │   │       │   │   ├── WinReader.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ImageCacheIdentifier.h
    │   │       │   │   │   ├── ReaderString.h
    │   │       │   │   │   ├── WinReader.h
    │   │       │   │   │   └── xvector.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Legacy.vcxproj
    │   │       │   ├── lifetime/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AutoPeg.h
    │   │       │   │   │   ├── AutoReentrantReferenceLock.h
    │   │       │   │   │   ├── ComposingTrackerExtensionWrapper.h
    │   │       │   │   │   ├── ComposingTrackerTargetWrapper.h
    │   │       │   │   │   ├── ComposingTrackerWrapper.h
    │   │       │   │   │   ├── DependencyObjectAbstractionHelpers.h
    │   │       │   │   │   ├── LifetimeExterns.h
    │   │       │   │   │   ├── LifetimeUtils.h
    │   │       │   │   │   ├── ReferenceTrackerExtension.h
    │   │       │   │   │   ├── ReferenceTrackerInterfaces.h
    │   │       │   │   │   ├── ReferenceTrackerLogging.h
    │   │       │   │   │   ├── ReferenceTrackerManager.h
    │   │       │   │   │   ├── TrackerPtr.h
    │   │       │   │   │   ├── TrackerPtrWrapper.h
    │   │       │   │   │   ├── TrackerTargetReference.h
    │   │       │   │   │   ├── WeakReferenceSource.h
    │   │       │   │   │   └── WeakReferenceSourceNoThreadId.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── ComposingTrackerExtensionWrapper.cpp
    │   │       │   │       ├── ComposingTrackerTargetWrapper.cpp
    │   │       │   │       ├── LifetimeUtils.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.Lifetime.vcxproj
    │   │       │   │       ├── ReferenceTrackerLogging.cpp
    │   │       │   │       ├── ReferenceTrackerManager.cpp
    │   │       │   │       ├── TrackerTargetReference.cpp
    │   │       │   │       ├── WeakReferenceSource.cpp
    │   │       │   │       └── WeakReferenceSourceNoThreadId.cpp
    │   │       │   ├── livereorderhelper/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── LiveReorderHelper.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── LiveReorderHelper.cpp
    │   │       │   │       └── Microsoft.UI.Xaml.LiveReorderHelper.vcxproj
    │   │       │   ├── math/
    │   │       │   │   ├── cmatrix.cpp
    │   │       │   │   ├── HitTestPolygon.cpp
    │   │       │   │   ├── inlined.cpp
    │   │       │   │   ├── math.cpp
    │   │       │   │   ├── MILMatrix.cpp
    │   │       │   │   ├── MILMatrix4x4.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── cmatrix.h
    │   │       │   │   │   └── HitTestPolygon.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Math.vcxproj
    │   │       │   ├── metadata/
    │   │       │   │   ├── MetadataAPI.cpp
    │   │       │   │   ├── StaticMetadata.g.cpp
    │   │       │   │   ├── TypeNameHelper.cpp
    │   │       │   │   ├── DynamicMetadataStorage/
    │   │       │   │   │   ├── DynamicMetadataStorage.cpp
    │   │       │   │   │   └── Microsoft.UI.Xaml.DynamicMetadataStorage.vcxproj
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── DependencyObjectTraits.g.h
    │   │       │   │   │   ├── DependencyObjectTraits.h
    │   │       │   │   │   ├── EnumDefs.g.h
    │   │       │   │   │   ├── EnumDefs.h
    │   │       │   │   │   ├── EnumValueTable.g.h
    │   │       │   │   │   ├── Indexes.g.h
    │   │       │   │   │   ├── TypeCheckData.g.h
    │   │       │   │   │   ├── TypeNameHelper.h
    │   │       │   │   │   ├── TypeNamePtr.h
    │   │       │   │   │   ├── TypeTableStructs.h
    │   │       │   │   │   └── TypeTableStructsPrivate.h
    │   │       │   │   ├── lib/
    │   │       │   │   │   └── Microsoft.UI.Xaml.Metadata.vcxproj
    │   │       │   │   └── mocks/
    │   │       │   │       ├── Microsoft.UI.Xaml.Tests.Isolated.Mocks.Framework.Metadata.vcxproj
    │   │       │   │       ├── MockClassInfo.cpp
    │   │       │   │       ├── MockClassInfo.h
    │   │       │   │       ├── MockDependencyProperty.cpp
    │   │       │   │       ├── MockDependencyProperty.h
    │   │       │   │       ├── MockDynamicMetadataStorage.cpp
    │   │       │   │       ├── MockDynamicMetadataStorage.h
    │   │       │   │       ├── MockXamlMetadataProvider.h
    │   │       │   │       └── MockXamlType.h
    │   │       │   ├── moco/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CalendarLayoutStrategyImpl.h
    │   │       │   │   │   ├── LayoutStrategyBase.h
    │   │       │   │   │   ├── NavigationIndices.h
    │   │       │   │   │   ├── StackingLayoutStrategyImpl.h
    │   │       │   │   │   └── WrappingLayoutStrategyImpl.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── CalendarLayoutStrategyImpl.cpp
    │   │       │   │       ├── LayoutStrategyBase.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.Components.Moco.vcxproj
    │   │       │   │       ├── StackingLayoutStrategyImpl.cpp
    │   │       │   │       └── WrappingLayoutStrategyImpl.cpp
    │   │       │   ├── mrt/
    │   │       │   │   ├── FileMappedMemory.cpp
    │   │       │   │   ├── FilePathResource.cpp
    │   │       │   │   ├── ModernResourceProvider.cpp
    │   │       │   │   ├── MRTResource.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── FileMappedMemory.h
    │   │       │   │   │   ├── FilePathResource.h
    │   │       │   │   │   ├── ModernResourceProvider.h
    │   │       │   │   │   ├── MRTKnownQualifierNames.h
    │   │       │   │   │   └── MRTResource.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Mrt.vcxproj
    │   │       │   ├── namescope/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── INameScopeDeferredElementCreator.h
    │   │       │   │   │   ├── NameScopeRoot.h
    │   │       │   │   │   └── NameScopeTable.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.NameScope.vcxproj
    │   │       │   │       ├── NameScopeRoot.cpp
    │   │       │   │       ├── NameScopeTable.cpp
    │   │       │   │       ├── NameScopeTableEntry.cpp
    │   │       │   │       ├── NameScopeTableEntry.h
    │   │       │   │       ├── StandardNameScopeTable.cpp
    │   │       │   │       ├── StandardNameScopeTable.h
    │   │       │   │       ├── TemplateNameScopeTable.cpp
    │   │       │   │       └── TemplateNameScopeTable.h
    │   │       │   ├── objectWriter/
    │   │       │   │   └── inc/
    │   │       │   │       ├── StreamOffsetToken.h
    │   │       │   │       └── SubObjectWriterResult.h
    │   │       │   ├── offerableheap/
    │   │       │   │   ├── OfferableMemory.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── OfferableMemory.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.OfferableHeap.vcxproj
    │   │       │   ├── OneCoreTransforms/
    │   │       │   │   ├── XamlOneCoreTransforms.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── XamlOneCoreTransforms.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.OneCoreTransforms.vcxproj
    │   │       │   ├── parser/
    │   │       │   │   └── inc/
    │   │       │   │       ├── ParserAPI.h
    │   │       │   │       ├── XamlPredicateHelpers.h
    │   │       │   │       ├── XamlPredicateService.h
    │   │       │   │       └── XbfVersioning.h
    │   │       │   ├── pch/
    │   │       │   │   ├── precomp.h
    │   │       │   │   ├── prod/
    │   │       │   │   │   └── Microsoft.UI.Xaml.Precomp.vcxproj
    │   │       │   │   ├── prodexcept/
    │   │       │   │   │   └── Microsoft.UI.Xaml.Precomp.vcxproj
    │   │       │   │   ├── ut/
    │   │       │   │   │   └── Microsoft.UI.Xaml.Precomp.vcxproj
    │   │       │   │   └── ut-nohybrid/
    │   │       │   │       └── Microsoft.UI.Xaml.Precomp.vcxproj
    │   │       │   ├── perf_guard/
    │   │       │   │   ├── Microsoft.UI.Xaml.PerfGuard.vcxproj
    │   │       │   │   ├── type_layout.cpp
    │   │       │   │   └── type_layout.h
    │   │       │   ├── pivot/
    │   │       │   │   ├── PivotCurveGenerator.cpp
    │   │       │   │   ├── PivotStateMachine.cpp
    │   │       │   │   ├── PivotStaticContentCurve.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── PivotCommon.h
    │   │       │   │   │   ├── PivotCurveGenerator.h
    │   │       │   │   │   ├── PivotStateMachine.h
    │   │       │   │   │   └── PivotStaticContentCurve.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Pivot.vcxproj
    │   │       │   ├── primitiveDependencyObjects/
    │   │       │   │   ├── CColor.cpp
    │   │       │   │   ├── CornerRadius.cpp
    │   │       │   │   ├── CString.cpp
    │   │       │   │   ├── Double.cpp
    │   │       │   │   ├── GridLength.cpp
    │   │       │   │   ├── Point.cpp
    │   │       │   │   ├── primitives.cpp
    │   │       │   │   ├── PropertyPath.cpp
    │   │       │   │   ├── Rect.cpp
    │   │       │   │   ├── Size.cpp
    │   │       │   │   ├── TextRange.cpp
    │   │       │   │   ├── Thickness.cpp
    │   │       │   │   ├── Type.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CornerRadius.h
    │   │       │   │   │   ├── CPropertyPath.h
    │   │       │   │   │   ├── CString.h
    │   │       │   │   │   ├── Double.h
    │   │       │   │   │   ├── Point.h
    │   │       │   │   │   ├── primitives.h
    │   │       │   │   │   ├── Rect.h
    │   │       │   │   │   ├── Size.h
    │   │       │   │   │   ├── TextRange.h
    │   │       │   │   │   └── Thickness.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.PrimitiveDependencyObjects.vcxproj
    │   │       │   ├── qualifiers/
    │   │       │   │   ├── ExtensibleQualifier.cpp
    │   │       │   │   ├── MinHeightQualifier.cpp
    │   │       │   │   ├── MinWidthQualifier.cpp
    │   │       │   │   ├── MultiQualifier.cpp
    │   │       │   │   ├── QualifierContext.cpp
    │   │       │   │   ├── QualifierFactory.cpp
    │   │       │   │   ├── VariantMap.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ExtensibleQualifier.h
    │   │       │   │   │   ├── IQualifier.h
    │   │       │   │   │   ├── IQualifierContextCallback.h
    │   │       │   │   │   ├── IVariantMapChangedCallback.h
    │   │       │   │   │   ├── MinHeightQualifier.h
    │   │       │   │   │   ├── MinWidthQualifier.h
    │   │       │   │   │   ├── MultiQualifier.h
    │   │       │   │   │   ├── QualifierContext.h
    │   │       │   │   │   ├── QualifierFactory.h
    │   │       │   │   │   ├── QualifierFlags.h
    │   │       │   │   │   └── VariantMap.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Qualifiers.vcxproj
    │   │       │   ├── relativepanel/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── RPGraph.h
    │   │       │   │   │   └── RPNode.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.RelativePanel.vcxproj
    │   │       │   │       ├── RPGraph.cpp
    │   │       │   │       └── RPNode.cpp
    │   │       │   ├── resources/
    │   │       │   │   ├── ct_hash.h
    │   │       │   │   ├── OverrideInfo.cpp
    │   │       │   │   ├── ResourceDictionary.cpp
    │   │       │   │   ├── ResourceDictionary2.cpp
    │   │       │   │   ├── ResourceLookupLogger.cpp
    │   │       │   │   ├── ResourceResolver.cpp
    │   │       │   │   ├── ScopedResources.cpp
    │   │       │   │   ├── ScopedResources_Cloning.cpp
    │   │       │   │   ├── ScopedResources_Cloning.h
    │   │       │   │   ├── ScopedResources_Types.h
    │   │       │   │   ├── ScopedResources_Util.cpp
    │   │       │   │   ├── ScopedResources_Util.h
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── OverrideInfo.h
    │   │       │   │   │   ├── ResourceDictionary2.h
    │   │       │   │   │   ├── ResourceDictionaryKey.h
    │   │       │   │   │   ├── ResourceLookupLogger.h
    │   │       │   │   │   ├── ResourceResolver.h
    │   │       │   │   │   └── ScopedResources.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.XamlResources.vcxproj
    │   │       │   ├── runtimeEnabledFeatures/
    │   │       │   │   ├── RuntimeEnabledFeatures.cpp
    │   │       │   │   ├── RuntimeFeatureData.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── RuntimeEnabledFeatures.h
    │   │       │   │   │   └── RuntimeEnabledFeaturesEnum.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.RuntimeEnabledFeatures.vcxproj
    │   │       │   ├── SatelliteBase/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── BindableToObservableVectorWrapper.h
    │   │       │   │   │   ├── ComTemplateLibrary.h
    │   │       │   │   │   ├── DllInitializedHelpers.h
    │   │       │   │   │   ├── LocalizationHelpers.h
    │   │       │   │   │   ├── ReferenceTrackerRuntimeClass.h
    │   │       │   │   │   ├── SatMacros.h
    │   │       │   │   │   ├── TrackerPtrFamily.h
    │   │       │   │   │   ├── ValueBoxer.h
    │   │       │   │   │   ├── XamlExtTraceLogging.h
    │   │       │   │   │   ├── XamlTypeInfo.h
    │   │       │   │   │   └── XamlWrlHelpers.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── BindableToObservableVectorWrapper.cpp
    │   │       │   │       ├── DllInitializedHelpers.cpp
    │   │       │   │       ├── lock.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.SatelliteBase.vcxproj
    │   │       │   │       └── XamlWrlHelpers.cpp
    │   │       │   ├── scaling/
    │   │       │   │   ├── CoreWindowRootScale.cpp
    │   │       │   │   ├── Microsoft.UI.Xaml.Scaling.vcxproj
    │   │       │   │   ├── RootScale.cpp
    │   │       │   │   ├── Transforms.cpp
    │   │       │   │   ├── XamlIslandRootScale.cpp
    │   │       │   │   └── inc/
    │   │       │   │       ├── CoreWindowRootScale.h
    │   │       │   │       ├── RootScale.h
    │   │       │   │       └── XamlIslandRootScale.h
    │   │       │   ├── simple/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── Operators.h
    │   │       │   │   │   ├── SimpleProperties.h
    │   │       │   │   │   ├── SimplePropertiesHelpers.h
    │   │       │   │   │   ├── SimplePropertiesMetadata.g.h
    │   │       │   │   │   ├── SimpleProperty.h
    │   │       │   │   │   └── SimplePropertyImpl.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.Framework.SimpleProperties.vcxproj
    │   │       │   │       ├── SimplePropertiesAdapter.cpp
    │   │       │   │       ├── SimplePropertiesAdapter.g.h
    │   │       │   │       └── SimplePropertiesHelpers.g.cpp
    │   │       │   ├── staticpal/
    │   │       │   │   ├── Threading.cpp
    │   │       │   │   ├── XamlBehaviorMode.cpp
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.StaticPal.vcxproj
    │   │       │   ├── style/
    │   │       │   │   ├── OptimizedStyle.cpp
    │   │       │   │   ├── Style.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── OptimizedStyle.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Style.vcxproj
    │   │       │   ├── Switcher/
    │   │       │   │   └── inc/
    │   │       │   │       └── Switcher.h
    │   │       │   ├── Telemetry/
    │   │       │   │   ├── GCInstrumentationAggregator.cpp
    │   │       │   │   ├── HighContrastTracingHelper.cpp
    │   │       │   │   ├── MediaTransportControlAggregationTelemetry.cpp
    │   │       │   │   ├── Microsoft.UI.Xaml.Instrumentation.vcxproj
    │   │       │   │   ├── RuntimeProfiler.cpp
    │   │       │   │   ├── XamlTraceSession.cpp
    │   │       │   │   └── inc/
    │   │       │   │       ├── GCInstrumentationAggregator.h
    │   │       │   │       ├── HighContrastTracingHelper.h
    │   │       │   │       ├── MediaTransportControlAggregationTelemetry.h
    │   │       │   │       ├── RuntimeProfiler.h
    │   │       │   │       ├── RuntimeProfiler_DynamicProfiler.h
    │   │       │   │       └── XamlTraceSession.h
    │   │       │   ├── terminateProcessOnOOM/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── XAMLTerminateProcessOnOOM.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.TerminateProcessOnOOM.vcxproj
    │   │       │   │       └── XAMLTerminateProcessOnOOM.cpp
    │   │       │   ├── text/
    │   │       │   │   ├── FocusableHelper.cpp
    │   │       │   │   ├── TextBlockViewHelpers.cpp
    │   │       │   │   ├── TextHighlighter.cpp
    │   │       │   │   ├── TextHighlighterCollection.cpp
    │   │       │   │   ├── TextHighlightMerge.cpp
    │   │       │   │   ├── TextHighlightRenderer.cpp
    │   │       │   │   ├── TextRangeCollection.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── FocusableHelper.h
    │   │       │   │   │   ├── HighlightRegion.h
    │   │       │   │   │   ├── IFocusable.h
    │   │       │   │   │   ├── TextBlockViewHelpers.h
    │   │       │   │   │   ├── TextCommon.h
    │   │       │   │   │   ├── TextHighlighter.h
    │   │       │   │   │   ├── TextHighlighterCollection.h
    │   │       │   │   │   ├── TextHighlightMerge.h
    │   │       │   │   │   ├── TextHighlightRenderer.h
    │   │       │   │   │   └── TextRangeCollection.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Text.vcxproj
    │   │       │   ├── themeanimationshelper/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── ThemeAnimationsHelper.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.ThemeAnimationsHelper.vcxproj
    │   │       │   │       └── ThemeAnimationsHelper.cpp
    │   │       │   ├── theming/
    │   │       │   │   ├── FrameworkTheming.cpp
    │   │       │   │   ├── ThemeResource.cpp
    │   │       │   │   ├── ThemeWalkResourceCache.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── FrameworkTheming.h
    │   │       │   │   │   ├── Theme.h
    │   │       │   │   │   ├── ThemeResource.h
    │   │       │   │   │   └── ThemeWalkResourceCache.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Theming.vcxproj
    │   │       │   ├── theminginterop/
    │   │       │   │   ├── SystemThemingInterop.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── SystemThemingInterop.h
    │   │       │   │   │   └── ThemingInterop.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.ThemingInterop.vcxproj
    │   │       │   ├── threading/
    │   │       │   │   ├── ThreadedJobQueue.cpp
    │   │       │   │   ├── ThreadPoolService.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── ThreadedJobQueue.h
    │   │       │   │   │   └── ThreadPoolService.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Threading.vcxproj
    │   │       │   ├── transforms/
    │   │       │   │   ├── CompositeTransform.cpp
    │   │       │   │   ├── CompositeTransform3D.cpp
    │   │       │   │   ├── HitTestParams.cpp
    │   │       │   │   ├── Matrix3DProjection.cpp
    │   │       │   │   ├── MatrixTransform.cpp
    │   │       │   │   ├── PerspectiveTransform3D.cpp
    │   │       │   │   ├── PlaneProjection.cpp
    │   │       │   │   ├── Projection.cpp
    │   │       │   │   ├── RotateTransform.cpp
    │   │       │   │   ├── ScaleTransform.cpp
    │   │       │   │   ├── SkewTransform.cpp
    │   │       │   │   ├── Transform.cpp
    │   │       │   │   ├── Transform3D.cpp
    │   │       │   │   ├── TransformCollection.cpp
    │   │       │   │   ├── TransformGroup.cpp
    │   │       │   │   ├── TranslateTransform.cpp
    │   │       │   │   ├── WinRTExpressionConversionContext.cpp
    │   │       │   │   ├── WinRTLocalExpressionBuilder.cpp
    │   │       │   │   ├── XamlLocalTransformBuilder.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CompositeTransform3D.h
    │   │       │   │   │   ├── HitTestParams.h
    │   │       │   │   │   ├── LocalTransformBuilder.h
    │   │       │   │   │   ├── PerspectiveTransform3D.h
    │   │       │   │   │   ├── Transform3D.h
    │   │       │   │   │   ├── WinRTExpressionConversionContext.h
    │   │       │   │   │   ├── WinRTLocalExpressionBuilder.h
    │   │       │   │   │   ├── WinRTLocalExpressionCache.h
    │   │       │   │   │   └── XamlLocalTransformBuilder.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.Transforms.vcxproj
    │   │       │   ├── UIBridgeFocus/
    │   │       │   │   ├── FocusController.cpp
    │   │       │   │   ├── Microsoft.UI.Xaml.UIBridgeFocus.vcxproj
    │   │       │   │   ├── NavigateFocusResult.cpp
    │   │       │   │   ├── NavigationFocusEventArgs.cpp
    │   │       │   │   └── inc/
    │   │       │   │       ├── FocusController.h
    │   │       │   │       ├── IFocusController.h
    │   │       │   │       ├── INavigationFocusEventArgs2.h
    │   │       │   │       ├── NavigateFocusResult.h
    │   │       │   │       └── NavigationFocusEventArgs.h
    │   │       │   ├── valueboxer/
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── BoxerBuffer.h
    │   │       │   │   │   ├── CValueBoxer.h
    │   │       │   │   │   ├── IValueBoxer.h
    │   │       │   │   │   ├── Value.h
    │   │       │   │   │   └── ValueBoxer.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── CValueBoxer.cpp
    │   │       │   │       ├── IValueBoxer.cpp
    │   │       │   │       ├── Microsoft.UI.Xaml.ValueBoxer.vcxproj
    │   │       │   │       └── Value.cpp
    │   │       │   ├── visualstateshelper/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── VisualStatesHelper.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── Microsoft.UI.Xaml.VisualStatesHelper.vcxproj
    │   │       │   │       └── VisualStatesHelper.cpp
    │   │       │   ├── vsm/
    │   │       │   │   ├── CVisualStateManager2.cpp
    │   │       │   │   ├── DeferredNameScopeEntry.cpp
    │   │       │   │   ├── DynamicTimelineHelper.cpp
    │   │       │   │   ├── DynamicTransitionStoryboardGenerator.cpp
    │   │       │   │   ├── OptimizedVisualStateManagerDataSource.cpp
    │   │       │   │   ├── OptimizedVisualStateManagerDataSource.h
    │   │       │   │   ├── StandardVisualStateManagerDataSource.cpp
    │   │       │   │   ├── StandardVisualStateManagerDataSource.h
    │   │       │   │   ├── TimelineLookupList.h
    │   │       │   │   ├── VisualState.cpp
    │   │       │   │   ├── VisualStateGroupContext.cpp
    │   │       │   │   ├── VisualStateManagerActuator.cpp
    │   │       │   │   ├── VisualStateManagerActuator.h
    │   │       │   │   ├── VisualStateManagerDataSource.cpp
    │   │       │   │   ├── VisualStateSetterHelper.cpp
    │   │       │   │   ├── VisualStateToken.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── CVisualStateManager2.h
    │   │       │   │   │   ├── DeferredNameScopeEntry.h
    │   │       │   │   │   ├── DynamicTimelineHelper.h
    │   │       │   │   │   ├── DynamicTransitionStoryboardGenerator.h
    │   │       │   │   │   ├── VisualState.h
    │   │       │   │   │   ├── VisualStateGroupContext.h
    │   │       │   │   │   ├── VisualStateManagerDataSource.h
    │   │       │   │   │   ├── VisualStateSetterHelper.h
    │   │       │   │   │   └── VisualStateToken.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.VisualStateMachine.vcxproj
    │   │       │   ├── WindowChrome/
    │   │       │   │   ├── CWindowChrome.cpp
    │   │       │   │   ├── Microsoft.UI.Xaml.WindowChrome.vcxproj
    │   │       │   │   ├── WindowHelpers.cpp
    │   │       │   │   └── inc/
    │   │       │   │       ├── BaseWindow.h
    │   │       │   │       ├── CWindowChrome.h
    │   │       │   │       └── WindowHelpers.h
    │   │       │   ├── winuri/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── winuri.h
    │   │       │   │   └── lib/
    │   │       │   │       ├── WinURI.cpp
    │   │       │   │       └── winuri.vcxproj
    │   │       │   ├── xamlDiagnostics/
    │   │       │   │   ├── BitmapData.cpp
    │   │       │   │   ├── ElementStateChangedBuilder.cpp
    │   │       │   │   ├── HandleMap.cpp
    │   │       │   │   ├── HandleStore.cpp
    │   │       │   │   ├── HandleStore.h
    │   │       │   │   ├── helpers.cpp
    │   │       │   │   ├── LiveVisualTree.cpp
    │   │       │   │   ├── ResourceOperations.cpp
    │   │       │   │   ├── Resources.cpp
    │   │       │   │   ├── RuntimeApplication.cpp
    │   │       │   │   ├── RuntimeCollection.cpp
    │   │       │   │   ├── RuntimeDictionary.cpp
    │   │       │   │   ├── RuntimeDictionaryKey.cpp
    │   │       │   │   ├── RuntimeDictionaryValue.cpp
    │   │       │   │   ├── RuntimeElement.cpp
    │   │       │   │   ├── RuntimeObject.cpp
    │   │       │   │   ├── RuntimeObjectCache.cpp
    │   │       │   │   ├── RuntimeProperty.cpp
    │   │       │   │   ├── RuntimeShareableObject.cpp
    │   │       │   │   ├── XamlDiagnostics.cpp
    │   │       │   │   ├── XamlDiagnosticsTestHooks.cpp
    │   │       │   │   ├── idl/
    │   │       │   │   │   ├── xamlom.vcxproj
    │   │       │   │   │   ├── XamlOM.WinUI.idl
    │   │       │   │   │   └── XamlOM.WinUI.Private.idl
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── BitmapData.h
    │   │       │   │   │   ├── defines.h
    │   │       │   │   │   ├── ElementStateChangedBuilder.h
    │   │       │   │   │   ├── HandleMap.h
    │   │       │   │   │   ├── helpers.h
    │   │       │   │   │   ├── helpersImpl.h
    │   │       │   │   │   ├── includes.h
    │   │       │   │   │   ├── ResourceOperations.h
    │   │       │   │   │   ├── RuntimeApplication.h
    │   │       │   │   │   ├── RuntimeCollection.h
    │   │       │   │   │   ├── RuntimeDictionary.h
    │   │       │   │   │   ├── RuntimeDictionaryKey.h
    │   │       │   │   │   ├── RuntimeDictionaryValue.h
    │   │       │   │   │   ├── RuntimeElement.h
    │   │       │   │   │   ├── RuntimeObject.h
    │   │       │   │   │   ├── RuntimeObjectCache.h
    │   │       │   │   │   ├── RuntimeProperty.h
    │   │       │   │   │   ├── RuntimeShareableObject.h
    │   │       │   │   │   └── XamlDiagnostics.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.XamlDiagnostics.vcxproj
    │   │       │   ├── XboxUtility/
    │   │       │   │   ├── inc/
    │   │       │   │   │   └── XboxUtility.h
    │   │       │   │   └── lib/
    │   │       │   │       └── Microsoft.UI.Xaml.XboxUtility.vcxproj
    │   │       │   └── xstring/
    │   │       │       ├── StringConversions.cpp
    │   │       │       ├── trimwhitespace.cpp
    │   │       │       ├── xstring_ptr.cpp
    │   │       │       ├── xstring_ptr_view.cpp
    │   │       │       ├── XStringBuilder.cpp
    │   │       │       ├── XStringUtils.cpp
    │   │       │       ├── xstrutil.cpp
    │   │       │       ├── inc/
    │   │       │       │   ├── HStringUtil.h
    │   │       │       │   ├── StringConversions.h
    │   │       │       │   ├── trimwhitespace.h
    │   │       │       │   ├── xstring_ptr.h
    │   │       │       │   ├── XStringBuilder.h
    │   │       │       │   ├── XStringUtils.h
    │   │       │       │   └── xstrutil.h
    │   │       │       └── lib/
    │   │       │           └── Microsoft.UI.Xaml.XString.vcxproj
    │   │       ├── control/
    │   │       │   ├── common/
    │   │       │   │   └── shared/
    │   │       │   │       ├── AbortableAsyncDownload.cpp
    │   │       │   │       ├── AsyncDownloadRequestManager.cpp
    │   │       │   │       ├── CommonBrowserHost.h
    │   │       │   │       ├── CommonBrowserHost.hpp
    │   │       │   │       ├── ControlBase.cpp
    │   │       │   │       ├── ControlBase.h
    │   │       │   │       ├── DownloadRequest.cpp
    │   │       │   │       ├── FrameCounter.cpp
    │   │       │   │       ├── FrameCounter.h
    │   │       │   │       ├── precomp.h
    │   │       │   │       ├── ResourceManager.cpp
    │   │       │   │       ├── ResourceManager.h
    │   │       │   │       ├── sources.props
    │   │       │   │       └── sl/
    │   │       │   │           ├── controlBase.vcxproj
    │   │       │   │           └── sources.g.props
    │   │       │   ├── download/
    │   │       │   │   ├── download.cpp
    │   │       │   │   ├── download.vcxproj
    │   │       │   │   └── precomp.hpp
    │   │       │   └── inc/
    │   │       │       ├── AbortableAsyncDownload.h
    │   │       │       ├── AsyncDownloadRequestManager.h
    │   │       │       ├── download.h
    │   │       │       ├── DownloadRequest.h
    │   │       │       ├── hal.h
    │   │       │       └── host.h
    │   │       ├── core/
    │   │       │   ├── common.props
    │   │       │   ├── dirs.proj
    │   │       │   ├── precomp.h
    │   │       │   ├── xcpcore.vcxproj
    │   │       │   ├── animation/
    │   │       │   │   ├── animation.cpp
    │   │       │   │   ├── ColorAnimation.cpp
    │   │       │   │   ├── ColorKeyFrame.cpp
    │   │       │   │   ├── DeferredAnimationOperation.cpp
    │   │       │   │   ├── DoubleAnimation.cpp
    │   │       │   │   ├── DoubleKeyFrame.cpp
    │   │       │   │   ├── Duration.cpp
    │   │       │   │   ├── DynamicTimeline.cpp
    │   │       │   │   ├── KeyFrame.cpp
    │   │       │   │   ├── KeyFrameCollection.cpp
    │   │       │   │   ├── KeySpline.cpp
    │   │       │   │   ├── KeyTime.cpp
    │   │       │   │   ├── ObjectAnimationUsingKeyFrames.cpp
    │   │       │   │   ├── ObjectKeyFrame.cpp
    │   │       │   │   ├── ParallelTimeline.cpp
    │   │       │   │   ├── PointAnimation.cpp
    │   │       │   │   ├── PointerAnimationUsingKeyFrames.cpp
    │   │       │   │   ├── PointerKeyFrame.cpp
    │   │       │   │   ├── PointKeyFrame.cpp
    │   │       │   │   ├── RepeatBehavior.cpp
    │   │       │   │   ├── storyboard.cpp
    │   │       │   │   ├── Timeline.cpp
    │   │       │   │   ├── TimelineCollection.cpp
    │   │       │   │   ├── TimelineGroup.cpp
    │   │       │   │   ├── timemgr.cpp
    │   │       │   │   ├── timer.cpp
    │   │       │   │   ├── timespan.cpp
    │   │       │   │   ├── TimingCollection.cpp
    │   │       │   │   └── triggers.cpp
    │   │       │   ├── common/
    │   │       │   │   ├── HeaderDependencyBridges.cpp
    │   │       │   │   ├── memorysurface.cpp
    │   │       │   │   └── values.cpp
    │   │       │   ├── compositor/
    │   │       │   │   ├── command.h
    │   │       │   │   ├── compositor-all.h
    │   │       │   │   ├── CompositorDirectManipulationViewport.cpp
    │   │       │   │   ├── CompositorDirectManipulationViewport.h
    │   │       │   │   ├── compositorscheduler.cpp
    │   │       │   │   ├── compositorscheduler.h
    │   │       │   │   ├── compositortree.cpp
    │   │       │   │   ├── compositortree.h
    │   │       │   │   ├── hardwarecommand.cpp
    │   │       │   │   ├── hardwarecommand.h
    │   │       │   │   ├── RefreshAlignedClock.cpp
    │   │       │   │   ├── RefreshAlignedClock.h
    │   │       │   │   ├── RefreshRateInfo.h
    │   │       │   │   ├── TransformToRoot.h
    │   │       │   │   ├── UIThreadScheduler.cpp
    │   │       │   │   ├── windowrendertarget.cpp
    │   │       │   │   └── windowrendertarget.h
    │   │       │   ├── controls/
    │   │       │   │   └── generated/
    │   │       │   │       ├── CAddDeleteThemeTransition.g.h
    │   │       │   │       ├── CAppBar.g.h
    │   │       │   │       ├── CAppBarAutomationPeer.g.h
    │   │       │   │       ├── CAppBarButton.g.h
    │   │       │   │       ├── CAppBarButtonAutomationPeer.g.h
    │   │       │   │       ├── CAppBarButtonTemplateSettings.g.h
    │   │       │   │       ├── CAppBarElementContainer.g.h
    │   │       │   │       ├── CAppBarLightDismiss.g.h
    │   │       │   │       ├── CAppBarLightDismissAutomationPeer.g.h
    │   │       │   │       ├── CAppBarSeparator.g.h
    │   │       │   │       ├── CAppBarTemplateSettings.g.h
    │   │       │   │       ├── CAppBarToggleButton.g.h
    │   │       │   │       ├── CAppBarToggleButtonAutomationPeer.g.h
    │   │       │   │       ├── CAppBarToggleButtonTemplateSettings.g.h
    │   │       │   │       ├── CApplicationBarService.g.h
    │   │       │   │       ├── CAutomationAnnotation.g.h
    │   │       │   │       ├── CAutomationPeerAnnotation.g.h
    │   │       │   │       ├── CAutoSuggestBox.g.h
    │   │       │   │       ├── CAutoSuggestBoxAutomationPeer.g.h
    │   │       │   │       ├── CAutoSuggestBoxQuerySubmittedEventArgs.g.h
    │   │       │   │       ├── CAutoSuggestBoxSuggestionChosenEventArgs.g.h
    │   │       │   │       ├── CAutoSuggestBoxTextChangedEventArgs.g.h
    │   │       │   │       ├── CBitmapIconSource.g.h
    │   │       │   │       ├── CButtonAutomationPeer.g.h
    │   │       │   │       ├── CButtonBase.g.h
    │   │       │   │       ├── CButtonBaseAutomationPeer.g.h
    │   │       │   │       ├── CCalendarDatePicker.g.h
    │   │       │   │       ├── CCalendarDatePickerAutomationPeer.g.h
    │   │       │   │       ├── CCalendarPanel.g.h
    │   │       │   │       ├── CCalendarScrollViewerAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewBaseItemAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewDayItemAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewHeaderAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewItemAutomationPeer.g.h
    │   │       │   │       ├── CCalendarViewTemplateSettings.g.h
    │   │       │   │       ├── CCarouselPanel.g.h
    │   │       │   │       ├── CCheckBox.g.h
    │   │       │   │       ├── CCheckBoxAutomationPeer.g.h
    │   │       │   │       ├── CCollectionView.g.h
    │   │       │   │       ├── CCollectionViewGroup.g.h
    │   │       │   │       ├── CComboBox.g.h
    │   │       │   │       ├── CComboBoxAutomationPeer.g.h
    │   │       │   │       ├── CComboBoxItem.g.h
    │   │       │   │       ├── CComboBoxItemAutomationPeer.g.h
    │   │       │   │       ├── CComboBoxItemDataAutomationPeer.g.h
    │   │       │   │       ├── CComboBoxLightDismiss.g.h
    │   │       │   │       ├── CComboBoxLightDismissAutomationPeer.g.h
    │   │       │   │       ├── CComboBoxTemplateSettings.g.h
    │   │       │   │       ├── CCommandBarOverflowPresenter.g.h
    │   │       │   │       ├── CCommandBarTemplateSettings.g.h
    │   │       │   │       ├── CCommandingContainer.g.h
    │   │       │   │       ├── CContentDialog.g.h
    │   │       │   │       ├── CContentDialogOpenCloseThemeTransition.g.h
    │   │       │   │       ├── CContentThemeTransition.g.h
    │   │       │   │       ├── CDatePicker.g.h
    │   │       │   │       ├── CDatePickerAutomationPeer.g.h
    │   │       │   │       ├── CDebugSettings.g.h
    │   │       │   │       ├── CDragItemThemeAnimation.g.h
    │   │       │   │       ├── CDragOverThemeAnimation.g.h
    │   │       │   │       ├── CDrillInThemeAnimation.g.h
    │   │       │   │       ├── CDrillOutThemeAnimation.g.h
    │   │       │   │       ├── CDropTargetItemThemeAnimation.g.h
    │   │       │   │       ├── CEdgeUIThemeTransition.g.h
    │   │       │   │       ├── CEntranceThemeTransition.g.h
    │   │       │   │       ├── CFaceplateContentPresenterAutomationPeer.g.h
    │   │       │   │       ├── CFadeInThemeAnimation.g.h
    │   │       │   │       ├── CFadeOutThemeAnimation.g.h
    │   │       │   │       ├── CFlipView.g.h
    │   │       │   │       ├── CFlipViewAutomationPeer.g.h
    │   │       │   │       ├── CFlipViewItem.g.h
    │   │       │   │       ├── CFlipViewItemAutomationPeer.g.h
    │   │       │   │       ├── CFlipViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── CFlyoutPresenter.g.h
    │   │       │   │       ├── CFlyoutPresenterAutomationPeer.g.h
    │   │       │   │       ├── CFontIconSource.g.h
    │   │       │   │       ├── CFrame.g.h
    │   │       │   │       ├── CFullWindowMediaRootAutomationPeer.g.h
    │   │       │   │       ├── CGridView.g.h
    │   │       │   │       ├── CGridViewAutomationPeer.g.h
    │   │       │   │       ├── CGridViewHeaderItem.g.h
    │   │       │   │       ├── CGridViewHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── CGridViewItem.g.h
    │   │       │   │       ├── CGridViewItemAutomationPeer.g.h
    │   │       │   │       ├── CGridViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── CGridViewItemTemplateSettings.g.h
    │   │       │   │       ├── CGroupedDataCollectionView.g.h
    │   │       │   │       ├── CGroupItem.g.h
    │   │       │   │       ├── CGroupItemAutomationPeer.g.h
    │   │       │   │       ├── CGroupStyle.g.h
    │   │       │   │       ├── CHub.g.h
    │   │       │   │       ├── CHubAutomationPeer.g.h
    │   │       │   │       ├── CHubSection.g.h
    │   │       │   │       ├── CHubSectionAutomationPeer.g.h
    │   │       │   │       ├── CHyperlinkButton.g.h
    │   │       │   │       ├── CHyperlinkButtonAutomationPeer.g.h
    │   │       │   │       ├── CIconSource.g.h
    │   │       │   │       ├── CInputPaneThemeTransition.g.h
    │   │       │   │       ├── CIRawElementProviderSimple.g.h
    │   │       │   │       ├── CItemAutomationPeer.g.h
    │   │       │   │       ├── CItemsControlAutomationPeer.g.h
    │   │       │   │       ├── CItemsWrapGrid.g.h
    │   │       │   │       ├── CIterableCollectionView.g.h
    │   │       │   │       ├── CLandmarkTargetAutomationPeer.g.h
    │   │       │   │       ├── CLayoutTransitionStaggerItem.g.h
    │   │       │   │       ├── CListBox.g.h
    │   │       │   │       ├── CListBoxAutomationPeer.g.h
    │   │       │   │       ├── CListBoxItem.g.h
    │   │       │   │       ├── CListBoxItemAutomationPeer.g.h
    │   │       │   │       ├── CListBoxItemDataAutomationPeer.g.h
    │   │       │   │       ├── CListView.g.h
    │   │       │   │       ├── CListViewAutomationPeer.g.h
    │   │       │   │       ├── CListViewBase.g.h
    │   │       │   │       ├── CListViewBaseAutomationPeer.g.h
    │   │       │   │       ├── CListViewBaseHeaderItem.g.h
    │   │       │   │       ├── CListViewBaseHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── CListViewBaseItemAutomationPeer.g.h
    │   │       │   │       ├── CListViewBaseItemDataAutomationPeer.g.h
    │   │       │   │       ├── CListViewBaseItemTemplateSettings.g.h
    │   │       │   │       ├── CListViewHeaderItem.g.h
    │   │       │   │       ├── CListViewHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── CListViewItem.g.h
    │   │       │   │       ├── CListViewItemAutomationPeer.g.h
    │   │       │   │       ├── CListViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── CListViewItemTemplateSettings.g.h
    │   │       │   │       ├── CMediaPlaybackItemConverter.g.h
    │   │       │   │       ├── CMediaPlayerElementAutomationPeer.g.h
    │   │       │   │       ├── CMediaTransportControls.g.h
    │   │       │   │       ├── CMediaTransportControlsAutomationPeer.g.h
    │   │       │   │       ├── CMenuFlyoutItem.g.h
    │   │       │   │       ├── CMenuFlyoutItemAutomationPeer.g.h
    │   │       │   │       ├── CMenuFlyoutItemBase.g.h
    │   │       │   │       ├── CMenuFlyoutItemTemplateSettings.g.h
    │   │       │   │       ├── CMenuFlyoutPresenterAutomationPeer.g.h
    │   │       │   │       ├── CMenuFlyoutPresenterTemplateSettings.g.h
    │   │       │   │       ├── CMenuFlyoutSeparator.g.h
    │   │       │   │       ├── CMenuFlyoutSubItemAutomationPeer.g.h
    │   │       │   │       ├── CMenuPopupThemeTransition.g.h
    │   │       │   │       ├── CModernCollectionBasePanel.g.h
    │   │       │   │       ├── CNamedContainerAutomationPeer.g.h
    │   │       │   │       ├── CNavigationTransitionInfo.g.h
    │   │       │   │       ├── CoreControlsGenerated.vcxproj
    │   │       │   │       ├── COrientedVirtualizingPanel.g.h
    │   │       │   │       ├── CPage.g.h
    │   │       │   │       ├── CPageStackEntry.g.h
    │   │       │   │       ├── CPaneThemeTransition.g.h
    │   │       │   │       ├── CPathIconSource.g.h
    │   │       │   │       ├── CPickerFlyoutThemeTransition.g.h
    │   │       │   │       ├── CPointerDownThemeAnimation.g.h
    │   │       │   │       ├── CPointerUpThemeAnimation.g.h
    │   │       │   │       ├── CPopInThemeAnimation.g.h
    │   │       │   │       ├── CPopOutThemeAnimation.g.h
    │   │       │   │       ├── CPopupAutomationPeer.g.h
    │   │       │   │       ├── CPopupRootAutomationPeer.g.h
    │   │       │   │       ├── CPopupThemeTransition.g.h
    │   │       │   │       ├── CPVLStaggerFunction.g.h
    │   │       │   │       ├── CRadioButton.g.h
    │   │       │   │       ├── CRadioButtonAutomationPeer.g.h
    │   │       │   │       ├── CRangeBaseAutomationPeer.g.h
    │   │       │   │       ├── CReorderThemeTransition.g.h
    │   │       │   │       ├── CRepeatButton.g.h
    │   │       │   │       ├── CRepeatButtonAutomationPeer.g.h
    │   │       │   │       ├── CRepositionThemeAnimation.g.h
    │   │       │   │       ├── CRepositionThemeTransition.g.h
    │   │       │   │       ├── CRootScrollViewer.g.h
    │   │       │   │       ├── CScrollBar.g.h
    │   │       │   │       ├── CScrollBarAutomationPeer.g.h
    │   │       │   │       ├── CScrollContentPresenter.g.h
    │   │       │   │       ├── CScrollViewerAutomationPeer.g.h
    │   │       │   │       ├── CSeekSliderAutomationPeer.g.h
    │   │       │   │       ├── CSelector.g.h
    │   │       │   │       ├── CSelectorAutomationPeer.g.h
    │   │       │   │       ├── CSelectorItem.g.h
    │   │       │   │       ├── CSelectorItemAutomationPeer.g.h
    │   │       │   │       ├── CSemanticZoomAutomationPeer.g.h
    │   │       │   │       ├── CSlider.g.h
    │   │       │   │       ├── CSliderAutomationPeer.g.h
    │   │       │   │       ├── CSplitCloseThemeAnimation.g.h
    │   │       │   │       ├── CSplitOpenThemeAnimation.g.h
    │   │       │   │       ├── CSplitViewLightDismissAutomationPeer.g.h
    │   │       │   │       ├── CSplitViewPaneAutomationPeer.g.h
    │   │       │   │       ├── CStandardUICommand.g.h
    │   │       │   │       ├── CSwipeBackThemeAnimation.g.h
    │   │       │   │       ├── CSwipeHintThemeAnimation.g.h
    │   │       │   │       ├── CSymbolIconSource.g.h
    │   │       │   │       ├── CTextHighlighterBase.g.h
    │   │       │   │       ├── CThemeAnimationBase.g.h
    │   │       │   │       ├── CThumb.g.h
    │   │       │   │       ├── CThumbAutomationPeer.g.h
    │   │       │   │       ├── CTickBar.g.h
    │   │       │   │       ├── CTimePicker.g.h
    │   │       │   │       ├── CTimePickerAutomationPeer.g.h
    │   │       │   │       ├── CToggleButton.g.h
    │   │       │   │       ├── CToggleButtonAutomationPeer.g.h
    │   │       │   │       ├── CToggleMenuFlyoutItem.g.h
    │   │       │   │       ├── CToggleMenuFlyoutItemAutomationPeer.g.h
    │   │       │   │       ├── CToggleSwitch.g.h
    │   │       │   │       ├── CToggleSwitchAutomationPeer.g.h
    │   │       │   │       ├── CToggleSwitchTemplateSettings.g.h
    │   │       │   │       ├── CToolTip.g.h
    │   │       │   │       ├── CToolTipAutomationPeer.g.h
    │   │       │   │       ├── CToolTipTemplateSettings.g.h
    │   │       │   │       ├── CVariableSizedWrapGrid.g.h
    │   │       │   │       ├── CVectorCollectionView.g.h
    │   │       │   │       ├── CVectorViewCollectionView.g.h
    │   │       │   │       ├── CVirtualizingPanel.g.h
    │   │       │   │       ├── CVirtualizingStackPanel.g.h
    │   │       │   │       ├── CWrapGrid.g.h
    │   │       │   │       ├── CXamlUICommand.g.h
    │   │       │   │       ├── GeneratedClasses.g.cpp
    │   │       │   │       ├── GeneratedClasses.g.h
    │   │       │   │       └── precomp.h
    │   │       │   ├── core/
    │   │       │   │   └── elements/
    │   │       │   │       ├── AccessKeyEvents.cpp
    │   │       │   │       ├── AdaptiveTrigger.cpp
    │   │       │   │       ├── AutomationEventsHelper.cpp
    │   │       │   │       ├── AutomationPeer.cpp
    │   │       │   │       ├── Binding.cpp
    │   │       │   │       ├── Border.cpp
    │   │       │   │       ├── BoundsGeometrySink.cpp
    │   │       │   │       ├── BringIntoViewRequestedEventArgs.cpp
    │   │       │   │       ├── brush.cpp
    │   │       │   │       ├── Button.cpp
    │   │       │   │       ├── cachemode.cpp
    │   │       │   │       ├── CalendarView.cpp
    │   │       │   │       ├── CalendarViewBaseItemChrome.cpp
    │   │       │   │       ├── canvas.cpp
    │   │       │   │       ├── CommandBar.cpp
    │   │       │   │       ├── CompositeTransform.cpp
    │   │       │   │       ├── ConnectedAnimationRoot.cpp
    │   │       │   │       ├── ContentControl.cpp
    │   │       │   │       ├── ContentPresenter.cpp
    │   │       │   │       ├── Control.cpp
    │   │       │   │       ├── CWindow.cpp
    │   │       │   │       ├── DefaultValues.cpp
    │   │       │   │       ├── DeferredElement.cpp
    │   │       │   │       ├── DeferredKeys.cpp
    │   │       │   │       ├── DeferredMapping.cpp
    │   │       │   │       ├── DependencyProperty.cpp
    │   │       │   │       ├── DependencyPropertyProxy.cpp
    │   │       │   │       ├── depends.cpp
    │   │       │   │       ├── DragEventArgs.cpp
    │   │       │   │       ├── ellipse.cpp
    │   │       │   │       ├── Enums.g.cpp
    │   │       │   │       ├── figure.cpp
    │   │       │   │       ├── Flyout.cpp
    │   │       │   │       ├── FlyoutBase.cpp
    │   │       │   │       ├── framework.cpp
    │   │       │   │       ├── FrameworkElementAutomationPeer.cpp
    │   │       │   │       ├── frameworkelementex.cpp
    │   │       │   │       ├── FullWindowMediaRoot.cpp
    │   │       │   │       ├── GeneralTransformHelper.cpp
    │   │       │   │       ├── geometry.cpp
    │   │       │   │       ├── GeometryBoundsHelper.cpp
    │   │       │   │       ├── GeometryGroupSink.cpp
    │   │       │   │       ├── Glyphs.cpp
    │   │       │   │       ├── gradient.cpp
    │   │       │   │       ├── Grid.cpp
    │   │       │   │       ├── GridDefinitions.cpp
    │   │       │   │       ├── GridLength.cpp
    │   │       │   │       ├── HitTestHelper.cpp
    │   │       │   │       ├── HitTestingGeometrySink.cpp
    │   │       │   │       ├── icon.cpp
    │   │       │   │       ├── ImageAutomationPeer.cpp
    │   │       │   │       ├── imagebase.cpp
    │   │       │   │       ├── imagebrush.cpp
    │   │       │   │       ├── ImageDecodeBoundsFinder.cpp
    │   │       │   │       ├── imagesource.cpp
    │   │       │   │       ├── ImageSurfaceWrapper.cpp
    │   │       │   │       ├── InputScope.cpp
    │   │       │   │       ├── ItemsControl.cpp
    │   │       │   │       ├── ItemsPresenter.cpp
    │   │       │   │       ├── ItemsStackPanel.cpp
    │   │       │   │       ├── layoutelement.cpp
    │   │       │   │       ├── LayoutTransition.cpp
    │   │       │   │       ├── line.cpp
    │   │       │   │       ├── ListViewBaseItem.cpp
    │   │       │   │       ├── ListViewBaseItemChrome.cpp
    │   │       │   │       ├── ListViewBaseItemSecondaryChrome.cpp
    │   │       │   │       ├── MatrixTransform.cpp
    │   │       │   │       ├── mediabase.cpp
    │   │       │   │       ├── MenuFlyout.cpp
    │   │       │   │       ├── MenuFlyoutSubItem.cpp
    │   │       │   │       ├── MultiParentShareableDependencyObject.cpp
    │   │       │   │       ├── NoParentShareableDependencyObject.cpp
    │   │       │   │       ├── NullExtension.cpp
    │   │       │   │       ├── panel.cpp
    │   │       │   │       ├── panelex.cpp
    │   │       │   │       ├── path.cpp
    │   │       │   │       ├── perspectiveplane.cpp
    │   │       │   │       ├── PointHitTestGeometrySink.cpp
    │   │       │   │       ├── PointHitTestHelper.cpp
    │   │       │   │       ├── polygon.cpp
    │   │       │   │       ├── PolygonHitTestGeometrySink.cpp
    │   │       │   │       ├── PolygonHitTestHelper.cpp
    │   │       │   │       ├── polyline.cpp
    │   │       │   │       ├── Popup.cpp
    │   │       │   │       ├── RangeBase.cpp
    │   │       │   │       ├── rectangle.cpp
    │   │       │   │       ├── RelativePanel.cpp
    │   │       │   │       ├── RenderTargetBitmap.cpp
    │   │       │   │       ├── RenderTargetBitmapRoot.cpp
    │   │       │   │       ├── RenderTargetBitmapWaitExecutor.cpp
    │   │       │   │       ├── RenderTargetElement.cpp
    │   │       │   │       ├── Resources.cpp
    │   │       │   │       ├── RichTextBlockAutomationPeer.cpp
    │   │       │   │       ├── RichTextBlockOverflowAutomationPeer.cpp
    │   │       │   │       ├── RootVisual.cpp
    │   │       │   │       ├── RotateTransform.cpp
    │   │       │   │       ├── ScaleTransform.cpp
    │   │       │   │       ├── ScrollContentControl.cpp
    │   │       │   │       ├── ScrollViewer.cpp
    │   │       │   │       ├── segment.cpp
    │   │       │   │       ├── SemanticZoom.cpp
    │   │       │   │       ├── Setter.cpp
    │   │       │   │       ├── shape.cpp
    │   │       │   │       ├── simple.cpp
    │   │       │   │       ├── SizeChangedEventArgs.cpp
    │   │       │   │       ├── SizeUtil.cpp
    │   │       │   │       ├── SkewTransform.cpp
    │   │       │   │       ├── SoftwareBitmapSource.cpp
    │   │       │   │       ├── SolidColorBrush.cpp
    │   │       │   │       ├── sources.props
    │   │       │   │       ├── SplitView.cpp
    │   │       │   │       ├── StackPanel.cpp
    │   │       │   │       ├── StaggerFunctions.cpp
    │   │       │   │       ├── StateTrigger.cpp
    │   │       │   │       ├── StateTriggerBase.cpp
    │   │       │   │       ├── Style.cpp
    │   │       │   │       ├── SurfaceImageSource.cpp
    │   │       │   │       ├── SvgImageSource.cpp
    │   │       │   │       ├── SwapChainBackgroundPanel.cpp
    │   │       │   │       ├── SwapChainElement.cpp
    │   │       │   │       ├── TargetPropertyPath.cpp
    │   │       │   │       ├── Template.cpp
    │   │       │   │       ├── TemplateBindingExtension.cpp
    │   │       │   │       ├── TemplateContent.cpp
    │   │       │   │       ├── TemplateNamescope.cpp
    │   │       │   │       ├── TextBlockAutomationPeer.cpp
    │   │       │   │       ├── ThemeResourceExtension.cpp
    │   │       │   │       ├── tilebrush.cpp
    │   │       │   │       ├── TiledSurface.cpp
    │   │       │   │       ├── TouchableRectangle.cpp
    │   │       │   │       ├── transform.cpp
    │   │       │   │       ├── TransformGeometrySink.cpp
    │   │       │   │       ├── TransformGroup.cpp
    │   │       │   │       ├── transforms.cpp
    │   │       │   │       ├── TransitionRoot.cpp
    │   │       │   │       ├── TransitionTarget.cpp
    │   │       │   │       ├── TranslateTransform.cpp
    │   │       │   │       ├── Type.cpp
    │   │       │   │       ├── UIAPatternProvider.cpp
    │   │       │   │       ├── uielement.cpp
    │   │       │   │       ├── UIElement.g.cpp
    │   │       │   │       ├── Viewbox.cpp
    │   │       │   │       ├── VirtualSurfaceimageSource.cpp
    │   │       │   │       ├── VisualState.cpp
    │   │       │   │       ├── VisualStateGroup.cpp
    │   │       │   │       ├── VisualStateManager.cpp
    │   │       │   │       ├── VisualTransition.cpp
    │   │       │   │       ├── visualtransitioncompleteddata.cpp
    │   │       │   │       ├── WriteableBitmap.cpp
    │   │       │   │       ├── XamlCompositionBrush.cpp
    │   │       │   │       ├── XamlIslandRootCollection.cpp
    │   │       │   │       ├── XamlPredicate.cpp
    │   │       │   │       ├── lib/
    │   │       │   │       │   └── elements.vcxproj
    │   │       │   │       ├── lib2/
    │   │       │   │       │   └── elements2.vcxproj
    │   │       │   │       ├── libexcept/
    │   │       │   │       │   └── elements.except.vcxproj
    │   │       │   │       ├── pch/
    │   │       │   │       │   ├── elements.pch.vcxproj
    │   │       │   │       │   └── precomp.h
    │   │       │   │       └── pchexcept/
    │   │       │   │           ├── elements.except.pch.vcxproj
    │   │       │   │           └── precomp.h
    │   │       │   ├── dethunk/
    │   │       │   │   └── elements/
    │   │       │   │       └── MediaQueue.cpp
    │   │       │   ├── dll/
    │   │       │   │   ├── CoreImports.cpp
    │   │       │   │   ├── DebugSource.cpp
    │   │       │   │   ├── dllentry.cpp
    │   │       │   │   ├── eventmgr.cpp
    │   │       │   │   ├── focusmgr.cpp
    │   │       │   │   ├── ImageReloadManager.cpp
    │   │       │   │   ├── purecall.cpp
    │   │       │   │   ├── rendertargetbitmapmgr.cpp
    │   │       │   │   ├── services.cpp
    │   │       │   │   ├── UriValidator.cpp
    │   │       │   │   ├── VisualTree.cpp
    │   │       │   │   ├── xcpcore.cpp
    │   │       │   │   └── xcpcore_namescope.cpp
    │   │       │   ├── error/
    │   │       │   │   ├── ErrorEventArgs.cpp
    │   │       │   │   └── ErrorService.cpp
    │   │       │   ├── hw/
    │   │       │   │   ├── AtlasRequestProvider.cpp
    │   │       │   │   ├── BaseContentRenderer.cpp
    │   │       │   │   ├── BaseContentRenderer.h
    │   │       │   │   ├── CompositorTreeHost.cpp
    │   │       │   │   ├── CompositorTreeHost.h
    │   │       │   │   ├── ContentRenderer.cpp
    │   │       │   │   ├── ContentRenderer.h
    │   │       │   │   ├── DManipData.cpp
    │   │       │   │   ├── DManipData.h
    │   │       │   │   ├── Effects.cpp
    │   │       │   │   ├── Effects.h
    │   │       │   │   ├── hw-all.h
    │   │       │   │   ├── hw.vcxproj
    │   │       │   │   ├── hwcompnode.cpp
    │   │       │   │   ├── hwcompnode.h
    │   │       │   │   ├── hwrealization.cpp
    │   │       │   │   ├── hwrealization.h
    │   │       │   │   ├── hwsurfacecache.cpp
    │   │       │   │   ├── hwsurfacecache.h
    │   │       │   │   ├── hwtexturemgr.cpp
    │   │       │   │   ├── hwtexturemgr.h
    │   │       │   │   ├── hwwalk.cpp
    │   │       │   │   ├── hwwalk.h
    │   │       │   │   ├── ManipulationTransform.cpp
    │   │       │   │   ├── ManipulationTransform.h
    │   │       │   │   ├── MaxTextureSizeProvider.cpp
    │   │       │   │   ├── precomp.h
    │   │       │   │   ├── VisualContentRenderer.cpp
    │   │       │   │   └── VisualContentRenderer.h
    │   │       │   ├── imaging/
    │   │       │   │   └── ImagingProvider/
    │   │       │   │       ├── AsyncImageFactory.cpp
    │   │       │   │       ├── AsyncImageFactory.h
    │   │       │   │       ├── AsyncReleaseTask.h
    │   │       │   │       ├── ImageProvider.cpp
    │   │       │   │       ├── ImageProvider.h
    │   │       │   │       ├── ImageProviderDecodeHandlerTask.cpp
    │   │       │   │       ├── ImageProviderDecodeHandlerTask.h
    │   │       │   │       └── LoadedImageSurface.cpp
    │   │       │   ├── inc/
    │   │       │   │   ├── AccessKeyHiddenEventArgs.h
    │   │       │   │   ├── AccessKeyInvokedEventArgs.h
    │   │       │   │   ├── AccessKeyShownEventArgs.h
    │   │       │   │   ├── ActivationAPI.h
    │   │       │   │   ├── Activators.g.h
    │   │       │   │   ├── AdaptiveTrigger.h
    │   │       │   │   ├── animation.h
    │   │       │   │   ├── application.h
    │   │       │   │   ├── AtlasRequestProvider.h
    │   │       │   │   ├── automation.h
    │   │       │   │   ├── AutomationAnnotationCollection.h
    │   │       │   │   ├── AutomationEventsHelper.h
    │   │       │   │   ├── AutomationPeer.h
    │   │       │   │   ├── AutomationPeerAnnotationCollection.h
    │   │       │   │   ├── AutomationPeerCollection.h
    │   │       │   │   ├── AutomationPeerEventArgs.h
    │   │       │   │   ├── BaseValueSource.h
    │   │       │   │   ├── BeginPrintEventArgs.h
    │   │       │   │   ├── BinaryFormatObjectWriter.h
    │   │       │   │   ├── Binding.h
    │   │       │   │   ├── BlockTextElement.h
    │   │       │   │   ├── Border.h
    │   │       │   │   ├── BoundsGeometrySink.h
    │   │       │   │   ├── BoundsWalkHitResult.h
    │   │       │   │   ├── BringIntoViewHandler.h
    │   │       │   │   ├── BringIntoViewRequestedEventArgs.h
    │   │       │   │   ├── brush.h
    │   │       │   │   ├── Button.h
    │   │       │   │   ├── cachemode.h
    │   │       │   │   ├── CalendarView.h
    │   │       │   │   ├── CalendarViewBaseItemChrome.h
    │   │       │   │   ├── CandidateWindowBoundsChangedEventArgs.h
    │   │       │   │   ├── canvas.h
    │   │       │   │   ├── CaretBrowsingCaret.h
    │   │       │   │   ├── CaretBrowsingGlobal.h
    │   │       │   │   ├── CControl.h
    │   │       │   │   ├── CDependencyObject.h
    │   │       │   │   ├── cdeployment.h
    │   │       │   │   ├── CDOAssociative.h
    │   │       │   │   ├── CDOAssociativeImpl.h
    │   │       │   │   ├── CDOSharedState.h
    │   │       │   │   ├── ChangedPropertyEventArgs.h
    │   │       │   │   ├── CharacterReceivedEventArgs.h
    │   │       │   │   ├── cinputscope.h
    │   │       │   │   ├── CircularMemoryLogger.h
    │   │       │   │   ├── CKeyboardAccelerator.h
    │   │       │   │   ├── CKeyboardAcceleratorCollection.h
    │   │       │   │   ├── CKeyboardAcceleratorInvokedEventArgs.h
    │   │       │   │   ├── CollectionViewSource.h
    │   │       │   │   ├── ColorAnimation.h
    │   │       │   │   ├── ColorAnimationUsingKeyFrames.h
    │   │       │   │   ├── ColorKeyFrame.h
    │   │       │   │   ├── ComboBoxTextSubmittedEventArgs.h
    │   │       │   │   ├── CommandBar.h
    │   │       │   │   ├── CommandBarElementCollection.h
    │   │       │   │   ├── CompositeTransform.h
    │   │       │   │   ├── CompressedObjectWriterStack.h
    │   │       │   │   ├── CompressedStackCacheHint.h
    │   │       │   │   ├── ConnectedAnimationRoot.h
    │   │       │   │   ├── ContentControl.h
    │   │       │   │   ├── ContentPresenter.h
    │   │       │   │   ├── ContextMenuEventArgs.h
    │   │       │   │   ├── ContextRequestedEventArgs.h
    │   │       │   │   ├── CoreAsyncAction.h
    │   │       │   │   ├── CoreEventArgsGroup.h
    │   │       │   │   ├── corep.h
    │   │       │   │   ├── CorePeggedPtr.h
    │   │       │   │   ├── CreateGroupFn.h
    │   │       │   │   ├── CreateParameters.h
    │   │       │   │   ├── CustomClassInfo.h
    │   │       │   │   ├── CustomDependencyProperty.h
    │   │       │   │   ├── CWindow.h
    │   │       │   │   ├── DebugSource.h
    │   │       │   │   ├── DeclareMacros.h
    │   │       │   │   ├── DeferredAnimationOperation.h
    │   │       │   │   ├── DeferredElement.h
    │   │       │   │   ├── DeferredKeys.h
    │   │       │   │   ├── DeferredMapping.h
    │   │       │   │   ├── DeferringWriter.h
    │   │       │   │   ├── DependencyObjectWrapper.h
    │   │       │   │   ├── DependencyPropertyProxy.h
    │   │       │   │   ├── depends.h
    │   │       │   │   ├── DeviceListener.h
    │   │       │   │   ├── DiagnosticsInterop_SimpleProperties.g.h
    │   │       │   │   ├── DirectManipulationContainer.h
    │   │       │   │   ├── DirectManipulationContainerHandler.h
    │   │       │   │   ├── DirectManipulationServiceSharedState.h
    │   │       │   │   ├── DirtyFlags.h
    │   │       │   │   ├── DisplayListener.h
    │   │       │   │   ├── DMContent.h
    │   │       │   │   ├── DMDeferredRelease.h
    │   │       │   │   ├── DMViewport.h
    │   │       │   │   ├── DOPointerCast.h
    │   │       │   │   ├── DoubleAnimation.h
    │   │       │   │   ├── DoubleAnimationUsingKeyFrames.h
    │   │       │   │   ├── DoubleKeyFrame.h
    │   │       │   │   ├── DoubleTappedEventArgs.h
    │   │       │   │   ├── DownloadProgressEventArgs.h
    │   │       │   │   ├── DragEventArgs.h
    │   │       │   │   ├── duration.h
    │   │       │   │   ├── DurationVO.h
    │   │       │   │   ├── DXamlServices.h
    │   │       │   │   ├── DynamicMetadataStorage.h
    │   │       │   │   ├── DynamicTimeline.h
    │   │       │   │   ├── EasingFunctions.h
    │   │       │   │   ├── EffectiveValue.h
    │   │       │   │   ├── EffectiveViewportChangedEventArgs.h
    │   │       │   │   ├── elements.h
    │   │       │   │   ├── ellipse.h
    │   │       │   │   ├── EndPrintEventArgs.h
    │   │       │   │   ├── EnterParams.h
    │   │       │   │   ├── Enums.g.h
    │   │       │   │   ├── EnumValueTable.h
    │   │       │   │   ├── ErrorEventArgs.h
    │   │       │   │   ├── ErrorService.h
    │   │       │   │   ├── EventArgs.h
    │   │       │   │   ├── eventmgr.h
    │   │       │   │   ├── ExceptionRoutedEventArgs.h
    │   │       │   │   ├── FacadeAnimationhelper.h
    │   │       │   │   ├── FacadeReferenceWrapper.h
    │   │       │   │   ├── FacadeStorage.h
    │   │       │   │   ├── figure.h
    │   │       │   │   ├── Flyout.h
    │   │       │   │   ├── FlyoutBase.h
    │   │       │   │   ├── FocusedElementRemovedEventArgs.h
    │   │       │   │   ├── FocusManagerGotFocusEventArgs.h
    │   │       │   │   ├── FocusManagerLostFocusEventArgs.h
    │   │       │   │   ├── focusmgr.h
    │   │       │   │   ├── FontAndScriptServices.h
    │   │       │   │   ├── FontFamily.h
    │   │       │   │   ├── framework.h
    │   │       │   │   ├── FrameworkElementAutomationPeer.h
    │   │       │   │   ├── frameworkelementex.h
    │   │       │   │   ├── FrameworkInputViewHandler.h
    │   │       │   │   ├── FullWindowMediaRoot.h
    │   │       │   │   ├── FxCallbacks.h
    │   │       │   │   ├── GeneralTransform.h
    │   │       │   │   ├── GeneralTransformHelper.h
    │   │       │   │   ├── geometry.h
    │   │       │   │   ├── GeometryBoundsHelper.h
    │   │       │   │   ├── GeometryGroupSink.h
    │   │       │   │   ├── GettingFocusEventArgs.h
    │   │       │   │   ├── Glyphs.h
    │   │       │   │   ├── gradient.h
    │   │       │   │   ├── Grid.h
    │   │       │   │   ├── GridCells.h
    │   │       │   │   ├── GridDefinitions.h
    │   │       │   │   ├── GridLength.h
    │   │       │   │   ├── GridViewItemChrome.h
    │   │       │   │   ├── GripperPopup.h
    │   │       │   │   ├── HeaderDependencyBridges.h
    │   │       │   │   ├── HitTestGeometrySink.h
    │   │       │   │   ├── HitTestHelper.h
    │   │       │   │   ├── HoldingEventArgs.h
    │   │       │   │   ├── HubSectionCollection.h
    │   │       │   │   ├── Hyperlink.h
    │   │       │   │   ├── HyperLinkAutomationPeer.h
    │   │       │   │   ├── HyperlinkClickEventArgs.h
    │   │       │   │   ├── IBackingStore.h
    │   │       │   │   ├── icon.h
    │   │       │   │   ├── ICustomResourceLoader.h
    │   │       │   │   ├── IHwndComponentHost.h
    │   │       │   │   ├── ImageAutomationPeer.h
    │   │       │   │   ├── imagebase.h
    │   │       │   │   ├── imagebrush.h
    │   │       │   │   ├── ImageDecodeBoundsFinder.h
    │   │       │   │   ├── ImageReloadManager.h
    │   │       │   │   ├── imagesource.h
    │   │       │   │   ├── ImageSurfaceWrapper.h
    │   │       │   │   ├── INamescope.h
    │   │       │   │   ├── InertiaExpansionBehavior.h
    │   │       │   │   ├── InertiaRotationBehavior.h
    │   │       │   │   ├── InertiaTranslationBehavior.h
    │   │       │   │   ├── InheritanceContextChangeKind.h
    │   │       │   │   ├── InheritedProperties.h
    │   │       │   │   ├── inline.h
    │   │       │   │   ├── InputActivationBehavior.h
    │   │       │   │   ├── InputManagerDMViewportEventHandler.h
    │   │       │   │   ├── InputPaneHandler.h
    │   │       │   │   ├── InputPointEventArgs.h
    │   │       │   │   ├── InputServices.h
    │   │       │   │   ├── InteractionManager.h
    │   │       │   │   ├── iobjectwritercallbacks.h
    │   │       │   │   ├── IParserCoreServices.h
    │   │       │   │   ├── IPLMListener.h
    │   │       │   │   ├── IsEnabledChangedEventArgs.h
    │   │       │   │   ├── IsTextTrimmedChangedEventArgs.h
    │   │       │   │   ├── ItemsControl.h
    │   │       │   │   ├── ItemsPresenter.h
    │   │       │   │   ├── ItemsStackPanel.h
    │   │       │   │   ├── IXamlSchemaObject.h
    │   │       │   │   ├── JupiterTextHelper.h
    │   │       │   │   ├── KeyboardEventArgs.h
    │   │       │   │   ├── KeyFrame.h
    │   │       │   │   ├── KeyFrameCollection.h
    │   │       │   │   ├── KeySpline.h
    │   │       │   │   ├── KeyTime.h
    │   │       │   │   ├── KeyTimeVO.h
    │   │       │   │   ├── KeyTipManager.h
    │   │       │   │   ├── LayoutCycleDebugSettings.h
    │   │       │   │   ├── layoutelement.h
    │   │       │   │   ├── LayoutManager.h
    │   │       │   │   ├── LayoutStorage.h
    │   │       │   │   ├── layouttransition.h
    │   │       │   │   ├── LayoutTransitionElement.h
    │   │       │   │   ├── LeaveParams.h
    │   │       │   │   ├── line.h
    │   │       │   │   ├── LineInfo.h
    │   │       │   │   ├── ListViewBaseItem.h
    │   │       │   │   ├── ListViewBaseItemChrome.h
    │   │       │   │   ├── ListViewBaseItemSecondaryChrome.h
    │   │       │   │   ├── ListViewItemChrome.h
    │   │       │   │   ├── LoadedImageSourceLoadCompletedEventArgs.h
    │   │       │   │   ├── LoadedImageSurface.h
    │   │       │   │   ├── LosingFocusEventArgs.h
    │   │       │   │   ├── ManagedObjectReference.h
    │   │       │   │   ├── ManagedTypeInfoProvider.h
    │   │       │   │   ├── ManipulationCompletedEventArgs.h
    │   │       │   │   ├── ManipulationDelta.h
    │   │       │   │   ├── ManipulationDeltaEventArgs.h
    │   │       │   │   ├── ManipulationEventArgs.h
    │   │       │   │   ├── ManipulationInertiaStartingEventArgs.h
    │   │       │   │   ├── ManipulationPivot.h
    │   │       │   │   ├── ManipulationStartedEventArgs.h
    │   │       │   │   ├── ManipulationStartingEventArgs.h
    │   │       │   │   ├── ManipulationVelocities.h
    │   │       │   │   ├── MarkupExtension.h
    │   │       │   │   ├── Matrix3DProjection.h
    │   │       │   │   ├── MatrixTransform.h
    │   │       │   │   ├── MaxTextureSizeProvider.h
    │   │       │   │   ├── mediabase.h
    │   │       │   │   ├── MediaQueue.h
    │   │       │   │   ├── memorysurface.h
    │   │       │   │   ├── MenuFlyout.h
    │   │       │   │   ├── MenuFlyoutItemBaseCollection.h
    │   │       │   │   ├── MenuFlyoutSubItem.h
    │   │       │   │   ├── MePullParser.h
    │   │       │   │   ├── MeScanner.h
    │   │       │   │   ├── MetadataAPI.h
    │   │       │   │   ├── ModifiedValue.h
    │   │       │   │   ├── MultiParentShareableDependencyObject.h
    │   │       │   │   ├── NativeTypeInfoProvider.h
    │   │       │   │   ├── NavigationEventArgs.h
    │   │       │   │   ├── networkingutilities.h
    │   │       │   │   ├── NetworkStatusEventArgs.h
    │   │       │   │   ├── NodeStreamCache.h
    │   │       │   │   ├── NoFocusCandidateFoundEventArgs.h
    │   │       │   │   ├── NoParentShareableDependencyObject.h
    │   │       │   │   ├── NullExtension.h
    │   │       │   │   ├── NullKeyedResource.h
    │   │       │   │   ├── ObjectAnimationUsingKeyFrames.h
    │   │       │   │   ├── ObjectKeyFrame.h
    │   │       │   │   ├── ObjectWriter.h
    │   │       │   │   ├── ObjectWriterCallbacksTemplateParentSetter.h
    │   │       │   │   ├── ObjectWriterCommonRuntime.h
    │   │       │   │   ├── ObjectWriterContext.h
    │   │       │   │   ├── ObjectWriterErrorService.h
    │   │       │   │   ├── ObjectWriterFrame.h
    │   │       │   │   ├── ObjectWriterNode.h
    │   │       │   │   ├── ObjectWriterNodeList.h
    │   │       │   │   ├── ObjectWriterNodeType.h
    │   │       │   │   ├── ObjectWriterRuntime.h
    │   │       │   │   ├── ObjectWriterRuntimeEncoder.h
    │   │       │   │   ├── ObjectWriterSettings.h
    │   │       │   │   ├── ObjectWriterStack.h
    │   │       │   │   ├── PALFontAndScriptServices.h
    │   │       │   │   ├── panel.h
    │   │       │   │   ├── panelex.h
    │   │       │   │   ├── ParallelTimeline.h
    │   │       │   │   ├── ParametricCurve.h
    │   │       │   │   ├── ParserErrorEventArgs.h
    │   │       │   │   ├── ParserErrorService.h
    │   │       │   │   ├── ParserSettings.h
    │   │       │   │   ├── ParserTypedefs.h
    │   │       │   │   ├── path.h
    │   │       │   │   ├── PCRenderDataList.h
    │   │       │   │   ├── perspectiveplane.h
    │   │       │   │   ├── PlaneProjection.h
    │   │       │   │   ├── PointAnimation.h
    │   │       │   │   ├── Pointer.h
    │   │       │   │   ├── PointerAnimationUsingKeyFrames.h
    │   │       │   │   ├── PointerCollection.h
    │   │       │   │   ├── pointereventargs.h
    │   │       │   │   ├── PointerKeyFrame.h
    │   │       │   │   ├── PointHitTestGeometrySink.h
    │   │       │   │   ├── PointHitTestHelper.h
    │   │       │   │   ├── PointKeyFrame.h
    │   │       │   │   ├── polygon.h
    │   │       │   │   ├── PolygonHitTestGeometrySink.h
    │   │       │   │   ├── PolygonHitTestHelper.h
    │   │       │   │   ├── polyline.h
    │   │       │   │   ├── Popup.h
    │   │       │   │   ├── PrintDocument.h
    │   │       │   │   ├── PrintPageEventArgs.h
    │   │       │   │   ├── PrintRoot.h
    │   │       │   │   ├── Projection.h
    │   │       │   │   ├── PropertyChangedParams.h
    │   │       │   │   ├── PropertyKind.h
    │   │       │   │   ├── PropertySetListener.h
    │   │       │   │   ├── RangeBase.h
    │   │       │   │   ├── RateChangedRoutedEventArgs.h
    │   │       │   │   ├── rectangle.h
    │   │       │   │   ├── RelativePanel.h
    │   │       │   │   ├── RenderData.h
    │   │       │   │   ├── RenderedEventArgs.h
    │   │       │   │   ├── RenderingEventArgs.h
    │   │       │   │   ├── RenderParams.h
    │   │       │   │   ├── RenderStateListener.h
    │   │       │   │   ├── RenderTargetBitmap.h
    │   │       │   │   ├── rendertargetbitmapmgr.h
    │   │       │   │   ├── RenderTargetBitmapRoot.h
    │   │       │   │   ├── RenderTargetBitmapWaitExecutor.h
    │   │       │   │   ├── RenderTargetElement.h
    │   │       │   │   ├── rendertypes.h
    │   │       │   │   ├── RenderWalkType.h
    │   │       │   │   ├── RepeatBehavior.h
    │   │       │   │   ├── RepeatBehaviorVO.h
    │   │       │   │   ├── Request.h
    │   │       │   │   ├── Resources.h
    │   │       │   │   ├── RichTextBlock.h
    │   │       │   │   ├── RichTextBlockAutomationPeer.h
    │   │       │   │   ├── RichTextBlockOverflow.h
    │   │       │   │   ├── RichTextBlockOverflowAutomationPeer.h
    │   │       │   │   ├── RichTextServicesHelper.h
    │   │       │   │   ├── RightTappedEventArgs.h
    │   │       │   │   ├── RootVisual.h
    │   │       │   │   ├── RotateTransform.h
    │   │       │   │   ├── RoutedEventArgs.h
    │   │       │   │   ├── runtimeErrorEventArgs.h
    │   │       │   │   ├── SavedContext.h
    │   │       │   │   ├── ScaleTransform.h
    │   │       │   │   ├── ScrollContentControl.h
    │   │       │   │   ├── ScrollViewer.h
    │   │       │   │   ├── segment.h
    │   │       │   │   ├── SemanticZoom.h
    │   │       │   │   ├── Setter.h
    │   │       │   │   ├── SetterBase.h
    │   │       │   │   ├── SetValueParams.h
    │   │       │   │   ├── Shadow.h
    │   │       │   │   ├── shape.h
    │   │       │   │   ├── ShareableDependencyObject.h
    │   │       │   │   ├── simple.h
    │   │       │   │   ├── SimplePropertiesCommon.g.h
    │   │       │   │   ├── SizeChangedEventArgs.h
    │   │       │   │   ├── SizeUtil.h
    │   │       │   │   ├── SkewTransform.h
    │   │       │   │   ├── SolidColorBrush.h
    │   │       │   │   ├── sort.h
    │   │       │   │   ├── SplitView.h
    │   │       │   │   ├── SplitViewPaneClosingEventArgs.h
    │   │       │   │   ├── SplitViewTemplateSettings.h
    │   │       │   │   ├── StackPanel.h
    │   │       │   │   ├── StaggerFunctions.h
    │   │       │   │   ├── StateTrigger.h
    │   │       │   │   ├── StateTriggerBase.h
    │   │       │   │   ├── storyboard.h
    │   │       │   │   ├── StoryboardCollection.h
    │   │       │   │   ├── Style.h
    │   │       │   │   ├── SurfaceImageSource.h
    │   │       │   │   ├── SvgImageSourceFailedEventArgs.h
    │   │       │   │   ├── SvgImageSourceOpenedEventArgs.h
    │   │       │   │   ├── SwapChainBackgroundPanel.h
    │   │       │   │   ├── SwapChainElement.h
    │   │       │   │   ├── SwapChainPanel.h
    │   │       │   │   ├── SwapChainPanelOwner.h
    │   │       │   │   ├── TappedEventArgs.h
    │   │       │   │   ├── TargetPropertyPath.h
    │   │       │   │   ├── Template.h
    │   │       │   │   ├── templatebindingdata.h
    │   │       │   │   ├── TemplateBindingExtension.h
    │   │       │   │   ├── TemplateContent.h
    │   │       │   │   ├── TemplateNamescope.h
    │   │       │   │   ├── TextBlock.h
    │   │       │   │   ├── TextBlockAutomationPeer.h
    │   │       │   │   ├── TextChangedEventArgs.h
    │   │       │   │   ├── TextCompositionEventArgs.h
    │   │       │   │   ├── TextContainer.h
    │   │       │   │   ├── TextControlCopyingToClipboardEventArgs.h
    │   │       │   │   ├── TextControlCuttingToClipboardEventArgs.h
    │   │       │   │   ├── TextControlPasteEventArgs.h
    │   │       │   │   ├── TextElement.h
    │   │       │   │   ├── TextElementCollection.h
    │   │       │   │   ├── TextElementTreeCollection.h
    │   │       │   │   ├── TextNavigationHelper.h
    │   │       │   │   ├── TextPointerWrapper.h
    │   │       │   │   ├── TextProvider.h
    │   │       │   │   ├── TextRangeProvider.h
    │   │       │   │   ├── TextSelection.h
    │   │       │   │   ├── TextSelectionNotify.h
    │   │       │   │   ├── TextView.h
    │   │       │   │   ├── ThemeResourceExtension.h
    │   │       │   │   ├── ThemeShadow.h
    │   │       │   │   ├── tilebrush.h
    │   │       │   │   ├── TiledSurface.h
    │   │       │   │   ├── Timeline.h
    │   │       │   │   ├── TimelineCollection.h
    │   │       │   │   ├── TimelineGroup.h
    │   │       │   │   ├── timemgr.h
    │   │       │   │   ├── timer.h
    │   │       │   │   ├── timespan.h
    │   │       │   │   ├── TimingCollection.h
    │   │       │   │   ├── TouchableRectangle.h
    │   │       │   │   ├── Transform.h
    │   │       │   │   ├── TransformCollection.h
    │   │       │   │   ├── TransformGeometrySink.h
    │   │       │   │   ├── TransformGroup.h
    │   │       │   │   ├── transforms.h
    │   │       │   │   ├── TransitionCollection.h
    │   │       │   │   ├── TransitionRoot.h
    │   │       │   │   ├── TransitionTarget.h
    │   │       │   │   ├── TranslateTransform.h
    │   │       │   │   ├── triggers.h
    │   │       │   │   ├── type.h
    │   │       │   │   ├── TypeTable.g.h
    │   │       │   │   ├── UIAPatternProvider.h
    │   │       │   │   ├── UIATextRange.h
    │   │       │   │   ├── UIDMContainer.h
    │   │       │   │   ├── UIDMContainerHandler.h
    │   │       │   │   ├── uielement.h
    │   │       │   │   ├── UIElementStructs.h
    │   │       │   │   ├── UIThreadScheduler.h
    │   │       │   │   ├── UriValidator.h
    │   │       │   │   ├── values.h
    │   │       │   │   ├── Viewbox.h
    │   │       │   │   ├── VirtualSurfaceimageSource.h
    │   │       │   │   ├── VisualStateChangedEventArgs.h
    │   │       │   │   ├── VisualStateCollection.h
    │   │       │   │   ├── VisualStateGroup.h
    │   │       │   │   ├── VisualStateManager.h
    │   │       │   │   ├── VisualTransition.h
    │   │       │   │   ├── VisualTransitionCollection.h
    │   │       │   │   ├── VisualTransitionCompletedData.h
    │   │       │   │   ├── VisualTree.h
    │   │       │   │   ├── WinBluePropertyTypeCompatHelper.h
    │   │       │   │   ├── WriteableBitmap.h
    │   │       │   │   ├── XamlAssembly.h
    │   │       │   │   ├── XamlBinaryFormatCommon.h
    │   │       │   │   ├── XamlBinaryFormatReader.h
    │   │       │   │   ├── xamlbinaryformatreader2.h
    │   │       │   │   ├── XamlBinaryFormatStringConverter.h
    │   │       │   │   ├── xamlbinaryformatsubreader2.h
    │   │       │   │   ├── xamlbinaryformatsubwriter2.h
    │   │       │   │   ├── XamlBinaryFormatValidator.h
    │   │       │   │   ├── XamlBinaryFormatWriter.h
    │   │       │   │   ├── XamlBinaryFormatWriter2.h
    │   │       │   │   ├── XamlBinaryMetadata.h
    │   │       │   │   ├── XamlBinaryMetadataReader.h
    │   │       │   │   ├── XamlBinaryMetadataReader2.h
    │   │       │   │   ├── XamlBinaryMetadataStore.h
    │   │       │   │   ├── XamlCompositionBrush.h
    │   │       │   │   ├── XamlContext.h
    │   │       │   │   ├── XamlDirectives.h
    │   │       │   │   ├── XamlFactoryKind.h
    │   │       │   │   ├── XamlIslandRoot.h
    │   │       │   │   ├── XamlIslandRootCollection.h
    │   │       │   │   ├── xamlmanagedruntime.h
    │   │       │   │   ├── XamlName.h
    │   │       │   │   ├── XamlNamespace.h
    │   │       │   │   ├── XamlNativeRuntime.h
    │   │       │   │   ├── XamlNode.h
    │   │       │   │   ├── XamlNodeStreamValidator.h
    │   │       │   │   ├── XamlNodeType.h
    │   │       │   │   ├── XamlOptimizedNodeList.h
    │   │       │   │   ├── XamlParser.h
    │   │       │   │   ├── XamlParserContext.h
    │   │       │   │   ├── XamlParserIncludes.h
    │   │       │   │   ├── XamlParserState.h
    │   │       │   │   ├── XamlPredicate.h
    │   │       │   │   ├── XamlProperty.h
    │   │       │   │   ├── XamlPropertyName.h
    │   │       │   │   ├── XamlPropertyToken.h
    │   │       │   │   ├── XamlPullParser.h
    │   │       │   │   ├── XamlQualifiedName.h
    │   │       │   │   ├── XamlQualifiedObject.h
    │   │       │   │   ├── XamlReader.h
    │   │       │   │   ├── XamlRuntime.h
    │   │       │   │   ├── XamlScanner.h
    │   │       │   │   ├── XamlScannerNode.h
    │   │       │   │   ├── XamlScannerStack.h
    │   │       │   │   ├── XamlSchemaContext.h
    │   │       │   │   ├── XamlSerializationHelper.h
    │   │       │   │   ├── XamlServiceProviderContext.h
    │   │       │   │   ├── XamlSortedAttributes.h
    │   │       │   │   ├── XamlSpecialXmlNamespace.h
    │   │       │   │   ├── XamlText.h
    │   │       │   │   ├── XamlTextReader.h
    │   │       │   │   ├── XamlTextReaderSettings.h
    │   │       │   │   ├── XamlTextSyntax.h
    │   │       │   │   ├── XamlToken.h
    │   │       │   │   ├── XamlType.h
    │   │       │   │   ├── XamlTypeInfoProvider.h
    │   │       │   │   ├── XamlTypeInfoProviderKind.h
    │   │       │   │   ├── XamlTypeName.h
    │   │       │   │   ├── XamlTypeNamespace.h
    │   │       │   │   ├── XamlTypeTokens.h
    │   │       │   │   ├── XamlUnknownXmlNamespace.h
    │   │       │   │   ├── XamlWriter.h
    │   │       │   │   ├── xamlxmlnamespace.h
    │   │       │   │   ├── XbfWriter.h
    │   │       │   │   └── xcptypes.h
    │   │       │   ├── input/
    │   │       │   │   ├── BringIntoViewHandler.cpp
    │   │       │   │   ├── CharacterReceivedEventArgs.cpp
    │   │       │   │   ├── CKeyboardAccelerator.cpp
    │   │       │   │   ├── CKeyboardAcceleratorInvokedEventArgs.cpp
    │   │       │   │   ├── DMContent.cpp
    │   │       │   │   ├── DMDeferredRelease.cpp
    │   │       │   │   ├── DMViewport.cpp
    │   │       │   │   ├── FocusedElementRemovedEventArgs.cpp
    │   │       │   │   ├── FocusManagerGotFocusEventArgs.cpp
    │   │       │   │   ├── FocusManagerLostFocusEventArgs.cpp
    │   │       │   │   ├── FrameworkInputViewHandler.cpp
    │   │       │   │   ├── GettingFocusEventArgs.cpp
    │   │       │   │   ├── Input.vcxproj
    │   │       │   │   ├── InputManagerDMViewportEventHandler.cpp
    │   │       │   │   ├── InputPaneHandler.cpp
    │   │       │   │   ├── InputPointEventArgs.cpp
    │   │       │   │   ├── InputServices.cpp
    │   │       │   │   ├── InteractionManager.cpp
    │   │       │   │   ├── KeyboardEventArgs.cpp
    │   │       │   │   ├── KeyTipManager.cpp
    │   │       │   │   ├── LosingFocusEventArgs.cpp
    │   │       │   │   ├── ManipulationEventArgs.cpp
    │   │       │   │   ├── NoFocusCandidateFoundEventArgs.cpp
    │   │       │   │   ├── ParametricCurve.cpp
    │   │       │   │   ├── PointerEventArgs.cpp
    │   │       │   │   ├── precomp.h
    │   │       │   │   └── RoutedEventArgs.cpp
    │   │       │   ├── layout/
    │   │       │   │   ├── EffectiveViewportChangedEventArgs.cpp
    │   │       │   │   ├── LayoutManager.cpp
    │   │       │   │   └── LayoutStorage.cpp
    │   │       │   ├── metadata/
    │   │       │   │   ├── Activators.g.cpp
    │   │       │   │   ├── dirs.proj
    │   │       │   │   ├── DynamicMetadata.g.cpp
    │   │       │   │   ├── ReflectionAPI.cpp
    │   │       │   │   ├── SimplePropertiesCommon.g.cpp
    │   │       │   │   └── dynamic/
    │   │       │   │       ├── dynamicmetadata.vcxproj
    │   │       │   │       └── precomp.h
    │   │       │   ├── native/
    │   │       │   │   ├── elements/
    │   │       │   │   │   ├── image.cpp
    │   │       │   │   │   └── PrintDocument.cpp
    │   │       │   │   ├── inc/
    │   │       │   │   │   ├── AgileCallback.h
    │   │       │   │   │   ├── core_media_native.h
    │   │       │   │   │   ├── image.h
    │   │       │   │   │   ├── MediaPlayerElement.h
    │   │       │   │   │   ├── MediaPlayerExtensions.h
    │   │       │   │   │   ├── MediaPlayerPresenter.h
    │   │       │   │   │   └── PowerModeRequestor.h
    │   │       │   │   ├── media/
    │   │       │   │   │   ├── mediaengine.vcxproj
    │   │       │   │   │   ├── MediaPlayerElement.cpp
    │   │       │   │   │   ├── MediaPlayerExtensions.cpp
    │   │       │   │   │   ├── MediaPlayerPresenter.cpp
    │   │       │   │   │   ├── PowerModeRequestor.cpp
    │   │       │   │   │   └── precomp.h
    │   │       │   │   └── text/
    │   │       │   │       ├── Common/
    │   │       │   │       │   ├── D2DTextDrawingContext.cpp
    │   │       │   │       │   ├── D2DTextDrawingContext.h
    │   │       │   │       │   ├── Native.Text.Common.vcxproj
    │   │       │   │       │   ├── precomp.h
    │   │       │   │       │   ├── SharedWicBitmap.cpp
    │   │       │   │       │   ├── SharedWicBitmap.h
    │   │       │   │       │   ├── TextHelpers.cpp
    │   │       │   │       │   ├── TextHelpers.h
    │   │       │   │       │   ├── WinTextCore.cpp
    │   │       │   │       │   └── WinTextCore.h
    │   │       │   │       └── Controls/
    │   │       │   │           ├── HWRenderTarget.cpp
    │   │       │   │           ├── HWRenderTarget.h
    │   │       │   │           ├── HWSolidColorBrush.cpp
    │   │       │   │           ├── HWSolidColorBrush.h
    │   │       │   │           ├── HWStrokeStyle.cpp
    │   │       │   │           ├── HWStrokeStyle.h
    │   │       │   │           ├── HwTextBitmap.cpp
    │   │       │   │           ├── HwTextBitmap.h
    │   │       │   │           ├── LinguisticsHelper.cpp
    │   │       │   │           ├── LinguisticsHelper.h
    │   │       │   │           ├── Native.Text.Controls.vcxproj
    │   │       │   │           ├── PasswordBox.cpp
    │   │       │   │           ├── PasswordBox.h
    │   │       │   │           ├── PasswordBoxAutomationPeer.cpp
    │   │       │   │           ├── PasswordBoxAutomationPeer.h
    │   │       │   │           ├── precomp.h
    │   │       │   │           ├── PrivateTextInputSettings.cpp
    │   │       │   │           ├── PrivateTextInputSettings.h
    │   │       │   │           ├── RichEditBox.cpp
    │   │       │   │           ├── RichEditBox.h
    │   │       │   │           ├── RichEditBoxAutomationPeer.cpp
    │   │       │   │           ├── RichEditBoxAutomationPeer.h
    │   │       │   │           ├── RichEditOleCallback.cpp
    │   │       │   │           ├── RichEditOleCallback.h
    │   │       │   │           ├── RichEditPal.h
    │   │       │   │           ├── RichTextBlockCommandHandler.cpp
    │   │       │   │           ├── RichTextBlockCommandHandler.h
    │   │       │   │           ├── TextBlockCommandHandler.cpp
    │   │       │   │           ├── TextBlockCommandHandler.h
    │   │       │   │           ├── TextBox.cpp
    │   │       │   │           ├── TextBox.h
    │   │       │   │           ├── TextBoxAutomationPeer.cpp
    │   │       │   │           ├── TextBoxAutomationPeer.h
    │   │       │   │           ├── TextBoxBase.h
    │   │       │   │           ├── TextBoxBaseAutomationPeer.cpp
    │   │       │   │           ├── TextBoxBaseAutomationPeer.h
    │   │       │   │           ├── TextBoxCommandHandler.cpp
    │   │       │   │           ├── TextBoxCommandHandler.h
    │   │       │   │           ├── TextBoxUIManagerEventSink.cpp
    │   │       │   │           ├── TextBoxUIManagerEventSink.h
    │   │       │   │           ├── TextBoxView.cpp
    │   │       │   │           ├── TextBoxView.h
    │   │       │   │           ├── TextContextMenu.cpp
    │   │       │   │           ├── TextContextMenu.h
    │   │       │   │           ├── TextContextMenuCommandHandler.cpp
    │   │       │   │           ├── TextContextMenuCommandHandler.h
    │   │       │   │           ├── TextControlsPinvokes.cpp
    │   │       │   │           ├── TextServicesHost.h
    │   │       │   │           ├── Util.cpp
    │   │       │   │           └── Util.h
    │   │       │   ├── networking/
    │   │       │   │   └── networkingutilities.cpp
    │   │       │   ├── optional/
    │   │       │   │   └── elements/
    │   │       │   │       ├── printing/
    │   │       │   │       │   ├── printpageeventargs.cpp
    │   │       │   │       │   └── printroot.cpp
    │   │       │   │       └── touch/
    │   │       │   │           ├── UIDMContainer.cpp
    │   │       │   │           └── UIDMContainerHandler.cpp
    │   │       │   ├── packaging/
    │   │       │   │   ├── application.cpp
    │   │       │   │   └── deployment.cpp
    │   │       │   ├── Parser/
    │   │       │   │   ├── binaryformatobjectwriter.cpp
    │   │       │   │   ├── CollectionInitializationStringParser.cpp
    │   │       │   │   ├── CollectionInitializationStringParser.h
    │   │       │   │   ├── DeferringWriter.cpp
    │   │       │   │   ├── LineInfo.cpp
    │   │       │   │   ├── ManagedTypeInfoProvider.cpp
    │   │       │   │   ├── MePullParser.cpp
    │   │       │   │   ├── MeScanner.cpp
    │   │       │   │   ├── NativeTypeInfoProvider.cpp
    │   │       │   │   ├── NodeStreamCache.cpp
    │   │       │   │   ├── ObjectWriter.cpp
    │   │       │   │   ├── ObjectWriterCallbacksTemplateParentSetter.cpp
    │   │       │   │   ├── ObjectWriterCommonRuntime.cpp
    │   │       │   │   ├── objectwritercontext.cpp
    │   │       │   │   ├── ObjectWriterErrorService.cpp
    │   │       │   │   ├── ObjectWriterFrame.cpp
    │   │       │   │   ├── ObjectWriterNode.cpp
    │   │       │   │   ├── objectwriternodelist.cpp
    │   │       │   │   ├── ObjectWriterRuntime.cpp
    │   │       │   │   ├── ObjectWriterRuntimeEncoder.cpp
    │   │       │   │   ├── ObjectWriterRuntimeFactory.cpp
    │   │       │   │   ├── ObjectWriterRuntimeFactory.h
    │   │       │   │   ├── ObjectWriterStack.cpp
    │   │       │   │   ├── parser.cpp
    │   │       │   │   ├── ParserErrorService.cpp
    │   │       │   │   ├── ParserStringConstants.cpp
    │   │       │   │   ├── ParserStringConstants.h
    │   │       │   │   ├── savedcontext.cpp
    │   │       │   │   ├── sources.props
    │   │       │   │   ├── StableXbfIndexes.g.h
    │   │       │   │   ├── StableXbfIndexMapping.g.cpp
    │   │       │   │   ├── WinBluePropertyTypeCompatHelper.cpp
    │   │       │   │   ├── XamlAssembly.cpp
    │   │       │   │   ├── XamlBinaryFileAccessFactories.cpp
    │   │       │   │   ├── XamlBinaryFileAccessFactories.h
    │   │       │   │   ├── XamlBinaryFormatReader.cpp
    │   │       │   │   ├── XamlBinaryFormatReader2.cpp
    │   │       │   │   ├── XamlBinaryFormatStringConverter.cpp
    │   │       │   │   ├── xamlbinaryformatsubreader2.cpp
    │   │       │   │   ├── XamlBinaryFormatSubWriter2.cpp
    │   │       │   │   ├── XamlBinaryFormatValidator.cpp
    │   │       │   │   ├── XamlBinaryFormatWriter.cpp
    │   │       │   │   ├── XamlBinaryFormatWriter2.cpp
    │   │       │   │   ├── XamlBinaryMetadataReader.cpp
    │   │       │   │   ├── XamlBinaryMetadataReader2.cpp
    │   │       │   │   ├── XamlBinaryMetadataStore.cpp
    │   │       │   │   ├── XamlContext.cpp
    │   │       │   │   ├── xamlmanagedruntime.cpp
    │   │       │   │   ├── XamlName.cpp
    │   │       │   │   ├── XamlNamespace.cpp
    │   │       │   │   ├── XamlNativeRuntime.cpp
    │   │       │   │   ├── XamlNativeRuntime_SimpleProperties.g.h
    │   │       │   │   ├── XamlNode.cpp
    │   │       │   │   ├── XamlNodeStreamValidator.cpp
    │   │       │   │   ├── XamlOptimizedNodeList.cpp
    │   │       │   │   ├── XamlParserContext.cpp
    │   │       │   │   ├── XamlParserState.cpp
    │   │       │   │   ├── XamlPredicateService.cpp
    │   │       │   │   ├── XamlProperty.cpp
    │   │       │   │   ├── XamlPropertyName.cpp
    │   │       │   │   ├── XamlPullParser.cpp
    │   │       │   │   ├── XamlQualifiedName.cpp
    │   │       │   │   ├── XamlQualifiedObject.cpp
    │   │       │   │   ├── XamlReader.cpp
    │   │       │   │   ├── XamlScanner.cpp
    │   │       │   │   ├── XamlScannerNode.cpp
    │   │       │   │   ├── XamlScannerStack.cpp
    │   │       │   │   ├── XamlSchemaContext.cpp
    │   │       │   │   ├── XamlSchemaContextRuntime.cpp
    │   │       │   │   ├── XamlServiceProviderContext.cpp
    │   │       │   │   ├── XamlSortedAttributes.cpp
    │   │       │   │   ├── XamlSpecialXmlNamespace.cpp
    │   │       │   │   ├── XamlText.cpp
    │   │       │   │   ├── XamlTextReader.cpp
    │   │       │   │   ├── XamlTextReaderSettings.cpp
    │   │       │   │   ├── XamlType.cpp
    │   │       │   │   ├── XamlTypeName.cpp
    │   │       │   │   ├── XamlTypeNamespace.cpp
    │   │       │   │   ├── XamlTypeTokens.cpp
    │   │       │   │   ├── XamlUnknownXmlNamespace.cpp
    │   │       │   │   ├── XamlWriter.cpp
    │   │       │   │   ├── XamlXmlNamespace.cpp
    │   │       │   │   ├── XbfMetadataApi.cpp
    │   │       │   │   ├── XbfMetadataApi.h
    │   │       │   │   ├── XbfWriter.cpp
    │   │       │   │   ├── core/
    │   │       │   │   │   └── Parser.Core.vcxproj
    │   │       │   │   ├── pch/
    │   │       │   │   │   ├── Parser.pch.vcxproj
    │   │       │   │   │   └── precomp.h
    │   │       │   │   ├── runtime/
    │   │       │   │   │   └── Parser.Runtime.vcxproj
    │   │       │   │   ├── staticcore/
    │   │       │   │   │   └── Parser.Core.Static.vcxproj
    │   │       │   │   └── staticpch/
    │   │       │   │       ├── Parser.pch.vcxproj
    │   │       │   │       └── precomp.h
    │   │       │   └── text/
    │   │       │       ├── coretext.vcxproj
    │   │       │       ├── precomp.h
    │   │       │       ├── BlockLayout/
    │   │       │       │   ├── BlockLayoutEngine.cpp
    │   │       │       │   ├── BlockLayoutEngine.h
    │   │       │       │   ├── BlockLayoutHelpers.cpp
    │   │       │       │   ├── BlockLayoutHelpers.h
    │   │       │       │   ├── BlockNode.cpp
    │   │       │       │   ├── BlockNode.h
    │   │       │       │   ├── BlockNodeBreak.cpp
    │   │       │       │   ├── BlockNodeBreak.h
    │   │       │       │   ├── ContainerDrawingContext.cpp
    │   │       │       │   ├── ContainerDrawingContext.h
    │   │       │       │   ├── ContainerNode.cpp
    │   │       │       │   ├── ContainerNode.h
    │   │       │       │   ├── DrawingContext.cpp
    │   │       │       │   ├── DrawingContext.h
    │   │       │       │   ├── LineMetrics.h
    │   │       │       │   ├── PageHostedObjectRun.cpp
    │   │       │       │   ├── PageHostedObjectRun.h
    │   │       │       │   ├── PageNode.cpp
    │   │       │       │   ├── PageNode.h
    │   │       │       │   ├── PageNodeBreak.cpp
    │   │       │       │   ├── PageNodeBreak.h
    │   │       │       │   ├── ParagraphDrawingContext.cpp
    │   │       │       │   ├── ParagraphDrawingContext.h
    │   │       │       │   ├── ParagraphNode.cpp
    │   │       │       │   ├── ParagraphNode.h
    │   │       │       │   ├── ParagraphNodeBreak.cpp
    │   │       │       │   ├── ParagraphNodeBreak.h
    │   │       │       │   ├── ParagraphTextSource.cpp
    │   │       │       │   └── ParagraphTextSource.h
    │   │       │       ├── Classification/
    │   │       │       │   ├── UcdData.bin
    │   │       │       │   ├── UcdData.h
    │   │       │       │   ├── UcdLookup.cpp
    │   │       │       │   ├── UcdProperties.h
    │   │       │       │   └── build/
    │   │       │       │       ├── UcdData.cpp
    │   │       │       │       └── UcdDataToCpp.pl
    │   │       │       ├── common/
    │   │       │       │   ├── BlockCollection.cpp
    │   │       │       │   ├── CaretBrowsingGlobal.cpp
    │   │       │       │   ├── chash.cpp
    │   │       │       │   ├── FocusRectangle.cpp
    │   │       │       │   ├── Gripper.cpp
    │   │       │       │   ├── InheritedProperties.cpp
    │   │       │       │   ├── InputProcessor.cpp
    │   │       │       │   ├── JupiterTextHelper.cpp
    │   │       │       │   ├── RichEditGripper.cpp
    │   │       │       │   ├── RichEditGripperChild.cpp
    │   │       │       │   ├── SelectionWordBreaker.cpp
    │   │       │       │   ├── text.cpp
    │   │       │       │   ├── textadapter.cpp
    │   │       │       │   ├── TextCore.cpp
    │   │       │       │   ├── TextFormatting.cpp
    │   │       │       │   ├── TextNavigationHelper.cpp
    │   │       │       │   ├── TextOptions.cpp
    │   │       │       │   ├── TextPosition.cpp
    │   │       │       │   ├── textrangeadapter.cpp
    │   │       │       │   ├── TextSelectionManager.cpp
    │   │       │       │   ├── TextSelectionSettings.cpp
    │   │       │       │   ├── Typography.cpp
    │   │       │       │   └── XcpTextGripperInputProcessor.cpp
    │   │       │       ├── Fonts/
    │   │       │       │   ├── CompositeFontFamily.cpp
    │   │       │       │   ├── FontFamily.cpp
    │   │       │       │   ├── FontTypeface.cpp
    │   │       │       │   ├── SharedName.cpp
    │   │       │       │   └── TypefaceCollection.cpp
    │   │       │       ├── Inc/
    │   │       │       │   ├── DWriteTextRenderer.h
    │   │       │       │   ├── DWriteTypes.h
    │   │       │       │   ├── DynamicArray.h
    │   │       │       │   ├── EmbeddedElementHost.h
    │   │       │       │   ├── FocusRectangle.h
    │   │       │       │   ├── Fonts.h
    │   │       │       │   ├── Gripper.h
    │   │       │       │   ├── InlineUIContainer.h
    │   │       │       │   ├── InputProcessor.h
    │   │       │       │   ├── ITextSelection.h
    │   │       │       │   ├── LineMetricsCache.h
    │   │       │       │   ├── LinkedRichTextBlockView.h
    │   │       │       │   ├── PlainTextPosition.h
    │   │       │       │   ├── RichEditGripper.h
    │   │       │       │   ├── RichEditGripperChild.h
    │   │       │       │   ├── RichEditGripperCommon.h
    │   │       │       │   ├── RichTextBlockBreak.h
    │   │       │       │   ├── RichTextBlockView.h
    │   │       │       │   ├── SelectionWordBreaker.h
    │   │       │       │   ├── Span.h
    │   │       │       │   ├── text.h
    │   │       │       │   ├── TextAdapter.h
    │   │       │       │   ├── TextBlockView.h
    │   │       │       │   ├── TextBoxHelpers.h
    │   │       │       │   ├── TextPosition.h
    │   │       │       │   ├── TextRangeAdapter.h
    │   │       │       │   ├── TextSchema.h
    │   │       │       │   ├── TextSelectionManager.h
    │   │       │       │   ├── TextSelectionSettings.h
    │   │       │       │   ├── TouchSelectionSnappingCalculator.h
    │   │       │       │   ├── TypefaceCollection.h
    │   │       │       │   └── XcpTextGripperInputProcessor.h
    │   │       │       ├── RichTextArea/
    │   │       │       │   ├── LineMetricsCache.cpp
    │   │       │       │   ├── paragraph.cpp
    │   │       │       │   ├── RichTextServicesHelper.cpp
    │   │       │       │   ├── TextElement.cpp
    │   │       │       │   ├── TextElementCollection.cpp
    │   │       │       │   ├── TextPointerWrapper.cpp
    │   │       │       │   └── TextSchema.cpp
    │   │       │       ├── RichTextBlock/
    │   │       │       │   ├── LinkedRichTextBlockView.cpp
    │   │       │       │   ├── RichTextBlock.cpp
    │   │       │       │   ├── RichTextBlockBreak.cpp
    │   │       │       │   ├── RichTextBlockOverflow.cpp
    │   │       │       │   └── RichTextBlockView.cpp
    │   │       │       ├── RichTextServices/
    │   │       │       │   ├── inc/
    │   │       │       │   │   ├── BlockLayout.h
    │   │       │       │   │   ├── CharacterHit.h
    │   │       │       │   │   ├── DirectionalControl.h
    │   │       │       │   │   ├── DirectionalControlRun.h
    │   │       │       │   │   ├── ElementType.h
    │   │       │       │   │   ├── EndOfLineRun.h
    │   │       │       │   │   ├── EndOfParagraphRun.h
    │   │       │       │   │   ├── FlowDirection.h
    │   │       │       │   │   ├── HiddenRun.h
    │   │       │       │   │   ├── ILayoutEngineHost.h
    │   │       │       │   │   ├── ILinkedTextContainer.h
    │   │       │       │   │   ├── ITextElement.h
    │   │       │       │   │   ├── LayoutNodeType.h
    │   │       │       │   │   ├── LineFormatter.h
    │   │       │       │   │   ├── LinkedContainer.h
    │   │       │       │   │   ├── LogicalDirection.h
    │   │       │       │   │   ├── ObjectRun.h
    │   │       │       │   │   ├── ObjectRunMetrics.h
    │   │       │       │   │   ├── Result.h
    │   │       │       │   │   ├── RtsInterop.h
    │   │       │       │   │   ├── TextAlignment.h
    │   │       │       │   │   ├── TextBounds.h
    │   │       │       │   │   ├── TextBreak.h
    │   │       │       │   │   ├── TextCharactersRun.h
    │   │       │       │   │   ├── TextCollapsingCharacters.h
    │   │       │       │   │   ├── TextCollapsingSymbol.h
    │   │       │       │   │   ├── TextDrawingContext.h
    │   │       │       │   │   ├── TextFormatter.h
    │   │       │       │   │   ├── TextFormatterCache.h
    │   │       │       │   │   ├── TextLine.h
    │   │       │       │   │   ├── TextLineBreak.h
    │   │       │       │   │   ├── TextObject.h
    │   │       │       │   │   ├── TextParagraphProperties.h
    │   │       │       │   │   ├── TextRun.h
    │   │       │       │   │   ├── TextRunCache.h
    │   │       │       │   │   ├── TextRunProperties.h
    │   │       │       │   │   ├── TextRunType.h
    │   │       │       │   │   └── TextSource.h
    │   │       │       │   ├── inci/
    │   │       │       │   │   ├── CharacterProperties.h
    │   │       │       │   │   ├── CharacterRunCollection.h
    │   │       │       │   │   ├── CharacterRunNode.h
    │   │       │       │   │   ├── CountedCharacterRunCollection.h
    │   │       │       │   │   ├── LineBreaking.h
    │   │       │       │   │   ├── Ls.h
    │   │       │       │   │   ├── SplayTreeBase.h
    │   │       │       │   │   ├── SplayTreeCollection.h
    │   │       │       │   │   ├── SplayTreeNode.h
    │   │       │       │   │   ├── TxMath.h
    │   │       │       │   │   └── TxPal.h
    │   │       │       │   ├── shared/
    │   │       │       │   │   ├── CharacterRunCollection.cpp
    │   │       │       │   │   ├── CharacterRunNode.cpp
    │   │       │       │   │   ├── CountedCharacterRunCollection.cpp
    │   │       │       │   │   ├── SplayTreeCollection.cpp
    │   │       │       │   │   ├── SplayTreeNode.cpp
    │   │       │       │   │   ├── TextBreak.cpp
    │   │       │       │   │   └── TextObject.cpp
    │   │       │       │   ├── TextFormatter/
    │   │       │       │   │   ├── DirectionalControlRun.cpp
    │   │       │       │   │   ├── EndOfLineRun.cpp
    │   │       │       │   │   ├── EndOfParagraphRun.cpp
    │   │       │       │   │   ├── HiddenRun.cpp
    │   │       │       │   │   ├── InlineObjectHandlers.cpp
    │   │       │       │   │   ├── InlineObjectHandlers.h
    │   │       │       │   │   ├── lineservicescallbacks.cpp
    │   │       │       │   │   ├── LineServicesCallbacks.h
    │   │       │       │   │   ├── LsClient.cpp
    │   │       │       │   │   ├── LsClient.h
    │   │       │       │   │   ├── LsHostContext.cpp
    │   │       │       │   │   ├── LsHostContext.h
    │   │       │       │   │   ├── LsParagraphSpan.cpp
    │   │       │       │   │   ├── LsParagraphSpan.h
    │   │       │       │   │   ├── LsRun.cpp
    │   │       │       │   │   ├── LsRun.h
    │   │       │       │   │   ├── LsRunCache.cpp
    │   │       │       │   │   ├── LsRunCache.h
    │   │       │       │   │   ├── LsSpan.cpp
    │   │       │       │   │   ├── LsSpan.h
    │   │       │       │   │   ├── LsTextFormatter.cpp
    │   │       │       │   │   ├── LsTextFormatter.h
    │   │       │       │   │   ├── LsTextLine.cpp
    │   │       │       │   │   ├── LsTextLine.h
    │   │       │       │   │   ├── LsTextLineBreak.cpp
    │   │       │       │   │   ├── LsTextLineBreak.h
    │   │       │       │   │   ├── ObjectRun.cpp
    │   │       │       │   │   ├── sources.props
    │   │       │       │   │   ├── TextAnalysisNode.h
    │   │       │       │   │   ├── TextCharactersRun.cpp
    │   │       │       │   │   ├── TextCollapsingCharacters.cpp
    │   │       │       │   │   ├── TextDpi.h
    │   │       │       │   │   ├── TextFormatter.cpp
    │   │       │       │   │   ├── TextFormatterCache.cpp
    │   │       │       │   │   ├── TextItemizer.cpp
    │   │       │       │   │   ├── TextItemizer.h
    │   │       │       │   │   ├── TextLine.cpp
    │   │       │       │   │   ├── TextParagraphProperties.cpp
    │   │       │       │   │   ├── TextRun.cpp
    │   │       │       │   │   ├── TextRunCache.cpp
    │   │       │       │   │   ├── TextRunData.cpp
    │   │       │       │   │   ├── TextRunData.h
    │   │       │       │   │   ├── TextRunProperties.cpp
    │   │       │       │   │   ├── TextSegment.cpp
    │   │       │       │   │   ├── TextSegment.h
    │   │       │       │   │   ├── TextStore.cpp
    │   │       │       │   │   └── TextStore.h
    │   │       │       │   ├── UnicodeData/
    │   │       │       │   │   ├── CharacterProperties.cpp
    │   │       │       │   │   └── LineBreaking.cpp
    │   │       │       │   └── xcp/
    │   │       │       │       ├── PALFontAndScriptServices.cpp
    │   │       │       │       ├── TxUtil.cpp
    │   │       │       │       └── TxUtil.h
    │   │       │       ├── shaping/
    │   │       │       │   └── inc/
    │   │       │       │       └── ShapingTypes.h
    │   │       │       ├── TextBlock/
    │   │       │       │   ├── CRun.cpp
    │   │       │       │   ├── DWriteTextRenderer.cpp
    │   │       │       │   ├── Hyperlink.cpp
    │   │       │       │   ├── Inline.cpp
    │   │       │       │   ├── InlineCollection.cpp
    │   │       │       │   ├── LineBreak.cpp
    │   │       │       │   ├── TextBlock.cpp
    │   │       │       │   └── TextBlockView.cpp
    │   │       │       ├── TextBox/
    │   │       │       │   ├── PlainTextPosition.cpp
    │   │       │       │   ├── TextBoxHelpers.cpp
    │   │       │       │   └── TextSelection.cpp
    │   │       │       └── TextLayout/
    │   │       │           └── InlineUIContainer.cpp
    │   │       ├── dxaml/
    │   │       │   ├── dirs.proj
    │   │       │   ├── dllsrv/
    │   │       │   │   ├── exts/
    │   │       │   │   │   ├── module.cpp
    │   │       │   │   │   ├── sources.props
    │   │       │   │   │   └── phone/
    │   │       │   │   │       ├── CreatorMap.inl
    │   │       │   │   │       ├── exports.cpp
    │   │       │   │   │       ├── Microsoft.UI.Xaml.Phone.def
    │   │       │   │   │       ├── Microsoft.UI.Xaml.Phone.rc
    │   │       │   │   │       ├── Microsoft.UI.Xaml.Phone.vcxproj
    │   │       │   │   │       ├── XamlTypeInfo.cpp
    │   │       │   │   │       ├── XamlTypeInfo.g.cpp
    │   │       │   │   │       ├── XamlTypeInfo.g.h
    │   │       │   │   │       └── XamlTypeInfo.g.rc
    │   │       │   │   └── winrt/
    │   │       │   │       ├── dirs.proj
    │   │       │   │       ├── Microsoft.UI.Xaml.Common.rc
    │   │       │   │       ├── Microsoft.UI.Xaml.def
    │   │       │   │       ├── precomp.h
    │   │       │   │       ├── sources.props
    │   │       │   │       ├── native/
    │   │       │   │       │   ├── Microsoft.ui.xaml.vcxproj
    │   │       │   │       │   └── themeresources.rc
    │   │       │   │       └── res/
    │   │       │   │           ├── dirs.proj
    │   │       │   │           ├── sources.props
    │   │       │   │           ├── 19h1/
    │   │       │   │           │   ├── Microsoft.UI.Xaml.19H1.rc
    │   │       │   │           │   └── Microsoft.ui.xaml.resources.19h1.vcxproj
    │   │       │   │           └── common/
    │   │       │   │               ├── Microsoft.ui.xaml.resources.common.vcxproj
    │   │       │   │               └── Microsoft.UI.Xaml.Resources.rc
    │   │       │   ├── lib/
    │   │       │   │   ├── AccessKeyEvents.h
    │   │       │   │   ├── AddPagesEventArgs_Partial.cpp
    │   │       │   │   ├── AppBar_Partial.cpp
    │   │       │   │   ├── AutomationElementIdentifiers.h
    │   │       │   │   ├── BindingExpressionBase_Partial.h
    │   │       │   │   ├── CalendarDatePickerAutomationPeer_Partial.h
    │   │       │   │   ├── CalendarPanel_Partial.h
    │   │       │   │   ├── CalendarView_Partial.h
    │   │       │   │   ├── CalendarViewDayItemAutomationPeer_Partial.h
    │   │       │   │   ├── CalendarViewDayItemChangingEventArgs_Partial.cpp
    │   │       │   │   ├── CascadingMenuHelper.cpp
    │   │       │   │   ├── CheckBoxAutomationPeer_Partial.h
    │   │       │   │   ├── CollectionViewGroup_Partial.h
    │   │       │   │   ├── CollectionViewSource_Partial.h
    │   │       │   │   ├── ComboBoxItemAutomationPeer_Partial.cpp
    │   │       │   │   ├── ComboBoxItemDataAutomationPeer_Partial.cpp
    │   │       │   │   ├── CommandBarOverflowPresenter_Partial.cpp
    │   │       │   │   ├── ContentControl_Partial.cpp
    │   │       │   │   ├── ContentDialogClosingEventArgs_Partial.h
    │   │       │   │   ├── ContentManager.cpp
    │   │       │   │   ├── ContentPresenter_Partial.h
    │   │       │   │   ├── ContextMenuEventArgs_Partial.cpp
    │   │       │   │   ├── DeferralManager.h
    │   │       │   │   ├── DependencyObjectCollection_Partial.cpp
    │   │       │   │   ├── DependencyObjectPropertyAccess.h
    │   │       │   │   ├── DependencyPropertyChangedEventArgs_Partial.h
    │   │       │   │   ├── DesktopWindowImpl.h
    │   │       │   │   ├── DesktopWindowXamlSource_Partial.cpp
    │   │       │   │   ├── DirectConnectedAnimationConfiguration_partial.cpp
    │   │       │   │   ├── DispatcherTimer_Partial.cpp
    │   │       │   │   ├── DisplayOrientationHelper.cpp
    │   │       │   │   ├── DragEventArgs_Partial.cpp
    │   │       │   │   ├── DragEventArgs_Partial.h
    │   │       │   │   ├── DragOperationDeferral_partial.h
    │   │       │   │   ├── DragOverThemeAnimation_Partial.h
    │   │       │   │   ├── DragUIOverride_Partial.cpp
    │   │       │   │   ├── DragUIOverride_Partial.h
    │   │       │   │   ├── EffectiveValueEntry.h
    │   │       │   │   ├── FaceplateContentPresenterAutomationPeer_partial.h
    │   │       │   │   ├── FlyoutBase_partial.cpp
    │   │       │   │   ├── FlyoutShowOptions_partial.h
    │   │       │   │   ├── FocusAsyncOperation.h
    │   │       │   │   ├── Frame_Partial.cpp
    │   │       │   │   ├── GridViewHeaderItem_Partial.h
    │   │       │   │   ├── GridViewItemAutomationPeer_Partial.cpp
    │   │       │   │   ├── GridViewItemDataAutomationPeer_partial.h
    │   │       │   │   ├── GridViewItemPresenter_Partial.cpp
    │   │       │   │   ├── GroupedDataCollectionView_Partial.h
    │   │       │   │   ├── GroupStyle_Partial.cpp
    │   │       │   │   ├── HubSectionCollection_Partial.cpp
    │   │       │   │   ├── HyperLinkButton_Partial.h
    │   │       │   │   ├── InlineUIContainer_Partial.cpp
    │   │       │   │   ├── INPCListenerBase.cpp
    │   │       │   │   ├── InputScopeNameFactory.cpp
    │   │       │   │   ├── InternalStringCollection.cpp
    │   │       │   │   ├── IsPropertyPresent_Partial.h
    │   │       │   │   ├── IsTypeNotPresent_Partial.h
    │   │       │   │   ├── ItemInvokeAdapter_Partial.cpp
    │   │       │   │   ├── ItemInvokeAdapter_Partial.h
    │   │       │   │   ├── ItemsStackPanel_Partial.cpp
    │   │       │   │   ├── IterableCollectionView_Partial.cpp
    │   │       │   │   ├── JoltInternalInterfaces.h
    │   │       │   │   ├── KeyboardAccelerator_Partial.cpp
    │   │       │   │   ├── ListBoxItemDataAutomationPeer_Partial.cpp
    │   │       │   │   ├── ListViewBase_Partial_Selection.cpp
    │   │       │   │   ├── ListViewBaseHeaderItem_Partial.cpp
    │   │       │   │   ├── ListViewHeaderItem_Partial.h
    │   │       │   │   ├── ListViewHeaderItemAutomationPeer_Partial.cpp
    │   │       │   │   ├── ListViewHeaderItemAutomationPeer_Partial.h
    │   │       │   │   ├── ListViewItemDataAutomationPeer_Partial.cpp
    │   │       │   │   ├── MapPropertyAccess.cpp
    │   │       │   │   ├── MapPropertyAccess.h
    │   │       │   │   ├── MediaPlayerPresenter_partial.cpp
    │   │       │   │   ├── MenuFlyout_Partial.h
    │   │       │   │   ├── MenuFlyoutItemAutomationPeer_Partial.cpp
    │   │       │   │   ├── MenuFlyoutItemAutomationPeer_Partial.h
    │   │       │   │   ├── MenuFlyoutPresenter_Partial.cpp
    │   │       │   │   ├── MenuFlyoutPresenterAutomationPeer_Partial.cpp
    │   │       │   │   ├── ModernCollectionBasePanel_CacheManager_Partial.cpp
    │   │       │   │   ├── ModernCollectionBasePanel_Partial.cpp
    │   │       │   │   ├── NavigationHistory.cpp
    │   │       │   │   ├── Page_Partial.cpp
    │   │       │   │   ├── PaginateEventArgs_Partial.cpp
    │   │       │   │   ├── PathIconSource_Partial.cpp
    │   │       │   │   ├── PointerRoutedEventArgs_Partial.cpp
    │   │       │   │   ├── PopupRoot_Partial.cpp
    │   │       │   │   ├── PopupThemeTransition_Partial.h
    │   │       │   │   ├── PropertyMetadata_Partial.cpp
    │   │       │   │   ├── PropertyPath.cpp
    │   │       │   │   ├── ProvideValueTargetProperty_Partial.cpp
    │   │       │   │   ├── RangeBase_Partial.h
    │   │       │   │   ├── RepeatButton_Partial.h
    │   │       │   │   ├── ScalarTransition_Partial.cpp
    │   │       │   │   ├── ScrollContentPresenter_Partial.h
    │   │       │   │   ├── ScrollEventArgs_Partial.h
    │   │       │   │   ├── ScrollItemAdapter_Partial.cpp
    │   │       │   │   ├── ScrollViewer_Partial.cpp
    │   │       │   │   ├── SectionsInViewChangedEventArgs_Partial.h
    │   │       │   │   ├── Selection.cpp
    │   │       │   │   ├── SelectorItem_Partial.cpp
    │   │       │   │   ├── SemanticZoomAutomationPeer_Partial.h
    │   │       │   │   ├── Setter_Partial.cpp
    │   │       │   │   ├── Shape_Partial.cpp
    │   │       │   │   ├── StartDragAsyncOperation.h
    │   │       │   │   ├── StateTriggerBase_Partial.h
    │   │       │   │   ├── StickyHeaderWrapper.cpp
    │   │       │   │   ├── TextControlHelper.h
    │   │       │   │   ├── ThemeShadow_Partial.cpp
    │   │       │   │   ├── ThemeShadow_Partial.h
    │   │       │   │   ├── ToggleButton_Partial.cpp
    │   │       │   │   ├── ToggleButtonAutomationPeer_Partial.h
    │   │       │   │   ├── ToggleSwitchAutomationPeer_Partial.h
    │   │       │   │   ├── Transition_Partial.h
    │   │       │   │   ├── UIElementWeakCollection_Partial.cpp
    │   │       │   │   ├── ValidationErrorsObservableVectorWrapper.cpp
    │   │       │   │   ├── Vector3Transition_Partial.cpp
    │   │       │   │   ├── VectorViewCollectionView_Partial.h
    │   │       │   │   ├── VisualTreeHelper.cpp
    │   │       │   │   ├── WindowChrome_Partial.cpp
    │   │       │   │   ├── WindowsXamlManager_Partial.cpp
    │   │       │   │   ├── WriteableBitmap_Partial.cpp
    │   │       │   │   ├── XamlIslandRoot_Partial.h
    │   │       │   │   ├── XamlShutdownCompletedOnThreadEventArgs_Partial.h
    │   │       │   │   ├── XamlSourceFocusNavigationRequest_Partial.h
    │   │       │   │   ├── XamlUICommand_Partial.h
    │   │       │   │   ├── xbfxamltypewrapper.cpp
    │   │       │   │   ├── winrtautomation/
    │   │       │   │   │   └── wrtdxamlautomation.vcxproj
    │   │       │   │   ├── winrtcontrols/
    │   │       │   │   │   └── wrtdxamlcontrols.vcxproj
    │   │       │   │   ├── winrtcontrols2/
    │   │       │   │   │   └── wrtdxamlcontrols2.vcxproj
    │   │       │   │   └── winrtgeneratedclasses/
    │   │       │   │       ├── AccessKeyDisplayDismissedEventArgs.g.cpp
    │   │       │   │       ├── AccessKeyDisplayDismissedEventArgs.g.h
    │   │       │   │       ├── AccessKeyDisplayRequestedEventArgs.g.cpp
    │   │       │   │       ├── AccessKeyDisplayRequestedEventArgs.g.h
    │   │       │   │       ├── AccessKeyInvokedEventArgs.g.cpp
    │   │       │   │       ├── AccessKeyInvokedEventArgs.g.h
    │   │       │   │       ├── AccessKeyManager.g.cpp
    │   │       │   │       ├── AccessKeyManager.g.h
    │   │       │   │       ├── AdaptiveTrigger.g.cpp
    │   │       │   │       ├── AdaptiveTrigger.g.h
    │   │       │   │       ├── AddDeleteThemeTransition.g.cpp
    │   │       │   │       ├── AddDeleteThemeTransition.g.h
    │   │       │   │       ├── AddPagesEventArgs.g.cpp
    │   │       │   │       ├── AddPagesEventArgs.g.h
    │   │       │   │       ├── Aggregate.g.cpp
    │   │       │   │       ├── AnchorRequestedEventArgs.g.cpp
    │   │       │   │       ├── AnchorRequestedEventArgs.g.h
    │   │       │   │       ├── AppBar.g.cpp
    │   │       │   │       ├── AppBar.g.h
    │   │       │   │       ├── AppBarAutomationPeer.g.cpp
    │   │       │   │       ├── AppBarAutomationPeer.g.h
    │   │       │   │       ├── AppBarButton.g.cpp
    │   │       │   │       ├── AppBarButton.g.h
    │   │       │   │       ├── AppBarButtonAutomationPeer.g.cpp
    │   │       │   │       ├── AppBarButtonAutomationPeer.g.h
    │   │       │   │       ├── AppBarButtonTemplateSettings.g.cpp
    │   │       │   │       ├── AppBarButtonTemplateSettings.g.h
    │   │       │   │       ├── AppBarElementContainer.g.cpp
    │   │       │   │       ├── AppBarElementContainer.g.h
    │   │       │   │       ├── AppBarLightDismiss.g.cpp
    │   │       │   │       ├── AppBarLightDismiss.g.h
    │   │       │   │       ├── AppBarLightDismissAutomationPeer.g.cpp
    │   │       │   │       ├── AppBarLightDismissAutomationPeer.g.h
    │   │       │   │       ├── AppBarSeparator.g.cpp
    │   │       │   │       ├── AppBarSeparator.g.h
    │   │       │   │       ├── AppBarTemplateSettings.g.cpp
    │   │       │   │       ├── AppBarTemplateSettings.g.h
    │   │       │   │       ├── AppBarToggleButton.g.cpp
    │   │       │   │       ├── AppBarToggleButton.g.h
    │   │       │   │       ├── AppBarToggleButtonAutomationPeer.g.cpp
    │   │       │   │       ├── AppBarToggleButtonAutomationPeer.g.h
    │   │       │   │       ├── AppBarToggleButtonTemplateSettings.g.cpp
    │   │       │   │       ├── AppBarToggleButtonTemplateSettings.g.h
    │   │       │   │       ├── ApplicationBarService.g.cpp
    │   │       │   │       ├── ApplicationBarService.g.h
    │   │       │   │       ├── ApplicationInitializationCallbackParams.g.cpp
    │   │       │   │       ├── ApplicationInitializationCallbackParams.g.h
    │   │       │   │       ├── ArcSegment.g.cpp
    │   │       │   │       ├── ArcSegment.g.h
    │   │       │   │       ├── AutomationAnnotation.g.cpp
    │   │       │   │       ├── AutomationAnnotation.g.h
    │   │       │   │       ├── AutomationAnnotationCollection.g.cpp
    │   │       │   │       ├── AutomationAnnotationCollection.g.h
    │   │       │   │       ├── AutomationPeer.g.cpp
    │   │       │   │       ├── AutomationPeer.g.h
    │   │       │   │       ├── AutomationPeerAnnotation.g.cpp
    │   │       │   │       ├── AutomationPeerAnnotation.g.h
    │   │       │   │       ├── AutomationPeerAnnotationCollection.g.cpp
    │   │       │   │       ├── AutomationPeerAnnotationCollection.g.h
    │   │       │   │       ├── AutomationPeerCollection.g.cpp
    │   │       │   │       ├── AutomationPeerCollection.g.h
    │   │       │   │       ├── AutomationPeerEventArgs.g.cpp
    │   │       │   │       ├── AutomationPeerEventArgs.g.h
    │   │       │   │       ├── AutomationProperty.g.cpp
    │   │       │   │       ├── AutomationProperty.g.h
    │   │       │   │       ├── AutoSuggestBox.g.cpp
    │   │       │   │       ├── AutoSuggestBox.g.h
    │   │       │   │       ├── AutoSuggestBoxAutomationPeer.g.cpp
    │   │       │   │       ├── AutoSuggestBoxAutomationPeer.g.h
    │   │       │   │       ├── AutoSuggestBoxQuerySubmittedEventArgs.g.cpp
    │   │       │   │       ├── AutoSuggestBoxQuerySubmittedEventArgs.g.h
    │   │       │   │       ├── AutoSuggestBoxSuggestionChosenEventArgs.g.cpp
    │   │       │   │       ├── AutoSuggestBoxSuggestionChosenEventArgs.g.h
    │   │       │   │       ├── AutoSuggestBoxTextChangedEventArgs.g.cpp
    │   │       │   │       ├── AutoSuggestBoxTextChangedEventArgs.g.h
    │   │       │   │       ├── BackEase.g.cpp
    │   │       │   │       ├── BackEase.g.h
    │   │       │   │       ├── BasedOnSetterCollection.g.cpp
    │   │       │   │       ├── BasedOnSetterCollection.g.h
    │   │       │   │       ├── BasicConnectedAnimationConfiguration.g.cpp
    │   │       │   │       ├── BasicConnectedAnimationConfiguration.g.h
    │   │       │   │       ├── BeginPrintEventArgs.g.cpp
    │   │       │   │       ├── BeginPrintEventArgs.g.h
    │   │       │   │       ├── BeginStoryboard.g.cpp
    │   │       │   │       ├── BeginStoryboard.g.h
    │   │       │   │       ├── BezierSegment.g.cpp
    │   │       │   │       ├── BezierSegment.g.h
    │   │       │   │       ├── Binding.g.cpp
    │   │       │   │       ├── Binding.g.h
    │   │       │   │       ├── BindingBase.g.cpp
    │   │       │   │       ├── BindingBase.g.h
    │   │       │   │       ├── BindingExpression.g.cpp
    │   │       │   │       ├── BindingExpression.g.h
    │   │       │   │       ├── BindingExpressionBase.g.cpp
    │   │       │   │       ├── BindingExpressionBase.g.h
    │   │       │   │       ├── BindingFailedEventArgs.g.cpp
    │   │       │   │       ├── BindingFailedEventArgs.g.h
    │   │       │   │       ├── BitmapCache.g.cpp
    │   │       │   │       ├── BitmapCache.g.h
    │   │       │   │       ├── BitmapIcon.g.cpp
    │   │       │   │       ├── BitmapIcon.g.h
    │   │       │   │       ├── BitmapIconSource.g.cpp
    │   │       │   │       ├── BitmapIconSource.g.h
    │   │       │   │       ├── BitmapImage.g.cpp
    │   │       │   │       ├── BitmapImage.g.h
    │   │       │   │       ├── BitmapSource.g.cpp
    │   │       │   │       ├── BitmapSource.g.h
    │   │       │   │       ├── Block.g.cpp
    │   │       │   │       ├── Block.g.h
    │   │       │   │       ├── BlockCollection.g.cpp
    │   │       │   │       ├── BlockCollection.g.h
    │   │       │   │       ├── Bold.g.cpp
    │   │       │   │       ├── Bold.g.h
    │   │       │   │       ├── Border.g.cpp
    │   │       │   │       ├── Border.g.h
    │   │       │   │       ├── BounceEase.g.cpp
    │   │       │   │       ├── BounceEase.g.h
    │   │       │   │       ├── Boxes.g.cpp
    │   │       │   │       ├── BringIntoViewOptions.g.cpp
    │   │       │   │       ├── BringIntoViewOptions.g.h
    │   │       │   │       ├── BringIntoViewRequestedEventArgs.g.cpp
    │   │       │   │       ├── BringIntoViewRequestedEventArgs.g.h
    │   │       │   │       ├── Brush.g.cpp
    │   │       │   │       ├── Brush.g.h
    │   │       │   │       ├── BrushCollection.g.cpp
    │   │       │   │       ├── BrushCollection.g.h
    │   │       │   │       ├── BrushTransition.g.cpp
    │   │       │   │       ├── BrushTransition.g.h
    │   │       │   │       ├── BudgetManager.g.cpp
    │   │       │   │       ├── BudgetManager.g.h
    │   │       │   │       ├── BuildTreeService.g.cpp
    │   │       │   │       ├── BuildTreeService.g.h
    │   │       │   │       ├── Button.g.cpp
    │   │       │   │       ├── Button.g.h
    │   │       │   │       ├── ButtonAutomationPeer.g.cpp
    │   │       │   │       ├── ButtonAutomationPeer.g.h
    │   │       │   │       ├── ButtonBase.g.cpp
    │   │       │   │       ├── ButtonBase.g.h
    │   │       │   │       ├── ButtonBaseAutomationPeer.g.cpp
    │   │       │   │       ├── ButtonBaseAutomationPeer.g.h
    │   │       │   │       ├── CacheMode.g.cpp
    │   │       │   │       ├── CacheMode.g.h
    │   │       │   │       ├── CalendarDatePicker.g.cpp
    │   │       │   │       ├── CalendarDatePicker.g.h
    │   │       │   │       ├── CalendarDatePickerAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarDatePickerAutomationPeer.g.h
    │   │       │   │       ├── CalendarDatePickerDateChangedEventArgs.g.cpp
    │   │       │   │       ├── CalendarDatePickerDateChangedEventArgs.g.h
    │   │       │   │       ├── CalendarLayoutStrategy.g.cpp
    │   │       │   │       ├── CalendarLayoutStrategy.g.h
    │   │       │   │       ├── CalendarPanel.g.cpp
    │   │       │   │       ├── CalendarPanel.g.h
    │   │       │   │       ├── CalendarScrollViewerAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarScrollViewerAutomationPeer.g.h
    │   │       │   │       ├── CalendarView.g.cpp
    │   │       │   │       ├── CalendarView.g.h
    │   │       │   │       ├── CalendarViewAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarViewAutomationPeer.g.h
    │   │       │   │       ├── CalendarViewBaseItem.g.cpp
    │   │       │   │       ├── CalendarViewBaseItem.g.h
    │   │       │   │       ├── CalendarViewBaseItemAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarViewBaseItemAutomationPeer.g.h
    │   │       │   │       ├── CalendarViewDayItem.g.cpp
    │   │       │   │       ├── CalendarViewDayItem.g.h
    │   │       │   │       ├── CalendarViewDayItemAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarViewDayItemAutomationPeer.g.h
    │   │       │   │       ├── CalendarViewDayItemChangingEventArgs.g.cpp
    │   │       │   │       ├── CalendarViewDayItemChangingEventArgs.g.h
    │   │       │   │       ├── CalendarViewHeaderAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarViewHeaderAutomationPeer.g.h
    │   │       │   │       ├── CalendarViewItem.g.cpp
    │   │       │   │       ├── CalendarViewItem.g.h
    │   │       │   │       ├── CalendarViewItemAutomationPeer.g.cpp
    │   │       │   │       ├── CalendarViewItemAutomationPeer.g.h
    │   │       │   │       ├── CalendarViewSelectedDatesChangedEventArgs.g.cpp
    │   │       │   │       ├── CalendarViewSelectedDatesChangedEventArgs.g.h
    │   │       │   │       ├── CalendarViewTemplateSettings.g.cpp
    │   │       │   │       ├── CalendarViewTemplateSettings.g.h
    │   │       │   │       ├── CandidateWindowBoundsChangedEventArgs.g.cpp
    │   │       │   │       ├── CandidateWindowBoundsChangedEventArgs.g.h
    │   │       │   │       ├── CanExecuteRequestedEventArgs.g.cpp
    │   │       │   │       ├── CanExecuteRequestedEventArgs.g.h
    │   │       │   │       ├── Canvas.g.cpp
    │   │       │   │       ├── Canvas.g.h
    │   │       │   │       ├── CarouselPanel.g.cpp
    │   │       │   │       ├── CarouselPanel.g.h
    │   │       │   │       ├── CharacterReceivedRoutedEventArgs.g.cpp
    │   │       │   │       ├── CharacterReceivedRoutedEventArgs.g.h
    │   │       │   │       ├── CheckBox.g.cpp
    │   │       │   │       ├── CheckBox.g.h
    │   │       │   │       ├── CheckBoxAutomationPeer.g.cpp
    │   │       │   │       ├── CheckBoxAutomationPeer.g.h
    │   │       │   │       ├── ChoosingGroupHeaderContainerEventArgs.g.cpp
    │   │       │   │       ├── ChoosingGroupHeaderContainerEventArgs.g.h
    │   │       │   │       ├── ChoosingItemContainerEventArgs.g.cpp
    │   │       │   │       ├── ChoosingItemContainerEventArgs.g.h
    │   │       │   │       ├── CircleEase.g.cpp
    │   │       │   │       ├── CircleEase.g.h
    │   │       │   │       ├── CleanUpVirtualizedItemEventArgs.g.cpp
    │   │       │   │       ├── CleanUpVirtualizedItemEventArgs.g.h
    │   │       │   │       ├── CollectionView.g.cpp
    │   │       │   │       ├── CollectionView.g.h
    │   │       │   │       ├── CollectionViewGroup.g.cpp
    │   │       │   │       ├── CollectionViewGroup.g.h
    │   │       │   │       ├── CollectionViewSource.g.cpp
    │   │       │   │       ├── CollectionViewSource.g.h
    │   │       │   │       ├── ColorAnimation.g.cpp
    │   │       │   │       ├── ColorAnimation.g.h
    │   │       │   │       ├── ColorAnimationUsingKeyFrames.g.cpp
    │   │       │   │       ├── ColorAnimationUsingKeyFrames.g.h
    │   │       │   │       ├── ColorDisplayNameHelper.g.cpp
    │   │       │   │       ├── ColorDisplayNameHelper.g.h
    │   │       │   │       ├── ColorKeyFrame.g.cpp
    │   │       │   │       ├── ColorKeyFrame.g.h
    │   │       │   │       ├── ColorKeyFrameCollection.g.cpp
    │   │       │   │       ├── ColorKeyFrameCollection.g.h
    │   │       │   │       ├── ColorPaletteResources.g.cpp
    │   │       │   │       ├── ColorPaletteResources.g.h
    │   │       │   │       ├── ColumnDefinition.g.cpp
    │   │       │   │       ├── ColumnDefinition.g.h
    │   │       │   │       ├── ColumnDefinitionCollection.g.cpp
    │   │       │   │       ├── ColumnDefinitionCollection.g.h
    │   │       │   │       ├── ComboBox.g.cpp
    │   │       │   │       ├── ComboBox.g.h
    │   │       │   │       ├── ComboBoxAutomationPeer.g.cpp
    │   │       │   │       ├── ComboBoxAutomationPeer.g.h
    │   │       │   │       ├── ComboBoxItem.g.cpp
    │   │       │   │       ├── ComboBoxItem.g.h
    │   │       │   │       ├── ComboBoxItemAutomationPeer.g.cpp
    │   │       │   │       ├── ComboBoxItemAutomationPeer.g.h
    │   │       │   │       ├── ComboBoxItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── ComboBoxItemDataAutomationPeer.g.h
    │   │       │   │       ├── ComboBoxLightDismiss.g.cpp
    │   │       │   │       ├── ComboBoxLightDismiss.g.h
    │   │       │   │       ├── ComboBoxLightDismissAutomationPeer.g.cpp
    │   │       │   │       ├── ComboBoxLightDismissAutomationPeer.g.h
    │   │       │   │       ├── ComboBoxTemplateSettings.g.cpp
    │   │       │   │       ├── ComboBoxTemplateSettings.g.h
    │   │       │   │       ├── ComboBoxTextSubmittedEventArgs.g.cpp
    │   │       │   │       ├── ComboBoxTextSubmittedEventArgs.g.h
    │   │       │   │       ├── CommandBar.g.cpp
    │   │       │   │       ├── CommandBar.g.h
    │   │       │   │       ├── CommandBarElementCollection.g.cpp
    │   │       │   │       ├── CommandBarElementCollection.g.h
    │   │       │   │       ├── CommandBarOverflowPresenter.g.cpp
    │   │       │   │       ├── CommandBarOverflowPresenter.g.h
    │   │       │   │       ├── CommandBarTemplateSettings.g.cpp
    │   │       │   │       ├── CommandBarTemplateSettings.g.h
    │   │       │   │       ├── CommandingContainer.g.cpp
    │   │       │   │       ├── CommandingContainer.g.h
    │   │       │   │       ├── CommandingContextChangedEventArgs.g.cpp
    │   │       │   │       ├── CommandingContextChangedEventArgs.g.h
    │   │       │   │       ├── CompositeTransform.g.cpp
    │   │       │   │       ├── CompositeTransform.g.h
    │   │       │   │       ├── CompositeTransform3D.g.cpp
    │   │       │   │       ├── CompositeTransform3D.g.h
    │   │       │   │       ├── ConnectedAnimation.g.cpp
    │   │       │   │       ├── ConnectedAnimation.g.h
    │   │       │   │       ├── ConnectedAnimationConfiguration.g.cpp
    │   │       │   │       ├── ConnectedAnimationConfiguration.g.h
    │   │       │   │       ├── ConnectedAnimationRoot.g.cpp
    │   │       │   │       ├── ConnectedAnimationRoot.g.h
    │   │       │   │       ├── ConnectedAnimationService.g.cpp
    │   │       │   │       ├── ConnectedAnimationService.g.h
    │   │       │   │       ├── ContainerContentChangingEventArgs.g.cpp
    │   │       │   │       ├── ContainerContentChangingEventArgs.g.h
    │   │       │   │       ├── ContentControl.g.cpp
    │   │       │   │       ├── ContentControl.g.h
    │   │       │   │       ├── ContentDialog.g.cpp
    │   │       │   │       ├── ContentDialog.g.h
    │   │       │   │       ├── ContentDialogButtonClickDeferral.g.cpp
    │   │       │   │       ├── ContentDialogButtonClickDeferral.g.h
    │   │       │   │       ├── ContentDialogButtonClickEventArgs.g.cpp
    │   │       │   │       ├── ContentDialogButtonClickEventArgs.g.h
    │   │       │   │       ├── ContentDialogClosedEventArgs.g.cpp
    │   │       │   │       ├── ContentDialogClosedEventArgs.g.h
    │   │       │   │       ├── ContentDialogClosingDeferral.g.cpp
    │   │       │   │       ├── ContentDialogClosingDeferral.g.h
    │   │       │   │       ├── ContentDialogClosingEventArgs.g.cpp
    │   │       │   │       ├── ContentDialogClosingEventArgs.g.h
    │   │       │   │       ├── ContentDialogOpenCloseThemeTransition.g.cpp
    │   │       │   │       ├── ContentDialogOpenCloseThemeTransition.g.h
    │   │       │   │       ├── ContentDialogOpenedEventArgs.g.cpp
    │   │       │   │       ├── ContentDialogOpenedEventArgs.g.h
    │   │       │   │       ├── ContentPresenter.g.cpp
    │   │       │   │       ├── ContentPresenter.g.h
    │   │       │   │       ├── ContentThemeTransition.g.cpp
    │   │       │   │       ├── ContentThemeTransition.g.h
    │   │       │   │       ├── ContextMenuEventArgs.g.cpp
    │   │       │   │       ├── ContextMenuEventArgs.g.h
    │   │       │   │       ├── ContextRequestedEventArgs.g.cpp
    │   │       │   │       ├── ContextRequestedEventArgs.g.h
    │   │       │   │       ├── Control.g.cpp
    │   │       │   │       ├── Control.g.h
    │   │       │   │       ├── ControlTemplate.g.cpp
    │   │       │   │       ├── ControlTemplate.g.h
    │   │       │   │       ├── CornerRadius.g.cpp
    │   │       │   │       ├── CornerRadius.g.h
    │   │       │   │       ├── CubicEase.g.cpp
    │   │       │   │       ├── CubicEase.g.h
    │   │       │   │       ├── CurrentChangingEventArgs.g.cpp
    │   │       │   │       ├── CurrentChangingEventArgs.g.h
    │   │       │   │       ├── CustomResource.g.cpp
    │   │       │   │       ├── CustomResource.g.h
    │   │       │   │       ├── CustomXamlResourceLoader.g.cpp
    │   │       │   │       ├── CustomXamlResourceLoader.g.h
    │   │       │   │       ├── DataContextChangedEventArgs.g.cpp
    │   │       │   │       ├── DataContextChangedEventArgs.g.h
    │   │       │   │       ├── DataErrorsChangedEventArgs.g.cpp
    │   │       │   │       ├── DataErrorsChangedEventArgs.g.h
    │   │       │   │       ├── DataTemplate.g.cpp
    │   │       │   │       ├── DataTemplate.g.h
    │   │       │   │       ├── DataTemplateKey.g.cpp
    │   │       │   │       ├── DataTemplateKey.g.h
    │   │       │   │       ├── DataTemplateSelector.g.cpp
    │   │       │   │       ├── DataTemplateSelector.g.h
    │   │       │   │       ├── DatePicker.g.cpp
    │   │       │   │       ├── DatePicker.g.h
    │   │       │   │       ├── DatePickerAutomationPeer.g.cpp
    │   │       │   │       ├── DatePickerAutomationPeer.g.h
    │   │       │   │       ├── DatePickerSelectedValueChangedEventArgs.g.cpp
    │   │       │   │       ├── DatePickerSelectedValueChangedEventArgs.g.h
    │   │       │   │       ├── DatePickerValueChangedEventArgs.g.cpp
    │   │       │   │       ├── DatePickerValueChangedEventArgs.g.h
    │   │       │   │       ├── DebugSettings.g.cpp
    │   │       │   │       ├── DebugSettings.g.h
    │   │       │   │       ├── DeferredElement.g.cpp
    │   │       │   │       ├── DeferredElement.g.h
    │   │       │   │       ├── DependencyObjectCollection.g.cpp
    │   │       │   │       ├── DependencyObjectCollection.g.h
    │   │       │   │       ├── DependencyObjectWrapper.g.cpp
    │   │       │   │       ├── DependencyObjectWrapper.g.h
    │   │       │   │       ├── DependencyPropertyChangedEventArgs.g.cpp
    │   │       │   │       ├── DependencyPropertyChangedEventArgs.g.h
    │   │       │   │       ├── DependencyPropertyProxy.g.cpp
    │   │       │   │       ├── DependencyPropertyProxy.g.h
    │   │       │   │       ├── Deployment.g.cpp
    │   │       │   │       ├── Deployment.g.h
    │   │       │   │       ├── DesktopWindowXamlSource.g.cpp
    │   │       │   │       ├── DesktopWindowXamlSource.g.h
    │   │       │   │       ├── DirectConnectedAnimationConfiguration.g.cpp
    │   │       │   │       ├── DirectConnectedAnimationConfiguration.g.h
    │   │       │   │       ├── DiscreteColorKeyFrame.g.cpp
    │   │       │   │       ├── DiscreteColorKeyFrame.g.h
    │   │       │   │       ├── DiscreteDoubleKeyFrame.g.cpp
    │   │       │   │       ├── DiscreteDoubleKeyFrame.g.h
    │   │       │   │       ├── DiscreteObjectKeyFrame.g.cpp
    │   │       │   │       ├── DiscreteObjectKeyFrame.g.h
    │   │       │   │       ├── DiscretePointKeyFrame.g.cpp
    │   │       │   │       ├── DiscretePointKeyFrame.g.h
    │   │       │   │       ├── DispatcherTimer.g.cpp
    │   │       │   │       ├── DispatcherTimer.g.h
    │   │       │   │       ├── DisplayMemberTemplate.g.cpp
    │   │       │   │       ├── DisplayMemberTemplate.g.h
    │   │       │   │       ├── DoubleAnimation.g.cpp
    │   │       │   │       ├── DoubleAnimation.g.h
    │   │       │   │       ├── DoubleAnimationUsingKeyFrames.g.cpp
    │   │       │   │       ├── DoubleAnimationUsingKeyFrames.g.h
    │   │       │   │       ├── DoubleCollection.g.cpp
    │   │       │   │       ├── DoubleCollection.g.h
    │   │       │   │       ├── DoubleKeyFrame.g.cpp
    │   │       │   │       ├── DoubleKeyFrame.g.h
    │   │       │   │       ├── DoubleKeyFrameCollection.g.cpp
    │   │       │   │       ├── DoubleKeyFrameCollection.g.h
    │   │       │   │       ├── DoubleTappedRoutedEventArgs.g.cpp
    │   │       │   │       ├── DoubleTappedRoutedEventArgs.g.h
    │   │       │   │       ├── DownloadProgressEventArgs.g.cpp
    │   │       │   │       ├── DownloadProgressEventArgs.g.h
    │   │       │   │       ├── DragCompletedEventArgs.g.cpp
    │   │       │   │       ├── DragCompletedEventArgs.g.h
    │   │       │   │       ├── DragDeltaEventArgs.g.cpp
    │   │       │   │       ├── DragDeltaEventArgs.g.h
    │   │       │   │       ├── DragEventArgs.g.cpp
    │   │       │   │       ├── DragEventArgs.g.h
    │   │       │   │       ├── DragItemsCompletedEventArgs.g.cpp
    │   │       │   │       ├── DragItemsCompletedEventArgs.g.h
    │   │       │   │       ├── DragItemsStartingEventArgs.g.cpp
    │   │       │   │       ├── DragItemsStartingEventArgs.g.h
    │   │       │   │       ├── DragItemThemeAnimation.g.cpp
    │   │       │   │       ├── DragItemThemeAnimation.g.h
    │   │       │   │       ├── DragOperationDeferral.g.cpp
    │   │       │   │       ├── DragOperationDeferral.g.h
    │   │       │   │       ├── DragOverThemeAnimation.g.cpp
    │   │       │   │       ├── DragOverThemeAnimation.g.h
    │   │       │   │       ├── DragStartedEventArgs.g.cpp
    │   │       │   │       ├── DragStartedEventArgs.g.h
    │   │       │   │       ├── DragStartingEventArgs.g.cpp
    │   │       │   │       ├── DragStartingEventArgs.g.h
    │   │       │   │       ├── DragUI.g.cpp
    │   │       │   │       ├── DragUI.g.h
    │   │       │   │       ├── DragUIOverride.g.cpp
    │   │       │   │       ├── DragUIOverride.g.h
    │   │       │   │       ├── DrillInThemeAnimation.g.cpp
    │   │       │   │       ├── DrillInThemeAnimation.g.h
    │   │       │   │       ├── DrillOutThemeAnimation.g.cpp
    │   │       │   │       ├── DrillOutThemeAnimation.g.h
    │   │       │   │       ├── DropCompletedEventArgs.g.cpp
    │   │       │   │       ├── DropCompletedEventArgs.g.h
    │   │       │   │       ├── DropTargetItemThemeAnimation.g.cpp
    │   │       │   │       ├── DropTargetItemThemeAnimation.g.h
    │   │       │   │       ├── Duration.g.cpp
    │   │       │   │       ├── Duration.g.h
    │   │       │   │       ├── DxamlCoreTestHooks.g.cpp
    │   │       │   │       ├── DxamlCoreTestHooks.g.h
    │   │       │   │       ├── DynamicOverflowItemsChangingEventArgs.g.cpp
    │   │       │   │       ├── DynamicOverflowItemsChangingEventArgs.g.h
    │   │       │   │       ├── DynamicTimeline.g.cpp
    │   │       │   │       ├── DynamicTimeline.g.h
    │   │       │   │       ├── EasingColorKeyFrame.g.cpp
    │   │       │   │       ├── EasingColorKeyFrame.g.h
    │   │       │   │       ├── EasingDoubleKeyFrame.g.cpp
    │   │       │   │       ├── EasingDoubleKeyFrame.g.h
    │   │       │   │       ├── EasingFunctionBase.g.cpp
    │   │       │   │       ├── EasingFunctionBase.g.h
    │   │       │   │       ├── EasingPointKeyFrame.g.cpp
    │   │       │   │       ├── EasingPointKeyFrame.g.h
    │   │       │   │       ├── EdgeUIThemeTransition.g.cpp
    │   │       │   │       ├── EdgeUIThemeTransition.g.h
    │   │       │   │       ├── EffectiveViewportChangedEventArgs.g.cpp
    │   │       │   │       ├── EffectiveViewportChangedEventArgs.g.h
    │   │       │   │       ├── ElasticEase.g.cpp
    │   │       │   │       ├── ElasticEase.g.h
    │   │       │   │       ├── ElementCompositionPreview.g.cpp
    │   │       │   │       ├── ElementCompositionPreview.g.h
    │   │       │   │       ├── ElementFactoryGetArgs.g.cpp
    │   │       │   │       ├── ElementFactoryGetArgs.g.h
    │   │       │   │       ├── ElementFactoryRecycleArgs.g.cpp
    │   │       │   │       ├── ElementFactoryRecycleArgs.g.h
    │   │       │   │       ├── ElementSoundPlayer.g.cpp
    │   │       │   │       ├── ElementSoundPlayer.g.h
    │   │       │   │       ├── ElementSoundPlayerService.g.cpp
    │   │       │   │       ├── ElementSoundPlayerService.g.h
    │   │       │   │       ├── Ellipse.g.cpp
    │   │       │   │       ├── Ellipse.g.h
    │   │       │   │       ├── EllipseGeometry.g.cpp
    │   │       │   │       ├── EllipseGeometry.g.h
    │   │       │   │       ├── EndPrintEventArgs.g.cpp
    │   │       │   │       ├── EndPrintEventArgs.g.h
    │   │       │   │       ├── EntranceThemeTransition.g.cpp
    │   │       │   │       ├── EntranceThemeTransition.g.h
    │   │       │   │       ├── ErrorEventArgs.g.cpp
    │   │       │   │       ├── ErrorEventArgs.g.h
    │   │       │   │       ├── EventTrigger.g.cpp
    │   │       │   │       ├── EventTrigger.g.h
    │   │       │   │       ├── ExceptionRoutedEventArgs.g.cpp
    │   │       │   │       ├── ExceptionRoutedEventArgs.g.h
    │   │       │   │       ├── ExecuteRequestedEventArgs.g.cpp
    │   │       │   │       ├── ExecuteRequestedEventArgs.g.h
    │   │       │   │       ├── ExponentialEase.g.cpp
    │   │       │   │       ├── ExponentialEase.g.h
    │   │       │   │       ├── ExternalObjectReference.g.cpp
    │   │       │   │       ├── ExternalObjectReference.g.h
    │   │       │   │       ├── FaceplateContentPresenterAutomationPeer.g.cpp
    │   │       │   │       ├── FaceplateContentPresenterAutomationPeer.g.h
    │   │       │   │       ├── FadeInThemeAnimation.g.cpp
    │   │       │   │       ├── FadeInThemeAnimation.g.h
    │   │       │   │       ├── FadeOutThemeAnimation.g.cpp
    │   │       │   │       ├── FadeOutThemeAnimation.g.h
    │   │       │   │       ├── FindNextElementOptions.g.cpp
    │   │       │   │       ├── FindNextElementOptions.g.h
    │   │       │   │       ├── FlipView.g.cpp
    │   │       │   │       ├── FlipView.g.h
    │   │       │   │       ├── FlipViewAutomationPeer.g.cpp
    │   │       │   │       ├── FlipViewAutomationPeer.g.h
    │   │       │   │       ├── FlipViewItem.g.cpp
    │   │       │   │       ├── FlipViewItem.g.h
    │   │       │   │       ├── FlipViewItemAutomationPeer.g.cpp
    │   │       │   │       ├── FlipViewItemAutomationPeer.g.h
    │   │       │   │       ├── FlipViewItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── FlipViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── FloatCollection.g.cpp
    │   │       │   │       ├── FloatCollection.g.h
    │   │       │   │       ├── Flyout.g.cpp
    │   │       │   │       ├── Flyout.g.h
    │   │       │   │       ├── FlyoutBase.g.cpp
    │   │       │   │       ├── FlyoutBase.g.h
    │   │       │   │       ├── FlyoutBaseClosingEventArgs.g.cpp
    │   │       │   │       ├── FlyoutBaseClosingEventArgs.g.h
    │   │       │   │       ├── FlyoutPresenter.g.cpp
    │   │       │   │       ├── FlyoutPresenter.g.h
    │   │       │   │       ├── FlyoutPresenterAutomationPeer.g.cpp
    │   │       │   │       ├── FlyoutPresenterAutomationPeer.g.h
    │   │       │   │       ├── FlyoutShowOptions.g.cpp
    │   │       │   │       ├── FlyoutShowOptions.g.h
    │   │       │   │       ├── FocusDisengagedEventArgs.g.cpp
    │   │       │   │       ├── FocusDisengagedEventArgs.g.h
    │   │       │   │       ├── FocusedElementRemovedEventArgs.g.cpp
    │   │       │   │       ├── FocusedElementRemovedEventArgs.g.h
    │   │       │   │       ├── FocusEngagedEventArgs.g.cpp
    │   │       │   │       ├── FocusEngagedEventArgs.g.h
    │   │       │   │       ├── FocusManager.g.cpp
    │   │       │   │       ├── FocusManager.g.h
    │   │       │   │       ├── FocusManagerGotFocusEventArgs.g.cpp
    │   │       │   │       ├── FocusManagerGotFocusEventArgs.g.h
    │   │       │   │       ├── FocusManagerLostFocusEventArgs.g.cpp
    │   │       │   │       ├── FocusManagerLostFocusEventArgs.g.h
    │   │       │   │       ├── FocusMovementResult.g.cpp
    │   │       │   │       ├── FocusMovementResult.g.h
    │   │       │   │       ├── FontFamily.g.cpp
    │   │       │   │       ├── FontFamily.g.h
    │   │       │   │       ├── FontIcon.g.cpp
    │   │       │   │       ├── FontIcon.g.h
    │   │       │   │       ├── FontIconSource.g.cpp
    │   │       │   │       ├── FontIconSource.g.h
    │   │       │   │       ├── Frame.g.cpp
    │   │       │   │       ├── Frame.g.h
    │   │       │   │       ├── FrameNavigationOptions.g.cpp
    │   │       │   │       ├── FrameNavigationOptions.g.h
    │   │       │   │       ├── FrameworkApplication.g.cpp
    │   │       │   │       ├── FrameworkApplication.g.h
    │   │       │   │       ├── FrameworkElement.g.cpp
    │   │       │   │       ├── FrameworkElement.g.h
    │   │       │   │       ├── FrameworkElementAutomationPeer.g.cpp
    │   │       │   │       ├── FrameworkElementAutomationPeer.g.h
    │   │       │   │       ├── FrameworkElementEx.g.cpp
    │   │       │   │       ├── FrameworkElementEx.g.h
    │   │       │   │       ├── FrameworkTemplate.g.cpp
    │   │       │   │       ├── FrameworkTemplate.g.h
    │   │       │   │       ├── FrameworkView.g.cpp
    │   │       │   │       ├── FrameworkView.g.h
    │   │       │   │       ├── FrameworkViewSource.g.cpp
    │   │       │   │       ├── FrameworkViewSource.g.h
    │   │       │   │       ├── FullWindowMediaRoot.g.cpp
    │   │       │   │       ├── FullWindowMediaRoot.g.h
    │   │       │   │       ├── FullWindowMediaRootAutomationPeer.g.cpp
    │   │       │   │       ├── FullWindowMediaRootAutomationPeer.g.h
    │   │       │   │       ├── GeneralTransform.g.cpp
    │   │       │   │       ├── GeneralTransform.g.h
    │   │       │   │       ├── GeneratorPosition.g.cpp
    │   │       │   │       ├── GeneratorPosition.g.h
    │   │       │   │       ├── Geometry.g.cpp
    │   │       │   │       ├── Geometry.g.h
    │   │       │   │       ├── GeometryCollection.g.cpp
    │   │       │   │       ├── GeometryCollection.g.h
    │   │       │   │       ├── GeometryGroup.g.cpp
    │   │       │   │       ├── GeometryGroup.g.h
    │   │       │   │       ├── GetPreviewPageEventArgs.g.cpp
    │   │       │   │       ├── GetPreviewPageEventArgs.g.h
    │   │       │   │       ├── GettingFocusEventArgs.g.cpp
    │   │       │   │       ├── GettingFocusEventArgs.g.h
    │   │       │   │       ├── Glyphs.g.cpp
    │   │       │   │       ├── Glyphs.g.h
    │   │       │   │       ├── GradientBrush.g.cpp
    │   │       │   │       ├── GradientBrush.g.h
    │   │       │   │       ├── GradientStop.g.cpp
    │   │       │   │       ├── GradientStop.g.h
    │   │       │   │       ├── GradientStopCollection.g.cpp
    │   │       │   │       ├── GradientStopCollection.g.h
    │   │       │   │       ├── GravityConnectedAnimationConfiguration.g.cpp
    │   │       │   │       ├── GravityConnectedAnimationConfiguration.g.h
    │   │       │   │       ├── Grid.g.cpp
    │   │       │   │       ├── Grid.g.h
    │   │       │   │       ├── GridLength.g.cpp
    │   │       │   │       ├── GridLength.g.h
    │   │       │   │       ├── GridView.g.cpp
    │   │       │   │       ├── GridView.g.h
    │   │       │   │       ├── GridViewAutomationPeer.g.cpp
    │   │       │   │       ├── GridViewAutomationPeer.g.h
    │   │       │   │       ├── GridViewHeaderItem.g.cpp
    │   │       │   │       ├── GridViewHeaderItem.g.h
    │   │       │   │       ├── GridViewHeaderItemAutomationPeer.g.cpp
    │   │       │   │       ├── GridViewHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── GridViewItem.g.cpp
    │   │       │   │       ├── GridViewItem.g.h
    │   │       │   │       ├── GridViewItemAutomationPeer.g.cpp
    │   │       │   │       ├── GridViewItemAutomationPeer.g.h
    │   │       │   │       ├── GridViewItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── GridViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── GridViewItemPresenter.g.cpp
    │   │       │   │       ├── GridViewItemPresenter.g.h
    │   │       │   │       ├── GridViewItemTemplateSettings.g.cpp
    │   │       │   │       ├── GridViewItemTemplateSettings.g.h
    │   │       │   │       ├── GroupedDataCollectionView.g.cpp
    │   │       │   │       ├── GroupedDataCollectionView.g.h
    │   │       │   │       ├── GroupItem.g.cpp
    │   │       │   │       ├── GroupItem.g.h
    │   │       │   │       ├── GroupItemAutomationPeer.g.cpp
    │   │       │   │       ├── GroupItemAutomationPeer.g.h
    │   │       │   │       ├── GroupStyle.g.cpp
    │   │       │   │       ├── GroupStyle.g.h
    │   │       │   │       ├── GroupStyleSelector.g.cpp
    │   │       │   │       ├── GroupStyleSelector.g.h
    │   │       │   │       ├── HasValidationErrorsChangedEventArgs.g.cpp
    │   │       │   │       ├── HasValidationErrorsChangedEventArgs.g.h
    │   │       │   │       ├── HoldingRoutedEventArgs.g.cpp
    │   │       │   │       ├── HoldingRoutedEventArgs.g.h
    │   │       │   │       ├── Hub.g.cpp
    │   │       │   │       ├── Hub.g.h
    │   │       │   │       ├── HubAutomationPeer.g.cpp
    │   │       │   │       ├── HubAutomationPeer.g.h
    │   │       │   │       ├── HubSection.g.cpp
    │   │       │   │       ├── HubSection.g.h
    │   │       │   │       ├── HubSectionAutomationPeer.g.cpp
    │   │       │   │       ├── HubSectionAutomationPeer.g.h
    │   │       │   │       ├── HubSectionCollection.g.cpp
    │   │       │   │       ├── HubSectionCollection.g.h
    │   │       │   │       ├── HubSectionHeaderClickEventArgs.g.cpp
    │   │       │   │       ├── HubSectionHeaderClickEventArgs.g.h
    │   │       │   │       ├── HWCompLeafNode.g.cpp
    │   │       │   │       ├── HWCompLeafNode.g.h
    │   │       │   │       ├── HWCompMediaNode.g.cpp
    │   │       │   │       ├── HWCompMediaNode.g.h
    │   │       │   │       ├── HWCompNode.g.cpp
    │   │       │   │       ├── HWCompNode.g.h
    │   │       │   │       ├── HWCompRenderDataNode.g.cpp
    │   │       │   │       ├── HWCompRenderDataNode.g.h
    │   │       │   │       ├── HWCompSwapChainNode.g.cpp
    │   │       │   │       ├── HWCompSwapChainNode.g.h
    │   │       │   │       ├── HWCompTreeNode.g.cpp
    │   │       │   │       ├── HWCompTreeNode.g.h
    │   │       │   │       ├── HWRedirectedCompTreeNodeWinRT.g.cpp
    │   │       │   │       ├── HWRedirectedCompTreeNodeWinRT.g.h
    │   │       │   │       ├── HWWindowedPopupCompTreeNodeWinRT.g.cpp
    │   │       │   │       ├── HWWindowedPopupCompTreeNodeWinRT.g.h
    │   │       │   │       ├── Hyperlink.g.cpp
    │   │       │   │       ├── Hyperlink.g.h
    │   │       │   │       ├── HyperlinkAutomationPeer.g.cpp
    │   │       │   │       ├── HyperlinkAutomationPeer.g.h
    │   │       │   │       ├── HyperlinkButton.g.cpp
    │   │       │   │       ├── HyperlinkButton.g.h
    │   │       │   │       ├── HyperlinkButtonAutomationPeer.g.cpp
    │   │       │   │       ├── HyperlinkButtonAutomationPeer.g.h
    │   │       │   │       ├── HyperlinkClickEventArgs.g.cpp
    │   │       │   │       ├── HyperlinkClickEventArgs.g.h
    │   │       │   │       ├── IChildTransitionContextProvider.g.h
    │   │       │   │       ├── IconElement.g.cpp
    │   │       │   │       ├── IconElement.g.h
    │   │       │   │       ├── IconSource.g.cpp
    │   │       │   │       ├── IconSource.g.h
    │   │       │   │       ├── IconSourceElement.g.cpp
    │   │       │   │       ├── IconSourceElement.g.h
    │   │       │   │       ├── IContainerContentChangingIterator.g.h
    │   │       │   │       ├── IContainerRecyclingContext.g.h
    │   │       │   │       ├── ICustomGeneratorItemsHost.g.h
    │   │       │   │       ├── IDragOperationDeferralTarget.g.h
    │   │       │   │       ├── IGeneratorHost.g.h
    │   │       │   │       ├── IGroupHeaderMapping.g.h
    │   │       │   │       ├── IItemContainerGenerator2.g.h
    │   │       │   │       ├── IItemLookupPanel.g.h
    │   │       │   │       ├── IKeyboardHeaderNavigationPanel.g.h
    │   │       │   │       ├── IKeyboardNavigationPanel.g.h
    │   │       │   │       ├── Image.g.cpp
    │   │       │   │       ├── Image.g.h
    │   │       │   │       ├── ImageAutomationPeer.g.cpp
    │   │       │   │       ├── ImageAutomationPeer.g.h
    │   │       │   │       ├── ImageBrush.g.cpp
    │   │       │   │       ├── ImageBrush.g.h
    │   │       │   │       ├── ImageSource.g.cpp
    │   │       │   │       ├── ImageSource.g.h
    │   │       │   │       ├── InertiaExpansionBehavior.g.cpp
    │   │       │   │       ├── InertiaExpansionBehavior.g.h
    │   │       │   │       ├── InertiaRotationBehavior.g.cpp
    │   │       │   │       ├── InertiaRotationBehavior.g.h
    │   │       │   │       ├── InertiaTranslationBehavior.g.cpp
    │   │       │   │       ├── InertiaTranslationBehavior.g.h
    │   │       │   │       ├── Inline.g.cpp
    │   │       │   │       ├── Inline.g.h
    │   │       │   │       ├── InlineCollection.g.cpp
    │   │       │   │       ├── InlineCollection.g.h
    │   │       │   │       ├── InlineUIContainer.g.cpp
    │   │       │   │       ├── InlineUIContainer.g.h
    │   │       │   │       ├── InputManager.g.cpp
    │   │       │   │       ├── InputManager.g.h
    │   │       │   │       ├── InputPaneThemeTransition.g.cpp
    │   │       │   │       ├── InputPaneThemeTransition.g.h
    │   │       │   │       ├── InputScope.g.cpp
    │   │       │   │       ├── InputScope.g.h
    │   │       │   │       ├── InputScopeName.g.cpp
    │   │       │   │       ├── InputScopeName.g.h
    │   │       │   │       ├── InputScopeNameCollection.g.cpp
    │   │       │   │       ├── InputScopeNameCollection.g.h
    │   │       │   │       ├── InputValidationCommand.g.cpp
    │   │       │   │       ├── InputValidationCommand.g.h
    │   │       │   │       ├── InputValidationContext.g.cpp
    │   │       │   │       ├── InputValidationContext.g.h
    │   │       │   │       ├── InputValidationError.g.cpp
    │   │       │   │       ├── InputValidationError.g.h
    │   │       │   │       ├── InputValidationErrorEventArgs.g.cpp
    │   │       │   │       ├── InputValidationErrorEventArgs.g.h
    │   │       │   │       ├── InteractionBase.g.cpp
    │   │       │   │       ├── InteractionBase.g.h
    │   │       │   │       ├── InternalTransform.g.cpp
    │   │       │   │       ├── InternalTransform.g.h
    │   │       │   │       ├── IOrientedPanel.g.h
    │   │       │   │       ├── IPaginatedPanel.g.h
    │   │       │   │       ├── IRawElementProviderSimple.g.cpp
    │   │       │   │       ├── IRawElementProviderSimple.g.h
    │   │       │   │       ├── IsApiContractNotPresent.g.cpp
    │   │       │   │       ├── IsApiContractNotPresent.g.h
    │   │       │   │       ├── IsApiContractPresent.g.cpp
    │   │       │   │       ├── IsApiContractPresent.g.h
    │   │       │   │       ├── IScrollInfo.g.h
    │   │       │   │       ├── IsEnabledChangedEventArgs.g.cpp
    │   │       │   │       ├── IsEnabledChangedEventArgs.g.h
    │   │       │   │       ├── IsPropertyNotPresent.g.cpp
    │   │       │   │       ├── IsPropertyNotPresent.g.h
    │   │       │   │       ├── IsPropertyPresent.g.cpp
    │   │       │   │       ├── IsPropertyPresent.g.h
    │   │       │   │       ├── IsTextTrimmedChangedEventArgs.g.cpp
    │   │       │   │       ├── IsTextTrimmedChangedEventArgs.g.h
    │   │       │   │       ├── IsTypeNotPresent.g.cpp
    │   │       │   │       ├── IsTypeNotPresent.g.h
    │   │       │   │       ├── IsTypePresent.g.cpp
    │   │       │   │       ├── IsTypePresent.g.h
    │   │       │   │       ├── ISupportInitialize.g.h
    │   │       │   │       ├── Italic.g.cpp
    │   │       │   │       ├── Italic.g.h
    │   │       │   │       ├── ItemAutomationPeer.g.cpp
    │   │       │   │       ├── ItemAutomationPeer.g.h
    │   │       │   │       ├── ItemClickEventArgs.g.cpp
    │   │       │   │       ├── ItemClickEventArgs.g.h
    │   │       │   │       ├── ItemCollection.g.cpp
    │   │       │   │       ├── ItemCollection.g.h
    │   │       │   │       ├── ItemContainerGenerator.g.cpp
    │   │       │   │       ├── ItemContainerGenerator.g.h
    │   │       │   │       ├── ItemIndexRange.g.cpp
    │   │       │   │       ├── ItemIndexRange.g.h
    │   │       │   │       ├── ItemInvokeAdapter.g.cpp
    │   │       │   │       ├── ItemInvokeAdapter.g.h
    │   │       │   │       ├── ItemsChangedEventArgs.g.cpp
    │   │       │   │       ├── ItemsChangedEventArgs.g.h
    │   │       │   │       ├── ItemsControl.g.cpp
    │   │       │   │       ├── ItemsControl.g.h
    │   │       │   │       ├── ItemsControlAutomationPeer.g.cpp
    │   │       │   │       ├── ItemsControlAutomationPeer.g.h
    │   │       │   │       ├── ItemsPanelTemplate.g.cpp
    │   │       │   │       ├── ItemsPanelTemplate.g.h
    │   │       │   │       ├── ItemsPresenter.g.cpp
    │   │       │   │       ├── ItemsPresenter.g.h
    │   │       │   │       ├── ItemsStackPanel.g.cpp
    │   │       │   │       ├── ItemsStackPanel.g.h
    │   │       │   │       ├── ItemsWrapGrid.g.cpp
    │   │       │   │       ├── ItemsWrapGrid.g.h
    │   │       │   │       ├── IterableCollectionView.g.cpp
    │   │       │   │       ├── IterableCollectionView.g.h
    │   │       │   │       ├── ITransitionContextProvider.g.h
    │   │       │   │       ├── ITreeBuilder.g.h
    │   │       │   │       ├── IXamlPredicate.g.h
    │   │       │   │       ├── KeyboardAccelerator.g.cpp
    │   │       │   │       ├── KeyboardAccelerator.g.h
    │   │       │   │       ├── KeyboardAcceleratorCollection.g.cpp
    │   │       │   │       ├── KeyboardAcceleratorCollection.g.h
    │   │       │   │       ├── KeyboardAcceleratorInvokedEventArgs.g.cpp
    │   │       │   │       ├── KeyboardAcceleratorInvokedEventArgs.g.h
    │   │       │   │       ├── KeyRoutedEventArgs.g.cpp
    │   │       │   │       ├── KeyRoutedEventArgs.g.h
    │   │       │   │       ├── KeySpline.g.cpp
    │   │       │   │       ├── KeySpline.g.h
    │   │       │   │       ├── KeyTime.g.cpp
    │   │       │   │       ├── KeyTime.g.h
    │   │       │   │       ├── LandmarkTargetAutomationPeer.g.cpp
    │   │       │   │       ├── LandmarkTargetAutomationPeer.g.h
    │   │       │   │       ├── LaunchActivatedEventArgs.g.cpp
    │   │       │   │       ├── LaunchActivatedEventArgs.g.h
    │   │       │   │       ├── LayoutTransitionElement.g.cpp
    │   │       │   │       ├── LayoutTransitionElement.g.h
    │   │       │   │       ├── LayoutTransitionElementUtilities.g.cpp
    │   │       │   │       ├── LayoutTransitionElementUtilities.g.h
    │   │       │   │       ├── LayoutTransitionStaggerItem.g.cpp
    │   │       │   │       ├── LayoutTransitionStaggerItem.g.h
    │   │       │   │       ├── LengthConverter.g.cpp
    │   │       │   │       ├── LengthConverter.g.h
    │   │       │   │       ├── Line.g.cpp
    │   │       │   │       ├── Line.g.h
    │   │       │   │       ├── LinearColorKeyFrame.g.cpp
    │   │       │   │       ├── LinearColorKeyFrame.g.h
    │   │       │   │       ├── LinearDoubleKeyFrame.g.cpp
    │   │       │   │       ├── LinearDoubleKeyFrame.g.h
    │   │       │   │       ├── LinearGradientBrush.g.cpp
    │   │       │   │       ├── LinearGradientBrush.g.h
    │   │       │   │       ├── LinearPointKeyFrame.g.cpp
    │   │       │   │       ├── LinearPointKeyFrame.g.h
    │   │       │   │       ├── LineBreak.g.cpp
    │   │       │   │       ├── LineBreak.g.h
    │   │       │   │       ├── LineGeometry.g.cpp
    │   │       │   │       ├── LineGeometry.g.h
    │   │       │   │       ├── LineSegment.g.cpp
    │   │       │   │       ├── LineSegment.g.h
    │   │       │   │       ├── ListBox.g.cpp
    │   │       │   │       ├── ListBox.g.h
    │   │       │   │       ├── ListBoxAutomationPeer.g.cpp
    │   │       │   │       ├── ListBoxAutomationPeer.g.h
    │   │       │   │       ├── ListBoxItem.g.cpp
    │   │       │   │       ├── ListBoxItem.g.h
    │   │       │   │       ├── ListBoxItemAutomationPeer.g.cpp
    │   │       │   │       ├── ListBoxItemAutomationPeer.g.h
    │   │       │   │       ├── ListBoxItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── ListBoxItemDataAutomationPeer.g.h
    │   │       │   │       ├── ListView.g.cpp
    │   │       │   │       ├── ListView.g.h
    │   │       │   │       ├── ListViewAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewAutomationPeer.g.h
    │   │       │   │       ├── ListViewBase.g.cpp
    │   │       │   │       ├── ListViewBase.g.h
    │   │       │   │       ├── ListViewBaseAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewBaseAutomationPeer.g.h
    │   │       │   │       ├── ListViewBaseHeaderItem.g.cpp
    │   │       │   │       ├── ListViewBaseHeaderItem.g.h
    │   │       │   │       ├── ListViewBaseHeaderItemAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewBaseHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── ListViewBaseItem.g.cpp
    │   │       │   │       ├── ListViewBaseItem.g.h
    │   │       │   │       ├── ListViewBaseItemAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewBaseItemAutomationPeer.g.h
    │   │       │   │       ├── ListViewBaseItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewBaseItemDataAutomationPeer.g.h
    │   │       │   │       ├── ListViewBaseItemPresenter.g.cpp
    │   │       │   │       ├── ListViewBaseItemPresenter.g.h
    │   │       │   │       ├── ListViewBaseItemSecondaryChrome.g.cpp
    │   │       │   │       ├── ListViewBaseItemSecondaryChrome.g.h
    │   │       │   │       ├── ListViewBaseItemTemplateSettings.g.cpp
    │   │       │   │       ├── ListViewBaseItemTemplateSettings.g.h
    │   │       │   │       ├── ListViewHeaderItem.g.cpp
    │   │       │   │       ├── ListViewHeaderItem.g.h
    │   │       │   │       ├── ListViewHeaderItemAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewHeaderItemAutomationPeer.g.h
    │   │       │   │       ├── ListViewItem.g.cpp
    │   │       │   │       ├── ListViewItem.g.h
    │   │       │   │       ├── ListViewItemAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewItemAutomationPeer.g.h
    │   │       │   │       ├── ListViewItemDataAutomationPeer.g.cpp
    │   │       │   │       ├── ListViewItemDataAutomationPeer.g.h
    │   │       │   │       ├── ListViewItemPresenter.g.cpp
    │   │       │   │       ├── ListViewItemPresenter.g.h
    │   │       │   │       ├── ListViewItemTemplateSettings.g.cpp
    │   │       │   │       ├── ListViewItemTemplateSettings.g.h
    │   │       │   │       ├── ListViewPersistenceHelper.g.cpp
    │   │       │   │       ├── ListViewPersistenceHelper.g.h
    │   │       │   │       ├── LoadedImageSourceLoadCompletedEventArgs.g.cpp
    │   │       │   │       ├── LoadedImageSourceLoadCompletedEventArgs.g.h
    │   │       │   │       ├── LoadedImageSurface.g.cpp
    │   │       │   │       ├── LoadedImageSurface.g.h
    │   │       │   │       ├── LosingFocusEventArgs.g.cpp
    │   │       │   │       ├── LosingFocusEventArgs.g.h
    │   │       │   │       ├── ManipulationCompletedRoutedEventArgs.g.cpp
    │   │       │   │       ├── ManipulationCompletedRoutedEventArgs.g.h
    │   │       │   │       ├── ManipulationDelta.g.cpp
    │   │       │   │       ├── ManipulationDelta.g.h
    │   │       │   │       ├── ManipulationDeltaRoutedEventArgs.g.cpp
    │   │       │   │       ├── ManipulationDeltaRoutedEventArgs.g.h
    │   │       │   │       ├── ManipulationInertiaStartingRoutedEventArgs.g.cpp
    │   │       │   │       ├── ManipulationInertiaStartingRoutedEventArgs.g.h
    │   │       │   │       ├── ManipulationPivot.g.cpp
    │   │       │   │       ├── ManipulationPivot.g.h
    │   │       │   │       ├── ManipulationStartedRoutedEventArgs.g.cpp
    │   │       │   │       ├── ManipulationStartedRoutedEventArgs.g.h
    │   │       │   │       ├── ManipulationStartingRoutedEventArgs.g.cpp
    │   │       │   │       ├── ManipulationStartingRoutedEventArgs.g.h
    │   │       │   │       ├── ManipulationVelocities.g.cpp
    │   │       │   │       ├── ManipulationVelocities.g.h
    │   │       │   │       ├── MarkupExtension.g.cpp
    │   │       │   │       ├── MarkupExtension.g.h
    │   │       │   │       ├── MarkupExtensionBase.g.cpp
    │   │       │   │       ├── MarkupExtensionBase.g.h
    │   │       │   │       ├── Matrix.g.cpp
    │   │       │   │       ├── Matrix.g.h
    │   │       │   │       ├── Matrix3D.g.cpp
    │   │       │   │       ├── Matrix3D.g.h
    │   │       │   │       ├── Matrix3DProjection.g.cpp
    │   │       │   │       ├── Matrix3DProjection.g.h
    │   │       │   │       ├── MatrixTransform.g.cpp
    │   │       │   │       ├── MatrixTransform.g.h
    │   │       │   │       ├── MediaBase.g.cpp
    │   │       │   │       ├── MediaBase.g.h
    │   │       │   │       ├── MediaFailedRoutedEventArgs.g.cpp
    │   │       │   │       ├── MediaFailedRoutedEventArgs.g.h
    │   │       │   │       ├── MediaPlaybackItemConverter.g.cpp
    │   │       │   │       ├── MediaPlaybackItemConverter.g.h
    │   │       │   │       ├── MediaPlayerElement.g.cpp
    │   │       │   │       ├── MediaPlayerElement.g.h
    │   │       │   │       ├── MediaPlayerElementAutomationPeer.g.cpp
    │   │       │   │       ├── MediaPlayerElementAutomationPeer.g.h
    │   │       │   │       ├── MediaPlayerPresenter.g.cpp
    │   │       │   │       ├── MediaPlayerPresenter.g.h
    │   │       │   │       ├── MediaSwapChainElement.g.cpp
    │   │       │   │       ├── MediaSwapChainElement.g.h
    │   │       │   │       ├── MediaTransportControls.g.cpp
    │   │       │   │       ├── MediaTransportControls.g.h
    │   │       │   │       ├── MediaTransportControlsAutomationPeer.g.cpp
    │   │       │   │       ├── MediaTransportControlsAutomationPeer.g.h
    │   │       │   │       ├── MediaTransportControlsHelper.g.cpp
    │   │       │   │       ├── MediaTransportControlsHelper.g.h
    │   │       │   │       ├── MediaTransportControlsThumbnailRequestedEventArgs.g.cpp
    │   │       │   │       ├── MediaTransportControlsThumbnailRequestedEventArgs.g.h
    │   │       │   │       ├── MenuFlyout.g.cpp
    │   │       │   │       ├── MenuFlyout.g.h
    │   │       │   │       ├── MenuFlyoutItem.g.cpp
    │   │       │   │       ├── MenuFlyoutItem.g.h
    │   │       │   │       ├── MenuFlyoutItemAutomationPeer.g.cpp
    │   │       │   │       ├── MenuFlyoutItemAutomationPeer.g.h
    │   │       │   │       ├── MenuFlyoutItemBase.g.cpp
    │   │       │   │       ├── MenuFlyoutItemBase.g.h
    │   │       │   │       ├── MenuFlyoutItemBaseCollection.g.cpp
    │   │       │   │       ├── MenuFlyoutItemBaseCollection.g.h
    │   │       │   │       ├── MenuFlyoutItemTemplateSettings.g.cpp
    │   │       │   │       ├── MenuFlyoutItemTemplateSettings.g.h
    │   │       │   │       ├── MenuFlyoutPresenter.g.cpp
    │   │       │   │       ├── MenuFlyoutPresenter.g.h
    │   │       │   │       ├── MenuFlyoutPresenterAutomationPeer.g.cpp
    │   │       │   │       ├── MenuFlyoutPresenterAutomationPeer.g.h
    │   │       │   │       ├── MenuFlyoutPresenterTemplateSettings.g.cpp
    │   │       │   │       ├── MenuFlyoutPresenterTemplateSettings.g.h
    │   │       │   │       ├── MenuFlyoutSeparator.g.cpp
    │   │       │   │       ├── MenuFlyoutSeparator.g.h
    │   │       │   │       ├── MenuFlyoutSubItem.g.cpp
    │   │       │   │       ├── MenuFlyoutSubItem.g.h
    │   │       │   │       ├── MenuFlyoutSubItemAutomationPeer.g.cpp
    │   │       │   │       ├── MenuFlyoutSubItemAutomationPeer.g.h
    │   │       │   │       ├── MenuPopupThemeTransition.g.cpp
    │   │       │   │       ├── MenuPopupThemeTransition.g.h
    │   │       │   │       ├── ModernCollectionBasePanel.g.cpp
    │   │       │   │       ├── ModernCollectionBasePanel.g.h
    │   │       │   │       ├── NamedContainerAutomationPeer.g.cpp
    │   │       │   │       ├── NamedContainerAutomationPeer.g.h
    │   │       │   │       ├── NavigatingCancelEventArgs.g.cpp
    │   │       │   │       ├── NavigatingCancelEventArgs.g.h
    │   │       │   │       ├── NavigationEventArgs.g.cpp
    │   │       │   │       ├── NavigationEventArgs.g.h
    │   │       │   │       ├── NavigationFailedEventArgs.g.cpp
    │   │       │   │       ├── NavigationFailedEventArgs.g.h
    │   │       │   │       ├── NavigationTransitionInfo.g.cpp
    │   │       │   │       ├── NavigationTransitionInfo.g.h
    │   │       │   │       ├── NoFocusCandidateFoundEventArgs.g.cpp
    │   │       │   │       ├── NoFocusCandidateFoundEventArgs.g.h
    │   │       │   │       ├── NotifyCollectionChangedEventArgs.g.cpp
    │   │       │   │       ├── NotifyCollectionChangedEventArgs.g.h
    │   │       │   │       ├── NullExtension.g.cpp
    │   │       │   │       ├── NullExtension.g.h
    │   │       │   │       ├── NullKeyedResource.g.cpp
    │   │       │   │       ├── NullKeyedResource.g.h
    │   │       │   │       ├── ObjectAnimationUsingKeyFrames.g.cpp
    │   │       │   │       ├── ObjectAnimationUsingKeyFrames.g.h
    │   │       │   │       ├── ObjectKeyFrame.g.cpp
    │   │       │   │       ├── ObjectKeyFrame.g.h
    │   │       │   │       ├── ObjectKeyFrameCollection.g.cpp
    │   │       │   │       ├── ObjectKeyFrameCollection.g.h
    │   │       │   │       ├── OrientedVirtualizingPanel.g.cpp
    │   │       │   │       ├── OrientedVirtualizingPanel.g.h
    │   │       │   │       ├── Page.g.cpp
    │   │       │   │       ├── Page.g.h
    │   │       │   │       ├── PageStackEntry.g.cpp
    │   │       │   │       ├── PageStackEntry.g.h
    │   │       │   │       ├── PaginateEventArgs.g.cpp
    │   │       │   │       ├── PaginateEventArgs.g.h
    │   │       │   │       ├── Panel.g.cpp
    │   │       │   │       ├── Panel.g.h
    │   │       │   │       ├── PanelEx.g.cpp
    │   │       │   │       ├── PanelEx.g.h
    │   │       │   │       ├── PaneThemeTransition.g.cpp
    │   │       │   │       ├── PaneThemeTransition.g.h
    │   │       │   │       ├── Paragraph.g.cpp
    │   │       │   │       ├── Paragraph.g.h
    │   │       │   │       ├── ParallelTimeline.g.cpp
    │   │       │   │       ├── ParallelTimeline.g.h
    │   │       │   │       ├── ParametricCurve.g.cpp
    │   │       │   │       ├── ParametricCurve.g.h
    │   │       │   │       ├── ParametricCurveCollection.g.cpp
    │   │       │   │       ├── ParametricCurveCollection.g.h
    │   │       │   │       ├── ParametricCurveSegment.g.cpp
    │   │       │   │       ├── ParametricCurveSegment.g.h
    │   │       │   │       ├── ParametricCurveSegmentCollection.g.cpp
    │   │       │   │       ├── ParametricCurveSegmentCollection.g.h
    │   │       │   │       ├── ParserServiceProvider.g.cpp
    │   │       │   │       ├── ParserServiceProvider.g.h
    │   │       │   │       ├── PasswordBox.g.cpp
    │   │       │   │       ├── PasswordBox.g.h
    │   │       │   │       ├── PasswordBoxAutomationPeer.g.cpp
    │   │       │   │       ├── PasswordBoxAutomationPeer.g.h
    │   │       │   │       ├── PasswordBoxPasswordChangingEventArgs.g.cpp
    │   │       │   │       ├── PasswordBoxPasswordChangingEventArgs.g.h
    │   │       │   │       ├── Path.g.cpp
    │   │       │   │       ├── Path.g.h
    │   │       │   │       ├── PathFigure.g.cpp
    │   │       │   │       ├── PathFigure.g.h
    │   │       │   │       ├── PathFigureCollection.g.cpp
    │   │       │   │       ├── PathFigureCollection.g.h
    │   │       │   │       ├── PathGeometry.g.cpp
    │   │       │   │       ├── PathGeometry.g.h
    │   │       │   │       ├── PathIcon.g.cpp
    │   │       │   │       ├── PathIcon.g.h
    │   │       │   │       ├── PathIconSource.g.cpp
    │   │       │   │       ├── PathIconSource.g.h
    │   │       │   │       ├── PathSegment.g.cpp
    │   │       │   │       ├── PathSegment.g.h
    │   │       │   │       ├── PathSegmentCollection.g.cpp
    │   │       │   │       ├── PathSegmentCollection.g.h
    │   │       │   │       ├── PerspectiveTransform3D.g.cpp
    │   │       │   │       ├── PerspectiveTransform3D.g.h
    │   │       │   │       ├── PickerFlyoutThemeTransition.g.cpp
    │   │       │   │       ├── PickerFlyoutThemeTransition.g.h
    │   │       │   │       ├── PlaneProjection.g.cpp
    │   │       │   │       ├── PlaneProjection.g.h
    │   │       │   │       ├── PointAnimation.g.cpp
    │   │       │   │       ├── PointAnimation.g.h
    │   │       │   │       ├── PointAnimationUsingKeyFrames.g.cpp
    │   │       │   │       ├── PointAnimationUsingKeyFrames.g.h
    │   │       │   │       ├── PointCollection.g.cpp
    │   │       │   │       ├── PointCollection.g.h
    │   │       │   │       ├── Pointer.g.cpp
    │   │       │   │       ├── Pointer.g.h
    │   │       │   │       ├── PointerAnimationUsingKeyFrames.g.cpp
    │   │       │   │       ├── PointerAnimationUsingKeyFrames.g.h
    │   │       │   │       ├── PointerCollection.g.cpp
    │   │       │   │       ├── PointerCollection.g.h
    │   │       │   │       ├── PointerDownThemeAnimation.g.cpp
    │   │       │   │       ├── PointerDownThemeAnimation.g.h
    │   │       │   │       ├── PointerKeyFrame.g.cpp
    │   │       │   │       ├── PointerKeyFrame.g.h
    │   │       │   │       ├── PointerKeyFrameCollection.g.cpp
    │   │       │   │       ├── PointerKeyFrameCollection.g.h
    │   │       │   │       ├── PointerRoutedEventArgs.g.cpp
    │   │       │   │       ├── PointerRoutedEventArgs.g.h
    │   │       │   │       ├── PointerUpThemeAnimation.g.cpp
    │   │       │   │       ├── PointerUpThemeAnimation.g.h
    │   │       │   │       ├── PointHelper.g.cpp
    │   │       │   │       ├── PointHelper.g.h
    │   │       │   │       ├── PointKeyFrame.g.cpp
    │   │       │   │       ├── PointKeyFrame.g.h
    │   │       │   │       ├── PointKeyFrameCollection.g.cpp
    │   │       │   │       ├── PointKeyFrameCollection.g.h
    │   │       │   │       ├── PolyBezierSegment.g.cpp
    │   │       │   │       ├── PolyBezierSegment.g.h
    │   │       │   │       ├── Polygon.g.cpp
    │   │       │   │       ├── Polygon.g.h
    │   │       │   │       ├── Polyline.g.cpp
    │   │       │   │       ├── Polyline.g.h
    │   │       │   │       ├── PolyLineSegment.g.cpp
    │   │       │   │       ├── PolyLineSegment.g.h
    │   │       │   │       ├── PolyQuadraticBezierSegment.g.cpp
    │   │       │   │       ├── PolyQuadraticBezierSegment.g.h
    │   │       │   │       ├── PopInThemeAnimation.g.cpp
    │   │       │   │       ├── PopInThemeAnimation.g.h
    │   │       │   │       ├── PopOutThemeAnimation.g.cpp
    │   │       │   │       ├── PopOutThemeAnimation.g.h
    │   │       │   │       ├── Popup.g.cpp
    │   │       │   │       ├── Popup.g.h
    │   │       │   │       ├── PopupAutomationPeer.g.cpp
    │   │       │   │       ├── PopupAutomationPeer.g.h
    │   │       │   │       ├── PopupRoot.g.cpp
    │   │       │   │       ├── PopupRoot.g.h
    │   │       │   │       ├── PopupRootAutomationPeer.g.cpp
    │   │       │   │       ├── PopupRootAutomationPeer.g.h
    │   │       │   │       ├── PopupThemeTransition.g.cpp
    │   │       │   │       ├── PopupThemeTransition.g.h
    │   │       │   │       ├── PowerEase.g.cpp
    │   │       │   │       ├── PowerEase.g.h
    │   │       │   │       ├── PrintDocument.g.cpp
    │   │       │   │       ├── PrintDocument.g.h
    │   │       │   │       ├── PrintPageEventArgs.g.cpp
    │   │       │   │       ├── PrintPageEventArgs.g.h
    │   │       │   │       ├── PrintRoot.g.cpp
    │   │       │   │       ├── PrintRoot.g.h
    │   │       │   │       ├── ProcessKeyboardAcceleratorEventArgs.g.cpp
    │   │       │   │       ├── ProcessKeyboardAcceleratorEventArgs.g.h
    │   │       │   │       ├── Projection.g.cpp
    │   │       │   │       ├── Projection.g.h
    │   │       │   │       ├── PropertyChangedEventArgs.g.cpp
    │   │       │   │       ├── PropertyChangedEventArgs.g.h
    │   │       │   │       ├── PropertyMetadata.g.cpp
    │   │       │   │       ├── PropertyMetadata.g.h
    │   │       │   │       ├── PropertyPath.g.cpp
    │   │       │   │       ├── PropertyPath.g.h
    │   │       │   │       ├── ProvideValueTargetProperty.g.cpp
    │   │       │   │       ├── ProvideValueTargetProperty.g.h
    │   │       │   │       ├── PVLStaggerFunction.g.cpp
    │   │       │   │       ├── PVLStaggerFunction.g.h
    │   │       │   │       ├── QuadraticBezierSegment.g.cpp
    │   │       │   │       ├── QuadraticBezierSegment.g.h
    │   │       │   │       ├── QuadraticEase.g.cpp
    │   │       │   │       ├── QuadraticEase.g.h
    │   │       │   │       ├── QuarticEase.g.cpp
    │   │       │   │       ├── QuarticEase.g.h
    │   │       │   │       ├── QuinticEase.g.cpp
    │   │       │   │       ├── QuinticEase.g.h
    │   │       │   │       ├── RadioButton.g.cpp
    │   │       │   │       ├── RadioButton.g.h
    │   │       │   │       ├── RadioButtonAutomationPeer.g.cpp
    │   │       │   │       ├── RadioButtonAutomationPeer.g.h
    │   │       │   │       ├── RangeBase.g.cpp
    │   │       │   │       ├── RangeBase.g.h
    │   │       │   │       ├── RangeBaseAutomationPeer.g.cpp
    │   │       │   │       ├── RangeBaseAutomationPeer.g.h
    │   │       │   │       ├── RangeBaseValueChangedEventArgs.g.cpp
    │   │       │   │       ├── RangeBaseValueChangedEventArgs.g.h
    │   │       │   │       ├── Rectangle.g.cpp
    │   │       │   │       ├── Rectangle.g.h
    │   │       │   │       ├── RectangleGeometry.g.cpp
    │   │       │   │       ├── RectangleGeometry.g.h
    │   │       │   │       ├── RectHelper.g.cpp
    │   │       │   │       ├── RectHelper.g.h
    │   │       │   │       ├── RelativePanel.g.cpp
    │   │       │   │       ├── RelativePanel.g.h
    │   │       │   │       ├── RelativeSource.g.cpp
    │   │       │   │       ├── RelativeSource.g.h
    │   │       │   │       ├── RenderedEventArgs.g.cpp
    │   │       │   │       ├── RenderedEventArgs.g.h
    │   │       │   │       ├── RenderingEventArgs.g.cpp
    │   │       │   │       ├── RenderingEventArgs.g.h
    │   │       │   │       ├── RenderTargetBitmap.g.cpp
    │   │       │   │       ├── RenderTargetBitmap.g.h
    │   │       │   │       ├── RenderTargetBitmapRoot.g.cpp
    │   │       │   │       ├── RenderTargetBitmapRoot.g.h
    │   │       │   │       ├── ReorderThemeTransition.g.cpp
    │   │       │   │       ├── ReorderThemeTransition.g.h
    │   │       │   │       ├── RepeatBehavior.g.cpp
    │   │       │   │       ├── RepeatBehavior.g.h
    │   │       │   │       ├── RepeatButton.g.cpp
    │   │       │   │       ├── RepeatButton.g.h
    │   │       │   │       ├── RepeatButtonAutomationPeer.g.cpp
    │   │       │   │       ├── RepeatButtonAutomationPeer.g.h
    │   │       │   │       ├── RepositionThemeAnimation.g.cpp
    │   │       │   │       ├── RepositionThemeAnimation.g.h
    │   │       │   │       ├── RepositionThemeTransition.g.cpp
    │   │       │   │       ├── RepositionThemeTransition.g.h
    │   │       │   │       ├── ResourceDictionary.g.cpp
    │   │       │   │       ├── ResourceDictionary.g.h
    │   │       │   │       ├── ResourceDictionaryCollection.g.cpp
    │   │       │   │       ├── ResourceDictionaryCollection.g.h
    │   │       │   │       ├── ResourceManagerRequestedEventArgs.g.cpp
    │   │       │   │       ├── ResourceManagerRequestedEventArgs.g.h
    │   │       │   │       ├── RichEditBox.g.cpp
    │   │       │   │       ├── RichEditBox.g.h
    │   │       │   │       ├── RichEditBoxAutomationPeer.g.cpp
    │   │       │   │       ├── RichEditBoxAutomationPeer.g.h
    │   │       │   │       ├── RichEditBoxSelectionChangingEventArgs.g.cpp
    │   │       │   │       ├── RichEditBoxSelectionChangingEventArgs.g.h
    │   │       │   │       ├── RichEditBoxTextChangingEventArgs.g.cpp
    │   │       │   │       ├── RichEditBoxTextChangingEventArgs.g.h
    │   │       │   │       ├── RichTextBlock.g.cpp
    │   │       │   │       ├── RichTextBlock.g.h
    │   │       │   │       ├── RichTextBlockAutomationPeer.g.cpp
    │   │       │   │       ├── RichTextBlockAutomationPeer.g.h
    │   │       │   │       ├── RichTextBlockOverflow.g.cpp
    │   │       │   │       ├── RichTextBlockOverflow.g.h
    │   │       │   │       ├── RichTextBlockOverflowAutomationPeer.g.cpp
    │   │       │   │       ├── RichTextBlockOverflowAutomationPeer.g.h
    │   │       │   │       ├── RightTappedRoutedEventArgs.g.cpp
    │   │       │   │       ├── RightTappedRoutedEventArgs.g.h
    │   │       │   │       ├── RootScrollViewer.g.cpp
    │   │       │   │       ├── RootScrollViewer.g.h
    │   │       │   │       ├── RootVisual.g.cpp
    │   │       │   │       ├── RootVisual.g.h
    │   │       │   │       ├── RotateTransform.g.cpp
    │   │       │   │       ├── RotateTransform.g.h
    │   │       │   │       ├── RoutedEvent.g.cpp
    │   │       │   │       ├── RoutedEvent.g.h
    │   │       │   │       ├── RoutedEventArgs.g.cpp
    │   │       │   │       ├── RoutedEventArgs.g.h
    │   │       │   │       ├── RowDefinition.g.cpp
    │   │       │   │       ├── RowDefinition.g.h
    │   │       │   │       ├── RowDefinitionCollection.g.cpp
    │   │       │   │       ├── RowDefinitionCollection.g.h
    │   │       │   │       ├── Run.g.cpp
    │   │       │   │       ├── Run.g.h
    │   │       │   │       ├── ScalarTransition.g.cpp
    │   │       │   │       ├── ScalarTransition.g.h
    │   │       │   │       ├── ScaleTransform.g.cpp
    │   │       │   │       ├── ScaleTransform.g.h
    │   │       │   │       ├── ScrollBar.g.cpp
    │   │       │   │       ├── ScrollBar.g.h
    │   │       │   │       ├── ScrollBarAutomationPeer.g.cpp
    │   │       │   │       ├── ScrollBarAutomationPeer.g.h
    │   │       │   │       ├── ScrollContentControl.g.cpp
    │   │       │   │       ├── ScrollContentControl.g.h
    │   │       │   │       ├── ScrollContentPresenter.g.cpp
    │   │       │   │       ├── ScrollContentPresenter.g.h
    │   │       │   │       ├── ScrollEventArgs.g.cpp
    │   │       │   │       ├── ScrollEventArgs.g.h
    │   │       │   │       ├── ScrollItemAdapter.g.cpp
    │   │       │   │       ├── ScrollItemAdapter.g.h
    │   │       │   │       ├── ScrollViewer.g.cpp
    │   │       │   │       ├── ScrollViewer.g.h
    │   │       │   │       ├── ScrollViewerAutomationPeer.g.cpp
    │   │       │   │       ├── ScrollViewerAutomationPeer.g.h
    │   │       │   │       ├── ScrollViewerView.g.cpp
    │   │       │   │       ├── ScrollViewerView.g.h
    │   │       │   │       ├── ScrollViewerViewChangedEventArgs.g.cpp
    │   │       │   │       ├── ScrollViewerViewChangedEventArgs.g.h
    │   │       │   │       ├── ScrollViewerViewChangingEventArgs.g.cpp
    │   │       │   │       ├── ScrollViewerViewChangingEventArgs.g.h
    │   │       │   │       ├── SecondaryContentRelationship.g.cpp
    │   │       │   │       ├── SecondaryContentRelationship.g.h
    │   │       │   │       ├── SectionsInViewChangedEventArgs.g.cpp
    │   │       │   │       ├── SectionsInViewChangedEventArgs.g.h
    │   │       │   │       ├── SeekSliderAutomationPeer.g.cpp
    │   │       │   │       ├── SeekSliderAutomationPeer.g.h
    │   │       │   │       ├── SelectionChangedEventArgs.g.cpp
    │   │       │   │       ├── SelectionChangedEventArgs.g.h
    │   │       │   │       ├── Selector.g.cpp
    │   │       │   │       ├── Selector.g.h
    │   │       │   │       ├── SelectorAutomationPeer.g.cpp
    │   │       │   │       ├── SelectorAutomationPeer.g.h
    │   │       │   │       ├── SelectorItem.g.cpp
    │   │       │   │       ├── SelectorItem.g.h
    │   │       │   │       ├── SelectorItemAutomationPeer.g.cpp
    │   │       │   │       ├── SelectorItemAutomationPeer.g.h
    │   │       │   │       ├── SemanticZoom.g.cpp
    │   │       │   │       ├── SemanticZoom.g.h
    │   │       │   │       ├── SemanticZoomAutomationPeer.g.cpp
    │   │       │   │       ├── SemanticZoomAutomationPeer.g.h
    │   │       │   │       ├── SemanticZoomLocation.g.cpp
    │   │       │   │       ├── SemanticZoomLocation.g.h
    │   │       │   │       ├── SemanticZoomViewChangedEventArgs.g.cpp
    │   │       │   │       ├── SemanticZoomViewChangedEventArgs.g.h
    │   │       │   │       ├── Setter.g.cpp
    │   │       │   │       ├── Setter.g.h
    │   │       │   │       ├── SetterBase.g.cpp
    │   │       │   │       ├── SetterBase.g.h
    │   │       │   │       ├── SetterBaseCollection.g.cpp
    │   │       │   │       ├── SetterBaseCollection.g.h
    │   │       │   │       ├── Shadow.g.cpp
    │   │       │   │       ├── Shadow.g.h
    │   │       │   │       ├── Shape.g.cpp
    │   │       │   │       ├── Shape.g.h
    │   │       │   │       ├── SineEase.g.cpp
    │   │       │   │       ├── SineEase.g.h
    │   │       │   │       ├── SizeChangedEventArgs.g.cpp
    │   │       │   │       ├── SizeChangedEventArgs.g.h
    │   │       │   │       ├── SizeHelper.g.cpp
    │   │       │   │       ├── SizeHelper.g.h
    │   │       │   │       ├── SkewTransform.g.cpp
    │   │       │   │       ├── SkewTransform.g.h
    │   │       │   │       ├── Slider.g.cpp
    │   │       │   │       ├── Slider.g.h
    │   │       │   │       ├── SliderAutomationPeer.g.cpp
    │   │       │   │       ├── SliderAutomationPeer.g.h
    │   │       │   │       ├── SoftwareBitmapSource.g.cpp
    │   │       │   │       ├── SoftwareBitmapSource.g.h
    │   │       │   │       ├── SolidColorBrush.g.cpp
    │   │       │   │       ├── SolidColorBrush.g.h
    │   │       │   │       ├── Span.g.cpp
    │   │       │   │       ├── Span.g.h
    │   │       │   │       ├── SplineColorKeyFrame.g.cpp
    │   │       │   │       ├── SplineColorKeyFrame.g.h
    │   │       │   │       ├── SplineDoubleKeyFrame.g.cpp
    │   │       │   │       ├── SplineDoubleKeyFrame.g.h
    │   │       │   │       ├── SplinePointKeyFrame.g.cpp
    │   │       │   │       ├── SplinePointKeyFrame.g.h
    │   │       │   │       ├── SplitCloseThemeAnimation.g.cpp
    │   │       │   │       ├── SplitCloseThemeAnimation.g.h
    │   │       │   │       ├── SplitOpenThemeAnimation.g.cpp
    │   │       │   │       ├── SplitOpenThemeAnimation.g.h
    │   │       │   │       ├── SplitView.g.cpp
    │   │       │   │       ├── SplitView.g.h
    │   │       │   │       ├── SplitViewLightDismissAutomationPeer.g.cpp
    │   │       │   │       ├── SplitViewLightDismissAutomationPeer.g.h
    │   │       │   │       ├── SplitViewPaneAutomationPeer.g.cpp
    │   │       │   │       ├── SplitViewPaneAutomationPeer.g.h
    │   │       │   │       ├── SplitViewPaneClosingEventArgs.g.cpp
    │   │       │   │       ├── SplitViewPaneClosingEventArgs.g.h
    │   │       │   │       ├── SplitViewTemplateSettings.g.cpp
    │   │       │   │       ├── SplitViewTemplateSettings.g.h
    │   │       │   │       ├── StackingLayoutStrategy.g.cpp
    │   │       │   │       ├── StackingLayoutStrategy.g.h
    │   │       │   │       ├── StackPanel.g.cpp
    │   │       │   │       ├── StackPanel.g.h
    │   │       │   │       ├── StaggerFunctionBase.g.cpp
    │   │       │   │       ├── StaggerFunctionBase.g.h
    │   │       │   │       ├── StandardUICommand.g.cpp
    │   │       │   │       ├── StandardUICommand.g.h
    │   │       │   │       ├── StartupEventArgs.g.cpp
    │   │       │   │       ├── StartupEventArgs.g.h
    │   │       │   │       ├── StateTrigger.g.cpp
    │   │       │   │       ├── StateTrigger.g.h
    │   │       │   │       ├── StateTriggerBase.g.cpp
    │   │       │   │       ├── StateTriggerBase.g.h
    │   │       │   │       ├── StateTriggerCollection.g.cpp
    │   │       │   │       ├── StateTriggerCollection.g.h
    │   │       │   │       ├── StaticResource.g.cpp
    │   │       │   │       ├── StaticResource.g.h
    │   │       │   │       ├── Storyboard.g.cpp
    │   │       │   │       ├── Storyboard.g.h
    │   │       │   │       ├── StoryboardCollection.g.cpp
    │   │       │   │       ├── StoryboardCollection.g.h
    │   │       │   │       ├── Style.g.cpp
    │   │       │   │       ├── Style.g.h
    │   │       │   │       ├── StyleSelector.g.cpp
    │   │       │   │       ├── StyleSelector.g.h
    │   │       │   │       ├── SurfaceImageSource.g.cpp
    │   │       │   │       ├── SurfaceImageSource.g.h
    │   │       │   │       ├── SvgImageSource.g.cpp
    │   │       │   │       ├── SvgImageSource.g.h
    │   │       │   │       ├── SvgImageSourceFailedEventArgs.g.cpp
    │   │       │   │       ├── SvgImageSourceFailedEventArgs.g.h
    │   │       │   │       ├── SvgImageSourceOpenedEventArgs.g.cpp
    │   │       │   │       ├── SvgImageSourceOpenedEventArgs.g.h
    │   │       │   │       ├── SwapChainBackgroundPanel.g.cpp
    │   │       │   │       ├── SwapChainBackgroundPanel.g.h
    │   │       │   │       ├── SwapChainElement.g.cpp
    │   │       │   │       ├── SwapChainElement.g.h
    │   │       │   │       ├── SwapChainPanel.g.cpp
    │   │       │   │       ├── SwapChainPanel.g.h
    │   │       │   │       ├── SwipeBackThemeAnimation.g.cpp
    │   │       │   │       ├── SwipeBackThemeAnimation.g.h
    │   │       │   │       ├── SwipeHintThemeAnimation.g.cpp
    │   │       │   │       ├── SwipeHintThemeAnimation.g.h
    │   │       │   │       ├── SymbolIcon.g.cpp
    │   │       │   │       ├── SymbolIcon.g.h
    │   │       │   │       ├── SymbolIconSource.g.cpp
    │   │       │   │       ├── SymbolIconSource.g.h
    │   │       │   │       ├── SystemBackdrop.g.cpp
    │   │       │   │       ├── SystemBackdrop.g.h
    │   │       │   │       ├── TappedRoutedEventArgs.g.cpp
    │   │       │   │       ├── TappedRoutedEventArgs.g.h
    │   │       │   │       ├── TargetPropertyPath.g.cpp
    │   │       │   │       ├── TargetPropertyPath.g.h
    │   │       │   │       ├── TemplateBinding.g.cpp
    │   │       │   │       ├── TemplateBinding.g.h
    │   │       │   │       ├── TemplateContent.g.cpp
    │   │       │   │       ├── TemplateContent.g.h
    │   │       │   │       ├── TextAdapter.g.cpp
    │   │       │   │       ├── TextAdapter.g.h
    │   │       │   │       ├── TextBlock.g.cpp
    │   │       │   │       ├── TextBlock.g.h
    │   │       │   │       ├── TextBlockAutomationPeer.g.cpp
    │   │       │   │       ├── TextBlockAutomationPeer.g.h
    │   │       │   │       ├── TextBox.g.cpp
    │   │       │   │       ├── TextBox.g.h
    │   │       │   │       ├── TextBoxAutomationPeer.g.cpp
    │   │       │   │       ├── TextBoxAutomationPeer.g.h
    │   │       │   │       ├── TextBoxBase.g.cpp
    │   │       │   │       ├── TextBoxBase.g.h
    │   │       │   │       ├── TextBoxBaseAutomationPeer.g.cpp
    │   │       │   │       ├── TextBoxBaseAutomationPeer.g.h
    │   │       │   │       ├── TextBoxBeforeTextChangingEventArgs.g.cpp
    │   │       │   │       ├── TextBoxBeforeTextChangingEventArgs.g.h
    │   │       │   │       ├── TextBoxSelectionChangingEventArgs.g.cpp
    │   │       │   │       ├── TextBoxSelectionChangingEventArgs.g.h
    │   │       │   │       ├── TextBoxTextChangingEventArgs.g.cpp
    │   │       │   │       ├── TextBoxTextChangingEventArgs.g.h
    │   │       │   │       ├── TextBoxView.g.cpp
    │   │       │   │       ├── TextBoxView.g.h
    │   │       │   │       ├── TextChangedEventArgs.g.cpp
    │   │       │   │       ├── TextChangedEventArgs.g.h
    │   │       │   │       ├── TextCompositionChangedEventArgs.g.cpp
    │   │       │   │       ├── TextCompositionChangedEventArgs.g.h
    │   │       │   │       ├── TextCompositionEndedEventArgs.g.cpp
    │   │       │   │       ├── TextCompositionEndedEventArgs.g.h
    │   │       │   │       ├── TextCompositionStartedEventArgs.g.cpp
    │   │       │   │       ├── TextCompositionStartedEventArgs.g.h
    │   │       │   │       ├── TextControlCopyingToClipboardEventArgs.g.cpp
    │   │       │   │       ├── TextControlCopyingToClipboardEventArgs.g.h
    │   │       │   │       ├── TextControlCuttingToClipboardEventArgs.g.cpp
    │   │       │   │       ├── TextControlCuttingToClipboardEventArgs.g.h
    │   │       │   │       ├── TextControlPasteEventArgs.g.cpp
    │   │       │   │       ├── TextControlPasteEventArgs.g.h
    │   │       │   │       ├── TextElement.g.cpp
    │   │       │   │       ├── TextElement.g.h
    │   │       │   │       ├── TextHighlighter.g.cpp
    │   │       │   │       ├── TextHighlighter.g.h
    │   │       │   │       ├── TextHighlighterBase.g.cpp
    │   │       │   │       ├── TextHighlighterBase.g.h
    │   │       │   │       ├── TextHighlighterCollection.g.cpp
    │   │       │   │       ├── TextHighlighterCollection.g.h
    │   │       │   │       ├── TextOptions.g.cpp
    │   │       │   │       ├── TextOptions.g.h
    │   │       │   │       ├── TextPointer.g.cpp
    │   │       │   │       ├── TextPointer.g.h
    │   │       │   │       ├── TextPointerWrapper.g.cpp
    │   │       │   │       ├── TextPointerWrapper.g.h
    │   │       │   │       ├── TextProvider.g.cpp
    │   │       │   │       ├── TextProvider.g.h
    │   │       │   │       ├── TextRangeAdapter.g.cpp
    │   │       │   │       ├── TextRangeAdapter.g.h
    │   │       │   │       ├── TextRangeCollection.g.cpp
    │   │       │   │       ├── TextRangeCollection.g.h
    │   │       │   │       ├── TextRangeProvider.g.cpp
    │   │       │   │       ├── TextRangeProvider.g.h
    │   │       │   │       ├── TextSelectionGripper.g.cpp
    │   │       │   │       ├── TextSelectionGripper.g.h
    │   │       │   │       ├── ThemeAnimationBase.g.cpp
    │   │       │   │       ├── ThemeAnimationBase.g.h
    │   │       │   │       ├── ThemeResource.g.cpp
    │   │       │   │       ├── ThemeResource.g.h
    │   │       │   │       ├── ThemeShadow.g.cpp
    │   │       │   │       ├── ThemeShadow.g.h
    │   │       │   │       ├── Thickness.g.cpp
    │   │       │   │       ├── Thickness.g.h
    │   │       │   │       ├── Thumb.g.cpp
    │   │       │   │       ├── Thumb.g.h
    │   │       │   │       ├── ThumbAutomationPeer.g.cpp
    │   │       │   │       ├── ThumbAutomationPeer.g.h
    │   │       │   │       ├── TickBar.g.cpp
    │   │       │   │       ├── TickBar.g.h
    │   │       │   │       ├── TileBrush.g.cpp
    │   │       │   │       ├── TileBrush.g.h
    │   │       │   │       ├── Timeline.g.cpp
    │   │       │   │       ├── Timeline.g.h
    │   │       │   │       ├── TimelineCollection.g.cpp
    │   │       │   │       ├── TimelineCollection.g.h
    │   │       │   │       ├── TimePicker.g.cpp
    │   │       │   │       ├── TimePicker.g.h
    │   │       │   │       ├── TimePickerAutomationPeer.g.cpp
    │   │       │   │       ├── TimePickerAutomationPeer.g.h
    │   │       │   │       ├── TimePickerSelectedValueChangedEventArgs.g.cpp
    │   │       │   │       ├── TimePickerSelectedValueChangedEventArgs.g.h
    │   │       │   │       ├── TimePickerValueChangedEventArgs.g.cpp
    │   │       │   │       ├── TimePickerValueChangedEventArgs.g.h
    │   │       │   │       ├── ToggleButton.g.cpp
    │   │       │   │       ├── ToggleButton.g.h
    │   │       │   │       ├── ToggleButtonAutomationPeer.g.cpp
    │   │       │   │       ├── ToggleButtonAutomationPeer.g.h
    │   │       │   │       ├── ToggleMenuFlyoutItem.g.cpp
    │   │       │   │       ├── ToggleMenuFlyoutItem.g.h
    │   │       │   │       ├── ToggleMenuFlyoutItemAutomationPeer.g.cpp
    │   │       │   │       ├── ToggleMenuFlyoutItemAutomationPeer.g.h
    │   │       │   │       ├── ToggleSwitch.g.cpp
    │   │       │   │       ├── ToggleSwitch.g.h
    │   │       │   │       ├── ToggleSwitchAutomationPeer.g.cpp
    │   │       │   │       ├── ToggleSwitchAutomationPeer.g.h
    │   │       │   │       ├── ToggleSwitchTemplateSettings.g.cpp
    │   │       │   │       ├── ToggleSwitchTemplateSettings.g.h
    │   │       │   │       ├── ToolTip.g.cpp
    │   │       │   │       ├── ToolTip.g.h
    │   │       │   │       ├── ToolTipAutomationPeer.g.cpp
    │   │       │   │       ├── ToolTipAutomationPeer.g.h
    │   │       │   │       ├── ToolTipService.g.cpp
    │   │       │   │       ├── ToolTipService.g.h
    │   │       │   │       ├── ToolTipTemplateSettings.g.cpp
    │   │       │   │       ├── ToolTipTemplateSettings.g.h
    │   │       │   │       ├── Transform.g.cpp
    │   │       │   │       ├── Transform.g.h
    │   │       │   │       ├── Transform3D.g.cpp
    │   │       │   │       ├── Transform3D.g.h
    │   │       │   │       ├── TransformCollection.g.cpp
    │   │       │   │       ├── TransformCollection.g.h
    │   │       │   │       ├── TransformGroup.g.cpp
    │   │       │   │       ├── TransformGroup.g.h
    │   │       │   │       ├── Transition.g.cpp
    │   │       │   │       ├── Transition.g.h
    │   │       │   │       ├── TransitionCollection.g.cpp
    │   │       │   │       ├── TransitionCollection.g.h
    │   │       │   │       ├── TransitionRoot.g.cpp
    │   │       │   │       ├── TransitionRoot.g.h
    │   │       │   │       ├── TransitionTarget.g.cpp
    │   │       │   │       ├── TransitionTarget.g.h
    │   │       │   │       ├── TranslateTransform.g.cpp
    │   │       │   │       ├── TranslateTransform.g.h
    │   │       │   │       ├── TriggerAction.g.cpp
    │   │       │   │       ├── TriggerAction.g.h
    │   │       │   │       ├── TriggerActionCollection.g.cpp
    │   │       │   │       ├── TriggerActionCollection.g.h
    │   │       │   │       ├── TriggerBase.g.cpp
    │   │       │   │       ├── TriggerBase.g.h
    │   │       │   │       ├── TriggerCollection.g.cpp
    │   │       │   │       ├── TriggerCollection.g.h
    │   │       │   │       ├── Typography.g.cpp
    │   │       │   │       ├── Typography.g.h
    │   │       │   │       ├── UIElement.g.cpp
    │   │       │   │       ├── UIElement.g.h
    │   │       │   │       ├── UIElementCollection.g.cpp
    │   │       │   │       ├── UIElementCollection.g.h
    │   │       │   │       ├── UIElementWeakCollection.g.cpp
    │   │       │   │       ├── UIElementWeakCollection.g.h
    │   │       │   │       ├── Underline.g.cpp
    │   │       │   │       ├── Underline.g.h
    │   │       │   │       ├── UnhandledExceptionEventArgs.g.cpp
    │   │       │   │       ├── UnhandledExceptionEventArgs.g.h
    │   │       │   │       ├── UserControl.g.cpp
    │   │       │   │       ├── UserControl.g.h
    │   │       │   │       ├── ValidationErrorsCollection.g.cpp
    │   │       │   │       ├── ValidationErrorsCollection.g.h
    │   │       │   │       ├── VariableSizedWrapGrid.g.cpp
    │   │       │   │       ├── VariableSizedWrapGrid.g.h
    │   │       │   │       ├── Vector3Transition.g.cpp
    │   │       │   │       ├── Vector3Transition.g.h
    │   │       │   │       ├── VectorChangedEventArgs.g.cpp
    │   │       │   │       ├── VectorChangedEventArgs.g.h
    │   │       │   │       ├── VectorCollectionView.g.cpp
    │   │       │   │       ├── VectorCollectionView.g.h
    │   │       │   │       ├── VectorViewCollectionView.g.cpp
    │   │       │   │       ├── VectorViewCollectionView.g.h
    │   │       │   │       ├── Viewbox.g.cpp
    │   │       │   │       ├── Viewbox.g.h
    │   │       │   │       ├── VirtualizingPanel.g.cpp
    │   │       │   │       ├── VirtualizingPanel.g.h
    │   │       │   │       ├── VirtualizingStackPanel.g.cpp
    │   │       │   │       ├── VirtualizingStackPanel.g.h
    │   │       │   │       ├── VirtualSurfaceImageSource.g.cpp
    │   │       │   │       ├── VirtualSurfaceImageSource.g.h
    │   │       │   │       ├── VisualState.g.cpp
    │   │       │   │       ├── VisualState.g.h
    │   │       │   │       ├── VisualStateChangedEventArgs.g.cpp
    │   │       │   │       ├── VisualStateChangedEventArgs.g.h
    │   │       │   │       ├── VisualStateCollection.g.cpp
    │   │       │   │       ├── VisualStateCollection.g.h
    │   │       │   │       ├── VisualStateGroup.g.cpp
    │   │       │   │       ├── VisualStateGroup.g.h
    │   │       │   │       ├── VisualStateGroupCollection.g.cpp
    │   │       │   │       ├── VisualStateGroupCollection.g.h
    │   │       │   │       ├── VisualStateManager.g.cpp
    │   │       │   │       ├── VisualStateManager.g.h
    │   │       │   │       ├── VisualTransition.g.cpp
    │   │       │   │       ├── VisualTransition.g.h
    │   │       │   │       ├── VisualTransitionCollection.g.cpp
    │   │       │   │       ├── VisualTransitionCollection.g.h
    │   │       │   │       ├── Window.g.cpp
    │   │       │   │       ├── Window.g.h
    │   │       │   │       ├── WindowActivatedEventArgs.g.cpp
    │   │       │   │       ├── WindowActivatedEventArgs.g.h
    │   │       │   │       ├── WindowChrome.g.cpp
    │   │       │   │       ├── WindowChrome.g.h
    │   │       │   │       ├── WindowCreatedEventArgs.g.cpp
    │   │       │   │       ├── WindowCreatedEventArgs.g.h
    │   │       │   │       ├── WindowEventArgs.g.cpp
    │   │       │   │       ├── WindowEventArgs.g.h
    │   │       │   │       ├── WindowSizeChangedEventArgs.g.cpp
    │   │       │   │       ├── WindowSizeChangedEventArgs.g.h
    │   │       │   │       ├── WindowsXamlManager.g.cpp
    │   │       │   │       ├── WindowsXamlManager.g.h
    │   │       │   │       ├── WindowVisibilityChangedEventArgs.g.cpp
    │   │       │   │       ├── WindowVisibilityChangedEventArgs.g.h
    │   │       │   │       ├── WrapGrid.g.cpp
    │   │       │   │       ├── WrapGrid.g.h
    │   │       │   │       ├── WrappingLayoutStrategy.g.cpp
    │   │       │   │       ├── WrappingLayoutStrategy.g.h
    │   │       │   │       ├── WriteableBitmap.g.cpp
    │   │       │   │       ├── WriteableBitmap.g.h
    │   │       │   │       ├── wrtdxamlgeneratedclasses.vcxproj
    │   │       │   │       ├── XamlBindingHelper.g.cpp
    │   │       │   │       ├── XamlBindingHelper.g.h
    │   │       │   │       ├── XamlCompositionBrushBase.g.cpp
    │   │       │   │       ├── XamlCompositionBrushBase.g.h
    │   │       │   │       ├── XamlIsland.g.cpp
    │   │       │   │       ├── XamlIsland.g.h
    │   │       │   │       ├── XamlIslandRoot.g.cpp
    │   │       │   │       ├── XamlIslandRoot.g.h
    │   │       │   │       ├── XamlIslandRootCollection.g.cpp
    │   │       │   │       ├── XamlIslandRootCollection.g.h
    │   │       │   │       ├── XamlLight.g.cpp
    │   │       │   │       ├── XamlLight.g.h
    │   │       │   │       ├── XamlLightCollection.g.cpp
    │   │       │   │       ├── XamlLightCollection.g.h
    │   │       │   │       ├── XamlMarkupHelper.g.cpp
    │   │       │   │       ├── XamlMarkupHelper.g.h
    │   │       │   │       ├── XamlReader.g.cpp
    │   │       │   │       ├── XamlReader.g.h
    │   │       │   │       ├── XamlRenderingBackgroundTask.g.cpp
    │   │       │   │       ├── XamlRenderingBackgroundTask.g.h
    │   │       │   │       ├── XamlResourceReferenceFailedEventArgs.g.cpp
    │   │       │   │       ├── XamlResourceReferenceFailedEventArgs.g.h
    │   │       │   │       ├── XamlRoot.g.cpp
    │   │       │   │       ├── XamlRoot.g.h
    │   │       │   │       ├── XamlRootChangedEventArgs.g.cpp
    │   │       │   │       ├── XamlRootChangedEventArgs.g.h
    │   │       │   │       ├── XamlShutdownCompletedOnThreadEventArgs.g.cpp
    │   │       │   │       ├── XamlShutdownCompletedOnThreadEventArgs.g.h
    │   │       │   │       ├── XamlSourceFocusNavigationRequest.g.cpp
    │   │       │   │       ├── XamlSourceFocusNavigationRequest.g.h
    │   │       │   │       ├── XamlUICommand.g.cpp
    │   │       │   │       └── XamlUICommand.g.h
    │   │       │   ├── manifest/
    │   │       │   │   └── manifest.vcxproj
    │   │       │   ├── themes/
    │   │       │   │   ├── generic.xaml
    │   │       │   │   └── autogen/
    │   │       │   │       ├── Directory.Build.props
    │   │       │   │       ├── Empty.cs
    │   │       │   │       ├── GenAllXbf.csproj
    │   │       │   │       └── SplitGenericXaml.cs
    │   │       │   └── tools/
    │   │       │       └── xamldiagnostics/
    │   │       │           └── tap/
    │   │       │               ├── DefaultResource.rc
    │   │       │               ├── dllentry.cpp
    │   │       │               ├── precomp.h
    │   │       │               ├── XamlDiagnosticsLauncher.h
    │   │       │               ├── XamlDiagnosticsTap.cpp
    │   │       │               ├── XamlDiagnosticsTap.def
    │   │       │               ├── XamlDiagnosticsTap.h
    │   │       │               └── XamlDiagnosticsTap.vcxproj
    │   │       ├── host/
    │   │       │   └── win/
    │   │       │       └── browserdesktop/
    │   │       │           ├── PlatWinBrowserHost.cpp
    │   │       │           ├── WinBrowserHost.cpp
    │   │       │           ├── WinBrowserHost.h
    │   │       │           ├── windwnreq.cpp
    │   │       │           └── windwnreq.h
    │   │       ├── inc/
    │   │       │   ├── APLock.h
    │   │       │   ├── AutomationCValue.h
    │   │       │   ├── CompositionRequirement.h
    │   │       │   ├── core.h
    │   │       │   ├── core_media.h
    │   │       │   ├── cvalue.h
    │   │       │   ├── CValueConvert.h
    │   │       │   ├── CValueStores.h
    │   │       │   ├── CValueTraits.h
    │   │       │   ├── CValueTypeConvert.h
    │   │       │   ├── CValueTypeInfo.h
    │   │       │   ├── CValueUtil.h
    │   │       │   ├── DataStructureFunctionSpecializations.h
    │   │       │   ├── DeferredElementStateChange.h
    │   │       │   ├── encodedptr.h
    │   │       │   ├── ErrorType.h
    │   │       │   ├── Events.h
    │   │       │   ├── FeatureFlags.h
    │   │       │   ├── HeaderTrimming.h
    │   │       │   ├── IndependentAnimationType.h
    │   │       │   ├── InitializationType.h
    │   │       │   ├── internaleventhandler.h
    │   │       │   ├── IVisualStateGroupCollectionTestHooks.h
    │   │       │   ├── IXamlTestHooks-errors.h
    │   │       │   ├── IXamlTestHooks-log.h
    │   │       │   ├── IXamlTestHooks-win.h
    │   │       │   ├── joltperf.h
    │   │       │   ├── localizedResource.h
    │   │       │   ├── mediaresource.h
    │   │       │   ├── mindebug.h
    │   │       │   ├── minpal.h
    │   │       │   ├── minxcptypes.h
    │   │       │   ├── MUX-ETWEvents.h
    │   │       │   ├── nonLocalizedResource.h
    │   │       │   ├── pal.h
    │   │       │   ├── perf.h
    │   │       │   ├── ReentrancyGuard.h
    │   │       │   ├── TextSurrogates.h
    │   │       │   ├── TraceLoggingInterop.h
    │   │       │   ├── TypeBits.h
    │   │       │   ├── UIACoreEnums.g.h
    │   │       │   ├── UIAEnums.g.h
    │   │       │   ├── UIAEnums.h
    │   │       │   ├── UIAStructs.h
    │   │       │   ├── ValueType.h
    │   │       │   ├── VisualDebugTags.h
    │   │       │   ├── windows.foundation.customattributes.h
    │   │       │   ├── windows.ui.core.corewindow-defs.h
    │   │       │   ├── WindowsAppSDK-ProductInfo.h
    │   │       │   ├── WinUIrc.ver
    │   │       │   ├── xcp_error.h
    │   │       │   ├── XcpAutoLock.h
    │   │       │   ├── XcpDirectManipulationViewportEventHandler.h
    │   │       │   ├── xcperrorresource.h
    │   │       │   ├── XcpInputPaneHandler.h
    │   │       │   ├── XcpList.h
    │   │       │   ├── xcpwindows.h
    │   │       │   ├── xmap.h
    │   │       │   ├── xmllite_error.h
    │   │       │   ├── xstringmap.h
    │   │       │   ├── xuriutils.h
    │   │       │   ├── fwd/
    │   │       │   │   ├── microsoft.ui.input.dragdrop.h
    │   │       │   │   ├── microsoft.ui.text.h
    │   │       │   │   ├── microsoft.ui.xaml.controls.h
    │   │       │   │   ├── microsoft.ui.xaml.h
    │   │       │   │   ├── microsoft.ui.xaml.hosting.h
    │   │       │   │   ├── microsoft.ui.xaml.input.h
    │   │       │   │   ├── microsoft.ui.xaml.interop.h
    │   │       │   │   ├── microsoft.ui.xaml.markup.h
    │   │       │   │   ├── microsoft.ui.xaml.media.animation.h
    │   │       │   │   ├── microsoft.ui.xaml.media.h
    │   │       │   │   ├── windows.applicationmodel.core.h
    │   │       │   │   ├── windows.applicationmodel.resources.h
    │   │       │   │   ├── windows.data.text.h
    │   │       │   │   ├── windows.foundation.h
    │   │       │   │   ├── windows.globalization.h
    │   │       │   │   ├── windows.graphics.h
    │   │       │   │   ├── windows.media.h
    │   │       │   │   ├── windows.storage.h
    │   │       │   │   ├── windows.system.h
    │   │       │   │   ├── windows.system.power.h
    │   │       │   │   ├── windows.ui.composition.h
    │   │       │   │   ├── windows.ui.core.h
    │   │       │   │   ├── windows.ui.popups.h
    │   │       │   │   ├── windows.ui.text.h
    │   │       │   │   └── windows.ui.viewmanagement.h
    │   │       │   ├── platformsdk-uplevel/
    │   │       │   │   └── dwrite_colr_paint_tree.h
    │   │       │   └── telemetry/
    │   │       │       └── MicrosoftTelemetry.h
    │   │       ├── pal/
    │   │       │   ├── common/
    │   │       │   │   ├── BasePALResource.cpp
    │   │       │   │   ├── CommonPlatformUtilities.cpp
    │   │       │   │   ├── CommonPrintingData.cpp
    │   │       │   │   ├── ctypes.cpp
    │   │       │   │   ├── downloadrequestinfo.cpp
    │   │       │   │   ├── matrix.cpp
    │   │       │   │   ├── MemoryStream.cpp
    │   │       │   │   ├── MemoryStreamBuffer.cpp
    │   │       │   │   ├── MsResourceHelpers.cpp
    │   │       │   │   ├── refcounting.cpp
    │   │       │   │   └── UriXStringGetters.cpp
    │   │       │   ├── inc/
    │   │       │   │   ├── BasePALResource.h
    │   │       │   │   ├── CommonPlatformUtilities.h
    │   │       │   │   ├── CommonPrintingData.h
    │   │       │   │   ├── CommonResourceProvider.h
    │   │       │   │   ├── ctypes.h
    │   │       │   │   ├── D3DCommon.idl
    │   │       │   │   ├── DataStructureFunctionProvider.h
    │   │       │   │   ├── downloadrequestinfo.h
    │   │       │   │   ├── macros.h
    │   │       │   │   ├── matrix.h
    │   │       │   │   ├── MemoryStream.h
    │   │       │   │   ├── MemoryStreamBuffer.h
    │   │       │   │   ├── memutils.h
    │   │       │   │   ├── monitorbuffer.h
    │   │       │   │   ├── MsResourceHelpers.h
    │   │       │   │   ├── PalAutomationServices.h
    │   │       │   │   ├── palcore.h
    │   │       │   │   ├── paldebugging.h
    │   │       │   │   ├── PalDirectManipulationCompositorService.h
    │   │       │   │   ├── PalDirectManipulationService.h
    │   │       │   │   ├── palexports.h
    │   │       │   │   ├── palfileuri.h
    │   │       │   │   ├── palgfx.h
    │   │       │   │   ├── PalInputPaneInteraction.h
    │   │       │   │   ├── palmemory.h
    │   │       │   │   ├── palnetwork.h
    │   │       │   │   ├── PalNotify.h
    │   │       │   │   ├── PalPrintingData.h
    │   │       │   │   ├── PalPrintingServices.h
    │   │       │   │   ├── PALProcessCharacteristics.h
    │   │       │   │   ├── PalResourceManager.h
    │   │       │   │   ├── paltext.h
    │   │       │   │   ├── palthread.h
    │   │       │   │   ├── paltouchservices.h
    │   │       │   │   ├── paltypes.h
    │   │       │   │   ├── PalWorkItem.h
    │   │       │   │   ├── real.h
    │   │       │   │   ├── refcounting.h
    │   │       │   │   ├── ReferenceCount.h
    │   │       │   │   ├── rendercounters.h
    │   │       │   │   ├── UriXStringGetters.h
    │   │       │   │   ├── xcontainers.h
    │   │       │   │   ├── xcpdebug.h
    │   │       │   │   ├── xcperror.h
    │   │       │   │   ├── xcpmath.h
    │   │       │   │   ├── xcpsafe.h
    │   │       │   │   ├── xlist.h
    │   │       │   │   ├── xqueue.h
    │   │       │   │   └── xstack.h
    │   │       │   └── win/
    │   │       │       ├── DWriteFontAndScriptServices.cpp
    │   │       │       ├── DWriteFontCollection.cpp
    │   │       │       ├── DWriteFontFace.cpp
    │   │       │       ├── DWriteFontFamily.cpp
    │   │       │       ├── DWriteTextAnalyzer.cpp
    │   │       │       ├── WinPlatformUtilities.cpp
    │   │       │       └── inc/
    │   │       │           ├── DWriteFontAndScriptServices.h
    │   │       │           ├── DWriteFontCollection.h
    │   │       │           ├── DWriteFontFace.h
    │   │       │           ├── DWriteFontFamily.h
    │   │       │           ├── DWriteTextAnalyzer.h
    │   │       │           └── WinPlatformUtilities.h
    │   │       ├── plat/
    │   │       │   └── win/
    │   │       │       ├── browserdesktop/
    │   │       │       │   ├── COMObjectWrapper.h
    │   │       │       │   ├── DirectManipulationFrameInfoProvider.cpp
    │   │       │       │   ├── DirectManipulationFrameInfoProvider.h
    │   │       │       │   ├── DirectManipulationService.h
    │   │       │       │   ├── DirectManipulationViewportEventHandler.cpp
    │   │       │       │   ├── DirectManipulationViewportEventHandler.h
    │   │       │       │   ├── early_init.cpp
    │   │       │       │   ├── FrameworkInputPaneHandler.cpp
    │   │       │       │   ├── FrameworkInputPaneHandler.h
    │   │       │       │   ├── InputPaneInteractionHelper.cpp
    │   │       │       │   ├── InputPaneInteractionHelper.h
    │   │       │       │   ├── PlatformServices.cpp
    │   │       │       │   ├── platwinbrowserdesktop.vcxproj
    │   │       │       │   ├── precomp.h
    │   │       │       │   ├── sources.g.props
    │   │       │       │   ├── sources.props
    │   │       │       │   ├── WinApplicationSingleton.cpp
    │   │       │       │   ├── WinTheme.cpp
    │   │       │       │   ├── WinThreadPool.cpp
    │   │       │       │   ├── WinThreadPool.h
    │   │       │       │   └── XcpCodeTracer.h
    │   │       │       ├── common/
    │   │       │       │   ├── math.cpp
    │   │       │       │   ├── Memory.cpp
    │   │       │       │   ├── purecall.cpp
    │   │       │       │   ├── WinFile.cpp
    │   │       │       │   ├── WinPrintingData.cpp
    │   │       │       │   ├── WinPrintingData.h
    │   │       │       │   ├── winstream.cpp
    │   │       │       │   └── winstream.h
    │   │       │       ├── desktop/
    │   │       │       │   ├── ApplicationDataProvider.cpp
    │   │       │       │   ├── ApplicationDataProvider.h
    │   │       │       │   ├── CommonResourceProvider.cpp
    │   │       │       │   ├── D2DAccelerated.cpp
    │   │       │       │   ├── D2DAccelerated.h
    │   │       │       │   ├── D2DAcceleratedBrushes.cpp
    │   │       │       │   ├── D2DAcceleratedBrushes.h
    │   │       │       │   ├── D2DAcceleratedPrimitives.cpp
    │   │       │       │   ├── D2DAcceleratedPrimitives.h
    │   │       │       │   ├── D2DAcceleratedRT.cpp
    │   │       │       │   ├── d2dacceleratedrt.h
    │   │       │       │   ├── D2DPrintingData.cpp
    │   │       │       │   ├── D2DPrintingData.h
    │   │       │       │   ├── D2DPrintTarget.cpp
    │   │       │       │   ├── D2DPrintTarget.h
    │   │       │       │   ├── D2DUtils.h
    │   │       │       │   ├── d3d11device.cpp
    │   │       │       │   ├── d3d11device.h
    │   │       │       │   ├── D3D11DeviceInstance.cpp
    │   │       │       │   ├── D3D11DeviceInstance.h
    │   │       │       │   ├── d3D11SharedDeviceGuard.h
    │   │       │       │   ├── DCompInteropCompositorPartnerCallback.cpp
    │   │       │       │   ├── DCompInteropCompositorPartnerCallback.h
    │   │       │       │   ├── DCompSurface.cpp
    │   │       │       │   ├── DCompSurface.h
    │   │       │       │   ├── DCompSurfaceFactoryManager.cpp
    │   │       │       │   ├── DCompSurfaceFactoryManager.h
    │   │       │       │   ├── DCompSurfaceMonitor.cpp
    │   │       │       │   ├── DCompSurfaceMonitor.h
    │   │       │       │   ├── ImageSharingEngineHost.cpp
    │   │       │       │   ├── ImageSharingEngineHost.h
    │   │       │       │   ├── ImageUtils.cpp
    │   │       │       │   ├── ImageUtils.h
    │   │       │       │   ├── LockableGraphicsPointer.h
    │   │       │       │   ├── Microsoft-Windows-XAML-ETW.man
    │   │       │       │   ├── PlatformServices.cpp
    │   │       │       │   ├── platwindesktop.vcxproj
    │   │       │       │   ├── precomp.h
    │   │       │       │   ├── ProcessCharacteristics.cpp
    │   │       │       │   ├── SystemMemoryBits.cpp
    │   │       │       │   ├── SystemMemoryBits.h
    │   │       │       │   ├── WindowLessSiteHost.cpp
    │   │       │       │   ├── windowsgraphicsdevicemanager.cpp
    │   │       │       │   ├── windowsgraphicsdevicemanager.h
    │   │       │       │   ├── windowspresenttarget.cpp
    │   │       │       │   └── windowspresenttarget.h
    │   │       │       └── etw/
    │   │       │           └── XamlETW.vcxproj
    │   │       ├── tools/
    │   │       │   ├── Directory.Build.Props
    │   │       │   ├── DumpXbf/
    │   │       │   │   ├── DumpXbf.csproj
    │   │       │   │   ├── FileFormat.cs
    │   │       │   │   ├── NativeMethods.cs
    │   │       │   │   ├── Program.cs
    │   │       │   │   ├── StreamImpl.cs
    │   │       │   │   ├── StreamWrapper.cs
    │   │       │   │   ├── XamlNodeTree.cs
    │   │       │   │   ├── XBFHeaderReader.cs
    │   │       │   │   ├── XBFReader.cs
    │   │       │   │   └── XBFReader2.cs
    │   │       │   ├── GenXbfDLL/
    │   │       │   │   ├── AccessKeyExportStub.cpp
    │   │       │   │   ├── CFocusManagerStub.cpp
    │   │       │   │   ├── comTemplateLibraryStub.cpp
    │   │       │   │   ├── ContentRootCoordinatorStub.cpp
    │   │       │   │   ├── CoreServicesStub.cpp
    │   │       │   │   ├── DependsStub.cpp
    │   │       │   │   ├── DumpAdapterMetadataProvider.cpp
    │   │       │   │   ├── DumpAdapterMetadataProvider.h
    │   │       │   │   ├── DumpHelper.cpp
    │   │       │   │   ├── DumpHelper.h
    │   │       │   │   ├── GenXbf.def
    │   │       │   │   ├── genxbf.rc
    │   │       │   │   ├── GenXbf.vcxproj
    │   │       │   │   ├── InputManagerStub.cpp
    │   │       │   │   ├── Main.cpp
    │   │       │   │   ├── MetadataAPIStub.cpp
    │   │       │   │   ├── MsWin.Build.Packages.Tools.GenXbf.ds
    │   │       │   │   ├── MsWin.Build.Packages.Tools.GenXBFLegacy.ds
    │   │       │   │   ├── ObjectWriterRuntimeFactory.cpp
    │   │       │   │   ├── PInvokesStub.cpp
    │   │       │   │   ├── PlatformStub.cpp
    │   │       │   │   ├── precomp.h
    │   │       │   │   ├── stubs.h
    │   │       │   │   ├── VisualTreeStub.cpp
    │   │       │   │   ├── XamlManagedRuntimeStub.cpp
    │   │       │   │   ├── XamlMetadataProviderStub.cpp
    │   │       │   │   ├── XamlMetadataProviderStub.h
    │   │       │   │   ├── XamlNativeRuntimeStub.cpp
    │   │       │   │   ├── XbfCoreServices.cpp
    │   │       │   │   ├── XbfMetadataProvider.h
    │   │       │   │   ├── xbfpal.cpp
    │   │       │   │   ├── XbfParserErrorService.cpp
    │   │       │   │   └── XbfParserErrorService.h
    │   │       │   ├── SplitGenericXaml/
    │   │       │   │   ├── Program.cs
    │   │       │   │   └── splitgenericxaml.proj
    │   │       │   ├── XbfParser/
    │   │       │   │   ├── XbfParser.sln
    │   │       │   │   ├── SampleXbfViewer/
    │   │       │   │   │   ├── App.config
    │   │       │   │   │   ├── App.xaml
    │   │       │   │   │   ├── App.xaml.cs
    │   │       │   │   │   ├── MainWindow.xaml
    │   │       │   │   │   ├── MainWindow.xaml.cs
    │   │       │   │   │   ├── SampleXbfViewer.csproj
    │   │       │   │   │   ├── XamlObjectViewModel.cs
    │   │       │   │   │   ├── XbfFileViewModel.cs
    │   │       │   │   │   └── Properties/
    │   │       │   │   │       ├── AssemblyInfo.cs
    │   │       │   │   │       ├── Resources.Designer.cs
    │   │       │   │   │       ├── Resources.resx
    │   │       │   │   │       ├── Settings.Designer.cs
    │   │       │   │   │       └── Settings.settings
    │   │       │   │   └── WidgetSpinner/
    │   │       │   │       ├── Directory.Build.props
    │   │       │   │       ├── ErrorService.cs
    │   │       │   │       ├── WidgetSpinner.cs
    │   │       │   │       ├── WidgetSpinner.csproj
    │   │       │   │       ├── Common/
    │   │       │   │       │   ├── Extensions.cs
    │   │       │   │       │   └── ScopeGuard.cs
    │   │       │   │       ├── Metadata/
    │   │       │   │       │   ├── StableXbfIndexMetadata.g.cs
    │   │       │   │       │   ├── XamlAssembly.cs
    │   │       │   │       │   ├── XamlObjectFactory.cs
    │   │       │   │       │   ├── XamlProperty.cs
    │   │       │   │       │   ├── XamlPropertyRegistry.cs
    │   │       │   │       │   ├── XamlType.cs
    │   │       │   │       │   ├── XamlTypeNamespace.cs
    │   │       │   │       │   ├── XamlTypeRegistry.cs
    │   │       │   │       │   ├── XamlXmlNamespace.cs
    │   │       │   │       │   └── KnownTypes/
    │   │       │   │       │       ├── XamlMarkupExtensions.cs
    │   │       │   │       │       └── XamlPrimitiveTypes.cs
    │   │       │   │       ├── Model/
    │   │       │   │       │   ├── TypeConvertedValue.cs
    │   │       │   │       │   ├── XamlObject.cs
    │   │       │   │       │   └── XamlPredicateAndArgs.cs
    │   │       │   │       ├── Parser/
    │   │       │   │       │   ├── XbfGrammarLexer.g4
    │   │       │   │       │   └── XbfGrammarParser.g4
    │   │       │   │       ├── Reader/
    │   │       │   │       │   ├── XbfReader.cs
    │   │       │   │       │   └── XbfReader.Utilities.cs
    │   │       │   │       ├── Writer/
    │   │       │   │       │   ├── ObjectWriter.cs
    │   │       │   │       │   └── ObjectWriter.CustomRuntimeData.cs
    │   │       │   │       └── XBF/
    │   │       │   │           ├── CustomRuntimeData.cs
    │   │       │   │           ├── DeferredElementCustomRuntimeData.cs
    │   │       │   │           ├── PersistedTypes.cs
    │   │       │   │           ├── ResourceDictionaryCustomRuntimeData.cs
    │   │       │   │           ├── StyleCustomRuntimeData.cs
    │   │       │   │           ├── VisualStateGroupCollectionCustomRuntimeData.cs
    │   │       │   │           ├── XbfFile.cs
    │   │       │   │           ├── XbfMetadata.cs
    │   │       │   │           ├── XbfNode.cs
    │   │       │   │           ├── XbfNode.Specializations.cs
    │   │       │   │           └── XbfNodeStream.cs
    │   │       │   └── XCPTypesAutoGen/
    │   │       │       ├── Directory.Build.props
    │   │       │       ├── JoltClasses.t.cs
    │   │       │       ├── TypeProxy.t.cpp
    │   │       │       ├── TypeProxy.t.cs
    │   │       │       ├── XCPTypesAutoGen.sln
    │   │       │       ├── Modules/
    │   │       │       │   ├── XamlOM.targets
    │   │       │       │   ├── AutoSuggestBox/
    │   │       │       │   │   ├── AssemblyInfo.cs
    │   │       │       │   │   ├── AutoSuggestBox.cs
    │   │       │       │   │   ├── AutoSuggestBoxAutomationPeer.cs
    │   │       │       │   │   ├── GlobalSuppressions.cs
    │   │       │       │   │   ├── XamlOM.AutoSuggestBox.csproj
    │   │       │       │   │   ├── XamlOM.AutoSuggestBox.Instant.proj
    │   │       │       │   │   └── XamlOM.AutoSuggestBox.Sources.targets
    │   │       │       │   ├── Controls/
    │   │       │       │   │   ├── AppBar.cs
    │   │       │       │   │   ├── AppBarAutomationPeer.cs
    │   │       │       │   │   ├── AppBarButton.cs
    │   │       │       │   │   ├── AppBarButtonAutomationPeer.cs
    │   │       │       │   │   ├── AppBarElementContainer.cs
    │   │       │       │   │   ├── AssemblyInfo.cs
    │   │       │       │   │   ├── ComboBox.cs
    │   │       │       │   │   ├── CommandBar.cs
    │   │       │       │   │   ├── Commanding.cs
    │   │       │       │   │   ├── GlobalSuppressions.cs
    │   │       │       │   │   ├── Hub.cs
    │   │       │       │   │   ├── HubAutomationPeer.cs
    │   │       │       │   │   ├── IconSource.cs
    │   │       │       │   │   ├── MenuFlyout.cs
    │   │       │       │   │   ├── Page.cs
    │   │       │       │   │   ├── PasswordBox.cs
    │   │       │       │   │   ├── RichEditBox.cs
    │   │       │       │   │   ├── RichTextBlock.cs
    │   │       │       │   │   ├── RichTextBlockOverflow.cs
    │   │       │       │   │   ├── TextBlock.cs
    │   │       │       │   │   ├── TextBox.cs
    │   │       │       │   │   ├── XamlOM.Controls.csproj
    │   │       │       │   │   ├── XamlOM.Controls.Instant.proj
    │   │       │       │   │   ├── XamlOM.Controls.Sources.targets
    │   │       │       │   │   ├── Calendar/
    │   │       │       │   │   │   └── Calendar.cs
    │   │       │       │   │   └── SplitView/
    │   │       │       │   │       ├── SplitView.cs
    │   │       │       │   │       └── SplitViewTemplateSettings.cs
    │   │       │       │   ├── ExtendedCore/
    │   │       │       │   │   ├── GlobalSuppressions.cs
    │   │       │       │   │   ├── Media3D.cs
    │   │       │       │   │   ├── XamlOM.ExCore.csproj
    │   │       │       │   │   ├── XamlOM.ExCore.Instant.proj
    │   │       │       │   │   └── XamlOM.ExCore.Sources.targets
    │   │       │       │   └── Phone/
    │   │       │       │       ├── AssemblyInfo.cs
    │   │       │       │       ├── Phone.cs
    │   │       │       │       ├── PhoneAutomationPeers.cs
    │   │       │       │       ├── Primitives.cs
    │   │       │       │       ├── XamlOM.Phone.csproj
    │   │       │       │       ├── XamlOM.Phone.Instant.proj
    │   │       │       │       └── XamlOM.Phone.Sources.targets
    │   │       │       ├── OM/
    │   │       │       │   ├── AttachedEventDefinition.cs
    │   │       │       │   ├── AttachedPropertyDefinition.cs
    │   │       │       │   ├── AttributeDefinition.cs
    │   │       │       │   ├── AttributeInstantiation.cs
    │   │       │       │   ├── ClassDefinition.cs
    │   │       │       │   ├── ClassVersion.cs
    │   │       │       │   ├── CollectionKind.cs
    │   │       │       │   ├── ConstructorDefinition.cs
    │   │       │       │   ├── ContractDefinition.cs
    │   │       │       │   ├── ContractReference.cs
    │   │       │       │   ├── ContractReferenceExtensions.cs
    │   │       │       │   ├── DelegateDefinition.cs
    │   │       │       │   ├── DependencyPropertyDefinition.cs
    │   │       │       │   ├── DeprecationDefinition.cs
    │   │       │       │   ├── DeprecationType.cs
    │   │       │       │   ├── EnumCategory.cs
    │   │       │       │   ├── EnumDefinition.cs
    │   │       │       │   ├── EnumValueDefinition.cs
    │   │       │       │   ├── EnumVersion.cs
    │   │       │       │   ├── EventDefinition.cs
    │   │       │       │   ├── EventHandlerKind.cs
    │   │       │       │   ├── FrameworkMoniker.AssemblyAttributes.cs
    │   │       │       │   ├── GlobalSuppressions.cs
    │   │       │       │   ├── Guids.cs
    │   │       │       │   ├── Helper.cs
    │   │       │       │   ├── MemberDefinition.cs
    │   │       │       │   ├── MethodBaseDefinition.cs
    │   │       │       │   ├── MethodDefinition.cs
    │   │       │       │   ├── Modifier.cs
    │   │       │       │   ├── ModuleDefinition.cs
    │   │       │       │   ├── NamespaceDefinition.cs
    │   │       │       │   ├── OM.csproj
    │   │       │       │   ├── OM.Instant.proj
    │   │       │       │   ├── OM.Sources.targets
    │   │       │       │   ├── OMContext.cs
    │   │       │       │   ├── OMContextView.cs
    │   │       │       │   ├── OMExtensions.cs
    │   │       │       │   ├── ParameterDefinition.cs
    │   │       │       │   ├── PropertyChangeCallbacktype.cs
    │   │       │       │   ├── PropertyDefinition.cs
    │   │       │       │   ├── PropertyInitializationType.cs
    │   │       │       │   ├── Simple.cs
    │   │       │       │   ├── Strictness.cs
    │   │       │       │   ├── TemplatePartDefinition.cs
    │   │       │       │   ├── ThreadingModelKind.cs
    │   │       │       │   ├── TypeDefinition.cs
    │   │       │       │   ├── TypeReference.cs
    │   │       │       │   ├── ValueType.cs
    │   │       │       │   ├── VelocityFeatures.cs
    │   │       │       │   ├── Version.cs
    │   │       │       │   ├── XamlClassFlags.cs
    │   │       │       │   ├── XamlEnumFlags.cs
    │   │       │       │   ├── XamlEventFlags.cs
    │   │       │       │   ├── XamlPropertyFlags.cs
    │   │       │       │   ├── XamlTypeFlags.cs
    │   │       │       │   ├── Idl/
    │   │       │       │   │   ├── IdlAttachedPropertyInfo.cs
    │   │       │       │   │   ├── IdlAttributeInfo.cs
    │   │       │       │   │   ├── IdlClassInfo.cs
    │   │       │       │   │   ├── IdlConstructorInfo.cs
    │   │       │       │   │   ├── IdlDelegateInfo.cs
    │   │       │       │   │   ├── IdlDependencyPropertyInfo.cs
    │   │       │       │   │   ├── IdlEnumInfo.cs
    │   │       │       │   │   ├── IdlEnumValueInfo.cs
    │   │       │       │   │   ├── IdlEventInfo.cs
    │   │       │       │   │   ├── IdlMemberInfo.cs
    │   │       │       │   │   ├── IdlMethodInfo.cs
    │   │       │       │   │   ├── IdlNamespaceInfo.cs
    │   │       │       │   │   ├── IdlPropertyInfo.cs
    │   │       │       │   │   ├── IdlTypeInfo.cs
    │   │       │       │   │   ├── IdlTypeRefInfo.cs
    │   │       │       │   │   └── IIdlInfo.cs
    │   │       │       │   └── Visitors/
    │   │       │       │       ├── HashVisitor.cs
    │   │       │       │       ├── IdlImportVisitor.cs
    │   │       │       │       └── OMVisitor.cs
    │   │       │       ├── RunCodeGen/
    │   │       │       │   ├── xamlgen.instantcompiler.targets
    │   │       │       │   ├── xamlgen.runcodegen.proj
    │   │       │       │   └── xamlgen.runcodegen.props
    │   │       │       ├── XamlGen/
    │   │       │       │   ├── CSVHelper.cs
    │   │       │       │   ├── DependencyGenerator.cs
    │   │       │       │   ├── EtwEvents-Diagnostics.man
    │   │       │       │   ├── EtwEvents-Localization.man
    │   │       │       │   ├── EtwEvents.man
    │   │       │       │   ├── GlobalSuppressions.cs
    │   │       │       │   ├── GuidCollisionDetector.cs
    │   │       │       │   ├── IndexGenerator.cs
    │   │       │       │   ├── PhoneIndexGenerator.cs
    │   │       │       │   ├── Program.cs
    │   │       │       │   ├── programparameters.cs
    │   │       │       │   ├── QueryHelper.cs
    │   │       │       │   ├── StableEtwMethodIndexes.g.csv
    │   │       │       │   ├── StableEventIndexes.g.csv
    │   │       │       │   ├── StableXbfIndexGenerator.cs
    │   │       │       │   ├── StableXbfPropertyIndexes.g.csv
    │   │       │       │   ├── StableXbfTypeIndexes.g.csv
    │   │       │       │   ├── TypeHandleGenerator.cs
    │   │       │       │   ├── TypeTableOptimizer.cs
    │   │       │       │   ├── XamlGen.csproj
    │   │       │       │   ├── XamlGen.Instant.proj
    │   │       │       │   ├── XamlGen.Sources.targets
    │   │       │       │   └── Templates/
    │   │       │       │       ├── MultiFileXamlCodeGenerator.cs
    │   │       │       │       ├── T4CodeGenerator.cs
    │   │       │       │       ├── XamlCodeGenerator.cs
    │   │       │       │       ├── Code/
    │   │       │       │       │   ├── Copyright.cs
    │   │       │       │       │   ├── Copyright.tt
    │   │       │       │       │   ├── CppCodeGenerator.cs
    │   │       │       │       │   ├── Factories.cs
    │   │       │       │       │   ├── Factories.tt
    │   │       │       │       │   ├── ParameterValidationModel.cs
    │   │       │       │       │   ├── StrictCheckModel.cs
    │   │       │       │       │   ├── Core/
    │   │       │       │       │   │   ├── Bodies/
    │   │       │       │       │   │   │   ├── Activators.cs
    │   │       │       │       │   │   │   ├── Activators.tt
    │   │       │       │       │   │   │   ├── Class.cs
    │   │       │       │       │   │   │   ├── Class.tt
    │   │       │       │       │   │   │   ├── Classes.cs
    │   │       │       │       │   │   │   ├── Classes.tt
    │   │       │       │       │   │   │   ├── Enums.cs
    │   │       │       │       │   │   │   ├── Enums.tt
    │   │       │       │       │   │   │   ├── EventArgsClass.cs
    │   │       │       │       │   │   │   ├── EventArgsClass.tt
    │   │       │       │       │   │   │   ├── EventArgsClasses.cs
    │   │       │       │       │   │   │   ├── EventArgsClasses.tt
    │   │       │       │       │   │   │   ├── LiftedSources.cs
    │   │       │       │       │   │   │   ├── LiftedSources.tt
    │   │       │       │       │   │   │   ├── SimplePropertiesCommon.cs
    │   │       │       │       │   │   │   ├── SimplePropertiesCommon.tt
    │   │       │       │       │   │   │   ├── SimplePropertiesHelpersBody.cs
    │   │       │       │       │   │   │   ├── SimplePropertiesHelpersBody.tt
    │   │       │       │       │   │   │   ├── UIElement.cs
    │   │       │       │       │   │   │   ├── UIElement.tt
    │   │       │       │       │   │   │   ├── UIElementSimplePropertiesCallbacks.cs
    │   │       │       │       │   │   │   └── UIElementSimplePropertiesCallbacks.tt
    │   │       │       │       │   │   └── Headers/
    │   │       │       │       │   │       ├── Activators.cs
    │   │       │       │       │   │       ├── Activators.tt
    │   │       │       │       │   │       ├── Class.cs
    │   │       │       │       │   │       ├── Class.tt
    │   │       │       │       │   │       ├── Classes.cs
    │   │       │       │       │   │       ├── Classes.tt
    │   │       │       │       │   │       ├── DiagnosticsInterop_SimpleProperties.cs
    │   │       │       │       │   │       ├── DiagnosticsInterop_SimpleProperties.tt
    │   │       │       │       │   │       ├── EnumDefs.cs
    │   │       │       │       │   │       ├── EnumDefs.tt
    │   │       │       │       │   │       ├── Enums.cs
    │   │       │       │       │   │       ├── Enums.tt
    │   │       │       │       │   │       ├── EnumValueTables.cs
    │   │       │       │       │   │       ├── EnumValueTables.tt
    │   │       │       │       │   │       ├── EventArgsClass.cs
    │   │       │       │       │   │       ├── EventArgsClass.tt
    │   │       │       │       │   │       ├── EventArgsClasses.cs
    │   │       │       │       │   │       ├── EventArgsClasses.tt
    │   │       │       │       │   │       ├── EventArgsProperty.cs
    │   │       │       │       │   │       ├── EventArgsProperty.tt
    │   │       │       │       │   │       ├── GeneratedClasses.cs
    │   │       │       │       │   │       ├── GeneratedClasses.tt
    │   │       │       │       │   │       ├── SimplePropertiesAdapter.cs
    │   │       │       │       │   │       ├── SimplePropertiesAdapter.tt
    │   │       │       │       │   │       ├── SimplePropertiesCommon.cs
    │   │       │       │       │   │       ├── SimplePropertiesCommon.tt
    │   │       │       │       │   │       ├── SimplePropertiesMetadata.cs
    │   │       │       │       │   │       ├── SimplePropertiesMetadata.tt
    │   │       │       │       │   │       ├── UIAEnums.cs
    │   │       │       │       │   │       ├── UIAEnums.tt
    │   │       │       │       │   │       ├── XamlNativeRuntime_SimpleProperties.cs
    │   │       │       │       │   │       └── XamlNativeRuntime_SimpleProperties.tt
    │   │       │       │       │   ├── Framework/
    │   │       │       │       │   │   ├── Bodies/
    │   │       │       │       │   │   │   ├── AggregateSource.cs
    │   │       │       │       │   │   │   ├── AggregateSource.tt
    │   │       │       │       │   │   │   ├── ApplyTemplateMethod.cs
    │   │       │       │       │   │   │   ├── ApplyTemplateMethod.tt
    │   │       │       │       │   │   │   ├── AttachedProperty.cs
    │   │       │       │       │   │   │   ├── AttachedProperty.tt
    │   │       │       │       │   │   │   ├── AttachedPropertyGetterBody.cs
    │   │       │       │       │   │   │   ├── AttachedPropertyGetterBody.tt
    │   │       │       │       │   │   │   ├── AttachedPropertySetterBody.cs
    │   │       │       │       │   │   │   ├── AttachedPropertySetterBody.tt
    │   │       │       │       │   │   │   ├── Boxes.cs
    │   │       │       │       │   │   │   ├── Boxes.tt
    │   │       │       │       │   │   │   ├── CheckAPICall.cs
    │   │       │       │       │   │   │   ├── CheckAPICall.tt
    │   │       │       │       │   │   │   ├── Class.cs
    │   │       │       │       │   │   │   ├── Class.tt
    │   │       │       │       │   │   │   ├── Classes.cs
    │   │       │       │       │   │   │   ├── Classes.tt
    │   │       │       │       │   │   │   ├── ClassFactory.cs
    │   │       │       │       │   │   │   ├── ClassFactory.tt
    │   │       │       │       │   │   │   ├── Constructor.cs
    │   │       │       │       │   │   │   ├── Constructor.tt
    │   │       │       │       │   │   │   ├── DependencyProperty.cs
    │   │       │       │       │   │   │   ├── DependencyProperty.tt
    │   │       │       │       │   │   │   ├── Event.cs
    │   │       │       │       │   │   │   ├── Event.tt
    │   │       │       │       │   │   │   ├── EventArgsClass.cs
    │   │       │       │       │   │   │   ├── EventArgsClass.tt
    │   │       │       │       │   │   │   ├── EventArgsClasses.cs
    │   │       │       │       │   │   │   ├── EventArgsClasses.tt
    │   │       │       │       │   │   │   ├── FieldGetter.cs
    │   │       │       │       │   │   │   ├── FieldGetter.tt
    │   │       │       │       │   │   │   ├── FieldSetter.cs
    │   │       │       │       │   │   │   ├── FieldSetter.tt
    │   │       │       │       │   │   │   ├── Method.cs
    │   │       │       │       │   │   │   ├── Method.tt
    │   │       │       │       │   │   │   ├── MethodBody.cs
    │   │       │       │       │   │   │   ├── MethodBody.tt
    │   │       │       │       │   │   │   ├── MethodEtwStart.cs
    │   │       │       │       │   │   │   ├── MethodEtwStart.tt
    │   │       │       │       │   │   │   ├── MethodEtwStop.cs
    │   │       │       │       │   │   │   ├── MethodEtwStop.tt
    │   │       │       │       │   │   │   ├── ParameterValidation.cs
    │   │       │       │       │   │   │   ├── ParameterValidation.tt
    │   │       │       │       │   │   │   ├── PInvokeMethodBody.cs
    │   │       │       │       │   │   │   ├── PInvokeMethodBody.tt
    │   │       │       │       │   │   │   ├── Property.cs
    │   │       │       │       │   │   │   ├── Property.tt
    │   │       │       │       │   │   │   ├── PropertyGetter.cs
    │   │       │       │       │   │   │   ├── PropertyGetter.tt
    │   │       │       │       │   │   │   ├── PropertyGetterBody.cs
    │   │       │       │       │   │   │   ├── PropertyGetterBody.tt
    │   │       │       │       │   │   │   ├── PropertySetter.cs
    │   │       │       │       │   │   │   ├── PropertySetter.tt
    │   │       │       │       │   │   │   ├── PropertySetterBody.cs
    │   │       │       │       │   │   │   ├── PropertySetterBody.tt
    │   │       │       │       │   │   │   ├── StrictCheck.cs
    │   │       │       │       │   │   │   ├── StrictCheck.tt
    │   │       │       │       │   │   │   ├── Struct.cs
    │   │       │       │       │   │   │   ├── Struct.tt
    │   │       │       │       │   │   │   ├── VirtualDispatchMethodBody.cs
    │   │       │       │       │   │   │   └── VirtualDispatchMethodBody.tt
    │   │       │       │       │   │   └── Headers/
    │   │       │       │       │   │       ├── AttachedProperty.cs
    │   │       │       │       │   │       ├── AttachedProperty.tt
    │   │       │       │       │   │       ├── Class.cs
    │   │       │       │       │   │       ├── Class.tt
    │   │       │       │       │   │       ├── Classes.cs
    │   │       │       │       │   │       ├── Classes.tt
    │   │       │       │       │   │       ├── ClassFactory.cs
    │   │       │       │       │   │       ├── ClassFactory.tt
    │   │       │       │       │   │       ├── Constructor.cs
    │   │       │       │       │   │       ├── Constructor.tt
    │   │       │       │       │   │       ├── ConstructorImpl.cs
    │   │       │       │       │   │       ├── ConstructorImpl.tt
    │   │       │       │       │   │       ├── DependencyProperty.cs
    │   │       │       │       │   │       ├── DependencyProperty.tt
    │   │       │       │       │   │       ├── Event.cs
    │   │       │       │       │   │       ├── Event.tt
    │   │       │       │       │   │       ├── EventArgsClass.cs
    │   │       │       │       │   │       ├── EventArgsClass.tt
    │   │       │       │       │   │       ├── EventArgsClasses.cs
    │   │       │       │       │   │       ├── EventArgsClasses.tt
    │   │       │       │       │   │       ├── EventSourceType.cs
    │   │       │       │       │   │       ├── EventSourceType.tt
    │   │       │       │       │   │       ├── ForwarderMemberModel.cs
    │   │       │       │       │   │       ├── ForwarderMethodModel.cs
    │   │       │       │       │   │       ├── ForwarderRequestedInterface.cs
    │   │       │       │       │   │       ├── Interface.cs
    │   │       │       │       │   │       ├── Interface.tt
    │   │       │       │       │   │       ├── InterfaceEvent.cs
    │   │       │       │       │   │       ├── InterfaceEvent.tt
    │   │       │       │       │   │       ├── InterfaceForwarder.cs
    │   │       │       │       │   │       ├── InterfaceForwarder.tt
    │   │       │       │       │   │       ├── InterfaceMethod.cs
    │   │       │       │       │   │       ├── InterfaceMethod.tt
    │   │       │       │       │   │       ├── InterfaceProperty.cs
    │   │       │       │       │   │       ├── InterfaceProperty.tt
    │   │       │       │       │   │       ├── Method.cs
    │   │       │       │       │   │       ├── Method.tt
    │   │       │       │       │   │       ├── MethodForwarder.cs
    │   │       │       │       │   │       ├── MethodForwarder.tt
    │   │       │       │       │   │       ├── MethodImpl.cs
    │   │       │       │       │   │       ├── MethodImpl.tt
    │   │       │       │       │   │       ├── Property.cs
    │   │       │       │       │   │       ├── Property.tt
    │   │       │       │       │   │       ├── PropertyImpl.cs
    │   │       │       │       │   │       ├── PropertyImpl.tt
    │   │       │       │       │   │       ├── Struct.cs
    │   │       │       │       │   │       ├── Struct.tt
    │   │       │       │       │   │       ├── Synonyms.cs
    │   │       │       │       │   │       ├── Synonyms.tt
    │   │       │       │       │   │       ├── UIAEnums.cs
    │   │       │       │       │   │       ├── UIAEnums.tt
    │   │       │       │       │   │       ├── VelocityFeatureMacros.cs
    │   │       │       │       │   │       └── VelocityFeatureMacros.tt
    │   │       │       │       │   └── Phone/
    │   │       │       │       │       ├── PhoneCppCodeGenerator.cs
    │   │       │       │       │       ├── Bodies/
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyEnum.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyEnum.tt
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyObject.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyObject.tt
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyReference.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyReference.tt
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyString.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyString.tt
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyValue.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetterBodyValue.tt
    │   │       │       │       │       │   ├── AttachedPropertyGetValue.cs
    │   │       │       │       │       │   ├── AttachedPropertyGetValue.tt
    │   │       │       │       │       │   ├── AttachedPropertyImpl.cs
    │   │       │       │       │       │   ├── AttachedPropertyImpl.tt
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyEnum.cs
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyEnum.tt
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyObject.cs
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyObject.tt
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyReference.cs
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyReference.tt
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyString.cs
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyString.tt
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyValue.cs
    │   │       │       │       │       │   ├── AttachedPropertySetterBodyValue.tt
    │   │       │       │       │       │   ├── AttachedPropertySetValue.cs
    │   │       │       │       │       │   ├── AttachedPropertySetValue.tt
    │   │       │       │       │       │   ├── Class.cs
    │   │       │       │       │       │   ├── Class.tt
    │   │       │       │       │       │   ├── ClassExplicitOverrides.cs
    │   │       │       │       │       │   ├── ClassExplicitOverrides.tt
    │   │       │       │       │       │   ├── EnumGetValue.cs
    │   │       │       │       │       │   ├── EnumGetValue.tt
    │   │       │       │       │       │   ├── EnumSetValue.cs
    │   │       │       │       │       │   ├── EnumSetValue.tt
    │   │       │       │       │       │   ├── Event.cs
    │   │       │       │       │       │   ├── Event.tt
    │   │       │       │       │       │   ├── Factory.cs
    │   │       │       │       │       │   ├── Factory.tt
    │   │       │       │       │       │   ├── InitializeImpl.cs
    │   │       │       │       │       │   ├── InitializeImpl.tt
    │   │       │       │       │       │   ├── InitializeProperty.cs
    │   │       │       │       │       │   ├── InitializeProperty.tt
    │   │       │       │       │       │   ├── InterfaceMethodImpl.cs
    │   │       │       │       │       │   ├── InterfaceMethodImpl.tt
    │   │       │       │       │       │   ├── Method.cs
    │   │       │       │       │       │   ├── Method.tt
    │   │       │       │       │       │   ├── MethodBody.cs
    │   │       │       │       │       │   ├── MethodBody.tt
    │   │       │       │       │       │   ├── MethodBodyVirtualDispatch.cs
    │   │       │       │       │       │   ├── MethodBodyVirtualDispatch.tt
    │   │       │       │       │       │   ├── ObjectGetValue.cs
    │   │       │       │       │       │   ├── ObjectGetValue.tt
    │   │       │       │       │       │   ├── ObjectSetValue.cs
    │   │       │       │       │       │   ├── ObjectSetValue.tt
    │   │       │       │       │       │   ├── ParameterValidation.cs
    │   │       │       │       │       │   ├── ParameterValidation.tt
    │   │       │       │       │       │   ├── Property.cs
    │   │       │       │       │       │   ├── Property.tt
    │   │       │       │       │       │   ├── PropertyGetter.cs
    │   │       │       │       │       │   ├── PropertyGetter.tt
    │   │       │       │       │       │   ├── PropertyGetterBody.cs
    │   │       │       │       │       │   ├── PropertyGetterBody.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyDispatch.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyDispatch.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyObject.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyObject.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyPrimitive.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyPrimitive.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyReference.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyReference.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyString.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyString.tt
    │   │       │       │       │       │   ├── PropertyGetterBodyValue.cs
    │   │       │       │       │       │   ├── PropertyGetterBodyValue.tt
    │   │       │       │       │       │   ├── PropertySetter.cs
    │   │       │       │       │       │   ├── PropertySetter.tt
    │   │       │       │       │       │   ├── PropertySetterBody.cs
    │   │       │       │       │       │   ├── PropertySetterBody.tt
    │   │       │       │       │       │   ├── PropertySetterBodyBoxer.cs
    │   │       │       │       │       │   ├── PropertySetterBodyBoxer.tt
    │   │       │       │       │       │   ├── PropertySetterBodyObject.cs
    │   │       │       │       │       │   ├── PropertySetterBodyObject.tt
    │   │       │       │       │       │   ├── PropertySetterBodyReference.cs
    │   │       │       │       │       │   ├── PropertySetterBodyReference.tt
    │   │       │       │       │       │   ├── PropertySetterBodyString.cs
    │   │       │       │       │       │   ├── PropertySetterBodyString.tt
    │   │       │       │       │       │   ├── PropertySetterBodyValue.cs
    │   │       │       │       │       │   ├── PropertySetterBodyValue.tt
    │   │       │       │       │       │   ├── ReferenceTypeGetValue.cs
    │   │       │       │       │       │   ├── ReferenceTypeGetValue.tt
    │   │       │       │       │       │   ├── ReferenceTypeSetValue.cs
    │   │       │       │       │       │   ├── ReferenceTypeSetValue.tt
    │   │       │       │       │       │   ├── RuntimeClassInitialize.cs
    │   │       │       │       │       │   ├── RuntimeClassInitialize.tt
    │   │       │       │       │       │   ├── StringGetValue.cs
    │   │       │       │       │       │   ├── StringGetValue.tt
    │   │       │       │       │       │   ├── StringSetValue.cs
    │   │       │       │       │       │   ├── StringSetValue.tt
    │   │       │       │       │       │   ├── Types.cs
    │   │       │       │       │       │   ├── Types.tt
    │   │       │       │       │       │   ├── ValueTypeGetValue.cs
    │   │       │       │       │       │   ├── ValueTypeGetValue.tt
    │   │       │       │       │       │   ├── ValueTypeSetValue.cs
    │   │       │       │       │       │   ├── ValueTypeSetValue.tt
    │   │       │       │       │       │   ├── XamlTypeInfo.cs
    │   │       │       │       │       │   └── XamlTypeInfo.tt
    │   │       │       │       │       ├── Headers/
    │   │       │       │       │       │   ├── AttachedProperty.cs
    │   │       │       │       │       │   ├── AttachedProperty.tt
    │   │       │       │       │       │   ├── Class.cs
    │   │       │       │       │       │   ├── Class.tt
    │   │       │       │       │       │   ├── Constructor.cs
    │   │       │       │       │       │   ├── Constructor.tt
    │   │       │       │       │       │   ├── ConstructorImpl.cs
    │   │       │       │       │       │   ├── ConstructorImpl.tt
    │   │       │       │       │       │   ├── Event.cs
    │   │       │       │       │       │   ├── Event.tt
    │   │       │       │       │       │   ├── Factory.cs
    │   │       │       │       │       │   ├── Factory.tt
    │   │       │       │       │       │   ├── GetPropertyMethod.cs
    │   │       │       │       │       │   ├── GetPropertyMethod.tt
    │   │       │       │       │       │   ├── InterfaceMethod.cs
    │   │       │       │       │       │   ├── InterfaceMethod.tt
    │   │       │       │       │       │   ├── Method.cs
    │   │       │       │       │       │   ├── Method.tt
    │   │       │       │       │       │   ├── MethodImpl.cs
    │   │       │       │       │       │   ├── MethodImpl.tt
    │   │       │       │       │       │   ├── PrivateProperty.cs
    │   │       │       │       │       │   ├── PrivateProperty.tt
    │   │       │       │       │       │   ├── Property.cs
    │   │       │       │       │       │   ├── Property.tt
    │   │       │       │       │       │   ├── PropertyImpl.cs
    │   │       │       │       │       │   ├── PropertyImpl.tt
    │   │       │       │       │       │   ├── RuntimeClass.cs
    │   │       │       │       │       │   ├── RuntimeClass.tt
    │   │       │       │       │       │   ├── SetPropertyMethod.cs
    │   │       │       │       │       │   ├── SetPropertyMethod.tt
    │   │       │       │       │       │   ├── Types.cs
    │   │       │       │       │       │   ├── Types.tt
    │   │       │       │       │       │   ├── XamlTypeInfo.cs
    │   │       │       │       │       │   └── XamlTypeInfo.tt
    │   │       │       │       │       └── Resources/
    │   │       │       │       │           ├── XamlTypeInfo.cs
    │   │       │       │       │           └── XamlTypeInfo.tt
    │   │       │       │       ├── Manifests/
    │   │       │       │       │   ├── Microsoft_Windows_DirectUI_EtwEvents.cs
    │   │       │       │       │   ├── Microsoft_Windows_DirectUI_EtwEvents.tt
    │   │       │       │       │   ├── Microsoft_Windows_Xaml_Etw.cs
    │   │       │       │       │   └── Microsoft_Windows_Xaml_Etw.tt
    │   │       │       │       ├── Metadata/
    │   │       │       │       │   ├── ClassActivationEntry.cs
    │   │       │       │       │   ├── ClassActivationEntry.tt
    │   │       │       │       │   ├── ClassNameInfoEntry.cs
    │   │       │       │       │   ├── ClassNameInfoEntry.tt
    │   │       │       │       │   ├── ClassPropertiesEntry.cs
    │   │       │       │       │   ├── ClassPropertiesEntry.tt
    │   │       │       │       │   ├── ClassTypeCheckEntry.cs
    │   │       │       │       │   ├── ClassTypeCheckEntry.tt
    │   │       │       │       │   ├── ClassTypeEntry.cs
    │   │       │       │       │   ├── ClassTypeEntry.tt
    │   │       │       │       │   ├── Copyright.cs
    │   │       │       │       │   ├── Copyright.tt
    │   │       │       │       │   ├── DependencyObjectTraits.cs
    │   │       │       │       │   ├── DependencyObjectTraits.tt
    │   │       │       │       │   ├── DynamicMetadataBody.cs
    │   │       │       │       │   ├── DynamicMetadataBody.tt
    │   │       │       │       │   ├── EnterPropertyEntry.cs
    │   │       │       │       │   ├── EnterPropertyEntry.tt
    │   │       │       │       │   ├── EnumActivationEntry.cs
    │   │       │       │       │   ├── EnumActivationEntry.tt
    │   │       │       │       │   ├── EnumNameInfoEntry.cs
    │   │       │       │       │   ├── EnumNameInfoEntry.tt
    │   │       │       │       │   ├── EnumPropertiesEntry.cs
    │   │       │       │       │   ├── EnumPropertiesEntry.tt
    │   │       │       │       │   ├── EnumTypeCheckEntry.cs
    │   │       │       │       │   ├── EnumTypeCheckEntry.tt
    │   │       │       │       │   ├── EnumTypeEntry.cs
    │   │       │       │       │   ├── EnumTypeEntry.tt
    │   │       │       │       │   ├── Indexes.cs
    │   │       │       │       │   ├── Indexes.tt
    │   │       │       │       │   ├── MetadataCodeGenerator.cs
    │   │       │       │       │   ├── NamespaceEntry.cs
    │   │       │       │       │   ├── NamespaceEntry.tt
    │   │       │       │       │   ├── ObjectPropertyEntry.cs
    │   │       │       │       │   ├── ObjectPropertyEntry.tt
    │   │       │       │       │   ├── PropertyEntry.cs
    │   │       │       │       │   ├── PropertyEntry.tt
    │   │       │       │       │   ├── PropertyRuntimeDataEntry.cs
    │   │       │       │       │   ├── PropertyRuntimeDataEntry.tt
    │   │       │       │       │   ├── RenderPropertyEntry.cs
    │   │       │       │       │   ├── RenderPropertyEntry.tt
    │   │       │       │       │   ├── StableXbfIndexes.cs
    │   │       │       │       │   ├── StableXbfIndexes.tt
    │   │       │       │       │   ├── StableXbfIndexMapping.cs
    │   │       │       │       │   ├── StableXbfIndexMapping.tt
    │   │       │       │       │   ├── StableXbfIndexMetadata.cs
    │   │       │       │       │   ├── StableXbfIndexMetadata.tt
    │   │       │       │       │   ├── StaticMetadataBody.cs
    │   │       │       │       │   ├── StaticMetadataBody.tt
    │   │       │       │       │   ├── TypeCheckData.cs
    │   │       │       │       │   ├── TypeCheckData.tt
    │   │       │       │       │   ├── TypeNameEntry.cs
    │   │       │       │       │   ├── TypeNameEntry.tt
    │   │       │       │       │   ├── TypeTableHeader.cs
    │   │       │       │       │   ├── TypeTableHeader.tt
    │   │       │       │       │   ├── TypeTableSlots.cs
    │   │       │       │       │   ├── TypeTableSlots.tt
    │   │       │       │       │   └── XbfMetadataCodeGenerator.cs
    │   │       │       │       └── ModernIDL/
    │   │       │       │           ├── Attribute.cs
    │   │       │       │           ├── Attribute.tt
    │   │       │       │           ├── Class.cs
    │   │       │       │           ├── Class.tt
    │   │       │       │           ├── Constructor.cs
    │   │       │       │           ├── Constructor.tt
    │   │       │       │           ├── Contract.cs
    │   │       │       │           ├── Contract.tt
    │   │       │       │           ├── Copyright.cs
    │   │       │       │           ├── Copyright.tt
    │   │       │       │           ├── Delegate.cs
    │   │       │       │           ├── Delegate.tt
    │   │       │       │           ├── Enum.cs
    │   │       │       │           ├── Enum.tt
    │   │       │       │           ├── Group.cs
    │   │       │       │           ├── Group.tt
    │   │       │       │           ├── Interface.cs
    │   │       │       │           ├── Interface.tt
    │   │       │       │           ├── MemberModel.cs
    │   │       │       │           ├── MethodModel.cs
    │   │       │       │           ├── ModelExtensionMethods.cs
    │   │       │       │           ├── ModernIDLCodeGenerator.cs
    │   │       │       │           ├── PropertyModel.cs
    │   │       │       │           ├── ReferenceAssembly.tt
    │   │       │       │           ├── RequestedInterface.cs
    │   │       │       │           ├── Struct.cs
    │   │       │       │           └── Struct.tt
    │   │       │       └── XamlOM/
    │   │       │           ├── GlobalSuppressions.cs
    │   │       │           ├── InternalsVisibleTo.cs
    │   │       │           ├── ProgramParameters.cs
    │   │       │           ├── XamlOM.csproj
    │   │       │           ├── XamlOM.Instant.proj
    │   │       │           ├── XamlOM.Sources.targets
    │   │       │           ├── Builders/
    │   │       │           │   ├── AllowCrossThreadAccess.cs
    │   │       │           │   ├── Attached.cs
    │   │       │           │   ├── ClassFlags.cs
    │   │       │           │   ├── CodeGen.cs
    │   │       │           │   ├── CollectionType.cs
    │   │       │           │   ├── Comment.cs
    │   │       │           │   ├── ContentProperty.cs
    │   │       │           │   ├── Contract.cs
    │   │       │           │   ├── CoreBaseType.cs
    │   │       │           │   ├── CoreEnumValue.cs
    │   │       │           │   ├── CoreType.cs
    │   │       │           │   ├── DefaultOverload.cs
    │   │       │           │   ├── DependencyPropertyModifier.cs
    │   │       │           │   ├── Deprecated.cs
    │   │       │           │   ├── DXamlComposability.cs
    │   │       │           │   ├── DXamlIdlGroup.cs
    │   │       │           │   ├── DXamlModifier.cs
    │   │       │           │   ├── DXamlTypeTableBaseType.cs
    │   │       │           │   ├── EnumFlags.cs
    │   │       │           │   ├── EventFlags.cs
    │   │       │           │   ├── EventHandlerType.cs
    │   │       │           │   ├── FieldBacked.cs
    │   │       │           │   ├── ForceSealed.cs
    │   │       │           │   ├── ForceVirtual.cs
    │   │       │           │   ├── Guids.cs
    │   │       │           │   ├── HideFromOldCodeGen.cs
    │   │       │           │   ├── Implements.cs
    │   │       │           │   ├── InstanceCountTelemetry.cs
    │   │       │           │   ├── MethodFlags.cs
    │   │       │           │   ├── Modifier.cs
    │   │       │           │   ├── Module.cs
    │   │       │           │   ├── Mutator.cs
    │   │       │           │   ├── NameAttributes.cs
    │   │       │           │   ├── Namespace.cs
    │   │       │           │   ├── NativeCategory.cs
    │   │       │           │   ├── NativeComment.cs
    │   │       │           │   ├── NativeCondition.cs
    │   │       │           │   ├── NativeOnly.cs
    │   │       │           │   ├── NativeStorageType.cs
    │   │       │           │   ├── OldCodeGenBaseType.cs
    │   │       │           │   ├── Optional.cs
    │   │       │           │   ├── OptionalReturnValue.cs
    │   │       │           │   ├── OrderHint.cs
    │   │       │           │   ├── PartialFactory.cs
    │   │       │           │   ├── PInvoke.cs
    │   │       │           │   ├── Platform.cs
    │   │       │           │   ├── PreserveThemeResourceExtension.cs
    │   │       │           │   ├── PrivateApiContract.cs
    │   │       │           │   ├── PropertyChange.cs
    │   │       │           │   ├── PropertyFlags.cs
    │   │       │           │   ├── PropertyInitialization.cs
    │   │       │           │   ├── PropertyKind.cs
    │   │       │           │   ├── ReadOnly.cs
    │   │       │           │   ├── RequiresMultipleAssociationCheck.cs
    │   │       │           │   ├── ReturnTypeIsOut.cs
    │   │       │           │   ├── Simple.cs
    │   │       │           │   ├── Strict.cs
    │   │       │           │   ├── TemplatePart.cs
    │   │       │           │   ├── ThreadingModel.cs
    │   │       │           │   ├── TypeFlags.cs
    │   │       │           │   ├── TypeTable.cs
    │   │       │           │   ├── UnderlyingDependencyProperty.cs
    │   │       │           │   ├── Unnamed.cs
    │   │       │           │   ├── VelocityFeature.cs
    │   │       │           │   ├── Version.cs
    │   │       │           │   └── VersionPostfix.cs
    │   │       │           ├── Model/
    │   │       │           │   ├── AccessKeys.cs
    │   │       │           │   ├── Contracts.cs
    │   │       │           │   ├── Declares.cs
    │   │       │           │   ├── FrameworkElement.cs
    │   │       │           │   ├── FrameworkElementEx.cs
    │   │       │           │   ├── FullWindowMediaRoot.cs
    │   │       │           │   ├── MediaPlayerElement.cs
    │   │       │           │   ├── MediaPlayerPresenter.cs
    │   │       │           │   ├── Microsoft.Internal.FrameworkUdk.cs
    │   │       │           │   ├── Microsoft.UI.Composition.cs
    │   │       │           │   ├── Microsoft.UI.Composition.SystemBackdrops.cs
    │   │       │           │   ├── Microsoft.UI.Content.cs
    │   │       │           │   ├── Microsoft.UI.cs
    │   │       │           │   ├── Microsoft.UI.Dispatching.cs
    │   │       │           │   ├── Microsoft.UI.Input.cs
    │   │       │           │   ├── Microsoft.UI.Windowing.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Automation.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Automation.Peers.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Automation.Provider.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Automation.Text.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Collections.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.ComponentModel.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Controls.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Controls.Primitives.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Data.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Documents.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Hosting.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Input.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Internal.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Interop.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Markup.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Media.Animation.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Media.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Media.Imaging.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Media.Media3D.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Motion.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Navigation.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Printing.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Resources.cs
    │   │       │           │   ├── Microsoft.UI.Xaml.Shapes.cs
    │   │       │           │   ├── Microsoft.Windows.ApplicationModel.Resources.cs
    │   │       │           │   ├── MS.Internal.Automation.cs
    │   │       │           │   ├── Namespaces.cs
    │   │       │           │   ├── PanelEx.cs
    │   │       │           │   ├── UIElement.cs
    │   │       │           │   ├── Windows.ApplicationModel.Activation.cs
    │   │       │           │   ├── Windows.ApplicationModel.Background.cs
    │   │       │           │   ├── Windows.ApplicationModel.Core.cs
    │   │       │           │   ├── Windows.ApplicationModel.cs
    │   │       │           │   ├── Windows.ApplicationModel.DataTransfer.cs
    │   │       │           │   ├── Windows.ApplicationModel.DataTransfer.DragDrop.cs
    │   │       │           │   ├── Windows.ApplicationModel.Search.cs
    │   │       │           │   ├── Windows.Devices.Geolocation.cs
    │   │       │           │   ├── Windows.Foundation.Collections.cs
    │   │       │           │   ├── Windows.Foundation.cs
    │   │       │           │   ├── Windows.Foundation.Metadata.cs
    │   │       │           │   ├── Windows.Foundation.Numerics.cs
    │   │       │           │   ├── Windows.Globalization.cs
    │   │       │           │   ├── Windows.Graphics.DirectX.cs
    │   │       │           │   ├── windows.graphics.imaging.cs
    │   │       │           │   ├── Windows.Graphics.Printing.cs
    │   │       │           │   ├── Windows.Media.Capture.cs
    │   │       │           │   ├── Windows.Media.Casting.cs
    │   │       │           │   ├── Windows.Media.Core.cs
    │   │       │           │   ├── Windows.Media.Playback.cs
    │   │       │           │   ├── Windows.Media.Protection.cs
    │   │       │           │   ├── Windows.Storage.cs
    │   │       │           │   ├── Windows.Storage.Streams.cs
    │   │       │           │   ├── Windows.System.cs
    │   │       │           │   ├── Windows.UI.Core.cs
    │   │       │           │   ├── Windows.UI.cs
    │   │       │           │   ├── Windows.UI.Text.cs
    │   │       │           │   └── Windows.UI.Xaml.Interop.cs
    │   │       │           ├── NewBuilders/
    │   │       │           │   ├── BuilderAttributes.cs
    │   │       │           │   ├── Contracts.cs
    │   │       │           │   ├── ExternalIdl.cs
    │   │       │           │   ├── HandWritten.cs
    │   │       │           │   ├── Helper.cs
    │   │       │           │   ├── HideFromNewCodeGen.cs
    │   │       │           │   ├── IdlAttributeTarget.cs
    │   │       │           │   ├── IdlType.cs
    │   │       │           │   ├── Imported.cs
    │   │       │           │   ├── LiftedOptions.cs
    │   │       │           │   ├── ModelFactory.cs
    │   │       │           │   ├── StubDelegate.cs
    │   │       │           │   └── TypeNameExtensions.cs
    │   │       │           └── Patterns/
    │   │       │               ├── AllowsMultipleAssociations.cs
    │   │       │               ├── AnimationPattern.cs
    │   │       │               ├── BuiltinStructPattern.cs
    │   │       │               ├── ControlPattern.cs
    │   │       │               ├── FrameworkTypePattern.cs
    │   │       │               └── WindowsTypePattern.cs
    │   │       └── win/
    │   │           ├── agcore.debug/
    │   │           │   └── CommonErrors.rc
    │   │           ├── inc/
    │   │           │   ├── PendingMessages.h
    │   │           │   ├── UIAHostEnvironmentInfo.h
    │   │           │   ├── UIAWrapper.h
    │   │           │   ├── WindowLessSiteHost.h
    │   │           │   ├── winpal.h
    │   │           │   ├── WPPTracing.h
    │   │           │   └── xcpwindow.h
    │   │           ├── shared/
    │   │           │   ├── PendingMessages.cpp
    │   │           │   ├── precomp.h
    │   │           │   ├── SafeArrayUtil.h
    │   │           │   ├── sources.props
    │   │           │   ├── UIAHostEnvironmentInfo.cpp
    │   │           │   ├── UIAWrapper.cpp
    │   │           │   ├── xcpwindow.cpp
    │   │           │   └── sl/
    │   │           │       └── shared.vcxproj
    │   │           └── UIUtils/
    │   │               ├── BrowserDesktopUIUtils.cpp
    │   │               ├── UIUtils.h
    │   │               └── winrt/
    │   │                   └── uiutils.vcxproj
    │   ├── external/
    │   │   └── inc/
    │   │       ├── gsl/
    │   │       │   ├── ReadMe.md
    │   │       │   ├── cgmanifest.json
    │   │       │   ├── gsl
    │   │       │   ├── gsl_algorithm
    │   │       │   ├── gsl_assert
    │   │       │   ├── gsl_byte
    │   │       │   ├── gsl_util
    │   │       │   ├── multi_span
    │   │       │   ├── pointers
    │   │       │   ├── span
    │   │       │   └── string_span
    │   │       └── SafeInt/
    │   │           ├── cgmanifest.json
    │   │           └── SafeInt.hpp
    │   ├── MergedWinMD/
    │   │   ├── Directory.Build.props
    │   │   ├── Directory.Build.targets
    │   │   ├── MergedWinMD.vcxproj
    │   │   └── private/
    │   │       └── MergedWinMD.vcxproj
    │   └── PackageStore/
    │       └── readme.md
    └── .github/
        ├── CODEOWNERS
        ├── PULL_REQUEST_TEMPLATE.md
        ├── ISSUE_TEMPLATE/
        │   ├── bug_report.yaml
        │   └── feature_proposal.md
        ├── policies/
        │   └── resourceManagement.yml
        └── workflows/
            ├── docs.yml
            └── similar-issues-bot.yml


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
![WinUI hero image](docs/images/header.png)

<h1 align="center">
    WinUI 3
</h1>
<p align="center">
  <a href="https://twitter.com/intent/follow?screen_name=windowsui">
    <img src="https://img.shields.io/twitter/follow/windowsui.svg?label=Follow WinUI on X" alt="Follow @windowsui" />
  </a>
</p>

<h3 align="center">
  <a href="https://aka.ms/windev">About WinUI</a>
  <span> · </span>
  <a href="https://learn.microsoft.com/windows/apps/desktop/">Documentation</a>
  <span> · </span>
  <a href="https://aka.ms/winui-releasenotes">Release notes</a>
</h3>

WinUI is a user interface layer that contains modern controls and styles for building Windows apps. The current generation is WinUI 3, which ships as part of the [Windows App SDK](https://aka.ms/winappsdk).

- **Modern UI:** WinUI embodies Fluent Design to enable intuitive, accessible, and powerful experiences and the latest user interface patterns.
- **Developers in control:** Use .NET with C# or C++ to write apps that run great on x86, x64 and ARM.
- **Optimized for modern experiences & hardware:** Create performant experiences with WinUI that are optimized for modern hardware.
- **Part of the Windows App SDK:** The [Windows App SDK](https://aka.ms/winappsdk) is a set of libraries, frameworks, components, and tools that you can use in your apps to access powerful Windows platform functionality from all kinds of apps on many versions of Windows. The Windows App SDK combines the powers of Win32 native applications alongside modern API usage techniques, so your apps light up everywhere your users are.
- **Powers key experiences in Windows:** Windows experiences and apps are built with WinUI. Its rich control set and styles make it easy to develop high-quality experiences used by millions every day.

<p align="center">
<img src="docs/images/winui_os.png" alt="Powers key experiences in Windows" width="480"/>
</br>
</p>

## 📋 Getting started with WinUI

For WinUI, your app's users must be on Windows 10 1809 - Build 17763 or newer (including Windows Insider Previews).

The full documentation of WinUI can be found on [Microsoft Learn](https://learn.microsoft.com/windows/apps/desktop/):
- [Get started with WinUI](https://learn.microsoft.com/windows/apps/get-started/start-here)
- [Build your first WinUI app](https://learn.microsoft.com/windows/apps/how-tos/hello-world-winui3)
- [WinUI & Windows App SDK samples](https://github.com/microsoft/WindowsAppSDK-Samples)

</br>

## 🖼️ WinUI 3 Gallery
Make sure to also check out the [WinUI 3 Gallery](https://aka.ms/winui-gallery), our interactive sample experience showing everything you can do with WinUI.

<p align="center">
<img src="docs/images/winui-gallery.png" alt="WinUI 3 Gallery" width="400"/>
</p>
<p align="center">
<a href="https://apps.microsoft.com/detail/WinUI%203%20Gallery/9P3JFPWWDZRC?launch=true
	&mode=mini">
	<img src="/docs/images/storeBadge.png" width="200"/>
</a>
</p>
</br>

## 📺 WinUI Community Call
The WinUI Community Call is your opportunity to learn about WinUI and to engage with the WinUI team and community. Join us online on YouTube at the [Windows Developer channel](https://www.youtube.com/playlist?list=PLI_J2v67C23ZqsolUDaHoFkF1GKvGrttB).

</br>

## 📢 Contributing to WinUI

The WinUI team welcomes your feedback! To understand how we handle incoming feature requests and bugs, please see our [contribution handling](docs/contribution_handling.md) guidelines.

For information on how to contribute, please see [Contributing to WinUI](CONTRIBUTING.md).

</br>

## 🛣️ Roadmap

For info on the WinUI release schedule and high level plans please see the [WinUI roadmap](https://aka.ms/winappsdk/plans).

</br>

## 🔧 WinUI 2 (for UWP)
WinUI 2 is a library of controls that provides Microsoft UI controls and features for [UWP apps](https://docs.microsoft.com/windows/uwp/index). Learn more about WinUI 2 [here](https://aka.ms/winui2) or download the source code [here](https://github.com/microsoft/microsoft-ui-xaml/tree/winui2/main).

You can get the WinUI 2 Gallery [on the Microsoft Store](https://www.microsoft.com/store/productId/9MSVH128X2ZT?ocid=pdpshare) and see the source code [here](https://github.com/microsoft/WinUI-Gallery/tree/winui2).
</br>

### Data/Telemetry

This project collects usage data and sends it to Microsoft to help improve our products and services. Note, however, that no data collection is performed when using your private builds.

### Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).

For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.



================================================
FILE: CODE_OF_CONDUCT.md
================================================
# Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).

For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


================================================
FILE: CONTRIBUTING.md
================================================
# Contributing to the Windows UI Library

We welcome your input and contributions to all aspects of WinUI, including bug reports, doc updates, feature proposals, and API spec discussions.

This document contains general guidance. More specific guidance is included in the documents linked below.

Note that all community interactions must abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

## How we work with contributions

For reporting security issues please see the [Security Policy](docs/SECURITY.md).

Contributions from the community in the form of feature requests and bugs are handled according to our [contribution handling](docs/contribution_handling.md) guidelines.

## New contributors

We mark the most straightforward issues with labels. These issues are the place to start if you are interested in contributing but new to the codebase.

* [good first issues](https://github.com/Microsoft/microsoft-ui-xaml/labels/good%20first%20issue)
* [help wanted](https://github.com/Microsoft/microsoft-ui-xaml/labels/help%20wanted)

Another great way to help is by voting and commenting on feature proposals:

* [feature request](https://github.com/Microsoft/microsoft-ui-xaml/labels/feature%20request)

## Code contribution guidelines

### Proposing new public APIs or UI

Please follow the [New Feature or API Process](docs/feature_proposal_process.md) before adding, removing, or changing public APIs or UI.
All new public APIs, new UI, or breaking changes to existing features **must** go through that process before submitting code changes.
You don't need to follow that process for bug fixes or other small changes.

### Contribution bar

The WinUI team accepts code changes that improve WinUI or fix bugs, as long as they follow the processes outlined below and broadly align with our [roadmap](docs/roadmap.md).

While we strive to accept all community contributions that meet the guidelines outlined here, please note that we may not merge changes that have narrowly-defined benefits due to compatibility risks and maintenance costs. We may also revert changes if they are found to be breaking.

### Code contribution process

For details see:

* [Setup and build environment](docs/developer_guide.md#Prerequisites)
* [Source code structure](docs/source_code_structure.md)
* [Contribution workflow](docs/contribution_workflow.md)
* [Coding style and conventions](docs/code_style_and_conventions.md)

### Contributor License Agreement

Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

### Copying files from other projects

The following rules must be followed for PRs that include files from another project:

* The license of the file is [permissive](https://en.wikipedia.org/wiki/Permissive_free_software_licence).
* The license of the file is left intact.
* The contribution is correctly attributed in the [3rd party notices](https://github.com/dotnet/coreclr/blob/master/THIRD-PARTY-NOTICES.TXT)
file in the repository, as needed.

## Documentation and usage samples

You can also read and contribute to the WinUI documentation here:
https://docs.microsoft.com/uwp/toolkits/winui

You can find usage examples of the controls available in WinUI in the Xaml Controls Gallery app:
 https://github.com/Microsoft/Xaml-Controls-Gallery/

 which can also be installed from the Windows Store:
 https://www.microsoft.com/p/xaml-controls-gallery/9msvh128x2zt

 ## API spec discussions

Before new features are added to WinUI, we always perform a thorough API review and spec discussion. This can range from a single new API to an entire new control featuring dozens of new APIs. Joining such a spec discussion is a great opportunity for developers to help ensuring that new WinUI APIs will look and feel natural. In addition, spec discussions are the follow-up to feature proposals and will go into much finer details than the initial proposal. As such, taking part in these discussions gives developers the chance to be involved in the complete development process of new WinUI features - from their initial high-level inception right down to specific implementation/behavior details. These discussions take place in the WInUI repository, i.e. this repository.



================================================
FILE: CONTRIBUTING_feedback_and_requests.md
================================================
# Contributing ideas, feedback, and requests

The WinUI team greatly values public feedback. We combine this feedback with our own internal strategy goals, weighing it alongside our existing commitments, resources, and private partnerships, to deliver maximum value for you.

The guide below outlines how you can formulate this feedback for maximum effect and influence on WinUI's direction.

## Phrasing constructively

When experiencing a pain-point, it can be natural to focus on the negatives and resolving things from the perspective of the negative. However, telling the team what you'd like to *prevent* is less helpful and actionable than telling the team what you'd like to *achieve*.

Your feedback is most effective when it is a constructive call to action on the team, and is clear and detailed – especially on the "why" so that we can make sure whatever it is that we arrive at together appropriately focuses on your goal and your intended outcome from start to finish.


**Examples of constructively phrased feedback:**

Instead of:

  - The state of the platform is disappointing. I am not going to consider WinUI until my trust has been earned.

Try this:
  - Deprecation of past frameworks has left me burned. The following would go a long way in earning my trust because my company is trying to launch an app next year and will need it supported for at least 5 more:
    - OSS
    - High-confidence 5-year roadmap
    - Guaranteed support timeline

    This feedback provides clear actionable items that the WinUI team can take into consideration and address.


## Sample areas where your feedback can have large impact

- ### Features
  - It's very helpful to specify the "why" behind your request, even if it seems obvious. Comparisons can help, but shouldn't replace explanation.
  - Ex: "I need `<`feature`>` so that I can achieve `<`goal`>`. Otherwise, I have to `<`alternative`>`."

  There are also usually great opportunities to have feature-related impact in our [spec repo](https://github.com/microsoft/microsoft-ui-xaml-specs/tree/master). Here, you can give direct feedback and help shape the new features and APIs that we're currently building.

- ### Future/Roadmap
  - We strive to be transparent about our [product roadmap](https://aka.ms/winui3/feature-roadmap). Great examples of feedback to help us achieve this are:
    - "I'd like to know the roadmap through `<`timeframe`>`. Otherwise, I can't do `<`goal`>`. "
    - "The roadmap `<`certain aspect - e.g., changes too much, not detailed enough, etc.`>`prevents me from being able to do `<`goal`>`. If you would instead `<`proposed alternative`>`, that would result in `<`clear benefit`>`."

- ### Ecosystem
  - It's helpful to be complete in explaining what another solution achieves for you and why it is important to you.
    - Ex:"I'd like WinUI 3 to work with `<`framework, language, library, technology, etc.`>`. Without this, I can't do `<`goal`>`."

- ### Prioritization within WinUI
  -  There is often trade-off required when adjusting priorities - please be clear in comparing what is more important vs. less important to you, and the reason why.
      - Ex: "I think `<`specific area or feature set`>` should be prioritized before `<`other specific area or feature set`>` so that I can achieve `<`goal`>`. Without this, I have to `<`alternative`>`. "

- ### Engagement
  - Engagement includes feedback about learning materials and resources. It is always helpful to know where you prefer to be engaged and how you prefer to learn.
    - "I would like to hear more about `<`specific topic`>` in `<`resource`>` so that I can achieve `<`goal`>`."
    - "`<`Resource`>` could be more inclusive and accessible if you considered `<`alternative`>` because `<`benefit`>`. Have you considered making these changes?"

   Many of the resources we provide are also open source themselves! It can sometimes be more effective to leave feedback on the more specific repo. This includes:
    - [documentation](https://github.com/MicrosoftDocs/windows-uwp)
    - [website (`gh-pages` branch of this repo)](https://github.com/microsoft/microsoft-ui-xaml/tree/gh-pages)
    - [Xaml Controls Gallery (sample app)](https://github.com/microsoft/Xaml-Controls-Gallery/tree/master)


- ### Team Process
  - Team process includes feedback about our repo and overall communication. Suggestions for improvement and proposed alternatives are very helpful here.
    - Ex: "`<`specific aspect of team process - e.g., response frequency, format`>` of the repo is making it hard for me to achieve `<`goal`>`. Please consider doing `<`alternative`>` instead because that would help `<`action`>`"


## Mutual respect

We strive to be respectful & empathetic toward each other, and we extend this to our fantastic community as well.

Our conduct guidelines help to ensure that discourse and feedback follows this same pattern of respect & empathy, and they also make it clear that non-constructive or hostile feedback is unacceptable. By following these guidelines, we can all enjoy the mutual respect that each WinUI team member, and each community member, deserve.

Refer to our [conduct guidelines](https://github.com/microsoft/microsoft-ui-xaml/blob/main/CODE_OF_CONDUCT.md) for more guidance here.



================================================
FILE: LICENSE
================================================
    MIT License

    Copyright (c) Microsoft Corporation. All rights reserved.

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE



================================================
FILE: privacy.md
================================================
# Data Collection

The software may collect information about you and your use of the software and send it to Microsoft. Microsoft may use this information to provide services and improve our products and services. You may turn off the telemetry as described in the repository. There are also some features in the software that may enable you and Microsoft to collect data from users of your applications. If you use these features, you must comply with applicable law, including providing appropriate notices to users of your applications together with a copy of Microsoft's privacy statement. Our privacy statement is located at https://go.microsoft.com/fwlink/?LinkID=824704. You can learn more about data collection and use in the help documentation and our privacy statement. Your use of the software operates as your consent to these practices.

For more information on telemetry implementation see the [developer guide](docs/developer_guide.md#Telemetry).



================================================
FILE: SECURITY.md
================================================
<!-- BEGIN MICROSOFT SECURITY.MD V0.0.5 BLOCK -->

## Security

Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/Microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [our GitHub organizations](https://opensource.microsoft.com/).

If you believe you have found a security vulnerability in any Microsoft-owned repository that meets [Microsoft's definition of a security vulnerability](https://docs.microsoft.com/en-us/previous-versions/tn-archive/cc751383(v=technet.10)), please report it to us as described below.

## Reporting Security Issues

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them to the Microsoft Security Response Center (MSRC) at [https://msrc.microsoft.com/create-report](https://msrc.microsoft.com/create-report).

If you prefer to submit without logging in, send email to [secure@microsoft.com](mailto:secure@microsoft.com).  If possible, encrypt your message with our PGP key; please download it from the [Microsoft Security Response Center PGP Key page](https://www.microsoft.com/en-us/msrc/pgp-key-msrc).

You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your original message. Additional information can be found at [microsoft.com/msrc](https://www.microsoft.com/msrc).

Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:

  * Type of issue (e.g. buffer overflow, SQL injection, cross-site scripting, etc.)
  * Full paths of source file(s) related to the manifestation of the issue
  * The location of the affected source code (tag/branch/commit or direct URL)
  * Any special configuration required to reproduce the issue
  * Step-by-step instructions to reproduce the issue
  * Proof-of-concept or exploit code (if possible)
  * Impact of the issue, including how an attacker might exploit the issue

This information will help us triage your report more quickly.

If you are reporting for a bug bounty, more complete reports can contribute to a higher bounty award. Please visit our [Microsoft Bug Bounty Program](https://microsoft.com/msrc/bounty) page for more details about our active programs.

## Preferred Languages

We prefer all communications to be in English.

## Policy

Microsoft follows the principle of [Coordinated Vulnerability Disclosure](https://www.microsoft.com/en-us/msrc/cvd).

<!-- END MICROSOFT SECURITY.MD BLOCK -->


================================================
FILE: docs/contribution_handling.md
================================================
# WinUI Repo Contribution Handling

The WinUI repo is intended as a place for the WinUI team to gather community feedback, discuss issues with the community, and provide insight into bug fixes that the team is working on before updates are released. Here, we'll outline how we handle feature requests and bugs that the community opens.

## Issues

Feature requests and bugs are tracked as GitHub issues.

For reporting security issues please see the [Security Policy](SECURITY.md).

For all other bugs and general issues please [file a new issue](https://github.com/Microsoft/microsoft-ui-xaml/issues/new/choose) using the Bug Report template.

Please file questions and discussions as discussions, not issues.

## Feature Proposals

Feature proposals for WinUI 3 are categorized based on the likely timeframe in which the feature team can consider them.

1. 	Short-term, less than a year
2.	Long-term, not likely in the next year

All feature proposals are automatically categorized as long-term and unlikely to be considered, although the WinUI team might change the priority based on customer and business needs. If the WinUI team does close a feature proposal, we will indicate the reason why and how it fits into our plans. Closing a proposal does not mean that the team will never consider it. We encourage the community to add comments or interact with a proposal at any time, even a closed one, to signal its importance to the team.

### Feature Planning

Our long term vision for WinUI is to be the best UX/UI native framework for Windows PCs that provides premium visuals, motion, accessibility, usability, and support for all input modalities.

The current details of what we plan long-term are shaped by evolving priorities that are subject to frequent change and are often confidential based on business and customer needs. However, we are happy to share our immediate plans for what's coming next in the next major release once the feature list is ready. Additionally, preview and experimental releases provide opportunities for the community to see what's new and what's changing on a more frequent basis.

For more info about our longer-term planning, see the [Windows App SDK feature roadmap](https://github.com/microsoft/WindowsAppSDK/blob/main/docs/roadmap.md). This page will be updated generally right after a major release, when the features for the next release are solidified enough to share.

## Bugs

### WinUI 2

The WinUI team is currently spending its time on WinUI 3. To help with this focus, any new bug filed against WinUI 2 is closed in this repo unless it's a security issue or is critical to our business priorities.

### WinUI 3

WinUI 3 bugs are triaged and prioritized based on how much the bug impacts one or more of the following criteria. If a bug has lower impact, it is less likely to be considered for fixing.

- Reliability
- Data corruption or loss
- Functionality (such as a major regression)
- Security
- Compatibility with applications
- User experience/usability
- Performance
- Compliance (such as legal compliance)
- Accessibility
- Build and deployment

Bugs filed in relation to preview and experimental releases are triaged with the same criteria as stable releases and are intended to assist in identifying and fixing those bugs before they make their way to a stable release.

Bugs filed on GitHub will be automatically mirrored to our internal bug tracking system and updates to them are automatically mirrored back to GitHub with appropriate tags. This way, the bugs we're working on and their progress are transparent. The only information we will reflect from our system externally is the state and release of the bug, not all the fine details; if a bug is resolved or closed, that's reflected on GitHub, and as bugs are worked on, the release for that fix will be reflected with a milestone on GitHub.


================================================
FILE: docs/contribution_workflow.md
================================================
# Contribution Workflow

You can contribute to WinUI with issues and PRs. Simply filing issues for
problems you encounter is a great way to contribute. Contributing
implementations is greatly appreciated.

Good issues to work on are issues tagged with
[help wanted](https://github.com/microsoft/microsoft-ui-xaml/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) or
[good first issue](https://github.com/microsoft/microsoft-ui-xaml/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22).

## Suggested Workflow

We use and recommend the following workflow:
1. Create an issue for your work.
    * You can skip this step for trivial changes.
    * Reuse an existing issue on the topic, if there is one.
    * If your change adds or changes public API or UI, first follow
    the [New Feature or API Process](feature_proposal_process.md).
    * Clearly state that you are going to take on implementing it, if that's
    the case. You can request that the issue be assigned to you. Note: The
    issue filer and the implementer don't have to be the same person.
2. Create a personal fork of the repository on GitHub (if you don't already
have one).
3. Create a branch off of main (`git checkout -b mybranch`).
    * Name the branch so that it clearly communicates your intentions.
    * Branches are useful since they isolate your changes from incoming changes
    from upstream. They also enable you to create multiple PRs from the same
    fork.
4. Make and commit your changes.
    * Please follow our [Commit Messages](#Commit-Messages)
    guidance.
5. Add new tests corresponding to your change, if applicable.
6. Build the repository with your changes.
    * Make sure that the builds are clean.
    * Make sure that the tests are all passing, including your new tests.
7. Create a pull request (PR) against the upstream repository's main branch.
    * Push your changes to your fork on GitHub (if you haven't already).
    - Note: It is okay for your PR to include a large number of commits. Once
    your change is accepted, you will be asked to squash your commits into one
    or some appropriately small number of commits before your PR is merged.
    - Note: It is okay to create your PR as "[WIP]" on the upstream repo before
    the implementation is done. This can be useful if you'd like to start the
    feedback process while you're still working on the implementation. State
    that this is the case in the initial PR comment.

## DOs and DON'Ts

Please do:
* **DO** follow existing coding style.
* **DO** give priority to the current style of the project or file you're
changing even if it diverges from the general guidelines.
* **DO** include tests when adding new features. When fixing bugs, start with
adding a test that highlights how the current behavior is broken.
* **DO** keep the discussions focused. When a new or related topic comes up
it's often better to create new issue than to side track the discussion.
* **DO** blog and tweet (or whatever) about your contributions, frequently!

Please do not:
* **DON'T** make PRs for style changes.
* **DON'T** surprise us with big pull requests. Instead, file an issue and
start a discussion so we can agree on a direction before you invest a large
amount of time.
* **DON'T** commit code that you didn't write (attesting this is part of the
[CLA](https://cla.microsoft.com)). If you find code that you think is a good
fit to add to WinUI, file an issue and start a discussion before proceeding.
* **DON'T** submit PRs that alter licensing related files or headers. If you
believe there's a problem with them, file an issue and we'll be happy to
discuss it.
* **DON'T** add or change public API or UI without filing an issue and
discussing it first: see the [New Feature or API Process](feature_proposal_process.md).

## Checks

Each pull request to `main` must pass the following checks:

###### [WinUI-Public-MUX-PR](https://dev.azure.com/ms/microsoft-ui-xaml/_build?definitionId=21)

This pipeline builds your change and runs automated tests.
These tests should match what you're able to run with local automated testing using Test Explorer.
It also creates a NuGet package to match your change.

###### license/cla

This check confirms that you have completed the [CLA](https://cla.microsoft.com).


Pull requests from a fork will not automatically trigger all of these checks. A member of the WinUI
team can trigger the Azure Pipeline checks by commenting `/azp run` on the PR. The Azure Pipelines
bot will then trigger the build.

In order to have PRs automatically merge once all checks have passed (including optional
checks), maintainers can apply the [auto merge](https://github.com/Microsoft/microsoft-ui-xaml/labels/auto%20merge)
label. It will take effect after an 8 hour delay.

### Other Pipelines

Unlike the above checks these are not required for all PRs, but you may see them on some PRs so we
define them here:

#### [WinUI-Public-MUX-CI](https://dev.azure.com/ms/microsoft-ui-xaml/_build?definitionId=20)

This pipeline extends [WinUI-Public-MUX-PR](https://dev.azure.com/ms/microsoft-ui-xaml/_build?definitionId=21)
to validate more platforms, adding Debug and ARM. It is run after your changes are merged to
main.

## Commit Messages

Please format commit messages as follows (based on [A Note About Git Commit Messages](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)):

```
Summarize change in 50 characters or less

Provide more detail after the first line. Leave one blank line below the
summary and wrap all lines at 72 characters or less.

If the change fixes an issue, leave another blank line after the final
paragraph and indicate which issue is fixed in the specific format below.

Fix #42
```


================================================
FILE: docs/debugging_buildfailures.md
================================================
# Capturing binlogs
Capturing and providing binlog files can help with debugging build and packaging issues. In order to collect binlogs, please follow these steps:

Generally, it is encouraged to collect binlog files through the CLI of MSBuild as they tend to be easier to diagnose, but both methods of creating binlog files are fine.

## Collecting binlogs through Visual Studio
1. Download the VS Project System Tools extension: [For VS 2019](https://marketplace.visualstudio.com/items?itemName=VisualStudioProductTeam.ProjectSystemTools) | [For VS 2022](https://marketplace.visualstudio.com/items?itemName=VisualStudioProductTeam.ProjectSystemTools2022)
3. Set the **Build Log File** verbosity to `Diagnostics`: `Tools->Options->Projects and Solutions->MSBuild project build log file verbosity`:<br/>
![Screenshot of Build and run options](./images/binlog-images/buildandrunoptions.png)

3. Go to View->Other Windows->Build Logging:<br/>
![Screenshot of Build Logging menu item](./images/binlog-images/buildlogging_menuitem.png)

4. To start taking logs, press the play button:<br/>
![Screenshot of Build Logging window](./images/binlog-images/buildlogging_window.png)

5. Run the steps that resulted in errors, e.g. building your project. The steps that failed show up as "Failed". Those files have the file extension ".binlog" and can be shared to help debugging build and packaging issues.

## Collection binlogs through the command line

To collect binlogs through the command line interface of MSBuild using the Visual Studio command line, you can use the `-bl` switch. Note that those commands should be used inside the Visual Studio command line.

For example, to build your solution in x86 release and collect binlogs, you can use the following:

`msbuild /p:Platform=x86 /p:Configuration=Release /bl`

If you encounter issues while creating app packages, you can use the following command to simulate collect binlogs:

`msbuild /p:AppxBundlePlatforms=x86 /p:Platform=x86 /p:Configuration=Release /p:BuildAppxUploadPackageForUap=true /bl`

In case of investigating build failures with the WinUI source code, please run the `devcmd.cmd` script at the root of the repository first.



================================================
FILE: docs/debugging_crashes.md
================================================
# Debugging Crashes

This document covers the following topics:
1. [How to get a crash dump](debugging_crashes.md#How-to-get-a-crash-dump)
2. [How to get a good callstack for crashes](debugging_crashes.md#How-to-get-a-good-callstack-for-crashes)

## How to get a crash dump

### Using Visual Studio

If the crash is in your app which you can launch from Visual Studio, or if you can attach to the app with Visual Studio prior to the crash, then you can use these steps:
1. If launching the app from Visual Studio, set Visual Studio to debug either as "Native Only" or as "Mixed (Managed and Native)" before launching the app.
If attaching to a running app, in the "Attach to Process" dialog be sure to change the "Attach to:" settings to include "Native" if it isn't shown for the process, and then attach.
2. Run the repro.
3. When the crash occurs and Visual Studio breaks in, select "Save Dump As..." from the Debug menu to save the dump.

Note: In some cases, Visual Studio's Diagnostic Tools may cause a crash which only occurs when debugging in Visual Studio with the Diagnostic Tools enabled.
This type of crash might manifest as a crash in your app, usually with a function name containing `Diagnostics` somewhere on the stack, or it may include a crash in a separate ScriptedSandbox64.exe process. If this situation appears to be happening, try turning off Tools | Options | Debugging | "Enable Diagnostic Tools while debugging" in Visual Studio settings and then run your scenario.

### Using WinDbg

In [WinDbg](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/debugger-download-tools), use `.dump /ma <filename>` to save a full memory dump to the specified file when the crash happens.
* If the crash happens sometime after app launch, then you can launch the app, attach to the app with WinDbg, and then do the repro steps to hit the crash.
* If the crash happens on launch, then [WinDbg Preview](https://www.microsoft.com/store/p/windbg/9pgjgd53tn86) is recommended, since it contains a "Launch app package" option in
"Start Debugging" which can launch and debug UWP and packaged apps from launch.

### Other options

Another option is to set some regkeys to tell Windows to keep some crash dumps locally (see https://docs.microsoft.com/en-us/windows/win32/wer/collecting-user-mode-dumps).
For example, running these commands in an administrative command prompt will set regkeys to tell Windows to save full (type=2) dumps into `C:\dumps`:

    reg add "HKLM\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps" /v DumpFolder /d "C:\dumps"
    reg add "HKLM\SOFTWARE\Microsoft\Windows\Windows Error Reporting\LocalDumps" /v DumpType /t REG_DWORD /d 2

After you repro the crash, you should find a dump in the specified folder.

You can automate crash dump collection and filing bugs by following these steps:
1. Download the script at https://aka.ms/RNW/analyze-crash.ps1, for example to `C:\temp`
2. Open an admin PowerShell. If you haven't enabled running unsigned scripts yet, do that by running: `Set-ExecutionPolicy Unrestricted`
3. Run the script and pass it the name of your app's exe: `C:\temp\analyze-crash.ps1 -ExeName MyApp -Repo microsoft/microsoft-ui-xaml`
The script will set up automatic crash dump collection for your app, download the native debugging tools (including the command-line debugger cdb), and ask you to reproduce the crash.

At this point you can launch the app (e.g. from Start menu if you've already deployed it to the local device). When the app crashes, it will generate a crash dump (`.dmp` file). You can then press enter to resume execution of the script, and the script will use `cdb` to automatically analyze the crash dump, and output the results to a file `analyze.log`.

The script will then copy the contents of the log to the clipboard, open the log file in notepad, and launch the browser to file an issue in the WinUI repo, where you can paste the stack trace into the bug template.

## How to get a good callstack for crashes

For some crashes, such as access violations, the direct crash callstack is usually the right stack to use.
But if it is a stowed exception crash, which has exception code: 0xc000027b, then more work is required to get the right callstack.

### Stowed Exception crashes (exception code: 0xc000027b)

Stowed exception crashes save away a possible error, which gets used later if no one handles the exception.
XAML sometimes decides the error is fatal immediately, in which case the direct crash stack may be good, but more frequently the stack has unwound before it was determined to be fatal.
This channel9 talk describes stowed exceptions in more detail: https://channel9.msdn.com/Shows/Inside/C000027B?term=stowed%20exception&lang-en=true.

For stowed exception crashes, you can get more info on the crash by loading a crash dump in WinDbg and then using !pde.dse to dump the stowed exceptions.
The !pde debugger extension is available [here](https://onedrive.live.com/?authkey=%21AJeSzeiu8SQ7T4w&id=DAE128BD454CF957%217152&cid=DAE128BD454CF957) in the PDE*.zip.
(It is linked off the channel9 page above.)
Put the appropiate x64 or x86 dll in that zip in the winext directory of a WinDbg install, and then "!pde.dse" should work on stowed exception crash dumps.

Frequently there will be multiple stowed exceptions, with some at the end which got handled/ignored.
Most commonly, the first stowed exception is the interesting one.
In some cases, the first stowed exception may be a re-throw of the second, so if the second stowed exception shows deeper into the same stack as the first, then the second exception may be the origination of the error.
The error code shown with each stowed exception is also valuable, since that provides the HRESULT associated with that exception.



================================================
FILE: docs/feature_proposal_process.md
================================================
# New Feature or API Process

We welcome community contributions and input to the WinUI Library, including feature ideas and code contributions.

This document outlines the process for how you can propose or contribute new features.

### You need to follow this process for:

* Code changes that add, remove, or alter public API
* Features that add or alter the user experience (e.g. new visual designs)
* Changing any core functionality documented on docs.microsoft.com

### You don't need to follow this process for:

* Fixing bugs
* Submitting PRs that don't alter major functionality or public API
(e.g. internal performance improvements)

## Process summary

![Image of process summary](feature_proposal_process_summary.png)

## Process details

0. Please search the [issue tracker](https://github.com/microsoft/microsoft-ui-xaml/issues) for a similar idea first: there may already be an issue you can contribute to.

1. **Create Issue**
All code changes must be tied to an Issue.
To propose a new feature or API please start by filing a new issue in the [issue tracker](https://github.com/microsoft/microsoft-ui-xaml/issues) using the [Feature Proposal template](https://github.com/Microsoft/microsoft-ui-xaml/issues/new?template=feature_proposal.md).
Include as much detail as you have. It's fine if it's not a complete design: just a summary and rationale is a good starting point.

2. **Wait for Team Owner**
We will assign a WinUI team owner to your issue. The WinUI team regularly triages all incoming issues.

3. **Discussion**
We'll keep the issue open for community discussion until the team owner decides it's ready or should be closed.
Note that if an issue isn't a high priority or has many open questions then it might stay open for a long time.

4. **Owner Review**
The WinUI team will review the proposal and either approve or close the issue based on whether it broadly aligns with the [WinUI roadmap](roadmap.md) and [contribution guidelines](../CONTRIBUTING.md).

5. **API Review**
If the feature adds new APIs then we'll start an API review in the [WinUI API review repo](https://github.com/microsoft/microsoft-ui-xaml-specs). All new public APIs must be reviewed before merging.

6. **Implementation**
A feature can be implemented by you, the WinUI team, or other community members.
Code contributions are greatly appreciated: feel free to work on any reviewed feature you proposed, or choose one in the backlog and send us a PR. Please let us know in the issue comments if you are actively working on implementing a feature so we can ensure it's assigned to you.
Our contribution guidelines can be found [here](../CONTRIBUTING.md).

7. **Merge**
Once a feature is complete and tested according to the [contribution guidelines](../CONTRIBUTING.md) you can send us a PR to merge it to main.

8. **Documentation and sample updates**
We will update the [documentation on docs.microsoft.com](https://docs.microsoft.com/windows/uwp) and if applicable add a sample to the [Xaml Controls Gallery](https://github.com/Microsoft/Xaml-Controls-Gallery) app.
Feel free to also contribute to docs and samples!
Once the docs and samples are updated we'll close the issue.

9. **Binaries**
We periodically produce signed prerelease binaries from the main branch which are published to [NuGet](https://www.nuget.org/profiles/winui): see the [Roadmap](roadmap.md) for info on build frequency.
After the feature has been sufficiently validated as part of a prerelease package we will include it in the next stable binary release on NuGet.



================================================
FILE: docs/roadmap.md
================================================
# Windows UI Library Overview

WinUI is the modern native UI platform for Windows with two active generations:

1. **WinUI 3**: The latest, 3rd generation of WinUI that ships the entire WinUI stack decoupled from the operating system as a part of the [Windows App SDK](https://docs.microsoft.com/windows/apps/windows-app-sdk/).

2. **WinUI 2**: The previous generation of the WinUI stack for UWP apps, consisting of a XAML and Visual Layer built directly into the Windows 10 operating system, and a controls library built on top of the OS, delivered via NuGet, and hosted at this repository. WinUI 2 will continue to be supported with bug, reliability, and security fixes.

**For a detailed look on the difference between WinUI 2 & 3, please view our [comparison table](https://docs.microsoft.com/windows/apps/winui/#comparison-of-winui-3-and-winui-2)

### Benefits of WinUI

WinUI provides a number of benefits which makes it the best way to create user interfaces for Windows apps:

1. **The native UI platform of Windows**
WinUI is the highly-optimized native UI platform used to create Windows itself, now made more broadly available for all developers to use to reach Windows. It's a thoroughly tested and proven UI platform that powers the operating system environment and essential experiences of 1 billion+ Windows 10 & 11 PC, XBox One, HoloLens, Surface Hub and other devices.

2. **The latest advancements in Fluent Design**
WinUI is Microsoft's main focus for native, accessible Windows UI and controls and is the definitive source for the [Fluent Design System](https://www.microsoft.com/design/fluent/) on Windows.
It will also support the latest composition and rendering innovations like vector animations, effects, shadows and lighting.

3. **Backward compatibility for new features**
New WinUI features will continue to be backward-compatible with a wide range of Windows 10 and 11 versions. With WinUI 3, you can start building and shipping apps with new features immediately as soon as they're released, without having to wait for your users to be running the latest update of Windows.

4. **Native development support**
WinUI can be used with .NET, but doesn't depend on .NET: WinUI is 100% C++ and can be used in unmanaged Windows apps, for example using standard C++17 via [C++/WinRT](https://docs.microsoft.com/windows/uwp/cpp-and-winrt-apis/).

5. **More frequent updates**
WinUI is planned to ship roughly every 6 months, with at least two preview builds per stable release.  This is more of a guideline than a rule, but that is what the team strives for.

6. **Open source development and community engagement**
 The WinUI 2 Controls Library is already open source on GitHub, and we're planning to add the full WinUI 3 framework into this repo as well. You can engage directly with Microsoft's core engineering team and contribute bug reports, feature ideas, and even code: see the [Contribution Guide](../CONTRIBUTING.md) for more info.  You can also try out the pre-release builds to see new in-development features and help shape their final form.

## WinUI 3

**[WinUI 3](https://docs.microsoft.com/windows/apps/winui/winui3/)** is the latest generation of native Windows UI, consisting of all the major UX layers of Windows decoupled and shipping as a standalone solution for you to use.

It focuses on enabling three main use cases:

1. **Modernizing existing apps**
    * Enabling you to extend existing Win32 (WPF, WinForms, MFC...) apps with modern Windows UI at your own pace using the upcoming release of [Xaml Islands](https://docs.microsoft.com/windows/apps/desktop/modernize/xaml-islands). Developers who currently use WinUI 2 for their app UX will be able to easily move to WinUI 3, as their syntax and capabilities are very similar
2. **Creating new Windows apps**
    * Enabling you to easily create new modern Windows apps with the flexibility offered by the [Windows App SDK](https://docs.microsoft.com/windows/apps/windows-app-sdk/)
3. **Enabling other frameworks**
    * Providing the native implementation for other frameworks like [React Native](https://github.com/Microsoft/react-native-windows) and .NET [MAUI](https://docs.microsoft.com/dotnet/maui/what-is-maui) when running on Windows.

WinUI 3 is available as a part of the [Windows App SDK](https://docs.microsoft.com/windows/apps/windows-app-sdk) for building stable and supported desktop/Win32 apps for production scenarios. You can download and read more about the latest releases of the Windows App SDK at the following documentation.

[Stable release channel for the Windows App SDK](https://docs.microsoft.com/windows/apps/windows-app-sdk/stable-channel)

We also ship experimental features as we develop them. You can read more about the Windows App SDK Experimental releases at the following documentation. Note that Experimental releases have limitations and known issues, so they are not equipped for production apps.

[Experimental release channel for the Windows App SDK](https://docs.microsoft.com/windows/apps/windows-app-sdk/experimental-channel).

### Roadmap

For more info about upcoming features in the next release of WinUI 3, see the [Windows App SDK feature roadmap](https://github.com/microsoft/WindowsAppSDK/blob/main/docs/roadmap.md).

## WinUI 2 Controls Library

WinUI 2 is a native user experience (UX) framework for both Windows desktop and UWP applications tightly integrated with Windows 10 and above SDKs.

The latest release of the **WinUI 2 Controls Library** was v2.8 which was released in July 2022. You can find a list of what was introduced in this release in the [release notes](https://learn.microsoft.com/en-us/windows/apps/winui/winui2/release-notes/winui-2.8).

At this time, there are no plans for a WinUI 2.9. However, WinUI 2 will continue to be supported through servicing releases with bug, reliability, and security fixes as needed.

For installation instructions see [Getting started with the Windows UI Library](https://docs.microsoft.com/windows/apps/winui/winui2/getting-started).



================================================
FILE: docs/SECURITY.md
================================================
<!-- BEGIN MICROSOFT SECURITY.MD V0.0.2 BLOCK -->

# Security

Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/Microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [many more](https://opensource.microsoft.com/).

If you believe you have found a security vulnerability in any Microsoft-owned repository that meets Microsoft's [definition](https://docs.microsoft.com/en-us/previous-versions/tn-archive/cc751383(v=technet.10)) of a security vulnerability, please report it to us as described below.

## Reporting Security Issues

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them to the Microsoft Security Response Center (MSRC) at [https://msrc.microsoft.com/create-report](https://msrc.microsoft.com/create-report).

If you prefer to submit without logging in, send email to [secure@microsoft.com](mailto:secure@microsoft.com).  If possible, encrypt your message with our PGP key; please download it from the the [Microsoft Security Response Center PGP Key page](https://www.microsoft.com/en-us/msrc/pgp-key-msrc).

You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your original message. Additional information can be found at [microsoft.com/msrc](https://www.microsoft.com/msrc).

Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:

* Type of issue (e.g. buffer overflow, SQL injection, cross-site scripting, etc.)
* Full paths of source file(s) related to the manifestation of the issue
* The location of the affected source code (tag/branch/commit or direct URL)
* Any special configuration required to reproduce the issue
* Step-by-step instructions to reproduce the issue
* Proof-of-concept or exploit code (if possible)
* Impact of the issue, including how an attacker might exploit the issue

This information will help us triage your report more quickly.

If you are reporting for a bug bounty, more complete reports can contribute to a higher bounty award. Please visit our [Microsoft Bug Bounty Program](https://microsoft.com/msrc/bounty) page for more details about our active programs.

## Preferred Languages

We prefer all communications to be in English.

## Policy

Microsoft follows the principle of [Coordinated Vulnerability Disclosure](https://www.microsoft.com/en-us/msrc/cvd).

<!-- END MICROSOFT SECURITY.MD BLOCK -->



================================================
FILE: docs/triage.md
================================================
# Issue/PR Management Information

## Overview

The WinUI team manages issues and PRs in the repo using a process we call "triage". It helps us keep issues
organized and focuses the attention of the different groups that work in our project.

For more info about our strategy for triaging bugs, see how we [handle contributions](contribution_handling.md).

### Triage labels

1. New and re-opened issues are marked with `needs-triage`.
2. Issues with `needs-assignee-attention` should be investigated by the assignee as top priority.
3. Issues with `needs-author-feedback` are waiting for the author to reply.

Because many groups are involved in WinUI we have `team-...` labels to help filter issues further for triage.

### Triage process

For each issue with `needs-triage`:
* Feature proposals:
  - Triage makes first pass to ask clarifying questions. If it's ok then:
     - Spec owner gets assigned
     - Gets added to `New proposal` in feature tracking board
     - Assigned owner is responsible for following the feature process
* Everything else:
  - If author needs to provide more info, ask in comments and add `needs-author-feedback`
  - Add a team label (`team-Controls`, `team-Framework`, etc) if missing
  - Add area tag(s)
  - Add tags for type of issue (`bug`, `test issue`, `spec issue`, `documentation`)
  - Change labels to `question` or `discussion` if appropriate
  - Consider adding `help wanted` or `good first issue` to encourage community engagement
  - Add `nice to have` for low priority issues

The temporary `needs-assignee-attention` label is intended for issues which need additional investigation, like debugging or another teams input, to determine how to route them.

### Backlog

[Assigned issues](https://github.com/microsoft/microsoft-ui-xaml/issues/assigned/*) are being investigated or worked on. This doesn't mean they *will* be fixed soon, just that they are on the short list for that person to investigate, and possibly fix. They may get unassigned.

[Unassigned issues](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+no%3Aassignee) are the backlog.

### Triage queries

Shortcuts to triage queries for the team. Note that these include closed issues because external comments on closed issues may not be
noticed, so we have a bot rule that adds `needs-triage` to closed issues too.

* [Controls Triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Aneeds-triage+-label%3Ateam-framework+-label%3Ateam-reach+-label%3Ateam-rendering+-label%3Ateam-ink+-label%3Ateam-compinput++-label%3Ateam-markup+)
* [Framework Triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Ateam-Framework+label%3Aneeds-triage+)
* [Markup Triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Ateam-Markup+label%3Aneeds-triage+)
* [Reach Triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Ateam-Reach+label%3Aneeds-triage+)
* [Rendering Triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Ateam-Rendering+label%3Aneeds-triage+)

* [Root node triage](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=label%3Aneeds-triage+-label%3Ateam-controls+-label%3Ateam-framework+-label%3Ateam-reach+-label%3Ateam-rendering+-label%3Ateam-ink+-label%3Ateam-compinput++-label%3Ateam-markup+) -- issues not assigned to a team yet.

We also need to monitor:
* [needs-assignee-attention](https://github.com/microsoft/microsoft-ui-xaml/labels/needs-assignee-attention)
* [needs-author-feedback](https://github.com/microsoft/microsoft-ui-xaml/labels/needs-author-feedback)

### Other useful links for contributors

* [good first issue](https://github.com/microsoft/microsoft-ui-xaml/labels/good%20first%20issue)
* [help wanted](https://github.com/microsoft/microsoft-ui-xaml/labels/help%20wanted)
* [unassigned bugs in WinUI 2.x](https://github.com/microsoft/microsoft-ui-xaml/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3Ateam-Controls+no%3Aassignee+-label%3A%22feature+proposal%22++-label%3Aneeds-winui-3+label%3Abug+-label%3Awinui3%CE%B1)

## Bot rules

1. New and re-opened issues get `needs-triage` label added
1. `needs-triage` label is added whenever `team-...` labels change so that the new team sees the status change on the issue.
1. If `feature proposal` is added or removed it gets added/removed from the [feature tracking project board](https://github.com/microsoft/microsoft-ui-xaml/projects/4) accordingly.
1. If `declined` is added, bot adds a friendly message and closes.
1. Tags issues/PR with release announcement.
1. When moving into `Front Burner` column, gets added to the `API review` board.
1. Adds `working on it` to bugs linked as being fixed by a PR.
1. Auto-merge PRs with the `auto merge` label on them.
1. Remove `needs-triage` label when an issue is closed.
1. Remove `needs-triage` when a closed issue has a reply by someone with write access to the repo.
1. Replace `needs-author-feedback` label with `needs-assignee-attention` (if assigned) or `needs-triage` (if unassigned).




================================================
FILE: docs/winrt-apis-for-desktop.md
================================================
# WinRT API changes for Desktop apps

The content from this doc has been moved to our official documentation site, and will continue to be maintained there.

You can find the updated doc at: [Windows Runtime APIs not supported in Desktop apps](https://docs.microsoft.com/windows/apps/desktop/modernize/desktop-to-uwp-supported-api).


================================================
FILE: docs/winui3_migration.md
================================================
# Migrating a UWP App To WinUI3

**It is recommended to use the  [try-convert](https://github.com/dotnet/try-convert/tree/feature/winui) tool for the full conversion process.**
**`try-convert` will automate most of the conversion steps.**

## Background

The purpose of the [try-convert WinUI3 feature](https://github.com/dotnet/try-convert/tree/feature/winui) is to create a porting solution to allow developers to convert WinUI2 projects to the new WinUI3 format.

- WinUI is a native user experience (UX) framework for both Windows Desktop and UWP applications. WinUI ships as part of the Windows OS.
[More on WinUI](http://aka.ms/winui), [Docs](https://docs.microsoft.com/en-us/windows/apps/winui)
- WinUI3 is the next version of WinUI. It runs on the native Windows 10 UI platform and supports both Windows Desktop and UWP apps. WinUI3 ships as a NuGet package.
[More on WinUI3](https://docs.microsoft.com/en-us/windows/apps/winui/winui3)

Converting an existing WinUI C# App to WinUI3 requires some changes to the C# source code. Most notably namespace changes from Windows.UI.* to Microsoft.UI.*

This porting assistance is provided in the form of Roslyn Analyzers and Code Fixes.
- A Code Analyzer provides on the fly code inspections for C# and creates diagnostics.
- A Code Fix consumes the diagnostics created by the Code Analyzer and modifies the C# file in-line.

See the [try-convert documentation](https://github.com/dotnet/try-convert/tree/feature/winui) for more information on these code analyzers and how to automoate the process with [try-convert](https://github.com/dotnet/try-convert/blob/feature/winui/WinUIConvert.md).




================================================
FILE: docs/images/BrowseInformation.PNG
================================================
[Non-text file]


================================================
FILE: specs/AnimatedVisualPlayer Spec.md
================================================
AnimatedVisualPlayer Spec
===

# Background

Today, developers can create animated visuals to use in their UI by using the
[AnimatedVisualPlayer](https://docs.microsoft.com/uwp/api/Microsoft.UI.Xaml.Controls.AnimatedVisualPlayer)
control.
`AnimatedVisualPlayer` can play any
[IAnimatedVisual](https://docs.microsoft.com/uwp/api/Microsoft.UI.Xaml.Controls.IAnimatedVisual)
implementation,
but the typical way to get an `IAnimatedVisual` implementation is to use
the LottieGen tool to generate code from a JSON file that was created from Adobe AfterEffects.

[More information on Lottie and AnimatedVisualPlayer](https://docs.microsoft.com/en-us/windows/communitytoolkit/animations/lottie)

There are some performance issues with the current implementation of LottieGen and AnimatedVisualPlayer:
1)	Complex Lottie animations can instantiate a lot of composition animations
which may impact performance and overall battery life.
2)	Lottie files that have a lot of complex animations
have some cost to performance even when they are paused.
The Idle (paused) Lottie animations use the same amount of CPU resources as
when they are playing the actual animation.

The new APIs here allow `AnimatedVisualPlayer`,
[AnimatedIcon](https://docs.microsoft.com/uwp/api/Microsoft.UI.Xaml.Controls.AnimatedIcon),
and the interface generated by LottieGen to be updated to help reduce the number of composition animations created
when the animation is idle or paused to help improve performance when a developer uses
Lottie Animations with `AnimatedVisualPlayer`.

This spec will focus on changes for LottieGen and `AnimatedVisualPlayer`.

This will require 3 changes:
1.	Create a new interface for which an implementation is generated by LottieGen called `IAnimatedVisual2`,
that can destroy and instantiate animations.
2.	Create a new interface `IAnimatedVisualSource3` from which to get the new `IAnimatedvisual2`
3.	Add a `AnimationOptimization` property to AnimatedVisualPlayer that will control
when animations should be destroyed and when they should be instantiated.
This will be implemented using the previous new interfaces.

# API Pages

## AnimatedVisualPlayer.AnimationOptimization property

Gets or sets a value that determines how animations are cached. Defaults to 'Latency'.

The two modes for the property will specify the behavior the AnimatedVisualPlayer will have
when the player is idle (when `PlayAsync` is not active).

|Mode| Behavior|
|---- | -------|
|Latency| AnimatedVisualPlayer will pre-create animations even before `PlayAsync()` is called,
and not destroy any when player is idle.
|Resources | AnimatedVisualPlayer will not create animations until `PlayAsync()` is called,
and will destroy them when it completes. If you call pause, this does not free up all
resources of the player. To truly stop the animation, call Stop.

Note: If you set the `Source` or `AnimationOptimization` of your player, the player will defer
processing of the source file until the layout is being formed.

If you have an animation that will start on click, you may want to initialize
the property to `None` and set `AnimationOptimization` to 'Always'
when the mouse enters this control,
and back to `None` when mouse leaves to ensure that the animation starts immediately on click,
but don't use up resources otherwise.

Setting the `AnimationOptimization` to `Latency` when the mouse enters the control will ensure that
the animation objects are preloaded so that the animation may start immediately when it needs to play.

If you call PlayAsync before animations are loaded, then the player won't start until all animations are loaded completely.

```c#
private void Player_PointerEntered(object sender, PointerRoutedEventArgs e)
{
    myanimatedvisualplayer.AnimationOptimization = AnimationOptimization.Latency;
}
async private void Player_PointerExited(object sender, PointerRoutedEventArgs e)
{
    myanimatedvisualplayer.AnimationOptimization = AnimationOptimization.Resources;
}

async private void Player_OnClick(object sender, PointerRoutedEventArgs e)
{
    myanimatedvisualplayer.PlayAsync(0.0, 1.0);
}

```

If `PlayAsync` is called and the animations have not been instantiated due to `AnimationOptimization` being set to `None`,
`PlayAsync` will instantiate the animations so it can play the visual.

# API Details

```c#
namespace Microsoft.UI.Xaml.Controls
{
  unsealed runtimeclass AnimatedVisualPlayer
  {
      // Existing ...

    //Sets the caching behavior of the AnimatedVisualPlayer
    AnimationOptimization AnimationOptimization;
  }

  public enum AnimationsCacheMode
  {
      Always = 0,
      None
  }
}
```

## IAnimatedVisual2 Interface

An extension to
[IAnimatedVisual](https://docs.microsoft.com/uwp/api/Microsoft.UI.Xaml.Controls.IAnimatedVisual)
that adds the ability to control when animation objects are created and destroyed.

| Method | Meaning |
|-------------|---------|
| CreateAnimations | Instantiates the animation visuals for the provided progress value of the animation. |
| DestroyAnimations | Destroys all animation visuals for a given animation.|

```c#
interface IAnimatedVisual2 requires IAnimatedVisual
{
    void InstantiateAnimations(Double progressHint);
    void DestroyAnimations();
};
```

## IAnimatedVisual2.InstantiateAnimations Method

Instantiates the animation visuals for the provided progress value of the animation.

```c#
void CreateAnimations();
```

## IAnimatedVisual2.DestroyAnimations Method

Destroys all animation visuals for a given animation.

```c#
void DestroyAnimations();
```
## IAnimatedVisualSource3 Interface

An extension to
[IAnimatedVisualSource](https://docs.microsoft.com/uwp/api/Microsoft.UI.Xaml.Controls.IAnimatedVisualSource)
that products an `IAnimatedVisualSource3`.

```c#
interface IAnimatedVisualSource3
{
    IAnimatedVisual2 TryCreateAnimatedVisual(
        Windows.UI.Composition.Compositor compositor,
        out Object diagnostics,
        Boolean instantiateAnimations,);
};

```



================================================
FILE: specs/api_spec_template.md
================================================
Please use this template for new/modified APIs:
https://github.com/microsoft/WindowsAppSDK/blob/main/specs/spec_template.md



================================================
FILE: specs/appwindow-spec.md
================================================
Window.AppWindow api
===
New api to simplify accessing [appwindow](https://docs.microsoft.com/en-us/windows/apps/windows-app-sdk/windowing/windowing-overview)
functionality through WinUI 3 code

# Background
Xaml has a [Window](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Window) API that
internally wraps an hwnd. Windows has an [AppWindow](https://docs.microsoft.com/uwp/api/Windows.UI.WindowManagement.AppWindow) class
that similarly wraps an hwnd in UWP. WinAppSDK has a new [AppWindow](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Windowing.AppWindow) which wraps an hwnd and works on Desktop.

You can get an AppWindow from a Xaml Window by calling a COM API to get Xaml and then
a DLL export API to convert the hwnd to an AppWindow. This spec adds a simple `Window.AppWindow`
property to make this much easier and more discoverable.

[Xaml Window](https://docs.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.xaml.window) will
expose AppWindow object directly to app developer through an api. Instead of writing a lot of boiler plate
code everywhere, app developer can use this api, reducing code bloat, and making appwindow apis easily
accessible from WinUI 3 code.

These *before* and *after* C# code examples illustrate how this api simplifies integrating appwindow apis in WinUI 3 codebase.

### Before
```c#
// This is needed to get any Window from inside a Xaml control
var xamlWindow = WindowHelper.GetWindowForElement(this); // api to get window object from UIElement (not a real api)

// unnecessary boiler plate code
var windowId = Win32Interop.GetWindowIdFromWindow(WindowNative.GetWindowHandle(xamlWindow));
var appWindow = AppWindow.GetFromWindowId(windowId);

//calling function foo  (not a real appwindow function)
appWindow.foo();
```

### After
```c#
// This is needed to get any Window from inside a Xaml control
var xamlWindow = WindowHelper.GetWindowForElement(this); // api to get window object from UIElement (not a real api)


//calling function foo directly
xamlWindow.AppWindow.foo();
```
Notice how `xamlWindow.AppWindow.foo()` doesn't require additional steps to call the function `foo`.


# API Pages

## Window.AppWindow property

Gets the `AppWindow` associated with this `Window`.
```c#
public Microsoft.UI.Windowing.AppWindow Window.AppWindow { get; }
```
### Sample example
```c#
var xamlWindow = WindowHelper.GetWindowForElement(this);
auto windowSize = xamlWindow.AppWindow.Size;
```

Mapping an hwnd to an AppWindow causes the hwnd to be subclassed, meaning that the timing of
when [AppWindow.GetFromWindowId](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Windowing.AppWindow.GetFromWindowId)
is first called can potentially have a behavioral side effect. To ensure this is predictable, the AppWindow
for Xaml's hwnd will be created during the Xaml Window's construction. Note that this could potentially be
an observable behavior change from the behavior before the introduction of this API.

New subclassing order with this new feature change:

* ContentAppWindowBridge
  &darr;
* AppWindow
  &darr;
* Xaml Window
&darr;
* DefaultWndProc


# API Details

```c# (but really MIDL3)
namespace Microsoft.UI.Xaml
{
   unsealed runtimeclass Window
  {
      ...
      Microsoft.UI.Windowing.AppWindow AppWindow{ get; };
  }
}
```

# Appendix
- Window.AppWindow api returns reference to the same appwindow object every time. It gets created
  during xaml window object's creation. There is minimal performance impact observed for this change.

- Since AppWindow is an abstraction for HWND, its lifetime will be same as that of HWND. The
  api cannot return null as AppWindow will always be present if Window object is there. If called after
  window has been closed, it will fail similarly to other WinUI 3 apis and return a failure HRESULT.

- There will be only one appwindow object per top level HWND, created during Window object creation.
  No new appwindow objects are created for child windows.

- Future scope : Since this api is limited to top level HWND, there should be a way to get app window object
  for top level HWND from one of its nested children HWND which doesn’t require app developer writing a lot of code.




================================================
FILE: specs/custom-iresourcemanager-spec.md
================================================
Providing a custom MRT Core `IResourceManager` for WinUI 3 to use
===

# Background

The WinUI 3 framework instantiates an MRT Core
[`ResourceManager`](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.windows.applicationmodel.resources.resourcemanager?view=windows-app-sdk-1.2)
in order to resolve resource URIs. While this default `ResourceManager` is generally sufficient,
there are some scenarios in which an app needs non-standard behavior in order to resolve a
particular resource URI. In order to address this requirement, this document describes a new
API that would allow an app to provide its own custom implementation of the
[`IResourceManager`](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.windows.applicationmodel.resources.iresourcemanager?view=windows-app-sdk-1.2)
interface for WinUI to use in lieu of its default `ResourceManager`.

# API Pages

_(Each of the following L2 sections correspond to a page that will be on docs.microsoft.com)_

## Application.ResourceManagerRequested Event

Raised during startup of a new WinUI thread to give the app a chance to provide its own
[`IResourceManager`](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.windows.applicationmodel.resources.iresourcemanager?view=windows-app-sdk-1.2)
implementation to be used by the framework for resolving resource URIs.

_Spec note: is there a version of the 'ResourceDictionary and XAML resource references' article that
links to the Windows App SDK documentation for relevant APIs?_

```c#
public event TypedEventHandler<Application, ResourceManagerRequestedEventArgs>
ResourceManagerRequested

```

### Remarks

It is strongly recommended that apps which need to listen for this event register their handler in
their `App` class's constructor so that it is available during initial app launch as in the
following example.

```c#
public App()
{
   this.InitializeComponent();

   ResourceManagerRequested += (_, e) =>
   {
      // CreateResourceManager() is a custom method that returns an instance of
      // Microsoft.Windows.ApplicationModel.Resources.IResourceManager.
      IResourceManager resourceManager = CreateResourceManager();
      e.ResourceManager = resourceManager;
   };
}
```

This event is raised once per WinUI thread during initialization. If you use the same
`IResourceManager` for multiple threads, then the `IResourceManager` must be thread-safe.



## ResourceManagerRequestedEventArgs Class

Provides event data for the `Application.ResourceManagerRequested` event.

```c#
public sealed class ResourceManagerRequestedEventArgs
```

### Remarks

`ResourceManagerRequestedEventArgs` is used to provide the WinUI 3 framework with a custom
implementation of the
[`IResourceManager`](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.windows.applicationmodel.resources.iresourcemanager?view=windows-app-sdk-1.2)
interface to be used for resolving resource URIs rather than the default `ResourceManager` that the
framework creates. In the event handler, you should instantiate your custom `IResourceManager` and
assign it to the `ResourceManagerRequestedEventArgs.CustomResourceManager` property. The value of this
property is initially `null`, and it is only checked by the framework once per event raise after
all registered event handlers have been invoked. If the property value is still `null` then the
framework will use the default `ResourceManager`.


## ResourceManagerRequestedEventArgs.CustomResourceManager Property

Sets the custom `IResourceManager` that should be used by WinUI to resolve MRT resources for the
current thread. If you leave the value `null` then the default `ResourceManager` will be used.

```c#
public IResourceManager ResourceManager { get; set; }
```


# API Details
```c#
namespace Microsoft.UI.Xaml
{
  runtimeclass Application
  {
    // existing ...

    event Windows.Foundation.TypedEventHandler<Application,Microsoft.UI.Xaml.ResourceManagerRequestedEventArgs>
        ResourceManagerRequested;
  };

  runtimeclass ResourceManagerRequestedEventArgs
  {
    IResourceManager CustomResourceManager;
  };
}

```




================================================
FILE: specs/DateTimePicker-Visual-Updates-Spec.md
================================================
MonochromaticOverlayPresenter
===

# Background

The `MonochromaticOverlayPresenter` API is a Xaml Framework Element that renders the portion of
another element at the same position (the portion of that element that it overlays),
while also applying a monochromatic colorization effect.
This allows the element to appear to be an overlay on top of the other element.

`MonochromaticOverlayPresenter` element is similar to several precedents:
* [CompositionMaskBrush](https://docs.microsoft.com/uwp/api/Windows.UI.Composition.CompositionMaskBrush),
which  is a brush that gets its content from another (source) brush.
* WPF's [VisualBrush](https://docs.microsoft.com/dotnet/api/System.Windows.Media.VisualBrush),
which uses an element's rendering to draw a brush.

A key difference in this new type is that it only renders the portion of the source
element which it intersects with in location.

This new `MonochromaticOverlayPresenter` will be used in the rendering of the
[DatePicker](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.DatePicker)
control (see more info in the Appendix).

# API Pages

## MonochromaticOverlayPresenter class

A [Framework Element](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.frameworkelement?view=winui-3.0-preview)
which renders another element at the same position (beneath it in the Z-order),
while also optionally applying a monochromatic colorization effect.

```csharp
public class MonochromaticOverlayPresenter : FrameworkElement
{
    public UIElement SourceElement { get; set; }
    public Color ReplacementColor { get; set; }
}
```

Set the `SourceElement` property to indicate which element's rendering should be re-rendered
by the `MonochromaticOverlayPresenter`.

The `MonochromaticOverlayPresenter` must overlap the source element; only the intersection
of the two elements will be rendered by the overlay.

Only the source element's rendering applies to the `MonochromaticOverlayPresenter`; the user
cannot interact with it using the mouse, or move keyboard focus to it. However,
`MonochromaticOverlayPresenter` will render system focus visuals, regardless of what the
[UseSystemFocusVisuals](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Control.UseSystemFocusVisuals)
property is set to.

To allow pointer events to get to the source element, set the overlay's
[UIElement.IsHitTestVisible](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.UIElement.IsHitTestVisible)
property to false.

> Note: the element set as the `SourceElement` cannot be an ancestor or in the descendancy of
the `MonochromaticOverlayPresenter`. However the `SourceElement` must be in the same XAML tree as
the `MonochromaticOverlayPresenter`.

If the `ReplacementColor` property is set and has a nonzero Alpha value, then the `SourceElement`
is treated as a mask: every non-transparent pixel will be replaced by this color. The RGB value
of the `ReplacementColor` (not the Alpha value) will override the RGB of the source.
The default value for `ReplacementColor` is
[Colors.Transparent](https://docs.microsoft.com/uwp/api/Windows.UI.Colors.Transparent).

### MonochromaticOverlayPresenter examples

The following example puts a `MonochromaticOverlayPresenter` on top of (z-ordered above)
some scrolling text, causing the center of the text to be highlighted, even as it's scrolling.
Things to note:
* The `MonochromaticOverlayPresenter` is sourcing from the `TextBlock`, it's also z-ordered above
the same `TextBlock`. If the `Background` and `SourceElement` properties weren't set,
it would have no effect; it would render the `TextBlock` exactly on top of itself.
* The `MonochromaticOverlayPresenter` is positioned and given a height such that it's a black band
across the center of the scrolling text.
* The `MonochromaticOverlayPresenter.IsHitTestVisible` property is set to False, so that input
still goes to the ScrollViewer that is z-ordered behind it.

```xml
<Grid Background="White" Width="150">
    <ScrollViewer x:Name="Source" Height="300">
        <TextBlock
            Foreground="Black"
            FontSize="30"
            Text="{x:Bind LoremIpsum}"
            TextWrapping="Wrap">
        </TextBlock>
    </ScrollViewer>

    <MonochromaticOverlayPresenter
        ReplacementColor="Green"
        SourceElement="{x:Bind Source}"
        Height="30"
        IsHitTestVisible="False"
        VerticalAlignment="Center"
        HorizontalAlignment="Stretch"/>
</Grid>
```

![Example showing the MonochromaticOverlayPresenter control overlaid on moving content within a ScrollViewer, changing the foreground color and background color of words that pass through.](images/api-example.gif)

The example below shows how the new `MonochromaticOverlayPresenter` API can be used to partially highlight a TextBlock.

```xml
 <Grid Background="{ThemeResource ApplicationPageBackgroundThemeBrush}">
        <StackPanel x:Name="Panel" Orientation="Vertical" HorizontalAlignment="Center" VerticalAlignment="Center">
            <Grid Margin="2,10,0,0">
                <TextBlock x:Name="Source" Text="This string will be partially highlighted"/>
                <MonochromaticOverlayPresenter
                    ReplacementColor="Black"
                    SourceElement="{x:Bind Source}"
                    Width="50"
                    VerticalAlignment="Stretch"
                    HorizontalAlignment="Center"
                    Background="LightBlue"/>
            </Grid>
        </StackPanel>
    </Grid>
```

> Todo: add a reflection example (classic use of VisualBrush in WPF)

### MonochromaticOverlayPresenter theme resources

You can modify the default Style and ControlTemplate to give the control a unique appearance.
For more info, see the
[Light-weight styling section](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/xaml-styles#lightweight-styling)
of the
[Styling controls](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/xaml-styles)
article.

`MonochromaticOverlayPresenter` defines the following new resource:

```xml
<StaticResource x:Key="DatePickerFlyoutPresenterHighlightForegroundColor" ResourceKey="TextOnAccentAAFillColorPrimary" />
```

## Other MonochromaticOverlayPresenter members

| Name | Description |
| - | - |
| SourceElement | Gets or sets the UIElement to render inside the `MonochromaticOverlayPresenter`. |
| ReplacementColor | Gets or sets the Color to use instead of the non-transparent pixels of the SourceElement.

# API Details

```csharp
namespace Microsoft.UI.Xaml.Controls.Primitives
{

[MUX_PROPERTY_CHANGED_CALLBACK(TRUE)]
[MUX_PROPERTY_CHANGED_CALLBACK_METHODNAME("OnPropertyChanged")]
unsealed runtimeclass MonochromaticOverlayPresenter : Windows.UI.Xaml.Controls.FrameworkElement
{
    MonochromaticOverlayPresenter();

    Windows.UI.Xaml.UIElement SourceElement { get; set; };
    Windows.UI.Color ReplacementColor { get; set; };

    static Windows.UI.Xaml.DependencyProperty SourceElementProperty{ get; };
    static Windows.UI.Xaml.DependencyProperty ReplacementColorProperty{ get; };
}

}
```

# Appendix
<!-- Anything else that you want to write down for posterity, but
that isn't necessary to understand the purpose and usage of the API.
For example, implementation details. -->

## DatePicker

In WinUI 2.2, controls began to be re-designed to have rounded corners, marking a shift in our overall design language.
There's more information on rounded corners in WinUI [here](https://docs.microsoft.com/en-us/windows/uwp/design/style/rounded-corner),
but the general purpose of the rounded corners design shift is to evoke warmth and trust,
and make the UI easier for users to visually process.
Since this shift, certain controls have adopted the new styling and recieved rounded corners, but some have not.
This creates a strong visual inconsistency in WinUI apps, where certain pieces of an app may look modern and others may look dated.
Examples of this include the DatePicker and TimePicker controls. While the corners of the controls themselves are rounded, the selection rectangle within the control is still squared off. Buttons and other areas inside these controls are also still squared off, making them look dated when placed alongside other controls that are more modernly designed, such as
[NavigationView](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/navigationview).

Recently, [ListView was given design updates](https://github.com/microsoft/microsoft-ui-xaml-specs/blob/user/anawish/ListViewGridViewDesignUpdates/active/ListViewGridView/listviewgridview-designupdates.md) to round the corners of its items. DatePicker and TimePicker should follow in these footsteps, and make sure that they adopt any of the ListView design elements that are relevant. This includes general rounding of selection visuals, as well as rounded grey backplates for items that get hovered.

This spec will detail a number of changes to update the designs of DatePicker and TimePicker so that they are more
visually aligned with modern WinUI controls. At a high level, some key parts of these updated styles are: a rounded selection rectangle; rounded backplates on items, buttons, and scroll buttons on  hover; and new animations that are aligned with other controls.

These visual changes to DatePicker and TimePicker will in part be made possible by the new `MonochromaticOverlayPresenter` API which is described above. This class provides the logic behind displaying the 'inverted' selection rectangle that spans across all three columns in DatePicker and TimePicker, and giving it the correct foreground color to have appropriate contrast over the accent colored background.

### Visual Examples
<!-- Use this section to provide a brief description of the feature.
For an example, see the introduction to the PasswordBox control
(http://docs.microsoft.com/windows/uwp/design/controls-and-patterns/password-box). -->

**DatePicker:**

As you can see on the left, the old version of DatePicker contains squared elements inside of it. The new version of DatePicker will round off these elements.

![Shows the old DatePicker visuals alongside the new DatePicker visuals](images/datepicker-evolution.PNG)

**TimePicker:**

Similarly to DatePicker, the old version of TimePicker contains squared elements inside of it. The new version of TimePicker will round off these elements.

![Shows the old TimePicker visuals alongside the new TimePicker visuals](images/timepicker-evolution.PNG)

**Rounded backplates and focus visuals**

As you can see in the mockup below, all buttons and items (individual cells) within DatePicker and TimePicker will receive a rounded grey backplate when hovered or pressed. In addition to this, columns within DatePicker and TimePicker will receive rounded focus rectangles (as shown below).

![Shows a DatePicker with scroll and check buttons being hovered, as well as the last column being focused upon](images/DPTP-other-states.PNG)


## Detailed Task Breakdown for styling implementation
The following steps apply to both DatePicker and TimePicker, unless otherwise noted.

1. The background color of the overall flyout should change, as shown in mockups above.

2. Selected items (entire rows) should have a rounded (4px corner radius) accent-color backplate. This backplate should have a 32px height, and have 4px margin on the left/right and 2px margin on the top/bottom from its overall footprint.

3. When items (individual cells, i.e. "November") are in a hover or pressed state, they will have a rounded (4px corner radius) grey backplate, with the same margins from its overall footprint as the selection row has described above. This backplate should also be 32px in height.

4. The scroll up/down button visuals should use caret icons (rather than the current chevron icons).

5. When the scroller buttons are hovered, they should have a rounded grey backplate that have a height of 12px, and a 4px margin on all sides from their overall button footprints.

6. The check and X buttons at the bottom of the Date/TimePicker should also be updated to use new icons as shown in mockups above.

7. On hover, the check and X buttons should also receive a rounded gray backplate with 4px margins on all sides from its overall button footprint.

8. Focus visuals for all buttons need to be rounded.

9. **DatePicker only**: Items in columns should now be left-aligned, rather than center-aligned as they were previously.

10. Columns within an expanded Date/TimePicker can be focused upon. For the column focus, the black focus rectangle will need to be rounded.

11. Animations: Date/TimePicker should have an opening/closing animation and use the same easing/timing as other controls.



================================================
FILE: specs/FooterMenuItemTemplate-spec.md
================================================
# Background

The [`NavigationView.FooterMenuItems`](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.footermenuitems?view=winui-2.5) property provides a way to place NavigationView items into a bottom-aligned (or right-aligned, if your NavigationView is in top mode) section of a NavigationView. This is distinct from the [`NavigationView.PaneFooter`](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.panefooter?view=winui-2.5) property, as only Navigation items should be placed in the Footer menu, while any kind of content can be placed in the PaneFooter.

<img src="images/footermenu-example.png" height="400" alt="Image of a NavigationView with labels pointing to main menu items and footer menu items"/>

Currently, the DataTemplate that's assigned to the [`NavigationView.MenuItemTemplate`](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.menuitemtemplate?view=winui-2.5) property is applied to all Navigation items in the NavigationView. This means that if you add both regular NavigationView menu items and NavigationView footer menu items, they will automatically have the same data template applied. This is an issue as there's no current way to provide a standardized data template for all footer menu items that's separate/different from the data template used for all main menu items.

# Description

In order to apply a data template to all items in the footer menu of your NavigationView, use the `NavigationView.FooterMenuItemTemplate` property. This property is similar to [NavigationView.MenuItemTemplate](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.menuitemtemplate?view=winui-2.5), but only applies to items placed in NavigationView's footer menu. It takes in a `DataTemplate` and applies that template to any Navigation item placed in the footer menu.

To apply different data templates to individual Navigation items within your footer menu based on certain criteria, use the `NavigationView.FooterMenuItemTemplateSelector`. This property is similar to the [NavigationView.MenuItemTemplateSelector](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.menuitemtemplateselector?view=winui-2.5), but only applies to items placed in NavigationView's footer menu.

The Settings item will not be affected by FooterMenuItemTemplate as it is not technically a part of the FooterMenuItems collection.

The [NavigationView.MenuItemTemplate](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.menuitemtemplate?view=winui-2.5) will only apply to Navigation items that are placed in the main menu of a NavigationView.


# Examples

Example showing how a NavigationView can have different object types for main and footer menu items, and apply a different DataTemplate to each.

```xml
<muxc:NavigationView x:Name="NavView" SelectionChanged="NavView_SelectionChanged"
                     MenuItemsSource="{x:Bind MainMenuItems}" FooterMenuItemSource="{x:Bind Accounts}">
    <muxc:NavigationView.MenuItemTemplate>
        <DataTemplate x:DataType="local:MainMenuItem">
            <muxc:NavigationViewItem Icon="{x:Bind ItemIcon}" Content="{x:Bind Name}" MenuItemsSource="{x:Bind Children}"/>
        </DataTemplate>
    </muxc:NavigationView.MenuItemTemplate>
    <muxc:NavigationView.FooterMenuItemTemplate>
        <DataTemplate x:DataType="local:AccountDataObject">
            <Grid>
                <Grid.ColumnDefinitions>
                    <ColumnDefinition Width="45"/>
                    <ColumnDefinition Width="*"/>
                </Grid.ColumnDefinitions>
                <Image Grid.Column="0" Source="{x:Bind ProfilePhoto}" Height="30" Width="30" HorizontalAlignment="Left"/>
                <TextBlock Grid.Column="1" Text="{x:Bind AccountName}" HorizontalAlignment="Left" VerticalAlignment="Center"/>
            </Grid>
        </DataTemplate>
    </muxc:NavigationView.FooterMenuItemTemplate>
</muxc:NavigationView>

```


# API Notes


The following APIs are members of `NavigationView`.

| Name | Description |
| - | - |
| FooterMenuItemTemplate | Gets or sets the [DataTemplate](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.datatemplate) used to display each footer menu item. |
| FooterMenuItemTemplateSelector | Gets or sets a reference to a custom [DataTemplateSelector](https://docs.microsoft.com/uwp/api/windows.ui.xaml.controls.datatemplateselector) logic class. The DataTemplateSelector referenced by this property returns a template to apply to Navigation items placed in the footer menu.


# API Details
<!-- The exact API, in MIDL3 format (https://docs.microsoft.com/en-us/uwp/midl-3/) -->

```csharp
[MUX_PREVIEW]
    {
        Windows.UI.Xaml.DataTemplate FooterMenuItemTemplate { get; set; };
        Windows.UI.Xaml.Controls.DataTemplateSelector FooterMenuItemTemplateSelector { get; set; };

        static Windows.UI.Xaml.DependencyProperty FooterMenuItemTemplateProperty { get; };
        static Windows.UI.Xaml.DependencyProperty FooterMenuItemTemplateSelectorProperty { get; };
    }

```



================================================
FILE: specs/NavigationViewTemplateSettings-OpenPaneLength.md
================================================
NavigationViewTemplateSettings.OpenPaneLength
===

# Background

_This spec adds an `OpenPaneLength` property to the Xaml
[NavigationViewTemplateSettings](https://docs.microsoft.com//windows/winui/api/microsoft.ui.xaml.controls.navigationviewtemplatesettings) class_

The (existing) WinUI [NavigationView](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.NavigationView) control has
a list of items you can view, and a content area that shows the selected item.
The list is shown in a pane that can be open, closed or partially open (compact).
The exact width of the open pane can be specified using the
[NavigationView.OpenPaneLength](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.NavigationView.OpenPaneLength)
property.

Example of compact pane:

![example of compact pane](images/nav-pane-closed.jpg)

Example of open pane:

![example of open pane](images/nav-pane-open.jpg)

The new property in this spec is a read-only `NavigationViewTemplateSettings.OpenPaneLength`,
to go along with the existing read/write `NavigationView.OpenPaneLength`.
It returns the `min` between `NavigationView.OpenPaneLength` and the window width.
This was necessary to fix a bug where the NavigationView pane contents were being cropped when
`OpenPaneLength` surpasses the window's width.
`NavigationViewTemplateSettings.OpenPaneLength` is set in `SplitView` and `ShadowCaster` template;
it was previously a simple template binding to `NavigationView.OpenPaneLength` property.

(Naming note: these APIs use "Length" rather than "Width" because
in the original design it was envisioned that there woould be a vertical mode in the future,
where this could represent a height too.)

TemplateSettings properties are not commonly used by app developers,
however, in situations when they copy a WinUI control's template into their own project,
there is a Xaml error when the TemplateSettings property is not public.
See [issue #6682](https://github.com/microsoft/microsoft-ui-xaml/issues/6682)
for more information on the error caused by non-public TemplateSettings.

# API Pages

## NavigationViewTemplateSettings.OpenPaneLength

Gets the `min` between `OpenPaneLength` and the window's width.
This is the calculated value of the width of the pane when opened and fully expanded. Defaults to 320.0 in [view pixels](https://docs.microsoft.com/uwp/api/Windows.Graphics.Display.DisplayInformation.RawPixelsPerViewPixel)

(Type: Double)

This example shows the `OpenPaneLength` property being used in the `ControlTemplate` for `NavigationView`
to pass through to the
[SplitView.OpenPaneLength](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.SplitView.OpenPaneLength).

```xml
<ControlTemplate TargetType="NavigationView">
    <!-- ... -->
    <SplitView
        OpenPaneLength="{Binding RelativeSource={RelativeSource TemplatedParent}, Path=TemplateSettings.OpenPaneWidth}"
        Background="{TemplateBinding Background}"
        BorderBrush="{ThemeResource NavigationViewItemSeparatorForeground}"
        BorderThickness="{ThemeResource NavigationViewBorderThickness}"
        CompactPaneLength="{TemplateBinding CompactPaneLength}"
        DisplayMode="Inline"
        IsPaneOpen="{Binding RelativeSource={RelativeSource TemplatedParent}, Path=IsPaneOpen, Mode=TwoWay}"
        IsTabStop="False"
        PaneBackground="{ThemeResource NavigationViewDefaultPaneBackground}">

```

_Spec note: Usage available to view in this PR: [#7341](https://github.com/microsoft/microsoft-ui-xaml/pull/7341)_

# API Details

```c# (but really MIDL3)
[webhosthidden]
unsealed runtimeclass NavigationViewTemplateSettings : Windows.UI.Xaml.DependencyObject
{
    // ...

    [MUX_DEFAULT_VALUE("320.0")]
    Double OpenPaneLength{ get; };

    static Windows.UI.Xaml.DependencyProperty OpenPaneLengthProperty{ get; };
}
```

# Appendix

The NavigationView pane is open when it is expanded to its full width.
It is visible when the pane is shown - even in compact mode.
See [NavigationView.IsPaneOpen](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.ispaneopen)
and [NavigationView.IsPaneVisible](https://docs.microsoft.com/windows/winui/api/microsoft.ui.xaml.controls.navigationview.ispanevisible)
for additional information on the distinction.



================================================
FILE: specs/Popup-AdditionalLayoutProperties-Spec.md
================================================
Popup additional layout properties
===

# Background

[Popups](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Primitives.Popup)
and
[flyouts](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Primitives.FlyoutBase)
in XAML are given two modes of display:
* They can either appear as part of the rest of XAML,
in which case they're confined to the bounds of the XAML root,
* Or they can appear in their own HWND, which
allows them to escape the bounds of the XAML root.  This is common for elements such as context menus.

[CommandBarFlyout](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CommandBarFlyout)
is one such element, but since it's defined in the WinUI 2 controls library
rather than in the OS, it does not
have access to the HWND used to allow it to escape the XAML root's bounds.  As such, it has no way to
determine which monitor it's being displayed in, which makes it unable to know whether it has enough visual space
to open the popup for its secondary commands _below_ its primary commands or whether it should open them above instead.

This new API adds three properties and an event to `Popup` which will allow apps to specify where it logically
desires a popup
to be displayed relative to another element, and then respond to where system XAML was able to actually place
the popup.  This will allow elements such as `CommandBarFlyout` to be able to rely on system XAML for the placement of their
child popups in a way that will take monitor or app bounds into account without needing to do that accounting manually.

## Visual Examples

**Opening down**

When CommandBarFlyout has enough space below its primary commands, we want it to open down.

Secondary commands flyout closed:

![Shows the CommandBarFlyout not yet open with sufficient monitor space below it](images/CommandBarFlyout-SufficientSpace.png)

Secondary commands flyout open:

![Shows the CommandBarFlyout opened down](images/CommandBarFlyout-SufficientSpace-Open.png)

**Opening up**

When CommandBarFlyout does *not* have enough space below its primary commands, we want it to be able to open up.

Secondary commands flyout closed:

![Shows the CommandBarFlyout not yet open with insufficient monitor space below it](images/CommandBarFlyout-InsufficientSpace.png)

Secondary commands flyout open:

![Shows the CommandBarFlyout opened up](images/CommandBarFlyout-InsufficientSpace-Open.png)

# API Pages

## Popup class

```csharp
class Popup
{
    // Existing APIs
    // ...

    // New APIs
    FrameworkElement PlacementTarget { get; set; }
    PopupPlacementMode DesiredPlacement { get; set; }
    PopupPlacementMode ActualPlacement { get; }

    public event System.EventHandler<object> ActualPlacementChanged;
}
```

The example below shows how the `Placement` APIs are used by the
[CommandBarFlyout](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CommandBarFlyout)
to position its
[CommandBarFlyoutCommandBar](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Primitives.CommandBarFlyoutCommandBar)'s
secondary commands Popup, and how to respond to the event raised when XAML places the Popup.

```xml
<!-- Part of the CommandBarFlyoutCommandBar's default template -->
<Popup
    x:Name="OverflowPopup"
    PlacementTarget="{Binding ElementName=PrimaryItemsRoot}"
    DesiredPlacement="Bottom">
</Popup>
```

```csharp
void OnApplyTemplate()
{
    m_overflowPopup = GetTemplateChild("OverflowPopup");
    m_overflowPopup.ActualPlacementChanged += OnOverflowPopupActualPlacementChanged;
}

void OnOverflowPopupActualPlacementChanged(object sender, object args)
{
    UpdateVisualState(useTransitions: false);
}

void UpdateVisualState(bool useTransitions)
{
    if (m_overflowPopup.ActualPlacement == PopupPlacementMode.Top)
    {
        VisualStateManager.GoToState(this, "ExpandedUp", useTransitions);
    }
    else
    {
        VisualStateManager.GoToState(this, "ExpandedDown", useTransitions);
    }
}
```

## Popup.PlacementTarget property

Use this property to describe which element the `Popup` should be positioned relative to.
Defaults to `null`.

If this is `null`, then `DesiredPlacement` is ignored, `ActualPlacement` is always `Auto`, and
`ActualPlacementChanged` is never raised.  If the `Popup` is in the visual tree, `PlacementTarget` will override what its
position would otherwise be set to by layout.  Setting `PlacementTarget` to an element under a different XAML root than
`Popup.XamlRoot` is invalid and will throw an `ArgumentException`.

Ignored if `DesiredPlacement` is `Auto`.

_Spec note: this property is analogous to the
[FlyoutBase.Target](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Primitives.FlyoutBase.Target)
property, but `Popup.Target` looked confusing, so we added the `Placement` prefix._

## Popup.DesiredPlacement property

Use this property to describe how you would ideally like the `Popup`
positioned relative to `PlacementTarget`.  Defaults to `Auto`.

If this is `Auto`, then `PlacementTarget` is ignored,
`ActualPlacement` is always `Auto` and `ActualPlacementChanged` is never raised.
If both `DesiredPlacement` and `PlacementTarget` are set and `HorizontalOffset` and/or `VerticalOffset`
are also set, then the latter two properties will offset the `Popup` from where it would have been
placed by `DesiredPlacement` and `PlacementTarget` alone.

Ignored if `PlacementTarget` is null.

## Popup.ActualPlacement property

Use this read-only property to determine where the popup was positioned.
Will always be `Auto` if either `PlacementTarget` and `DesiredPlacement` are not set.

## Popup.ActualPlacementChanged event

Raised whenever XAML changes the value of `ActualPlacement`,
which allows apps to respond to where a `Popup` was placed.

For example, use this to determine the visual state to go into,
based on whether a `Popup` is appearing above or below `PlacementTarget`.

This event is raised before the screen is refreshed, meaning that any visual changes made
in response to this event can be made before anything is drawn to the screen at the new position.
Will never be raised if either `PlacementTarget` and `DesiredPlacement` are not set.

## PopupPlacementMode enum

_Spec note: This is designed to align with the existing
[FlyoutPlacementMode](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Primitives.FlyoutPlacementMode)
enum, with the exception of the absence of "Full".  "Full" is absent since developers should use a Flyout
if they want something full-screen._

```csharp
enum PopupPlacementMode
{
    Auto,
    Top,
    Bottom,
    Left,
    Right,
    TopEdgeAlignedLeft,
    TopEdgeAlignedRight,
    BottomEdgeAlignedLeft,
    BottomEdgeAlignedRight,
    LeftEdgeAlignedTop,
    LeftEdgeAlignedBottom,
    RightEdgeAlignedTop,
    RightEdgeAlignedBottom
}
```

_Spec note: The meaning of "Left" and "Right" are swapped if
[FlowDirection](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.frameworkelement.flowdirection)
is `RightToLeft`._

# API Details

```csharp
namespace Windows.UI.Xaml.Controls.Primitives
{
    [webhosthidden]
    enum PopupPlacementMode
    {
        Auto,
        Top,
        Bottom,
        Left,
        Right,
        TopEdgeAlignedLeft,
        TopEdgeAlignedRight,
        BottomEdgeAlignedLeft,
        BottomEdgeAlignedRight,
        LeftEdgeAlignedTop,
        LeftEdgeAlignedBottom,
        RightEdgeAlignedTop,
        RightEdgeAlignedBottom
    };

    [webhosthidden]
    interface IPopup2
    {
        Windows.UI.Xaml.FrameworkElement PlacementTarget;
        Windows.UI.Xaml.Controls.Primitives.PopupPlacementMode DesiredPlacement;
        Windows.UI.Xaml.Controls.Primitives.PopupPlacementMode ActualPlacement { get; };

        event Windows.Foundation.EventHandler<Object> ActualPlacementChanged;

        static Windows.UI.Xaml.DependencyProperty PlacementTargetProperty{ get; };
        static Windows.UI.Xaml.DependencyProperty DesiredPlacementProperty{ get; };
        static Windows.UI.Xaml.DependencyProperty ActualPlacementProperty{ get; };
    };
}
```



================================================
FILE: specs/public-api-review-process.md
================================================
WinUI Platform Public Spec Review Process
===

## Introduction
We are excited to formally re-introduce a community feedback process to our API authoring workflow! This will leverage the collective wisdom and insights of the community, allowing us to develop more robust and comprehensive APIs that meet the needs of our diverse user base.

We assure our community that their input is invaluable to us, and we are dedicated to fostering a transparent and collaborative environment. By adopting this structured feedback process outlined below, we aim to set clear expectations and handle all contributions with the utmost professionalism and consideration.


## Public Post on Github
- The drafted spec from is posted as a PR under the `./specs/` directory.

    - Example PR: [Popup placement properties API spec](https://github.com/microsoft/microsoft-ui-xaml/pull/4905)
    - Every spec will link to this public spec markdown file. <!-- TODO: Add link once it is public -->
- A dedicated discussion thread will be created to announce that we are actively gathering feedback for the API.
- A Github issue with `spec-review` tag will be created to represent the new API proposal. It will be tracked in the Github API Spec Review Board:

    > [API Specs Review](https://github.com/orgs/microsoft/projects/1328/views/1)

    - If the proposed API addresses any existing Github issues, the existing issue will be linked to the `spec-review` issue representing the API proposal.

## Gather Feedback
The issue is open for a predefined period of **1 month** to gather feedback from the community.
The start and end dates will be outlined in the spec and in the [API Specs Review](https://github.com/orgs/microsoft/projects/1328/views/1) Board.

- Community members can provide feedback by **commenting directly on the PR**, or through a **code suggestion** with Github tools.
- Feedback should be constructive and specific, addressing potential use cases, design concerns, and functionality.

> **Examples of constructive feedback:**
>
> - Developer use cases and edge cases – sample code and screenshots of such scenarios are very much welcomed.
>
>    - ~~Don't: "You should use a ToggleButton and have it to the left"~~
>    - Do: "Can I customize the content here? Here is some code and screenshots showcasing my needed scenario.”
>
> - Consistent API naming conventions – and comparisons of said APIs across WinUI and industry standards.
>
>   - ~~Don't: "This is a bad name, it should be called something different."~~
>   - Do: "Normally, these types of properties are named IsFoo, like IsFoo on X's BarControl. < link to learn.microsoft.com  API property page or other framework's documentation />"
>
> - Raised accessibility concerns and use cases
>
>   - ~~Don't: "This control is not accessible."~~
>   - Do: "How does this control support screen readers? Here is an example of how it should announce state changes to ensure accessibility."
> - Raised usability concerns with different languages
>
>    - ~~Don't: "This won't work support other languages."~~
>    - Do: “How will the control layout handle RTL languages? Here is an example of what could appear on the control.”
>
> - Inquiries and suggestions regarding scenarios and usages
>
>    - ~~Don't: "This control is missing features."~~
>    - Do: “Does it have an orientation property to toggle horizontal and vertical? Here is an example of how this property can be used in different scenarios.”

## Handle Feedback

We are commited to respond to all feedback in different manners depending on the feedback category.

**Feedback categorization:** In general, feedback will be prioritized into the categories below based on relevance, impact, and feasibility.

- **Immediate Action:** Feedback that will be addressed in the current specification iteration due to its high relevance and feasibility.
- **Deferred Action:** Feedback that is valuable but not feasible for immediate implementation. This will be considered for future updates.
- **Not Planned:** Feedback that is not aligned with current goals or is not feasible to implement. Reasons for this will be clearly communicated.
- **Discussion:** Feedback is an open-ended discussion, and no immediate action is necessary.

<br>

**Acknowledgment:** All feedback will be acknowledged by at least one of the following means:

- **Immediate & Deferred Action:**

    - Final post calling out specific points that influenced decisions

        *and / or*

    - In-line response to comments

        *and / or*

    - “Resolve comment” to signify that the feedback  has been incorporated into the spec draft

        *and / or*

    - Directly commit the suggestion if it is done via code suggestion with Github tools, and it is appropriate

- **Not Planned:**

    - In-line response to comments explaining reasoning

        *and*

    - “Resolve comment” to signify that it is not planned

- **Discussion:**

    - A “eye” emoji by the author / poster to signify that it is read.

## Consolidate Feedback

We will carefully consider each contribution and update the spec to reflect the accepted feedback. A summary of changes will be shared, highlighting each significant feedback point. Finally, the PR containing the final spec is merged in.


### Passive Monitoring of Relevant Feedback and Issues

- Continuous monitoring for any late feedback or issues is passively maintained.
- Future enhancements or changes based on post-implementation feedback are considered in subsequent spec reviews.


================================================
FILE: specs/xaml-backdrop-api.md
================================================


Xaml Backdrop APIs
===

# Background

Composition in WinAppSDK has a general
[ISystemBackdropController](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.ISystemBackdropController)
interface that's concretely implemented by
[MicaController](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.MicaController)
and [DesktopAcrylicController](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.DesktopAcrylicController).
A backdrop is a visual effect you can use as the background for your window (or island).
For example the Desktop Acrylic backdrop lets you set as the background of your window the desktop wallpaper behind it, but visually modified.
[More info](https://learn.microsoft.com/en-us/windows/apps/design/style/acrylic).

These existing Mica and Desktop Acrylic controllers allow you to set the backdrops onto a
[WindowId](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.WindowId),
and there's currently only an awkward way to get a `WindowId` from a Xaml object such as
[Window](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.Window).

The awkwardness only begins there; you also need to work with a _system_
[DispatcherQueue](https://docs.microsoft.com/uwp/api/Windows.System.DispatcherQueue),
coordinate with the
[Loaded](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.FrameworkElement.Loaded)
event, and check
[IsSupported](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.MicaController.IsSupported)
to see if you need to provide a fallback (Mica isn't supported on Windows 10).

So it's a great feature and works, but it's difficult to use.
[Here's a full code example of the current solution](https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/system-backdrop-controller#example-use-mica-in-a-windows-appsdkwinui-3-app).

The purpose of the new APIs here are to make backdrops much easier to use in a Xaml app,
allowing you to simply set a backdrop as a property on a `Window`.


# API Pages

## Window.SystemBackdrop property

_This description will also apply to `SystemBackdrop` properties on `Popup`, `FlyoutBase`,
and `DesktopWindowXamlSource`._

Sets a `SystemBackdrop` to apply that backdrop to this `Window`.

This backdrop is what will render behind the content specified in `Window.Content`.
If all of the content is fully opaque, this backdrop will have no visible effect.

The following example creates a Window with a Mica backdrop.

```xml
<Window
    x:Class="App3.MainWindow"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml" >

    <Window.SystemBackdrop>
        <MicaBackdrop/>
    </Window.SystemBackdrop>

    <Grid ColumnDefinitions="Auto,*">

        // This area has a transparent background, so the Mica backdrop will be mostly visible
        // For example if there are buttons here, the backdrop will show up in
        // the margins and gaps between the button text
        <local:NavigationControls/>

        // This area has an opaque background, so the Mica backdrop won't be visible
        <local:ContentArea Background="White"/>

    </Grid>
</Window>
```


## MicaBackdrop class

_Same description applies to `DesktopAcrylicBackdrop` class_

_See also the base class: `SystemBackdrop`_

Use this class to set a backdrop on a
[Window](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.Window),
[Popup](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.Controls.Primitives.Popup)\*,
or [FlyoutBase](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.Controls.Primitives.FlyoutBase)\* (such as a `Flyout` or `MenuFlyout`).
* `Popup`/`MenuFlyout` `SystemBackdrop` support is not  available in WinAppSDK 1.3.0, but is expected to light up in a subsequent release. Note also `SystemBackdrop` will only work in "windowed" popups, i.e. those with *ShouldConstrainToRootBounds=False*.

For example:

```xml
<Window x:Class="MyApp.MainWindow">

    <Window.SystemBackdrop>
        <MicaBackdrop MicaKind="BaseAlt"/>
    </Window.SystemBackdrop>

</Window>
```

Note that `MicaBackdrop` isn't supported on all systems.
In such cases a solid color will be used instead of the Mica effect.


## SystemBackdrop class

Use this class to create a custom system backdrop.
You don't create this class directly, but subclass it to add your custom support (note the protected constructor). This class is the base of built-in backdrop materials `MicaBackdrop` and `DesktopAcrylicBackdrop`.

Generally, the custom material overrides `OnTargetConnected` to create and configure a backing [ISystemBackdropController](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.isystembackdropcontroller?view=windows-app-sdk-1.3), which will manage the [CompositionBrush](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.compositionbrush?view=windows-app-sdk-1.3) used to fill the backdrop region. The brush's ultimate pixel rendering is affected by the environment/policy (set via [SystemBackdropConfiguration](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.systembackdropconfiguration?view=windows-app-sdk-1.3)) and material's appearence parameters, exposed via general (eg `ICompositionControllerWithTargets.SystemBackdropState` ∈ { _`Active` / `Fallback` / `HighContast`_ }) and material-specfic (eg `MicaController.Kind` ∈ { _`Base` / `BaseAlt`_} _SystemBackdropController_ properties.

* The controllers available today (`MicaController` and `DesktopAcrylicContoller`) support the following parameters for customizing their appearence: [FallbackColor](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.desktopacryliccontroller.fallbackcolor?view=windows-app-sdk-1.3), [LuminosityOpacity](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.desktopacryliccontroller.luminosityopacity?view=windows-app-sdk-1.3), [TintColor](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.micacontroller.tintcolor?view=windows-app-sdk-1.3), and [TintOpacity](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.micacontroller.tintopacity?view=windows-app-sdk-1.3).
* The provided Xaml backdrop materials `MicaBackdrop` and `DesktopAcrylicBackdrop` currently do not expose `FallbackColor` or the material customization properties (`TintOpacity`, etc), instead relying on the default Light/Dark configurations of the underlying `MicaController` and `DesktopAcrylicController`. To customize these properties, createa a custom material class deriving from SystemBackdrop that exposes the desired properties.

The following example shows a simple custom system backdrop class that's implemented using
[MicaController](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.MicaController).


```cs
public class MicaSystemBackdrop : SystemBackdrop
{
    MicaController _micaController;

    protected override void OnTargetConnected(ICompositionSupportsSystemBackdrop connectedTarget, XamlRoot xamlRoot)
    {
        // Calling the base OnTargetConnected initializes the default configuration object
        // returned by GetDefaultSystemBackdropConfiguration() to reflect environment changes
        // affecting this SystemBackdrop instance (specified by {connecteedTarget, XamlRoot}).
        base.OnTargetConnected(connectedTarget, xamlRoot);

        // Although this sample does not support sharing MicaSystemBackdrop instances
        // (eg Window1.SystemBackdrop = Window2.SystemBackdrop = myMicaSystemBackdrop)
        // such sharing is possible and is supported by the built-in DestkopAcrylicBackdrop and
        // MicaBackdrop materials. To implement sharing in a custom material, vectorize the
        // backing ICompositionController storage to keep a separate instance for each usage
        // context (eg via map keyed on connectedTarget). Note that SystemBackdrop similarly
        // vectorizes the associated default configuration objects returned by
        // GetDefaultSystemBackdropConfiguration(connectedTarget, xamlRoot), ensuring
        // the configuration reflects each usage context when SystemBacdkrop is shared.
        if(_micaController != null)
        {
            throw new Exception("This controller cannot be shared");
        }

        SetControllerConfig(connectedTarget, xamlRoot);

        _micaController = new MicaController();
        _micaController.AddSystemBackdropTarget(connectedTarget);
    }

    protected override void OnTargetDisconnected(ICompositionSupportsSystemBackdrop disconnectedTarget)
    {
        base.OnTargetDisconnected(disconnectedTarget);

        _micaController.RemoveSystemBackdropTarget(disconnectedTarget);
        _micaController = null;
    }

    void SetControllerConfig(ICompositionSupportsSystemBackdrop connectedTarget, XamlRoot xamlRoot)
    {
        var config = GetDefaultSystemBackdropConfiguration(connectedTarget, xamlRoot);
        _micaController.SetSystemBackdropConfiguration(config);
    }
}
```

## SystemBackdrop.GetDefaultSystemBackdropConfiguration method

Returns a default
[SystemBackdropConfiguration](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.SystemBackdropConfiguration)
object that is set and maintained automatically for each `SystemBackdrop` usage context (i.e `connectedTarget`), and can be passed to
[ISystemBackdropControllerWithTargets.SetSystemBackdropConfiguration](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Composition.SystemBackdrops.ISystemBackdropControllerWithTargets.SetSystemBackdropConfiguration) to apply the default policy.

The properties on `SystemBackdropConfiguration` you receive may change over time:

* `Theme`: set based on [ElementTheme](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.ElementTheme) of the target element (obtained from xamlRoot.Content)
   * If `FallbackColor`, `LuminosityOpacity`, `TintColor`, or `TintOpacity` are modified by the material's implementation, changes to associated [SystemBackdropConfiguration.Theme](https://learn.microsoft.com/en-us/windows/windows-app-sdk/api/winrt/microsoft.ui.composition.systembackdrops.systembackdropconfiguration.theme?view=windows-app-sdk-1.3) will no longer automatically toggle the controller's theme (since  default Dark and Light configurations are no longer apopropriate). In this case, the material's appearence properties need to be manually updated to match the new Theme in `SystemBackdrop.OnDefaultSystemBackdropConfigurationChanged`.

* `IsInputActive`: true if the target of the `SystemBackdrop` is in the active window.

* `IsHighContrast`: true if the target of the `SystemBackdrop` is in high contrast mode.


## SystemBackdrop.OnDefaultSystemBackdropConfigurationChanged virtual protected method

Override this method to be called when one of the properrties (described above) on the object returned by `GetDefaultSystemBackdropConfiguration` has changed.

* This is useful when implementing a custom `SystemBackdropConfiguration` that incorporates some of the tracked property states but is different in some way from the default policy. First, obtain a  `SystemBackdropConfiguration` object from `GetDefaultSystemBackdropConfiguration` as usual, but do not apply it via `CompositionContoller.SetSystemBackdropConfiguration`. Instead  create an additional `SystemBackdropConfiguration` object that is updated on `OnDefaultSystemBackdropConfigurationChanged` by applying custom logic to the tracked property (eg ignoring Theme change). The second `SystemBackdropConfiguration` object is hooked up to `CompositionContoller.SetSystemBackdropConfiguration`, applying the custom policy.

## Other `SystemBackdrop` members

| Member | Description |
| - | - |
| `OnTargetConnected` virtual method | Called when this object is attached to a valid container, for example when set on `Window.SystemBackdrop`. Override to create and configure the underlying `CompositionController` and its `SystemBackdropConfiguration`. |
| `OnTargetDisconnected` virtual method | Called when this object is cleared from its container |



# API Details

```c# (but really MIDL3)
namespace Microsoft.UI.Xaml.Media
{
  [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
  [webhosthidden]
  unsealed runtimeclass MicaBackdrop : Microsoft.UI.Xaml.Media.SystemBackdrop
  {
      MicaBackdrop();

      Microsoft.UI.Composition.SystemBackdrops.MicaKind Kind { get; set; };

      static Microsoft.UI.Xaml.DependencyProperty KindProperty { get; };
  }

  [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
  [webhosthidden]
  unsealed runtimeclass DesktopAcrylicBackdrop : Microsoft.UI.Xaml.Media.SystemBackdrop
  {
      DesktopAcrylicBackdrop();
  }

  [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
  [webhosthidden]
  [constructor_name("Microsoft.UI.Xaml.Media.ISystemBackdropFactory")]
  unsealed runtimeclass SystemBackdrop
      : Microsoft.UI.Xaml.DependencyObject
  {
      [method_name("CreateInstance")] protected SystemBackdrop();

      overridable void OnTargetConnected(
        Microsoft.UI.Composition.ICompositionSupportsSystemBackdrop connectedTarget,
        Microsoft.UI.Xaml.XamlRoot xamlRoot);

      overridable void OnTargetDisconnected(
        Microsoft.UI.Composition.ICompositionSupportsSystemBackdrop disconnectedTarget);

      Microsoft.UI.Composition.SystemBackdrops.SystemBackdropConfiguration GetDefaultSystemBackdropConfiguration(
        Microsoft.UI.Composition.ICompositionSupportsSystemBackdrop target,
        Microsoft.UI.Xaml.XamlRoot xamlRoot);

      overridable void OnDefaultSystemBackdropConfigurationChanged(
        Microsoft.UI.Composition.ICompositionSupportsSystemBackdrop target,
        Microsoft.UI.Xaml.XamlRoot xamlRoot);
  };
}

namespace Microsoft.UI.Xaml
{
  [contract(Microsoft.UI.Xaml.WinUIContract, 1)]
  [webhosthidden]
  [contentproperty("Content")]
  unsealed runtimeclass Window
  {
    // ... existing ...

      [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
      {
          Microsoft.UI.Xaml.Media.SystemBackdrop SystemBackdrop;
      }
  }
}

namespace Microsoft.UI.Xaml.Controls.Primitives
{
  [contract(Microsoft.UI.Xaml.WinUIContract, 1)]
  [webhosthidden]
  [contentproperty("Child")]
  runtimeclass Popup
      : Microsoft.UI.Xaml.FrameworkElement
  {
    // ... Existing ...

    [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
    {
        Microsoft.UI.Xaml.Media.SystemBackdrop SystemBackdrop;
        static Microsoft.UI.Xaml.DependencyProperty SystemBackdropProperty{ get; };
    }
  }

  [contract(Microsoft.UI.Xaml.WinUIContract, 1)]
  [webhosthidden]
  [constructor_name("Microsoft.UI.Xaml.Controls.Primitives.IFlyoutBaseFactory")]
  unsealed runtimeclass FlyoutBase
      : Microsoft.UI.Xaml.DependencyObject
  {
    // ... existing ...

    [contract(Microsoft.UI.Xaml.WinUIContract, 4)]
    {
        Microsoft.UI.Xaml.Media.SystemBackdrop SystemBackdrop;
        static Microsoft.UI.Xaml.DependencyProperty SystemBackdropProperty{ get; };
    }
  }

}
```




================================================
FILE: specs/xaml-resource-references-tracing-spec.md
================================================
Tracing XAML resource reference lookup failures
===

# Background

A XAML resource is an item in a
[ResourceDictionary](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.ResourceDictionary)
that can be referenced in markup with a `{StaticResource}` or `{ThemeResource}` reference.
For example:

```xml
<StackPanel >
    <StackPanel.Resources>
        <SolidColorBrush x:Key="myBrush" Color="Red"/>
    </StackPanel.Resources>

    <Rectangle Fill="{StaticResource myBrush}"/>
```

`ResourceDictionary`s can be defined in multiple places, so the resource reference is resolved
as a search.

Failure to resolve a XAML resource reference is one of
the most common causes of app crashes. Such failures manifest in the _native code_ debug output with the
message "Cannot find a Resource with the Name/Key *foo*", and generally fall into one of two
buckets:

1. The referenced resource legitimately does not exist, e.g. the referenced key is misspelled or
the intended matching resource has not been added to the app.
2. The referenced resource *does* exist in the app, but it is not reachable from the reference
at run-time.

Unfortunately, the stowed exception message is the *only* information provided about the error,
which makes it difficult or, more often, outright impossible to debug.

This spec describes a new
API on the `DebugSettings` class that developers can use to access more detailed information about
the resource reference lookup failure.
The new APIs here are patterned after the existing
[DebugSettings.BindingFailed](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.DebugSettings.BindingFailed)
and
[DebugSettings.IsBindingTracingEnabled](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.DebugSettings.IsBindingTracingEnabled)
APIs.


# API Pages

_(Updates to the
[DebugSettings](https://docs.microsoft.com/windows/windows-app-sdk/api/winrt/Microsoft.UI.Xaml.DebugSettings)
class)_

## DebugSettings.XamlResourceReferenceFailed Event

Occurs when a
[XAML resource reference](https://learn.microsoft.com/en-us/windows/apps/design/style/xaml-resource-dictionary)
cannot be resolved.

_Spec note: This API is similar to the `DebugSettings.BindingFailed` event. Like XAML resource references,
Bindings cannot be modeled solely through static evaluation, e.g. at compile-time, and so a run-time
event when a failure occurs is the best approach for providing developers with a means of determining the
root cause._

_Spec note: is there a version of the 'ResourceDictionary and XAML resource references' article that
links to the Windows App SDK documentation for relevant APIs?_

```c#
public event TypedEventHandler<DebugSettings,XamlResourceReferenceFailedEventArgs>
XamlResourceReferenceFailed

```

### Remarks

`IsXamlResourceReferenceTracingEnabled` must be `true` in order for this event to be raised.

Error information is also logged to the native debug output when the event is raised,
so attaching a `XamlResourceReferenceFailed` handler yourself is an advanced scenario for
getting the raw message programmatically.

## DebugSettings.IsXamlResourceReferenceTracingEnabled Property

Gets or sets a value indicating that when a XAML resource reference error occurs,
the `XamlResourceReferenceFailed` event should be raised,
and error information should be logged in the native debug output.

```c#
public bool IsXamlResourceReferenceTracingEnabled { get; set; }
```

### Remarks

This property is `true` by default. When XAML resource reference tracing is enabled and you
run your app with the native debugger attached, any  XAML resource reference errors appear
in the **Output** window in Microsoft Visual Studio.


## XamlResourceReferenceFailedEventArgs Class

Provides event data for the `DebugSettings.XamlResourceReferenceFailed` event.

```c#
public sealed class XamlResourceReferenceFailedEventArgs
```

### Remarks

`XamlResourceReferenceFailedEventArgs` is used for debugging XAML resource references. Register the event
handler using `DebugSettings`. It will receive a reference to this class. You'll mainly be
interested in the `Message` value, which you could log or send to **Debug** output.

The message in the event data contains the following information about the failed XAML resource
reference:

* The URI of the XAML page containing each `ResourceDictionary` that was searched
* The order in which the `ResourceDictionary`s were searched

You can use this information to investigate why the XAML resource reference could not be resolved;
perhaps the `ResourceDictionary` it is contained in was not in the list of searched
`ResourceDictionary`s, or perhaps that `ResourceDictionary` was searched which could indicate that
an incorrect resource key was specified.

Below is an example message from the WinUI Gallery sample app after an incorrect resource reference
(`OutputTextBlockStyl` rather than `OutputTextBlockStyle`) was deliberately inserted. If you know
that the desired resource is defined in `App.xaml`, then the failure to locate it in there is a
strong indicator of an erroneous reference.

Note: The below example output is for illustrative purposes only. The precise format of the message is
implementation-defined and may change in the future. Applications should not attempt to parse the message.

```
Beginning search for resource with key 'OutputTextBlockStyl'.
  Searching dictionary 'ms-appx:///Controls/ControlExample.xaml' for resource with key 'OutputTextBlockStyl'.
  Finished searching dictionary 'ms-appx:///Controls/ControlExample.xaml'.
  Searching dictionary 'Framework-defined colors' for resource with key 'OutputTextBlockStyl'.
  Finished searching dictionary 'Framework-defined colors'.
  Searching dictionary 'Framework ThemeResources.xbf' for resource with key 'OutputTextBlockStyl'.
    Searching theme dictionary (active theme: 'Light') for resource with key 'OutputTextBlockStyl'.
      Searching dictionary '<anonymous dictionary>' for resource with key 'OutputTextBlockStyl'.
      Finished searching dictionary '<anonymous dictionary>'.
    Finished searching theme dictionary (active theme: 'Light').
  Finished searching dictionary 'Framework ThemeResources.xbf'.
  Searching dictionary 'ms-appx:///App.xaml' for resource with key 'OutputTextBlockStyl'.
    Searching merged dictionary with index '1' for resource with key 'OutputTextBlockStyl'.
      Searching dictionary 'ms-appx:///Microsoft.UI.Xaml/Themes/themeresources.xaml' for resource with key 'OutputTextBlockStyl'.
        Searching theme dictionary (active theme: 'Light') for resource with key 'OutputTextBlockStyl'.
          Searching dictionary 'ms-appx:///Microsoft.UI.Xaml/Themes/themeresources.xaml' for resource with key 'OutputTextBlockStyl'.
          Finished searching dictionary 'ms-appx:///Microsoft.UI.Xaml/Themes/themeresources.xaml'.
        Finished searching theme dictionary (active theme: 'Light').
      Finished searching dictionary 'ms-appx:///Microsoft.UI.Xaml/Themes/themeresources.xaml'.
    Finished searching merged dictionary with index '1'.
    Searching merged dictionary with index '0' for resource with key 'OutputTextBlockStyl'.
      Searching dictionary 'ms-appx:///ItemTemplates.xaml' for resource with key 'OutputTextBlockStyl'.
      Finished searching dictionary 'ms-appx:///ItemTemplates.xaml'.
    Finished searching merged dictionary with index '0'.
    Searching theme dictionary (active theme: 'Light') for resource with key 'OutputTextBlockStyl'.
      Searching dictionary 'ms-appx:///App.xaml' for resource with key 'OutputTextBlockStyl'.
      Finished searching dictionary 'ms-appx:///App.xaml'.
    Finished searching theme dictionary (active theme: 'Light').
  Finished searching dictionary 'ms-appx:///App.xaml'.
Finished search for resource with key 'OutputTextBlockStyl'.
```


## XamlResourceReferenceFailedEventArgs.Message Property

A human-readable explanation (in English) of the XAML resource reference failure.

```c#
public string Message { get; }
```


# API Details
```c#
namespace Microsoft.UI.Xaml
{
  runtimeclass DebugSettings
  {
    // existing ...

    Boolean IsXamlResourceReferenceTracingEnabled;
    event Windows.Foundation.TypedEventHandler<Microsoft.UI.Xaml.DebugSettings,Microsoft.UI.Xaml.XamlResourceReferenceFailedEventArgs> XamlResourceReferenceFailed;
  };

  runtimeclass XamlResourceReferenceFailedEventArgs
  {
    String Message{ get; };
  };
}

```



================================================
FILE: specs/CalendarView/CalendarViewSpec1.md
================================================

# Background

The XAML [CalendarView](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CalendarView)
control shows the user a calendar and lets them pick a date (range).

A new set of `CalendarView` styling properties are introduced to allow greater customization of the
control's rendering in upcoming Windows OS releases.
These properties will be used in WinUI to align the CalendarView's styling with the rest of the
standard controls.

With this change, `CalendarView` still has its existing visualization (styles/templates) that
don't use these properties, and new ones that do.
By default, the older visualization is used.
The new visualization can be enabled by setting a boolean resource value
(see `CalendarViewBaseItemRoundedChromeEnabled` below).
And the `WinUI2`
[controls library](https://www.nuget.org/packages/Microsoft.UI.Xaml/))
sets this boolean. The end result is that these properties are ignored by default, but
come into play when an app is using WinUI2.

# Conceptual

## Today styling

The following properties of type
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
are used to customize the current day's rendering when `CalendarView.IsTodayHighlighted` is True:
`TodayBackground`, `TodayBlackoutBackground`, `TodayBlackoutForeground`,
`TodayHoverBackground`, `TodayPressedBackground`, `TodaySelectedInnerBorderBrush`.

### Showcasing the TodayBackground property in the month, year and decade views

The value of the `TodayBackground` property is used in the month, year and decade display modes
of the `CalendarView`:

```xml
<CalendarView TodayBackground='{StaticResource AccentFillColorDefaultBrush}'/>
```

![Default Today Month Background.](images/TodayMonthBackground.png)
![Default Today Year Background.](images/TodayYearBackground.png)
![Default Today Decade Background.](images/TodayDecadeBackground.png)

### Showcasing the TodayHoverBackground property - current date is hovered

The value of the `TodayHoverBackground` property is used when the user
hovers a pointer over the current date:

```xml
<CalendarView TodayHoverBackground='{StaticResource AccentFillColorSecondaryBrush}'/>
```

![Hover Today Background.](images/HoverTodayBackground.png)

### Showcasing the TodayPressedBackground property

The value of the `TodayPressedBackground` property is used when the user
clicks/taps the current date:

```xml
<CalendarView TodayPressedBackground='{StaticResource AccentFillColorTertiaryBrush}'/>
```

![Pressed Today Background.](images/PressedTodayBackground.png)

### Showcasing the `TodaySelectedInnerBorderBrush` property - current date is selected

The example sets the color to be used on the inner border for the current date when it is selected:

```xml
<CalendarView TodaySelectedInnerBorderBrush='{StaticResource TextOnAccentFillColorPrimaryBrush}'/>
```

![Selected Today Border.](images/SelectedTodayBorder.png)

## Blacked Out styling

The following properties of type
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
are used to customize the calendar items that are blacked out in the month view:
`BlackoutForeground`, `TodayBlackoutBackground`, `TodayBlackoutForeground`, `BlackoutStrikethroughBrush`.
A blacked out day is one that the user cannot select.

_Spec note: `BlackoutForeground` is an existing property, the other three are new to this spec._

_Spec note: how to set a blackout date isn't documented very well,
[issue](https://github.com/MicrosoftDocs/winrt-api/issues/1989)._

_Spec note:_
_"Not Brush" properties:_
_Background, BlackoutForeground, CalendarItemBackground, CalendarItemForeground, ContentLinkBackgroundColor, ContentLinkForegroundColor, Disabled, DragBackground, DragForeground, Effect, Enabled, Fill, Foreground, HeaderBackground, HeaderForeground, Mask, OutOfScopeBackground, OutOfScopeForeground, PaneBackground, PlaceholderBackground, PlaceholderForeground, PointerOverBackground, PointerOverForeground, PressedBackground, PressedForeground, RevealBackground, SelectedBackground, SelectedDisabledBackground, SelectedForeground, SelectedPointerOverBackground, SelectedPressedBackground, SelectionHighlightColor, SelectionHighlightColorWhenNotFocused, Source, Stroke, SystemBackdrop, TodayForeground_

_"Brush" properties:_
_ActualImageBrush, BorderBrush, Brush, CalendarItemBorderBrush, CheckBoxBorderBrush, CheckBoxBrush, CheckBoxDisabledBorderBrush, CheckBoxDisabledBrush, CheckBoxPointerOverBorderBrush, CheckBoxPointerOverBrush, CheckBoxPressedBorderBrush, CheckBoxPressedBrush, CheckBoxSelectedBrush, CheckBoxSelectedDisabledBrush, CheckBoxSelectedPointerOverBrush, CheckBoxSelectedPressedBrush, CheckBrush, CheckDisabledBrush, CheckHintBrush, CheckPressedBrush, CheckSelectingBrush, CompositionBrush, FillBrush, FocusBorderBrush, FocusSecondaryBorderBrush, FocusVisualPrimaryBrush, FocusVisualSecondaryBrush, GlyphBrush, HoverBorderBrush, PointerOverBorderBrush, PressedBorderBrush, RevealBorderBrush, SelectedBorderBrush, SelectedBrush, SelectedDisabledBorderBrush, SelectedHoverBorderBrush, SelectedInnerBorderBrush, SelectedPointerOverBorderBrush, SelectedPressedBorderBrush, SelectionIndicatorBrush, SelectionIndicatorDisabledBrush, SelectionIndicatorPointerOverBrush, SelectionIndicatorPressedBrush, StrokeBrush_

_TODO: See if we can describe a pattern to follow going forward._

### Showcasing the TodayBlackoutBackground and TodayBlackoutForeground properties

`TodayBlackoutForeground` takes precedence over the `BlackoutForeground` value, and `TodayBlackoutBackground` takes precedence over the `BlackoutBackground` value.

```xml
<CalendarView TodayBlackoutBackground='{StaticResource AccentFillColorTertiaryBrush}' TodayBlackoutForeground='{StaticResource TextOnAccentFillColorPrimaryBrush}' />
```

![Blacked Out Today Background And Foreground.](images/BlackoutTodayBackgroundAndForeground.png)

### Showcasing the BlackoutStrikethroughBrush property

This example sets the color of the strikethrough on the text of blacked out days.

The `BlackoutStrikethroughBrush` property only applies to non-Today days. For Today, the `TodayBlackoutForeground` brush is used for the strikethrough line.

![Blacked Out Sundays.](images/BlackoutStrikethroughBrush.png)

## Out Of Scope styling

Out-of-scope calendar items are the items that are visible but not part
of the selection. For example in month view if April is selected, days
from the end of March and/or the beginning of May may be seen.

The following properties of type
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
are used to customize the calendar items that are outside the current scope
(month, year, or decade):
`OutOfScopeHoverForeground`, `OutOfScopePressedForeground`.

### Showcasing the `OutOfScopeHoverForeground` property

This example shows the month of April and the beginning of May. Since
`IsOutOfScopeEnabled` is set, the May days are out-of-scope, use different brushes than in-scope days,
but are still selectable.

```xml
<CalendarView IsOutOfScopeEnabled='true' OutOfScopeHoverForeground='{StaticResource TextFillColorPrimaryBrush}'/>
```

In this screenshot the mouse is hovered over the out-of-scope 4th of May,
so the `OutOfScopeHoverForeground` color is displayed.

![Hover Out Of Scope Foreground.](images/HoverOutOfScopeForeground.png)

### Showcasing the OutOfScopePressedForeground property

This example shows the month of April and the beginning of May. Since
`IsOutOfScopeEnabled` is set, the May days are out-of-scope, use different brushes than in-scope days,
but are still selectable.

```xml
<CalendarView IsOutOfScopeEnabled='true' OutOfScopePressedForeground='{StaticResource TextFillColorTertiaryBrush}'/>
```

In this screenshot the 4th of May is being pressed,
so the `OutOfScopePressedForeground` color is displayed.

![Pressed Out Of Scope Foreground.](images/PressedOutOfScopeForeground.png)

## Item background styling

The `CalendarItemHoverBackground`, `CalendarItemPressedBackground` properties of type
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
are used to customize the background rendering of items in any of the `CalendarView's`
[DisplayModes](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CalendarDatePicker.DisplayMode).
The current date in the month view uses the `TodayHoverBackground` and `TodayPressedBackground` brushes though.

### Showcasing the CalendarItemHoverBackground property - February is hovered

This example sets the
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
to use as the background when a pointer moves over any non-Today calendar item.

```xml
<CalendarView CalendarItemHoverBackground='{StaticResource SubtleFillColorSecondaryBrush}'/>
```

![Hover Item Background.](images/HoverItemBackground.png)

### Showcasing the CalendarItemPressedBackground property - 2034 is pressed

This example sets the
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
to use as the background when a non-Today calendar item is pressed.

```xml
<CalendarView CalendarItemPressedBackground='{StaticResource SubtleFillColorTertiaryBrush}'/>
```

![Pressed Item Background.](images/PressedItemBackground.png)

## Disabled styling

The following properties of type
[Brush](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Media.Brush)
are used to customize the rendering of a disabled CalendarView
(when the `CalendarView`
[Control.IsEnabled](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.Control.IsEnabled)
is False):
`DisabledForeground`, `SelectedDisabledBorderBrush`, `CalendarItemDisabledBackground`,
`TodayDisabledBackground`.

### Showcasing a disabled month view

In this example the 12th and 20th of April are selected:

``` csharp
calendarView1.SelectedDates.Add(new DateTime(2021, 4, 12));
calendarView1.SelectedDates.Add(new DateTime(2021, 4, 20));

calendarView1.IsEnabled = false;
```

![A disabled CalendarView.](images/DisabledCalendarView.png)

Note that the current date's text still uses the `TodayForeground` brush.

## Day item positioning

The `CalendarView`'s `DayItemMargin`, `MonthYearMargin`, `FirstOfMonthLabelMargin`,
and `FirstOfYearDecadeLabelMargin` properties of type
[Thickness](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Thickness)
allow positioning the day, month, year, first-of-month and first-of-year labels within a calendar item.

### Showcasing the DayItemMargin and FirstOfMonthLabelMargin properties

Here the Month view has
[CalendarView.IsGroupLabelVisible](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CalendarView.IsGroupLabelVisible)
set to True and the group and main labels do not overlap because
`CalendarView.DayItemMargin.Top` is set to the default 6 pixels.

``` csharp
calendarView1.DayItemMargin = new Thickness(0, 6, 0, 0);

calendarView1.IsGroupLabelVisible = true;
```

April 1st is selected and May 1st is hovered.

![A month view with visible group labels.](images/MonthViewWithVisibleGroupLabels.png)

_Spec note:_
_Recommend: draw a margin/anatomy diagram._
_https://user-images.githubusercontent.com/12550607/117088217-a388e980-ad06-11eb-9b91-5d1bb7a06a52.png_

### Showcasing the MonthYearMargin and FirstOfYearDecadeLabelMargin properties

A Year view has
[CalendarView.IsGroupLabelVisible](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.CalendarView.IsGroupLabelVisible)
set to True with `CalendarView.MonthYearItemMargin.Top` and
`CalendarView.FirstOfYearDecadeLabelMargin.Top` set to 6 and 2 pixels respectively.

``` csharp
calendarView1.MonthYearItemMargin = new Thickness(0, 6, 0, 0);
calendarView1.FirstOfYearDecadeLabelMargin = new Thickness(0, 2, 0, 0);

calendarView1.IsGroupLabelVisible = true;
```

January 2021 is hovered.

![A year view with visible group labels.](images/YearViewWithVisibleGroupLabels.png)

## CalendarView theme resources

You can modify the look of a CalendarView by specifying Xaml resources in your app.
For more info, see the
[lightweight styling guide](https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/xaml-styles#lightweight-styling).

The new properties in this spec have default values according to new resources:

| Property | Resource key
| - | - |
| BlackoutBackground | CalendarViewBlackoutBackground |
| BlackoutStrikethroughBrush | CalendarViewBlackoutStrikethroughBrush |
| CalendarItemDisabledBackground | CalendarViewCalendarItemDisabledBackground |
| CalendarItemHoverBackground | CalendarViewCalendarItemHoverBackground |
| CalendarItemPressedBackground | CalendarViewCalendarItemPressedBackground |
| DayItemMargin | CalendarViewDayItemMargin |
| DisabledForeground | CalendarViewDisabledForeground |
| FirstOfMonthLabelMargin | CalendarViewFirstOfMonthLabelMargin |
| FirstOfYearDecadeLabelMargin | CalendarViewFirstOfYearDecadeLabelMargin |
| MonthYearItemMargin | CalendarViewMonthYearItemMargin |
| OutOfScopeHoverForeground | CalendarViewOutOfScopeHoverForeground |
| OutOfScopePressedForeground | CalendarViewOutOfScopePressedForeground |
| SelectedDisabledBorderBrush | CalendarViewSelectedDisabledBorderBrush |
| SelectedDisabledForeground | CalendarViewSelectedDisabledForeground |
| SelectedHoverForeground | CalendarViewSelectedHoverForeground |
| SelectedPressedForeground | CalendarViewSelectedPressedForeground |
| TodayBackground | CalendarViewTodayBackground |
| TodayBlackoutBackground | CalendarViewTodayBlackoutBackground |
| TodayBlackoutForeground | CalendarViewTodayBlackoutForeground |
| TodayDisabledBackground | CalendarViewTodayDisabledBackground |
| TodayHoverBackground | CalendarViewTodayHoverBackground |
| TodayPressedBackground | CalendarViewTodayPressedBackground |
| TodaySelectedInnerBorderBrush | CalendarViewTodaySelectedInnerBorderBrush |


# API Pages

_Spec note: the following remarks apply to each of the new properties_

This property is used by the `CalendarView` control only when a boolean resource named `CalendarViewBaseItemRoundedChromeEnabled` is set to True in the
[Application.Resources](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Application.Resources).

```xml
    <x:Boolean x:Key="CalendarViewBaseItemRoundedChromeEnabled">True</x:Boolean>
```

This property is used by the
[WinUI2 controls library](https://docs.microsoft.com/en-us/windows/apps/winui/winui2/),
which sets this boolean resource to enable it.
So using WinUI2 in your app causes this property to be enabled.

## CalendarView.DayItemMargin

`public Windows.UI.Xaml.Thickness DayItemMargin { get; set; }`

Gets or sets the margin applied to the main label inside a calendar day item.

This property is only used by the CalendarView control when a boolean theme resource named `CalendarViewBaseItemRoundedChromeEnabled` is set to True.

```xml
    <x:Boolean x:Key="CalendarViewBaseItemRoundedChromeEnabled">True</x:Boolean>
```
## CalendarView.MonthYearItemMargin

`public Windows.UI.Xaml.Thickness MonthYearItemMargin { get; set; }`

Gets or sets the margin applied to the main label inside a calendar month or year item.


## CalendarView.FirstOfMonthLabelMargin

`public Windows.UI.Xaml.Thickness FirstOfMonthLabelMargin { get; set; }`

Gets or sets the margin used to display the first-of-month banner in the calendar.

## CalendarView.FirstOfYearDecadeLabelMargin

`public Windows.UI.Xaml.Thickness FirstOfYearDecadeLabelMargin { get; set; }`

Gets or sets the margin used to display the first of year/decade banner in the calendar.

## CalendarView.CalendarItemCornerRadius

`public Windows.UI.Xaml.CornerRadius CalendarItemCornerRadius { get; set; }`

Gets or sets the corner radius for a calendar item's visuals.

The visuals affected are the background of the current date, the border around selected items, the density bars as well as the focus cue.

When this property is left unset, the CalendarView automatically uses a corner radius that is half the item size so that the various visuals appear circular.

In this example, because the items size is 40x40px, the automatic corner radius is 20px:

![Unset CalendarItemCornerRadius property resulting in circular visuals.](images/DefaultCalendarItemCornerRadius.png)

When set, the CalendarView instead adopts the property value for the various visuals.

In this example, the CalendarItemCornerRadius property is set to 4px:

![CalendarItemCornerRadius property set to 4 resulting in rounded square visuals.](images/CalendarItemCornerRadiusSetToFour.png)

## CalendarView.DisabledForeground

`public Windows.UI.Xaml.Media.Brush DisabledForeground { get; set; }`

Gets or sets a brush that provides the foreground of a calendar item while it's disabled.

## CalendarView.BlackoutStrikethroughBrush

`public Windows.UI.Xaml.Media.Brush BlackoutStrikethroughBrush { get; set; }`

Gets or sets a brush for the strikethrough line over calendar items while they are blacked out.
The strikethrough line for the current date uses the `CalendarView.TodayBlackoutForeground` brush though.

## CalendarView.SelectedDisabledBorderBrush

`public Windows.UI.Xaml.Media.Brush SelectedDisabledBorderBrush { get; set; }`

Gets or sets a brush that provides the border of a selected calendar item while it's disabled.

## CalendarView.SelectedDisabledForeground

`public Windows.UI.Xaml.Media.Brush SelectedDisabledForeground { get; set; }`

Gets or sets a brush that provides the foreground of a selected calendar item while it's disabled.

## CalendarView.SelectedHoverForeground

`public Windows.UI.Xaml.Media.Brush SelectedHoverForeground { get; set; }`

Gets or sets a brush that provides the foreground of a selected calendar item while the pointer is over it.

## CalendarView.SelectedPressedForeground

`public Windows.UI.Xaml.Media.Brush SelectedPressedForeground { get; set; }`

Gets or sets a brush that provides the foreground of a selected calendar item while it's pressed.

## CalendarView.CalendarItemHoverBackground

`public Windows.UI.Xaml.Media.Brush CalendarItemHoverBackground { get; set; }`

Gets or sets a brush that provides the background of a calendar item while the pointer is over it.

## CalendarView.CalendarItemPressedBackground

`public Windows.UI.Xaml.Media.Brush CalendarItemPressedBackground { get; set; }`

Gets or sets a brush that provides the background of a calendar item while it's pressed.

## CalendarView.CalendarItemDisabledBackground

`public Windows.UI.Xaml.Media.Brush CalendarItemDisabledBackground { get; set; }`

Gets or sets a brush that provides the background of a calendar item while it's disabled.


## CalendarView.OutOfScopeHoverForeground

`public Windows.UI.Xaml.Media.Brush OutOfScopeHoverForeground { get; set; }`

Gets or sets a brush that provides the foreground of calendar items that are outside the current scope (month, year, or decade) while the pointer is over them.

_Spec note:_
_Specify precedence order:_
_Today+Blackout
Today
Blackout
OutOfScope
Normal item_

## CalendarView.OutOfScopePressedForeground

`public Windows.UI.Xaml.Media.Brush OutOfScopePressedForeground { get; set; }`

Gets or sets a brush that provides the foreground of calendar items that are outside the current scope (month, year, or decade) while they are pressed.

## CalendarView.TodayBackground

`public Windows.UI.Xaml.Media.Brush TodayBackground { get; set; }`

Gets or sets a brush that provides the background of the calendar item for the current date.

## CalendarView.BlackoutBackground

`public Windows.UI.Xaml.Media.Brush BlackoutBackground { get; set; }`

Gets or sets a brush that provides the background of calendar items while they are blacked out.

## CalendarView.TodayBlackoutBackground

`public Windows.UI.Xaml.Media.Brush TodayBlackoutBackground { get; set; }`

Gets or sets a brush that provides the background of the calendar item for the current date while it's blacked out.

## CalendarView.TodayBlackoutForeground

`public Windows.UI.Xaml.Media.Brush TodayBlackoutForeground { get; set; }`

Gets or sets a brush that provides the foreground of the calendar item for the current date while it's blacked out.
It is also used for its strikethrough line.

## CalendarView.TodayHoverBackground

`public Windows.UI.Xaml.Media.Brush TodayHoverBackground { get; set; }`

Gets or sets a brush that provides the background of the calendar item for the current date while the pointer is over it.

## CalendarView.TodayPressedBackground

`public Windows.UI.Xaml.Media.Brush TodayPressedBackground { get; set; }`

Gets or sets a brush that provides the background of the calendar item for the current date while it's pressed.

## CalendarView.TodayDisabledBackground

`public Windows.UI.Xaml.Media.Brush TodayDisabledBackground { get; set; }`

Gets or sets a brush that provides the background of the calendar item for the current date while it's disabled.

## CalendarView.TodaySelectedInnerBorderBrush

`public Windows.UI.Xaml.Media.Brush TodaySelectedInnerBorderBrush { get; set; }`

Gets or sets a brush that provides the border of the calendar item for the current date while it's selected.


# API Details

    [contract(Windows.Foundation.UniversalApiContract, 1)]
    [webhosthidden]
    [static_name("Windows.UI.Xaml.Controls.ICalendarViewStatics", 7260f1c4-2f5d-41bd-99bb-4571b20b79a8)]
    [constructor_name("Windows.UI.Xaml.Controls.ICalendarViewFactory", 3d8f82e3-6cc6-423e-8d7c-7014d954ddef)]
    [interface_name("Windows.UI.Xaml.Controls.ICalendarView", cd639203-dfb5-4312-ac07-c0391824607b)]
    unsealed runtimeclass CalendarView
        : Windows.UI.Xaml.Controls.Control
    {
        // Existing CalendarView APIs not shown here.

        [contract(Windows.Foundation.UniversalApiContract, 14)]
        {
            Windows.UI.Xaml.Thickness DayItemMargin;
            Windows.UI.Xaml.Thickness MonthYearItemMargin;
            Windows.UI.Xaml.Thickness FirstOfMonthLabelMargin;
            Windows.UI.Xaml.Thickness FirstOfYearDecadeLabelMargin;

            Windows.UI.Xaml.CornerRadius CalendarItemCornerRadius;

            Windows.UI.Xaml.Media.Brush DisabledForeground;
            Windows.UI.Xaml.Media.Brush BlackoutStrikethroughBrush;
            Windows.UI.Xaml.Media.Brush SelectedDisabledBorderBrush;
            Windows.UI.Xaml.Media.Brush SelectedDisabledForeground;
            Windows.UI.Xaml.Media.Brush SelectedHoverForeground;
            Windows.UI.Xaml.Media.Brush SelectedPressedForeground;
            Windows.UI.Xaml.Media.Brush CalendarItemHoverBackground;
            Windows.UI.Xaml.Media.Brush CalendarItemPressedBackground;
            Windows.UI.Xaml.Media.Brush CalendarItemDisabledBackground;
            Windows.UI.Xaml.Media.Brush OutOfScopeHoverForeground;
            Windows.UI.Xaml.Media.Brush OutOfScopePressedForeground;
            Windows.UI.Xaml.Media.Brush BlackoutBackground;
            Windows.UI.Xaml.Media.Brush TodayBackground;
            Windows.UI.Xaml.Media.Brush TodayBlackoutBackground;
            Windows.UI.Xaml.Media.Brush TodayBlackoutForeground;
            Windows.UI.Xaml.Media.Brush TodayHoverBackground;
            Windows.UI.Xaml.Media.Brush TodayPressedBackground;
            Windows.UI.Xaml.Media.Brush TodayDisabledBackground;
            Windows.UI.Xaml.Media.Brush TodaySelectedInnerBorderBrush;

            static Windows.UI.Xaml.DependencyProperty DayItemMarginProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty MonthYearItemMarginProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty FirstOfMonthLabelMargin{ get; };
            static Windows.UI.Xaml.DependencyProperty FirstOfYearDecadeLabelMargin{ get; };

            static Windows.UI.Xaml.DependencyProperty CalendarItemCornerRadiusProperty{ get; };

            static Windows.UI.Xaml.DependencyProperty DisabledForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty BlackoutStrikethroughBrushProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty SelectedDisabledBorderBrushProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty SelectedDisabledForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty SelectedHoverForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty SelectedPressedForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty CalendarItemHoverBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty CalendarItemPressedBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty CalendarItemDisabledBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty OutOfScopeHoverForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty OutOfScopePressedForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty BlackoutBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayBlackoutBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayBlackoutForegroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayHoverBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayPressedBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodayDisabledBackgroundProperty{ get; };
            static Windows.UI.Xaml.DependencyProperty TodaySelectedInnerBorderBrushProperty{ get; };
        }
    };

# Appendix

## New CalendarViewBaseItemRoundedChromeEnabled resource

The new `CalendarViewBaseItemRoundedChromeEnabled` boolean resource is similar to other ones
introduced recently:

```xml
    <x:Boolean x:Key="CalendarViewBaseItemRoundedChromeEnabled">False</x:Boolean>

    <x:Boolean x:Key="HyperlinkUnderlineVisible">True</x:Boolean>
    <x:Boolean x:Key="ListViewBaseItemRoundedChromeEnabled">False</x:Boolean>
    <x:Boolean x:Key="ThemeShadowIsUsingDropShadows">False</x:Boolean>
```

## Fitting the new property names among the old ones

The new properties were named to fit well with the CalendarView existing properties:

New property name | Similar old property names
------ | ------
BlackoutBackground | BlackoutForeground, OutOfScopeBackground
BlackoutStrikethroughBrush | HoverBorderBrush, FocusBorderBrush
CalendarItemCornerRadius | CalendarItemBorderThickness, CalendarItemBorderBrush, CalendarItemForeground
CalendarItemDisabledBackground | CalendarItemBackground, CalendarItemForeground
CalendarItemHoverBackground | CalendarItemBackground, CalendarItemForeground
CalendarItemPressedBackground | CalendarItemBackground, CalendarItemForeground
DayItemMargin | DayItemFontFamily, DayItemFontSize, DayItemFontStyle
DisabledForeground | PressedForeground, SelectedForeground, BlackoutForeground
FirstOfMonthLabelMargin | FirstOfMonthLabelFontFamily, FirstOfMonthLabelFontSize, FirstOfMonthLabelFontStyle
FirstOfYearDecadeLabelMargin | FirstOfYearDecadeLabelFontFamily, FirstOfYearDecadeLabelFontSize, FirstOfYearDecadeLabelFontStyle
MonthYearItemMargin | MonthYearItemFontFamily, MonthYearItemFontSize, MonthYearItemFontStyle
OutOfScopeHoverForeground | OutOfScopeForeground, OutOfScopeBackground
OutOfScopePressedForeground | OutOfScopeForeground, OutOfScopeBackground
SelectedDisabledBorderBrush | SelectedHoverBorderBrush, SelectedPressedBorderBrush
SelectedDisabledForeground | SelectedForeground
SelectedHoverForeground | SelectedForeground, SelectedHoverBorderBrush
SelectedPressedForeground | SelectedForeground, SelectedPressedBorderBrush
TodayBackground | TodayForeground, OutOfScopeBackground
TodayBlackoutBackground | TodayForeground, OutOfScopeBackground
TodayBlackoutForeground | TodayForeground, OutOfScopeForeground
TodayDisabledBackground | OutOfScopeBackground, TodayForeground
TodayHoverBackground | TodayHoverBorderBrush, TodayForeground
TodayPressedBackground | OutOfScopeBackground, TodayForeground
TodaySelectedInnerBorderBrush | TodayHoverBorderBrush, TodayPressedBorderBrush

## Example ResourceDictionary for CalendarView

```xml
<ResourceDictionary
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml">
    <ResourceDictionary.ThemeDictionaries>
        <ResourceDictionary x:Key="Default">
            <StaticResource x:Key="CalendarViewFocusVisualPrimaryBrush" ResourceKey="FocusStrokeColorOuterBrush" />
            <StaticResource x:Key="CalendarViewFocusVisualSecondaryBrush" ResourceKey="FocusStrokeColorInnerBrush" />
            <StaticResource x:Key="CalendarViewFocusBorderBrush" ResourceKey="AccentFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewBlackoutStrikethroughBrush" ResourceKey="ControlStrongStrokeColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewSelectedHoverBorderBrush" ResourceKey="AccentFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedPressedBorderBrush" ResourceKey="SubtleFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedDisabledBorderBrush" ResourceKey="AccentFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewSelectedBorderBrush" ResourceKey="AccentFillColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewHoverBorderBrush" ResourceKey="SubtleFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewPressedBorderBrush" ResourceKey="SubtleFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewTodaySelectedInnerBorderBrush" ResourceKey="TextOnAccentFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewTodayForeground" ResourceKey="TextOnAccentFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewDisabledForeground" ResourceKey="TextFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewBlackoutForeground" ResourceKey="TextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedForeground" ResourceKey="AccentTextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedHoverForeground" ResourceKey="AccentTextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedPressedForeground" ResourceKey="AccentTextFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewSelectedDisabledForeground" ResourceKey="AccentTextFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewPressedForeground" ResourceKey="TextFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewOutOfScopeForeground" ResourceKey="TextFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewOutOfScopeHoverForeground" ResourceKey="TextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewOutOfScopePressedForeground" ResourceKey="TextFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemBackground" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemHoverBackground" ResourceKey="SubtleFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemPressedBackground" ResourceKey="SubtleFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemDisabledBackground" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemBorderBrush" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewCalendarItemForeground" ResourceKey="TextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewTodayBackground" ResourceKey="AccentFillColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewTodayBlackoutBackground" ResourceKey="AccentFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewTodayBlackoutForeground" ResourceKey="TextOnAccentFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewTodayHoverBackground" ResourceKey="AccentFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewTodayPressedBackground" ResourceKey="AccentFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewTodayDisabledBackground" ResourceKey="AccentFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewBlackoutBackground" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewOutOfScopeBackground" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewForeground" ResourceKey="TextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewBackground" ResourceKey="ControlFillColorInputActiveBrush" />
            <StaticResource x:Key="CalendarViewBorderBrush" ResourceKey="ControlStrokeColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewWeekDayForegroundDisabled" ResourceKey="TextFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonBackground" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonBackgroundPointerOver" ResourceKey="SubtleFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonBackgroundPressed" ResourceKey="SubtleFillColorTertiaryBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonForeground" ResourceKey="ControlStrongFillColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonForegroundPointerOver" ResourceKey="ControlStrongFillColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonForegroundPressed" ResourceKey="ControlStrongFillColorDefaultBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonForegroundDisabled" ResourceKey="ControlStrongFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewHeaderNavigationButtonForegroundPointerOver" ResourceKey="TextFillColorPrimaryBrush" />
            <StaticResource x:Key="CalendarViewHeaderNavigationButtonForegroundPressed" ResourceKey="TextFillColorSecondaryBrush" />
            <StaticResource x:Key="CalendarViewHeaderNavigationButtonForegroundDisabled" ResourceKey="TextFillColorDisabledBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonBorderBrushPointerOver" ResourceKey="SubtleFillColorTransparentBrush" />
            <StaticResource x:Key="CalendarViewNavigationButtonBorderBrush" ResourceKey="SubtleFillColorTransparentBrush" />
        </ResourceDictionary>
        <ResourceDictionary x:Key="HighContrast">
            ...
        </ResourceDictionary>
        <ResourceDictionary x:Key="Light">
            ...
        </ResourceDictionary>
    </ResourceDictionary.ThemeDictionaries>

    <x:Boolean x:Key="CalendarViewBaseItemRoundedChromeEnabled">True</x:Boolean>
    <Thickness x:Key="CalendarViewDayItemMargin">0,6,0,0</Thickness>
    <Thickness x:Key="CalendarViewMonthYearItemMargin">0,6,0,0</Thickness>
    <Thickness x:Key="CalendarViewFirstOfMonthLabelMargin">0,1,0,0</Thickness>
    <Thickness x:Key="CalendarViewFirstOfYearDecadeLabelMargin">0,2,0,0</Thickness>

    <Style x:Key="CalendarViewDefaultStyle" TargetType="CalendarView">
        <Setter Property="BlackoutStrikethroughBrush" Value="{ThemeResource CalendarViewBlackoutStrikethroughBrush}" /> *
        <Setter Property="SelectedHoverBorderBrush" Value="{ThemeResource CalendarViewSelectedHoverBorderBrush}" />
        <Setter Property="SelectedPressedBorderBrush" Value="{ThemeResource CalendarViewSelectedPressedBorderBrush}" />
        <Setter Property="SelectedDisabledBorderBrush" Value="{ThemeResource CalendarViewSelectedDisabledBorderBrush}" /> *
        <Setter Property="SelectedBorderBrush" Value="{ThemeResource CalendarViewSelectedBorderBrush}" />
        <Setter Property="HoverBorderBrush" Value="{ThemeResource CalendarViewHoverBorderBrush}" />
        <Setter Property="PressedBorderBrush" Value="{ThemeResource CalendarViewPressedBorderBrush}" />
        <Setter Property="CalendarItemBorderBrush" Value="{ThemeResource  CalendarViewCalendarItemBorderBrush}" />
        <Setter Property="TodaySelectedInnerBorderBrush" Value="{ThemeResource  CalendarViewTodaySelectedInnerBorderBrush}" /> *
        <Setter Property="TodayForeground" Value="{ThemeResource CalendarViewTodayForeground}" />
        <Setter Property="DisabledForeground" Value="{ThemeResource CalendarViewDisabledForeground}" /> *
        <Setter Property="BlackoutForeground" Value="{ThemeResource CalendarViewBlackoutForeground}" />
        <Setter Property="SelectedForeground" Value="{ThemeResource CalendarViewSelectedForeground}" />
        <Setter Property="SelectedHoverForeground" Value="{ThemeResource CalendarViewSelectedHoverForeground}" /> *
        <Setter Property="SelectedPressedForeground" Value="{ThemeResource CalendarViewSelectedPressedForeground}" /> *
        <Setter Property="SelectedDisabledForeground" Value="{ThemeResource CalendarViewSelectedDisabledForeground}" /> *
        <Setter Property="PressedForeground" Value="{ThemeResource CalendarViewPressedForeground}" />
        <Setter Property="OutOfScopeForeground" Value="{ThemeResource CalendarViewOutOfScopeForeground}" />
        <Setter Property="OutOfScopeHoverForeground" Value="{ThemeResource CalendarViewOutOfScopeHoverForeground}" /> *
        <Setter Property="OutOfScopePressedForeground" Value="{ThemeResource CalendarViewOutOfScopePressedForeground}" /> *
        <Setter Property="CalendarItemForeground" Value="{ThemeResource CalendarViewCalendarItemForeground}" />
        <Setter Property="TodayBackground" Value="{ThemeResource CalendarViewTodayBackground}" /> *
        <Setter Property="TodayBlackoutBackground" Value="{ThemeResource CalendarViewTodayBlackoutBackground}" /> *
        <Setter Property="TodayBlackoutForeground" Value="{ThemeResource CalendarViewTodayBlackoutForeground}" /> *
        <Setter Property="TodayHoverBackground" Value="{ThemeResource CalendarViewTodayHoverBackground}" /> *
        <Setter Property="TodayPressedBackground" Value="{ThemeResource CalendarViewTodayPressedBackground}" /> *
        <Setter Property="TodayDisabledBackground" Value="{ThemeResource CalendarViewTodayDisabledBackground}" /> *
        <Setter Property="BlackoutBackground" Value="{ThemeResource CalendarViewBlackoutBackground}" /> *
        <Setter Property="OutOfScopeBackground" Value="{ThemeResource CalendarViewOutOfScopeBackground}" />
        <Setter Property="CalendarItemBackground" Value="{ThemeResource CalendarViewCalendarItemBackground}" />
        <Setter Property="CalendarItemHoverBackground" Value="{ThemeResource CalendarViewCalendarItemHoverBackground}" /> *
        <Setter Property="CalendarItemPressedBackground" Value="{ThemeResource CalendarViewCalendarItemPressedBackground}" /> *
        <Setter Property="CalendarItemDisabledBackground" Value="{ThemeResource CalendarViewCalendarItemDisabledBackground}" /> *
        <Setter Property="Foreground" Value="{ThemeResource CalendarViewForeground}" />
        <Setter Property="Background" Value="{ThemeResource CalendarViewBackground}" />
        <Setter Property="BorderBrush" Value="{ThemeResource CalendarViewBorderBrush}" />
        <Setter Property="DayItemFontFamily" Value="XamlAutoFontFamily" />
        <Setter Property="DayItemFontSize" Value="{ThemeResource CalendarViewDayItemFontSize}" />
        <Setter Property="DayItemMargin" Value="{ThemeResource CalendarViewDayItemMargin}" /> *
        <Setter Property="FirstOfMonthLabelFontFamily" Value="XamlAutoFontFamily" />
        <Setter Property="FirstOfMonthLabelFontSize" Value="{ThemeResource CalendarViewFirstOfMonthLabelFontSize}" />
        <Setter Property="FirstOfMonthLabelMargin" Value="{ThemeResource CalendarViewFirstOfMonthLabelMargin}" /> *
        <Setter Property="MonthYearItemFontFamily" Value="XamlAutoFontFamily" />
        <Setter Property="MonthYearItemFontSize" Value="{ThemeResource CalendarViewMonthYearItemFontSize}" />
        <Setter Property="MonthYearItemMargin" Value="{ThemeResource CalendarViewMonthYearItemMargin}" /> *
        <Setter Property="FirstOfYearDecadeLabelFontFamily" Value="XamlAutoFontFamily" />
        <Setter Property="FirstOfYearDecadeLabelFontSize" Value="{ThemeResource CalendarViewFirstOfYearDecadeLabelFontSize}" />
        <Setter Property="FirstOfYearDecadeLabelMargin" Value="{ThemeResource CalendarViewFirstOfYearDecadeLabelMargin}" /> *
        <Setter Property="CalendarItemBorderThickness" Value="1" />
        <Setter Property="BorderThickness" Value="1" />
        <Setter Property="HorizontalAlignment" Value="Left" />
        <Setter Property="VerticalAlignment" Value="Center" />
        <Setter Property="HorizontalContentAlignment" Value="Stretch" />
        <Setter Property="VerticalContentAlignment" Value="Stretch" />
        <Setter Property="IsTabStop" Value="False" />
        <Setter Property="UseSystemFocusVisuals" Value="{StaticResource UseSystemFocusVisuals}" />
        <Setter Property="CornerRadius" Value="{ThemeResource ControlCornerRadius}" />
        <Setter Property="Template">
          ...
        </Setter>
    </Style>
</ResourceDictionary>
```


================================================
FILE: specs/ColorPicker/ColorPicker.Orientation.md
================================================
ColorPicker.Orientation
===

# Background

The Xaml [ColorPicker](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.ColorPicker)
control is a flyout that lets a user pick a color using a color spectrum, sliders, and text input.

This spec has an update to the existing `ColorPicker` control.
The aim of this new API is, to make the ColorPicker more versatile to use and
provide different layouting ways to maximize the space available
by adding an `Orientation` property.


# Conceptual pages (How To)

#### Specify the layout direction

Use the `Orientation` property to control whether the `ColorPicker` should take up
more vertical space or more horizontal space.

```xaml
<muxc:ColorPicker IsAlphaEnabled="True" Orientation="Vertical"/>
```
![Vertical ColorPicker](./images/ColorPicker_VerticalMode.png)

```xaml
<muxc:ColorPicker IsAlphaEnabled="True" Orientation="Horizontal"/>
```
![Horizontal ColorPicker](./images/ColorPicker_HorizontalMode.png)


# API Pages

## ColorPicker.Orientation property

Gets or sets the orientation in which the parts of the ColorPicker will be laid out.
Defaults to `Vertical`.

Using the orientation, you can specify whether the editing controls should be laid out underneath
the color area (vertical orientation) or to the side of it (horizontal orientation).

| Orientation | Meaning |
|-------------|---------|
| Horizontal  | The editing controls will be put to the side of the color spectrum.|
| Vertical    | The editing controls will be put underneath the color spectrum.|

### Note
When the `Orientation` property is set to `Horizontal`, the ColorPicker will NOT respect the IsMoreButton enabled property.
Instead, the text input fields will always be displayed to the side of the ColorPicker.
In addition to that, when in `Horizontal` mode, when the text input fields are being used, there will be a margin of `122px` to the right of the input fields.
This margin accounts for the different localizations of the different localizations of the labels of said fields and ensures that those labels will not be cut off.
This margin is determined by the `ColorPickerTextInputHorizontalOrientationMargin` lightweight styling resource.
If your app is only available in English, you can override this resource and set the margin to `74px` to improve the horizontal footprint of the control.
The resource does have not have any effect when the `Orientation` is set to `Vertical`.

# API Details

```c# (but really MIDL3)

namespace Microsoft.UI.Xaml.Controls
{
  [webhosthidden]
  unsealed runtimeclass ColorPicker
  {
      // Existing ...

      // Gets or sets the Orientation of the ColorPicker
      Windows.UI.Xaml.Controls.Orientation Orientation;
  }
}
```



================================================
FILE: specs/images/datepicker-evolution.PNG
================================================
[Non-text file]


================================================
FILE: specs/images/DPTP-other-states.PNG
================================================
[Non-text file]


================================================
FILE: specs/images/timepicker-evolution.PNG
================================================
[Non-text file]


================================================
FILE: specs/InfoBadge/InfoBadge-spec.md
================================================


Spec: InfoBadge control
===

# Background

A badge is a small piece of UI that usually displays a dot, number, or icon and serves to bring the user’s attention to where it’s placed, alerting them of something. In the example below, a badge with the number 9 is displayed on a Navigation item.

![Example of an InfoBadge in NavigationView](images/infobadge-example1.png)

There is currently no built-in way to show badges  in your WinUI app, and developers must create their own implementations. This blocks app developers from easily displaying notifications or indicating that new content is available, henceforth making a more difficult barrier to entry for a wide variety of app types that the WinUI platform should support (mail, messaging, social media).

### NavigationView Context
NavigationView is the most common scenario in which InfoBadge will be used, and is the recommended way of displaying notifications/alerts that can be seen and accessed app-wide. In addition to this, NavigationView has a bit of a complicated architecture where it has multiple display modes, which poses a difficulty for developers looking to integrate InfoBadge into their NavigationView. For that reason, NavigationView items will have specific APIs to support badging. For InfoBadge placement in all other controls and scenarios, developers will use the placement and positioning (Margin, Alignment, etc) APIs that are built into InfoBadge itself.


# Conceptual pages (How To)

Badging is the least intrusive and most intuitive way to display notifications or bring focus to something within an app. An InfoBadge is a small piece of UI that can be added into an app and customized to display a number, icon, or a simple dot. **InfoBadge is built into NavigationView but can also be added as a standalone element in the XAML tree, allowing you to place InfoBadge into any control or piece of UI of your choosing.** When using an InfoBadge somewhere other than NavigationView, you will be responsible for programmatically determining when to show/dismiss the InfoBadge and where to place the InfoBadge. An InfoBadge should be used to bring the user’s focus to an area – whether that be for notifications, indicating new content, or showing an alert.

There are three InfoBadge types that you can choose from - dot, icon, and numeric, as shown in order below.

![Dot, icon, and numeric InfoBadges](images/infobadge-example2.png)

### Dot InfoBadge
The dot InfoBadge is a simple ellipsis with a default size of 4px by 4px. It has no border, and is never meant to hold text or anything else inside of it.

The dot InfoBadge should be used for general scenarios in which you want to guide the user’s focus towards the InfoBadge – i.e. indicating new content or updates are available.

### Icon InfoBadge
The icon InfoBadge is a 16px by 16px ellipsis that holds an icon inside of it. InfoBadge has an `IconSource` property which provides flexibility for the types of supported icons.

The icon InfoBadge should be used to send a quick message along with getting the user’s attention – i.e. alerting the user that something non-blocking in the application has gone wrong, an extra important update is available, or that something specific in the app is currently enabled (like a countdown timer going).

Note that if you'd like to use BitmapIcon for the `IconSource` of your InfoBadge, you are responsible for ensuring that the BitmapIcon fits inside of the InfoBadge (either by changing the size of the icon, or changing the size of the InfoBadge).

### Numeric InfoBadge
The numeric InfoBadge is also a 16px by 16px ellipsis that holds a number inside of it. The width of this ellipsis will automatically expand as the number grows to multiple digits, with a smooth animation.

The numeric InfoBadge should be used for showing that there are a specific number of items that need attention – i.e. new emails/messages.

## Preset InfoBadge styles
To help support the most common scenarios in which InfoBadges are used, WinUI provides built-in, preset InfoBadge styles. While you can customize your InfoBadge to use any color/icon/number combination that you desire, these built-in presets are a quick option to make sure that your InfoBadge is compliant with accessibility guidelines and is proportional in terms of icon sizing (if you’re using an icon InfoBadge).

### List of style presets
The following InfoBadge style presets each use one of the following colors for the background fill of the InfoBadge:

![Colors available through InfoBadge style presets](images/color-breakdown.PNG)

| Style Name                      | Color                   | Icon |
|---------------------------------|-------------------------|------|
| AttentionIconInfoBadgeStyle     | Attention/Informational | ![Asterisk InfoBadge icon](images/asterisk-badge-icon.png)|
| InformationalIconInfoBadgeStyle | Attention/Informational |![Informational InfoBadge icon](images/informational-badge-icon.png)      |
| SuccessIconInfoBadgeStyle       | Success                 |![Success InfoBadge icon](images/checkmark-badge-icon.png)      |
| CautionIconInfoBadgeStyle       | Caution                 |![Caution InfoBadge icon](images/caution-badge-icon.png)      |
| CriticalIconInfoBadgeStyle      | Critical                | ![Error InfoBadge icon](images/error-badge-icon.png)     |
| AttentionDotInfoBadgeStyle      | Attention/Informational | None |
| InformationalDotInfoBadgeStyle  | Attention/Informational | None |
| SuccessDotInfoBadgeStyle        | Success                 | None |
| CautionDotInfoBadgeStyle        | Caution                 | None |
| CriticalDotInfoBadgeStyle       | Critical                | None |

<br/>
To use a preset InfoBadge style, you'd use the following markup:

```xml
<InfoBadge x:Name="InfoBadge1" Style="{ThemeResource AttentionIconInfoBadgeStyle}"/>
```

## How and when to use an InfoBadge
### When to use an InfoBadge
An InfoBadge should be used when you want to bring the user’s focus to a certain area of your app in an unintrusive way. When an InfoBadge appears, it is meant to bring focus to an area and then let the user get back into their flow, giving them the choice of whether or not to look into the details of why the InfoBadge appeared. InfoBadges should only represent messages that are dismissible and non-permanent – an InfoBadge should have specific rules as to when it can appear, disappear, and/or change.

Examples of appropriate InfoBadge usage:
-	Indicating new messages have arrived
-	Indicating new articles are available to read
-	Indicating that there are new options available on a page
-	Indicating that there might be an issue with an item on a certain page that does not block the app from functioning

### When NOT to use an InfoBadge:

An InfoBadge should not be used to display critical errors or convey highly important messages that need immediate action. InfoBadges should not be used in cases where they need to be interacted with immediately to continue usage of the app.

Examples of inappropriate InfoBadge usage:
-	Indicating an urgent matter on a page within the app that needs to be addressed before continuing to use the app
-	Appearing in an app with no way for the user to dismiss the InfoBadge
-	Using the InfoBadge as a permanent way of bringing the user’s focus to an area, without a way for the user to dismiss the InfoBadge.
-	Using an InfoBadge as a regular Icon or image in your app

## Using an InfoBadge in NavigationView
Using InfoBadge in a NavigationView is the recommended approach for showing app-wide notifications and alerts. To enable or customize the InfoBadge on a NavigationViewItem, assign the `NavigationViewItem.InfoBadge` property to an InfoBadge object in your app.

In Left-Expanded mode, InfoBadge will appear right-aligned to the edge of the NavigationViewItem.

![Left-expanded NavigationView with an InfoBadge](images/navview-example1.png)

In Left-Compact mode, InfoBadge will appear overlayed on the top right corner of the icon.

![Left-compact NavigationView with an InfoBadge](images/navview-example2.png)

In Top mode, InfoBadge will be displayed aligned to the upper right hand corner of the overall item.

![Top mode NavigationView with an InfoBadge](images/navview-example3.png)

It is not recommended to use different types of InfoBadges in one NavigationView, i.e. attach a numeric InfoBadge to one NavigationViewItem and a dot InfoBadge to another NavigationViewItem in the same NavigationView.

### Hierarchy and overflow
If you have a hierarchical NavigationView , InfoBadge will appear right-aligned on child items when they are expanded, regardless of PaneDisplayMode. Parent items in a hierarchical NavigationView will follow the same design/placement patterns as described above.

The parent NavigationViewItem and child NavigationView items will each have their own InfoBadge property, so you can bind the value of the parent’s InfoBadge to factors that determine that children’s InfoBadge values (such as showing the sum of the children's numeric InfoBadges on the parent's InfoBadge). The below image shows a hierarchical NavigationView with its PaneDisplayMode set to Top, where one top-level (parent) item has a numeric InfoBadge on it.

![Hierarchical NavigationView with an InfoBadge](images/navview-example5.png)

For overflow scenarios in a top-mode NavigationView (i.e. when the window size changes and NavigationView items are placed inside of the overflow menu), the overflow button has its own InfoBadge (`NavigationView.OverflowButtonInfoBadge`) that can be assigned and changed based on the InfoBadges that may be present on overflow items:

![Overflowing NavigationView with an InfoBadge](images/navview-example6.png)

To access the list of items present in the overflow menu, use the `NavigationView.OverflowItems` collection. You can hook up to the Changed event for this collection to accurately check when items are being moved into the overflow menu. Once you know which items are in the overflow menu, you can update the `NavigationView.OverflowButtonInfoBadge` to represent InfoBadge information/status on the overflow button itself while the overflow navigation items are hidden.

## Using an InfoBadge in another control
Use InfoBadge as you would any other control – simply add the InfoBadge markup where you’d like it to appear. Since InfoBadge inherits from `Control`, it has all the built-in positioning properties such as margin, alignment, padding, and more which you can take advantage of to position your InfoBadge exactly where you want it. Once the InfoBadge is positioned, use the `IsOpen` property to make the InfoBadge appear and disappear based on user actions, program logic, counters, etc. Note that the `IsOpen` property is set to `true` by default.

If you’re placing an InfoBadge inside of another control, such as a Button or a ListViewItem, note that it is not recommended for the InfoBadge to be visible past the footprint of the parent control. So if your InfoBadge is inside of a button, for instance, it should not be visible past the corners of the Button’s overall footprint.

## Changing, hiding, and switching between types of InfoBadge
To show or hide an InfoBadge, simply set the `InfoBadge.IsOpen` property to the appropriate value. On showing and hiding, the InfoBadge will animate.

You can change the icon or number displayed in an InfoBadge while it is being shown. Decrementing or incrementing a numeric InfoBadge based on user action can be achieved by setting/manipulating the value of `InfoBadge.Value`. Changing the icon of an InfoBadge can be achieved by setting `InfoBadge.IconSource` to a new `IconSource` object. When changing icons, ensure that the new icon is the same size as the old icon to avoid a jarring visual effect.

### Default behavior
If neither `InfoBadge.Value` nor `InfoBadge.IconSource` are set, the InfoBadge defaults to showing a dot. On creation of the InfoBadge, both of these properties default to their sentinel values, hence the InfoBadge defaulting to show a dot. If both the `Value` and `IconSource` properties are set, the InfoBadge will honor the `Value` property and display a number value.  In order to hide an InfoBadge once any of its properties have been set, the `IsOpen` property will need to be set to `false`.

You can also change the InfoBadge’s type while it is being shown. To change the type of InfoBadge, be sure that the current type’s corresponding property (`Value` or `IconSource`) is set to its sentinel value (-1 or `null`), and set the new type’s property equal to an appropriate value. To change the type of InfoBadge from numeric or icon to a dot type InfoBadge, make sure that `InfoBadge.Value` is set to -1 and `InfoBadge.IconSource` is set to `null`.

Depending on how you’ve positioned your InfoBadge, be aware that this may cause items to shift as the shape of the InfoBadge may change.

## Accessibility
The InfoBadge control does not have any accessibility built in to it, as the control is not focusable and cannot be interacted with. To ensure your app is fully accessible, we recommend that the parent element of the InfoBadge should be focusable and accessible by tab, and that the parent element announces the InfoBadge to screenreaders.

## Examples
### Create an InfoBadge
**Creating a dot InfoBadge**:
```xml
<InfoBadge />
```

**Creating a numeric InfoBadge**:
```xml
<InfoBadge x:Name="emailInfoBadge" Value="{x:Bind numUnreadMail}"/>
```

In most scenarios, you’ll want to bind the `Value` property of the InfoBadge to a changing integer value in your app’s backend so you can easily increment/decrement and show/hide the InfoBadge based on that specific value.

**Creating an Icon InfoBadge**:
```xml
<InfoBadge x:Name="SyncStatusInfoBadge">
    <InfoBadge.IconSource>
        <SymbolIcon Symbol="Sync"/>
    </InfoBadge.IconSource>
</InfoBadge>
```

## Placing an InfoBadge inside another control
Here’s a Button that has an InfoBadge placed in its upper right hand corner. This example can be applied to many controls other than Button as well – it simply shows how to place, position, and show an InfoBadge inside of another WinUI control.

```xml
<Button Background="LightGray" Padding="0" Width="200" Height="50"
  HorizontalContentAlignment="Stretch" VerticalContentAlignment="Stretch">
    <Button.Content>
        <Grid HorizontalAlignment="Stretch" VerticalAlignment="Stretch"
  Width="Auto" Height="Auto">
            <SymbolIcon Symbol="Sync" HorizontalAlignment="Center"></SymbolIcon>
            <InfoBadge Background="Red" HorizontalAlignment="Right"
    VerticalAlignment="Top">
                <InfoBadge.IconSource>
                    <FontIcon FontFamily="Segoe MDL2 Assets" Glyph="&#F13C;"/>
                </InfoBadge.IconSource>
            </InfoBadge>
        </Grid>
    </Button.Content>
</Button>
```

## Using InfoBadge with a style preset
The markup below would create an InfoBadge that takes on the color and icon of the “Attention Icon” preset style.

```xml
<InfoBadge x:Name="InfoBadge1" Style="{ThemeResource AttentionIconInfoBadgeStyle}"/>
```

## Increment a numeric InfoBadge in a NavigationView
Here’s a NavigationView that uses an InfoBadge to display the number of new emails in the inbox, and increments the number shown in the InfoBadge when a new message is recieved.

**XAML Markup:**
```xml
<NavigationView>
    <NavigationView.MenuItems>
        <NavigationViewItem Content="Home" Icon="Home"/>
        <NavigationViewItem Content="Account" Icon="Contact"/>
        <NavigationViewItem x:Name="InboxPage" Content="Inbox" Icon="Mail">
            <NavigationViewItem.InfoBadge>
                    <InfoBadge x:Name="bg1" Value="{x:Bind numUnreadMail}"/>
            </NavigationViewItem.InfoBadge>
        </NavigationViewItem>
    </NavigationView.MenuItems>
    <Frame x:Name="contentFrame" />
</NavigationView>
```

**C# code-behind:**
```csharp
int numUnreadMail;

public void onNewMessageArrival(object sender, RoutedEventArgs msg){

    numUnreadMail += 1;

    /* Simply updating the numUnreadMail variable will cause the
    InfoBadge to increment if it’s currently visible.  */
}
```

## Hide a dot InfoBadge after its corresponding page has been clicked in NavigationView

This example shows a NavigationViewItem with a dot InfoBadge that gets hidden once the user navigates to the page being represented by the NavigationViewItem.

**XAML Markup:**
```xml
<NavigationView x:Name="nvSample">
    <NavigationView.MenuItems>
        <NavigationViewItem Content="Home" Icon="Home" Tag="Home" >
            <NavigationViewItem.InfoBadge>
                    <InfoBadge />
            </NavigationViewItem.InfoBadge>
            </NavigationViewItem>
        <NavigationViewItem  Content="Account" Icon="Contact" Tag="Contact" />
        <NavigationViewItem Content="Inbox" Icon="Mail" Tag="Mail" />
    <NavigationView.MenuItems>
    <Frame x:Name="contentFrame" />
</NavigationView>
 ```

**C# Code-behind:**
```csharp
// This function is called when any NavigationViewItem is clicked.
private void NavView_ItemInvoked(NavigationView sender,
                                 NavigationViewItemInvokedEventArgs args)
{
    // Check if the Settings item was clicked:
    if (args.IsSettingsInvoked == true)
    {
        NavView_Navigate("settings", args.RecommendedNavigationTransitionInfo);
    }
    else if (args.InvokedItemContainer != null)
    {
        NavigationViewItem current = args.InvokedItemContainer as NavigationViewItem;
        // If the clicked NavigationViewItem had an InfoBadge, hide the InfoBadge.
        if (current.InfoBadge.IsOpen){
                current.InfoBadge.IsOpen = false;
        }

        //Navigate to the appropriate page.
        var navItemTag = args.InvokedItemContainer.Tag.ToString();
        NavView_Navigate(navItemTag, args.RecommendedNavigationTransitionInfo);
    }
}
 ```

## Define an InfoBadge in code for a NavigationViewItem
This example defines NavigationViewItems in code, and initializes and updates a numeric InfoBadge that is shown when a message is received.

XAML Markup:

```xml
<muxc:NavigationView>
    <muxc:NavigationView.MenuItemTemplate>
        <DataTemplate x:DataType="local:CustomNavObject">
            <muxc:NavigationViewItem Content="{x:Bind Title}" Icon="{x:Bind ItemIcon}"
                                     InfoBadge="{x:Bind ItemInfoBadge}">
            </muxc:NavigationViewItem>
        </DataTemplate>
    </muxc:NavigationView.MenuItemTemplate>
</muxc:NavigationView>
```

C# Code-behind:
```csharp
public sealed partial class MainPage : Page
{

    public MainPage()
    {
        this.InitializeComponent();


        // Initialize icons for NavigationView items
        SymbolIcon HomeIcon = new SymbolIcon(Symbol.Home);
        SymbolIcon AcctIcon = new SymbolIcon(Symbol.Contact);
        SymbolIcon MailIcon = new SymbolIcon(Symbol.Mail);

        // Initialize an InfoBadge for the Mail item that is not visible on page load
        InfoBadge MailBadge = new InfoBadge();
        MailBadge.Value = 0;
        MailBadge.IsOpen = false;

        //Populate NavigationView
        List<CustomNavObject> navItems = new List<CustomNavObject>(){
            new CustomNavObject("Home", "home", HomeIcon),
            new CustomNavObject("Account", "acct", AccountIcon),
            new CustomNavObject("Mail", "mail", MailIcon, MailBadge)
        };
    }

    // This function is called when a new message is received.
    private void OnMessageReceived(string msg)
    {
        //Once a new message is received, update the InfoBadge being shown on the Mail navigation item.
           MailBadge.Value +=1;
           MailBadge.IsOpen = true;
    }
}

public class CustomNavObject
{
    public string Title { get; set; }
    public string Tag { get; set; }
    public IconSource ItemIcon { get; set; }
    public InfoBadge ItemInfoBadge { get; set; }

    public CustomNavObject(string title, string tag, IconSource icon)
    {
        Title = title;
        Tag = tag;
        ItemIcon =  icon;
    }

    public CustomNavObject(string title, string tag, IconSource icon, InfoBadge badge)
    {
        Title = title;
        Tag = tag;
        ItemIcon =  icon;
        ItemInfoBadge = badge;
    }

}
```

# API Pages


## InfoBadge class

Represents a control that displays brief status as an icon, number, or dot.

`public class InfoBadge : Control`

### Example
Here's an example of a simple InfoBadge that's set to display the number of unread emails:

```xml
<InfoBadge x:Name="emailInfoBadge" Value="{x:Bind numUnreadMail}"/>
```
### Remarks

If neither `InfoBadge.Value` nor `InfoBadge.IconSource` are set, the InfoBadge defaults to showing a dot. If both of these properties are set, the value appears in a numeric InfoBadge.

If `InfoBadge.IconSource` is set to null, the InfoBadge defaults to displaying a dot. If `InfoBadge.Value` is set to -1, InfoBadge also defaults to displaying a dot. In order to hide the InfoBadge, the `InfoBadge.IsOpen` property needs to be set to False.


## InfoBadge.Value property

Gets or sets the integer to be displayed in a numeric InfoBadge.

` public int InfoBadge.Value { get; set; }`

### Remarks
There is no maximum value for this property. The InfoBadge will continue to stretch to display large numbers, so ensure that your layout accounts for that if you expect to have large values displayed in an InfoBadge.

## InfoBadge.IconSource property

Gets or sets the icon to be used inside of the Icon InfoBadge.

`public IconSource InfoBadge.IconSource { get; set; }`

## InfoBadge.IsOpen property

Gets or sets the current visibility of the InfoBadge.

`public Boolean InfoBadge.IsOpen { get; set; }`

_Spec note: This property changes the visibility of an InfoBadge by changing its opacity value._

### Remarks
This property defaults to true.

If this property is changed, the InfoBadge will display a showing or hiding animation.

## NavigationViewItem.InfoBadge property

Gets or sets the InfoBadge object to display on the NavigationViewItem.

`public InfoBadge NavigationViewItem.InfoBadge { get; set; }`

## NavigationView.OverflowButtonInfoBadge property

Gets or sets the InfoBadge to display on the NavigationView’s overflow button.

`public InfoBadge NavigationView.OverflowButtonInfoBadge { get; set; }`

### Remarks
The `NavigationView.OverflowButtonInfoBadge` is only displayed when the NavigationView has overflow items. Unlike a normal InfoBadge, this particular InfoBadge sets its `IsOpen` property to `false` by default. So, this InfoBadge will not be visible unless you set the `IsOpen` property to `true`.

## NavigationView.OverflowItems

Gets the collection of NavigationViewItems currently being shown in the overflow menu.

`public ObservableCollection<object> NavigationView.OverflowItems { get; }`


## New ThemeResources
```xml
<Style x:Key="AttentionIconInfoBadgeStyle" TargetType="InfoBadge"></Style>
```
```xml
<Style x:Key="InformationalIconInfoBadgeStyle" TargetType="InfoBadge"></Style>
```
```xml
<Style x:Key="SuccessIconInfoBadgeStyle" TargetType="InfoBadge"></Style>
```
```xml
<Style x:Key="CautionIconInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="CriticalIconInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="AttentionDotInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="InformationalDotInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="SuccessDotInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="CautionDotInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

```xml
<Style x:Key="CriticalDotInfoBadgeStyle" TargetType="InfoBadge"></Style>
```

# API Details
## InfoBadge API Details
```c# (but really MIDL3)
[MUX_PUBLIC]
[webhosthidden]
unsealed runtimeclass InfoBadge : Windows.UI.Xaml.Controls.Control
{
    InfoBadge();

    Microsoft.UI.Xaml.Controls.IconSource Icon { get; set; }
    int Value { get; set; }
    Boolean IsOpen { get; set; }

    static Windows.UI.Xaml.DependencyProperty IconProperty { get; };
    static Windows.UI.Xaml.DependencyProperty ValueProperty { get; };
    static Windows.UI.Xaml.DependencyProperty IsOpenProperty { get; };
}
```

## NavigationViewItem API Details
```csharp
[MUX_PUBLIC]
[webhosthidden]
unsealed runtimeclass NavigationViewItem : NavigationViewItemBase
{
    NavigationViewItem();

    // Existing members have been excluded

    Microsoft.UI.Xaml.Controls.InfoBadge InfoBadge { get; set; }

    static Windows.UI.Xaml.DependencyProperty InfoBadgeProperty { get; }
}
```

## NavigationView API Details
```c#
[MUX_PUBLIC]
[webhosthidden]
[MUX_PROPERTY_CHANGED_CALLBACK(TRUE)]
[MUX_PROPERTY_CHANGED_CALLBACK_METHODNAME("OnPropertyChanged")]
unsealed runtimeclass NavigationView : Windows.UI.Xaml.Controls.ContentControl
{
    NavigationView();

    // Existing members have been excluded

    Microsoft.UI.Xaml.Controls.InfoBadge OverflowButtonInfoBadge { get; set; }
    System.Collections.ObjectModel.ObservableCollection<System.Object> OverflowItems { get; }

    static Windows.UI.Xaml.DependencyProperty OverflowButtonInfoBadgeProperty { get; }

}
```


# Appendix

## Accessibility Information
The InfoBadge comes at a default size that meets accessibility requirements. Developers can customize many aspects of the InfoBadge including its height/width/color, etc. but it’s important that the default InfoBadge adheres to our accessibility guidelines for size and color.

The InfoBadge’s parent item should be focusable and accessible by tab. The InfoBadge itself should not be focusable as it cannot be directly interacted with, and InfoBadge should not block input. However, the recommended approach is for the parent item to announce InfoBadge as a part of its narrator announcement.

NavigationView will have new built-in accessibility support for InfoBadge. When you're tabbing through a NavigationView and you land on a NavigationViewItem with an InfoBadge on it, the screenreader will announce that there is an InfoBadge on this item. If the InfoBadge in question is numeric, the screenreader will announce the InfoBadge's value as well.

The InfoBadge itself is not dismissible via click or other action. It is completely up to the developer to determine when to show and hide the InfoBadge.

The default background color of an InfoBadge is set to SystemColorHighlightColor, which is the accent color. The number or icon inside of an InfoBadge has the foreground color set to SystemColorHighlightTextColor by default. These colors ensure that the InfoBadge will adhere to high contrast accessibility guidelines.



================================================
FILE: specs/InfoBadge/images/color-breakdown.PNG
================================================
[Non-text file]


================================================
FILE: specs/ScrollingControls/ScrollPresenter.md
================================================
**WinUI** API Specification : **ScrollPresenter**
===============================================

# Background

(Full Summary, Rationale, and High-Level Plan in the proposal on GitHub: [A more flexible ScrollViewer](https://github.com/Microsoft/microsoft-ui-xaml/issues/108))

This spec describes a building block for the new `ScrollView` control (which is described in a
[separate spec](ScrollView.md)): the `ScrollPresenter`. This pair of controls replaces the existing
pair `ScrollViewer` and `ScrollContentPresenter`

|   | Current | New
-|-|-
Primary control | [ScrollViewer](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.ScrollViewer) | `ScrollView`
Primitive scroller | [ScrollContentPresenter](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.ScrollContentPresenter) | `ScrollPresenter` (this spec)

`ScrollPresenter` is similar to the `ScrollContentPresenter` used in the old `ScrollViewer` control
template as it applies the clipping, translation and scaling of the `ScrollView` content.
It is present in the `ScrollView`'s default control template alongside the two `ScrollBar` controls.

![Scroll controls](./images/scroll-controls.jpg)

Contrary to the old `ScrollContentPresenter` element though, the `ScrollPresenter` is a fully functional
and reusable primitive component with a public object model that is very similar to the `ScrollView`
object model.
In most cases, the `ScrollView` control merely forwards an API call to the identical API of its
inner `ScrollPresenter`.

The typical usage of a `ScrollPresenter` is that of a building block for a more complex control,
like the `ScrollView`.

Here the `ScrollPresenter` is used as part of a scrolling/zooming control which
employs custom UI widgets to control the translation and scale in lieu of two scrollbars.

```xml
<UserControl
    x:Class="AcmeApp.MyScroller"
    xmlns=http://schemas.microsoft.com/winfx/2006/xaml/presentation
    xmlns:muxp="using:Microsoft.UI.Xaml.Controls.Primitives">
    <Grid>
        <muxp:ScrollPresenter x:Name="scrollPresenter"/>
        <acme:ScrollController x:Name="scrollController" HorizontalAlignment="Right"/>
        <acme:ZoomController x:Name="zoomController" HorizontalAlignment="Right" VerticalAlignment="Top"/>
    </Grid>
</UserControl>
```

_Spec note:_
_Mike: "What's a ScrollController?"_

It can be used as a top level element too, as in the following example.

```xml
<Page
    xmlns=http://schemas.microsoft.com/winfx/2006/xaml/presentation
    xmlns:muxp="using:Microsoft.UI.Xaml.Controls.Primitives">
    <muxp:ScrollPresenter Width="500" Height="400" Background="Beige">
        <TextBlock Text="{x:Bind AllTheText}" TextWrapping="Wrap"/>
    </muxp:ScrollPresenter>
</Page>
```


Xaml has a [ScrollViewer](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.ScrollViewer) control
for scrolling content, using scroll bars and panning, etc. Typical uses are as the root of a page whose
content might not fit; and a ListView, which internally uses a ScrollViewer for its list of items.

For example the following shows a large text block that wraps horizontally and scrolls vertically:

```xml
<Page xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation">
    <ScrollViewer>
        <TextBlock Text="{x:Bind AllTheText}" TextWrapping="Wrap" />
    </ScrollViewer>
</Page>
```

# Table of Contents

[[_TOC_]]


# Conceptual pages (how to)

`ScrollPresenter` is a container control that lets the user scroll (and pan), and zoom its content.

A `ScrollPresenter` enables content to be displayed in a smaller area than its actual size. The user
can use touch to pan and zoom the content, or the keyboard and mouse wheel to scroll and zoom the content.

The area that includes all of the content of the `ScrollPresenter` is the *extent*. The visible area of
the content is the *viewport*.

![Viewport and Extent](images/ViewportAndExtent.jpg)


A second kind of scrolling element, providing just clipping and translation of content, and

The `ScrollPresenter` can be used as a primitive building block for controls like the `ScrollView` which
adds the default user interaction widgets (scrollbars, scroll indicator, etc.) and policy.
Indeed the `ScrollView` defined in the [separate spec](ScrollView.md) uses a `ScrollPresenter` as
part of its implementation (in its ControlTemplate).

Contrary to the `ScrollView` which is a Control, the `ScrollPresenter` is a FrameworkElement and
as such it does not receive keyboard focus. Its parent `ScrollView` has the
built-in logic to decide whether to scroll the viewport or move focus in response to a key event.

The `ScrollPresenter` does not impose any particular policy.
Again it is the parent `ScrollView` that sets the properties on its inner `ScrollPresenter`
to values chosen to match common usage,
for example the basic `<ScrollView/>` is configured for vertical scrolling.


## Snap points examples

The `ScrollPresenter` element exposes three collections to set scroll and zoom snap points.
(A snap point is a position that is a natural stopping place for scrolling or zooming to land on.)

| **Type**                                                    | **Snap points collection** |
|-------------------------------------------------------------|----------------------------|
| Windows.Foundation.Collections.IVector<ScrollSnapPointBase> | HorizontalSnapPoints       |
| Windows.Foundation.Collections.IVector<ScrollSnapPointBase> | VerticalSnapPoints         |
| Windows.Foundation.Collections.IVector<ZoomSnapPointBase>   | ZoomSnapPoints             |

At the end of a scroll inertia (for example the scrolling that continues briefly after touch input),
the `ScrollPresenter`'s HorizontalOffset property will land at a value which depends on the
HorizontalSnapPoints collection (same for VerticalOffset and VerticalSnapPoints).
Likewise, at the end of a zoom inertia, the `ScrollPresenter`'s ZoomFactor property will land at
a value which depends on the ZoomSnapPoints collection.

Two types of scroll snap points exist, and they both derive from `ScrollSnapPointBase`: `ScrollSnapPoint`
and `RepeatedScrollSnapPoint`.

A `ScrollSnapPoint` is a single point characterized by an alignment and value.
The alignment enumeration of `Near`, `Center` or `Far` indicates where the snap point is located in
relation to the viewport.
For example, for a horizontal snap point, the `Near` alignment corresponds to the left edge of the viewport.
`Center` means the middle of the viewport, and finally `Far` means the right edge.

_Spec note:_
_Mike: "So in RTL and horizontal, "Near" means the right side?"_

A `RepeatedScrollSnapPoint` defines multiple equidistant points.
It is characterized by an alignment, an interval, an offset, a start and end.
The interval determines the equidistance between two successive points.
The points are shifted from 0 by an amount defined by the offset.
The start and end define a domain in which the snap points are effective.

### Setting horizontal repeated snap points

In this example, a horizontal repeated snap point is defined at values -10, 50, 110, 170, 230 and 290.

![Repeater Scroll Snap points](images/RepeatedSnapPoints.png)

The natural rest point is defined as the landing point after inertia if no snap points were present.
That natural rest point defines which snap point value is activated.
In this case, if the natural rest point is before the _start_ 10 or after the _end_ 270,
no snap point value is activated and inertia carries on without the influence of the repeated snap point.
If however the natural rest point is in the \[10, 270\] domain,
the closest snap point value to the natural rest point is activated.
For example if the natural rest point is 95, the final HorizontalOffset property will be 110 instead of 95.
Because the provided _alignment_ is Near, the snap point values align with the left edge of the `ScrollPresenter`.
The applicable ranges, or attraction zones, of the snap point values -10, 50, 110, 170, 230, 290 are
respectively \[10, 20\], \]20, 80\], \]80, 140\], \]140, 200\], \]200, 260\] and \]260, 270\].
If an activated horizontal snap point value is out-of-bounds, i.e. smaller than 0 or greater than ScrollableWidth,
the content will first animate to that out-of-bounds position then animate back to the closest in-bounds position.

_Spec note:_
_Mike: "Curious how much of this is ScrollPresenter and how much is InteractionTracker?"_

```csharp
RepeatedScrollSnapPoint snapPoint =
    new RepeatedScrollSnapPoint(
        offset: 50,
        interval: 60,
        start: 10,
        end: 270,
        alignment: ScrollSnapPointsAlignment.Near);
myScrollPresenter.HorizontalSnapPoints.Add(snapPoint);
```

### Setting vertical repeated snap points

This example uses a vertical StackPanel in a `ScrollPresenter` with identically sized children.
All the children are 200px tall and the goal is to have their top edge snap at the top edge of the viewport.
A `RepeatedScrollSnapPoint` with Near alignment can be used for that purpose.

```csharp
RepeatedScrollSnapPoint snapPoint =
    new RepeatedScrollSnapPoint(
        offset: 0,
        interval: 200,
        start: 0,
        end: myScrollPresenter.Content.ActualSize.Y,
        alignment: ScrollSnapPointsAlignment.Near);
myScrollPresenter.VerticalSnapPoints.Add(snapPoint);
```

### Setting vertical irregular snap points

This example showcases a vertical StackPanel in a `ScrollPresenter`.
That panel has 4 chidren elements of variable heights,
each of them being assigned a snap point so that their center snaps vertically to the center of the viewport
as much as possible.

![Repeated Scroll Snap points](images/VerticalScrollSnapPoints.png)

The viewport is 610px tall, the 4 children are 360px, 290px, 220px and 160px tall.
Since the desired alignment is Center, the content snap points will align to the middle of the viewport,
at position 610/2=305px.
The ideal snap points for the 4 children are respectively at positions 180, 505, 760 and 950 from the top
of the StackPanel.
Without the restriction of the content staying in-bounds, the 4 children's center would align with the
viewport's center.
The content extent being 1030px tall, the `ScrollPresenter`'s VerticalOffset property can vary from 0 to
ScrollableHeight = 1030 - 610 = 420.
To avoid the content first animating out-of-bounds and then animating in-bounds,
the snap points can be moved to 305, 505, 725 and 725.
Only the second child is not affected by boundary restrictions.
The two last children get the same snap point at position 725.

```csharp
ScrollSnapPoint snapPoint1 = new ScrollSnapPoint(
    snapPointValue: 305, alignment: ScrollSnapPointsAlignment.Center);

ScrollSnapPoint snapPoint2 = new ScrollSnapPoint(
    snapPointValue: 505, alignment: ScrollSnapPointsAlignment.Center);

ScrollSnapPoint snapPoint3 = new ScrollSnapPoint(
    snapPointValue: 725, alignment: ScrollSnapPointsAlignment.Center);

myScrollPresenter.VerticalSnapPoints.Add(snapPoint1);
myScrollPresenter.VerticalSnapPoints.Add(snapPoint2);
myScrollPresenter.VerticalSnapPoints.Add(snapPoint3);
```

The applicable ranges, or attraction zones, for snapPoint1,
snapPoint2 and snapPoint3 are \]-inf, 405\], \]405, 615\] and \]615, +inf\[.
So for example, if the natural rest point at the beginning of an inertial phase is 600,
the HorizontalOffset will animate to the snap point 505 instead.


### Setting repeated zoom snap points

A `RepeatedZoomSnapPoint` is set on the `ScrollPresenter` in order to have its ZoomFactor snap to
values 0.1, 0.2, 0.3, etc... at the end of an inertial zoom.

```csharp
RepeatedZoomSnapPoint snapPoint =
    new RepeatedZoomSnapPoint(
        offset: 0,
        interval: 0.1,
        start: 0,
        end: myScrollPresenter.MaxZoomFactor);
myScrollPresenter.ZoomSnapPoints.Add(snapPoint);
```

### Setting irregular zoom snap points

In this case the goal is to set zoom snap points at values 0.15, 0.3, 0.6, 1.2, 2.4, 4.8 and 9.6.
Seven individual `ZoomSnapPoint` instances are added to the ZoomSnapPoints collection:

```csharp
for (double snapPointValue = 0.15; snapPointValue < 10.0; snapPointValue *= 2.0)
{
    myScrollPresenter.ZoomSnapPoints.Add(new ZoomSnapPoint(snapPointValue));
}
```

## Custom scroll controller example

The `ScrollPresenter`'s HorizontalScrollController and VerticalScrollController properties allow to
use custom scrollbar widgets instead of the default `ScrollBar` control.

_Spec note:_
_Mike: "What does "default" mean here? The ScrollPresenter doesn't have default scroll bars, does it?"_

| **Type**                                                | **Scroll controller properties** |
|---------------------------------------------------------|----------------------------------|
| Microsoft.UI.Xaml.Controls.Primitives.IScrollController | HorizontalScrollController       |
| Microsoft.UI.Xaml.Controls.Primitives.IScrollController | VerticalScrollController         |

Those widgets need to implement the IScrollController interface which standardizes the communication between
the `ScrollPresenter` and its 2 scroll controllers.
In this example, the vertical `ScrollBar` found in a `ScrollView`'s default control template is hidden and
replaced with a custom timeline scrubber in a Photos Gallery application.
The TimelineScrubber control presents a timeline for the photos being scrolled through.
The default horizontal `ScrollBar` is left intact.

![Custom vertical scroll controller](images/VerticalTimelineScrubber.png)

```csharp
myScrollView.VerticalScrollBarVisibility = ScrollingScrollBarVisibility.Hidden;

ScrollPresenter myScrollPresenter = myScrollView.GetValue(ScrollView.ScrollPresenterProperty) as ScrollPresenter;

myScrollPresenter.VerticalScrollController = myTimelineScrubber;
```

_Spec note:_
_Mike: "Why using GetValue here, is this a DP with no property accessors?"_

An alternate approach would be to use a custom control template for that `ScrollView` instance with a TimelineScrubber
named "PART_VerticalScrollBar" instead of a vertical `ScrollBar`.


# API Notes

## ScrollPresenter class

Provides primitive scroll and zoom supports for content.

### ScrollPresenter.HorizontalSnapPoints property

Gets the collection of snap points affecting the `ScrollPresenter.HorizontalOffset` property.
This collection is empty by default.
Horizontal snap points cause the HorizontalOffset property to settle at deterministic values at the end of inertia.

In this example, the `ScrollPresenter.HorizontalOffset` property lands at value 500.0 or 1500.0,
whichever is closest to the position where the content would have stopped without the presence of snap points.

```csharp
ScrollSnapPoint snapPoint1 = new ScrollSnapPoint(snapPointValue: 500.0, alignment: ScrollSnapPointsAlignment.Near);
ScrollSnapPoint snapPoint2 = new ScrollSnapPoint(snapPointValue: 1500.0, alignment: ScrollSnapPointsAlignment.Near);

myScrollPresenter.HorizontalSnapPoints.Add(snapPoint1);
myScrollPresenter.HorizontalSnapPoints.Add(snapPoint2);
```

### ScrollPresenter.VerticalSnapPoints property

Gets the collection of snap points affecting the `ScrollPresenter.VerticalOffset` property.
This collection is empty by default.
Vertical snap points cause the VerticalOffset property to settle at deterministic values at the end of inertia.

In this example, the `ScrollPresenter.VerticalOffset` property lands at value 500.0 or 1500.0,
whichever is closest to the position where the content would have stopped without the presence of snap points.

```csharp
ScrollSnapPoint snapPoint1 = new ScrollSnapPoint(snapPointValue: 500.0, alignment: ScrollSnapPointsAlignment.Near);
ScrollSnapPoint snapPoint2 = new ScrollSnapPoint(snapPointValue: 1500.0, alignment: ScrollSnapPointsAlignment.Near);

myScrollPresenter.VerticalSnapPoints.Add(snapPoint1);
myScrollPresenter.VerticalSnapPoints.Add(snapPoint2);
```

### ScrollPresenter.ZoomSnapPoints property

Gets the collection of snap points affecting the `ScrollPresenter.ZoomFactor` property.
This collection is empty by default.
Zoom snap points cause the ZoomFactor property to settle at deterministic values at the end of inertia.

In this example, the `ScrollPresenter.ZoomFactor` property lands at value 2.5 or 5.0,
whichever is closest to the zoom factor where the content would have stopped without the presence of snap points.

```csharp
ZoomSnapPoint snapPoint1 = new ZoomSnapPoint(snapPointValue: 2.5);
ZoomSnapPoint snapPoint2 = new ZoomSnapPoint(snapPointValue: 5.0);

myScrollPresenter.ZoomSnapPoints.Add(snapPoint1);
myScrollPresenter.ZoomSnapPoints.Add(snapPoint2);
```

### ScrollPresenter.HorizontalScrollController property

Gets or sets the `IScrollController` implementation that can drive the horizontal scrolling of the `ScrollPresenter`.
The component that implements IScrollController is typically a UI widget like a `ScrollBar` the user can
interact with to control the scrolling offset in one direction.
The default HorizontalScrollController property value is null.

```csharp
myScrollPresenter.HorizontalScrollController = myTimelineScrubber;
```

See [this section](#sample-iscrollController-implementations) for a couple of full `IScrollController`
implementation samples.

### ScrollPresenter.VerticalScrollController property

Gets or sets the `IScrollController` implementation that can drive the vertical scrolling of the `ScrollPresenter`.
The component that implements IScrollController is typically a UI widget like a `ScrollBar` the user can
interact with to control the scrolling offset in one direction.
The default VerticalScrollController property value is null.

```csharp
myScrollPresenter.VerticalScrollController = myTimelineScrubber;
```

See [this section](#sample-iscrollController-implementations) for a couple of full `IScrollController`
implementation samples.


## IScrollController interface

The `ScrollPresenter` exposes two read-write properties of type IScrollController representing optional
scrollbar-like widgets that can participate in setting the scrolling offsets of the content.
Those widgets are the implementers of the IScrollController interface, while the `ScrollController`
is the consumer.

Throughout the remainder of this interface description, the term `ScrollPresenter` is used,
but the consumer of the IScrollController interface is not necessarily a ScrollPresenter.
It may be some alternative scrolling control.


## IScrollController.AreInteractionsAllowed property (Boolean)

This read-only property indicates whether the scroll controller can perform user interactions or not.

_Spec note:_
_Mike: "How does the controller indicate that this has changed? Do we need a change event
that can be raised after the control gets disabled?"_

The scroll controller returns False for example when it is a disabled control.

The `ScrollView` control accesses this property to evaluate its ComputedHorizontalScrollBarVisibility
and ComputedVerticalScrollBarVisibility dependency properties,
as well as the visibility of its scroll controller separator element (Template part named PART_ScrollBarsSeparator).

For example, when the ScrollView.HorizontalScrollBarVisibility property is `ScrollingScrollBarVisibility.Auto`
and the horizontal IScrollController implementation's `AreInteractionsAllowed` property returns False,
the `ComputedHorizontalScrollBarVisibility` dependency property is set to `Visibility.Collapsed`.

_Spec note:_
_Mike: "We usually use "ActualFoo" rather than "ComputedFoo""_

## IScrollController.IsInteracting property (Boolean)

This read-only property indicates whether the scroll controller is handling a user interaction or not.

A scroll controller may return True for example when the user is dragging a thumb to control the scrolling
offset of the `ScrollPresenter`.

A UI-thread-independent pan performed with the InteractionElement property must not cause the IsInteracting
property to return `True` though.
It would prevent the user from being able to interrupt inertia from such a pan by touching the
`ScrollPresenter`'s content.

_Spec note:_
_Mike: "Are any of these APIs called from off the UI thread?"_

The `ScrollView` control for example accesses this property to keep auto-hiding scroll controllers visible
during a user interaction.
(That auto-hiding behavior is dependent on the
[UISettings.AutoHideScrollBars](https://docs.microsoft.com/uwp/api/Windows.UI.ViewManagement.UISettings.AutoHideScrollBars)
property evaluation.)

When returning True, this property prevents the `ScrollPresenter` from initiating a new pan of its content
when the user touches it.


## IScrollController.InteractionElement property (UIElement)

This read-only property returns a UIElement that can be panned with touch off the UI-thread like the
`ScrollPresenter`'s content.

_Spec note:_
_Mike: "Can't tell what this means? Is this saying that you could go from this element to a comp Visual
and do background input on it?"_

A scroll controller can return null instead of a UIElement, indicating that none of its UI pieces can be
panned off the UI-thread.
In that case the `ScrollPresenter` does not invoke the IsInteractionElementRailEnabled,
InteractionElementScrollOrientation and SetExpressionAnimationSources APIs.

## IScrollController.IsInteractionElementRailEnabled property (Boolean)

This read-only property indicates whether the UIElement returned by the InteractionElement property
must use railing during a UI-thread-independent pan.
Railing locks the movement of the element on one orientation, horizontal or vertical.

This property is only invoked when the InteractionElement property returns a non-null UIElement.

## IScrollController.InteractionElementScrollOrientation property (Orientation)

This read-only property returns the panning orientation of the UIElement returned by the
InteractionElement property.

This property is only invoked when the InteractionElement property returns a non-null UIElement.

## IScrollController.SetExpressionAnimationSources

```cs
void SetExpressionAnimationSources(
    Microsoft.UI.Composition.CompositionPropertySet propertySet,
    String minOffsetPropertyName,
    String maxOffsetPropertyName,
    String offsetPropertyName,
    String multiplierPropertyName)
```

This method is invoked by the `ScrollPresenter` to provide a CompositionPropertySet populated
with 4 properties.

The scroll controller is meant to read 3 of those properties and write 1 of them.
The 3 readable scalar properties are identified by the names minOffsetPropertyName, maxOffsetPropertyName
and offsetPropertyName - they represent the minimum, maximum and current scrolling offset values.

The 1 writeable property is also a scalar one, identified by the provided multiplierPropertyName name.
The scroll controller is in charge of writing into this scalar property, providing a number that
represents the relative movement of the InteractionElement and ScrollPresenter content.
The property value represents a ratio. Both negative and positive ratios/multipliers are supported.

For example, for a typical scrollbar thumb, the finger on the InteractionElement may go down by 2 pixels,
causing the ScrollPresenter content to go up by 10 pixels.
To achieve this, the scroll controller is expected to write -5.0f into the multiplierPropertyName property.
The `ScrollPresenter` consumes that multiplierPropertyName scalar property in expression animations it builds
internally to translate finger movement to content movement.

All 4 animated scalars can be used in the scroll controller's expression animations,
to position the InteractionElement's IVisual for example.

This method is only invoked when the InteractionElement property returns a non-null UIElement.

## IScrollController.SetScrollMode

```cs
void SetScrollMode(Microsoft.UI.Xaml.Controls.ScrollingScrollMode scrollMode)
```

This method is invoked by the `ScrollPresenter` to indicate whether scrolling through user input is
turned on or not.
For example, the `ScrollPresenter` uses 4 of its properties for these calls:
HorizontalScrollController.SetScrollMode(HorizontalScrollMode) and VerticalScrollController.SetScrollMode(VerticalScrollMode).

_Spec note:_
_Mike: "I'm confused about what this sentence is saying. Uses which 4 properties for those SetScrollMode
calls? (Or do I need to understand the number of properties?)"_

## IScrollController.SetValues

```cs
void SetValues(Double minOffset, Double maxOffset, Double offset, Double viewport)
```

_Spec note:_
_Mike: "A more meaningful name? SetDimensionValues?"_

This method is invoked by the `ScrollPresenter` to provide dimension information to the scroll controller.

_minOffset_ and  _maxOffset_ indicate the minimum and maximum offsets allowed for the relevant scrolling
orientation, at idle.
_offset_ indicates the current offset value, which is not necessarily between those minimum and maximum
offsets because of overpan situations.
_viewport_ indicates the size of the `ScrollPresenter`'s viewport.

The scroll controller can use those dimensions to adjust the size and position of a UIElement, for example
a draggable thumb on the UI thread.

## IScrollController.GetScrollAnimation

```cs
CompositionAnimation GetScrollAnimation(
    Int32 correlationId,
    Windows.Foundation.Numerics.Vector2 currentPosition,
    Microsoft.UI.Composition.CompositionAnimation defaultAnimation)
```

The scroll controller can request an animated scroll by raising its ScrollToRequested or
ScrollByRequested event.
In response, the `ScrollPresenter` does not raise its ScrollAnimationStarting event.
Instead it invokes this GetScrollAnimation method to give the scroll controller the opportunity
to customize the animation that is about to be launched.
The scroll controller is given the correlationId for the operation,
the current position of the content and default composition animation which is a Vector3KeyFrameAnimation
about to be launched by default.
The correlationId is the one provided earlier in ScrollControllerScrollToRequestedEventArgs.CorrelationId
or in ScrollControllerScrollByRequestedEventArgs.CorrelationId.
The scroll controller can then return: null or an unchanged _defaultAnimation_ to use that default animation,
a modified version of _defaultAnimation_, or a brand-new custom animation.

## IScrollController.NotifyScrollCompleted

```cs
void NotifyScrollCompleted(Int32 correlationId)
```

This method is invoked by the `ScrollPresenter` to indicate that a scrolling operation initiated through
a ScrollToRequested, ScrollByRequested or AddScrollVelocityRequested event has completed.
It provides the operation's correlationId which was exposed earlier in
ScrollControllerScrollToRequestedEventArgs.CorrelationId, ScrollControllerScrollByRequestedEventArgs.CorrelationId
or ScrollControllerAddScrollVelocityRequestedEventArgs.CorrelationId.

## IScrollController.ScrollToRequested  event

```cs
event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerScrollToRequestedEventArgs> ScrollToRequested
```

The scroll controller can request a scroll to a particular offset by raising its ScrollToRequested event.
The `ScrollPresenter` handles the event and provides a correlationId in
ScrollControllerScrollToRequestedEventArgs.CorrelationId for the operation that is about to start.
The scroll controller can for example make such a request when a thumb is dragged to a new position.

## IScrollController.ScrollByRequested event

```cs
Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerScrollByRequestedEventArgs> ScrollByRequested
```

The scroll controller can request a scroll by a particular offset delta by raising its ScrollByRequested event.
The `ScrollPresenter` handles the event and provides a correlationId in ScrollControllerScrollByRequestedEventArgs.CorrelationId
for the operation that is about to start.
The scroll controller can for example make such a request when a button is clicked to move a thumb by an increment.

## IScrollController.AddScrollVelocityRequested

```cs
event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerAddScrollVelocityRequestedEventArgs> AddScrollVelocityRequested
```

The scroll controller can request a scroll by adding velocity to the `ScrollPresenter` content through
the AddScrollVelocityRequested event.

_Spec note:_
_Mike: "Don't understand what this means. Is this the case where we're in inertia and the pointer touches again?"_

## IScrollController.InteractionRequested event

```cs
event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerInteractionRequestedEventArgs> InteractionRequested
```

This event can be raised by the scroll controller when the user attempts to initiate a UI-thread-independent pan,
with touch or a pen, using the UIElement returned by the InteractionElement property.

_Spec note:_
_Mike: "It's only for the off thread case? So the controller raises the event off thread?"_

The `ScrollPresenter` sets the ScrollControllerInteractionRequestedEventArgs.Handled property to True when
it successfully initiated such a pan. This event is not meant to be raised when the InteractionElement property
returns null.

_Spec note:_
_Mike: "The event is named "interaction" but the description says "pan". Is it just for panning?"_

## IScrollController.InteractionInfoChanged event

```cs
event Windows.Foundation.TypedEventHandler<IScrollController, Object> InteractionInfoChanged
```

This event is raised by the scroll controller after any of its properties AreInteractionsAllowed, IsInteracting,
IsInteractionElementRailEnabled, InteractionElement, or InteractionElementScrollOrientation changed.

_Spec note:_
_Mike: "Can we leave off the list of properties and just say "any of its properties"?"_

## ScrollControllerScrollToRequestedEventArgs class

Used by the ScrollToRequested event which is raised when the scroll controller requests a scroll
to a particular offset.

| **Member**                                 | **Description**                                                                                                                                |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| ScrollControllerScrollToRequestedEventArgs | Constructor with _offset_ and _options_ parameters invoked by the scroll controller.                                                           |
| Offset                                     | Gets the target offset.                                                                                                                        |
| Options                                    | Gets the options for the scroll operation which determine whether the scroll is animated or not and whether snap points are applied or not.    |
| CorrelationId                              | Gets or sets the correlation ID associated with the offset change. This value is set by the `ScrollPresenter` which is fulfilling the request. |


## ScrollControllerScrollByRequestedEventArgs class

Used by the ScrollByRequested event which is raised when the scroll controller requests a scroll by
a particular offset delta.

| **Member**                                 | **Description**                                                                                                                                |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| ScrollControllerScrollByRequestedEventArgs | Constructor with _offsetDelta_ and _options_ parameters invoked by the scroll controller.                                                      |
| OffsetDelta                                | Gets the offset change requested. May be positive or negative.                                                                                 |
| Options                                    | Gets the options for the scroll operation which determine whether the scroll is animated or not and whether snap points are applied or not.    |
| CorrelationId                              | Gets or sets the correlation ID associated with the offset change. This value is set by the `ScrollPresenter` which is fulfilling the request. |


## ScrollControllerAddScrollVelocityRequestedEventArgs class

Used by the AddScrollVelocityRequested event which is raised when the scroll controller requests a scroll by
adding velocity to the `ScrollPresenter` content.

| **Member**                                          | **Description**                                                                                                                                |
|-----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| ScrollControllerAddScrollVelocityRequestedEventArgs | Constructor with _offsetVelocity_ and _inertiaDecayRate_ parameters invoked by the scroll controller.                                          |
| OffsetVelocity                                      | Gets the offset velocity change requested. May be positive or negative.                                                                        |
| InertiaDecayRate                                    | Gets the inertia decay rate, between 0.0 and 1.0, for the requested scroll operation. It affects the inertial velocity decrease (decay). The closer the value is to 1.0, the faster the deceleration. A value of 0.0 represents no decay and results in a constant velocity scroll. The returned value may be null which causes the default decay rate of 0.95 to be used. |
| CorrelationId                                       | Gets or sets the correlation ID associated with the offset change. This value is set by the `ScrollPresenter` which is fulfilling the request. |


## ScrollControllerInteractionRequestedEventArgs class

Used by the InteractionRequested event which is raised when the scroll controller attempts to initiate
a UI-thread-independent pan, with touch or a pen, using the UIElement returned by the InteractionElement property.

| **Member**                                    | **Description**                                                                                                                                                                                                          |
|-----------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ScrollControllerInteractionRequestedEventArgs | Constructor with _pointerPoint_ parameter invoked by the scroll controller.                                                                                                                                              |
| PointerPoint                                  | Microsoft.UI.Input.PointerPoint instance associated with the user gesture triggering the InteractionRequested event. A scroll controller may retrieve it from a Microsoft.UI.Xaml.Input.PointerRoutedEventArgs instance. |
| Handled                                       | Gets or sets a value indicating whether the pan manipulation was successfully initiated or not. The `ScrollPresenter` sets this property while it processes the InteractionRequested event.                              |


# API Details

## Shared enumerations and structures between `ScrollView` and `ScrollPresenter`

Present in namespace Microsoft.UI.Xaml.Controls:

```csharp
enum ScrollingContentOrientation
{
    Vertical = 0,
    Horizontal = 1,
    None = 2,
    Both = 3,
};

enum ScrollingInteractionState
{
    Idle = 0,
    Interaction = 1,
    Inertia = 2,
    Animation = 3,
};

enum ScrollingScrollMode
{
    Enabled = 0,
    Disabled = 1,
};

enum ScrollingZoomMode
{
    Enabled = 0,
    Disabled = 1,
};

enum ScrollingChainMode
{
    Auto = 0,
    Always = 1,
    Never = 2,
};

enum ScrollingRailMode
{
    Enabled = 0,
    Disabled = 1,
};

[flags]
enum ScrollingInputKinds
{
    None = 0x00,
    Touch = 0x01,
    Pen = 0x02,
    MouseWheel = 0x04,
    Keyboard = 0x08,
    Gamepad = 0x10,
    All = 0xFFFFFFFF,
};

enum ScrollingAnimationMode
{
    Disabled = 0,
    Enabled = 1,
    Auto = 2,
};

enum ScrollingSnapPointsMode
{
    Default = 0,
    Ignore = 1,
};
```

_Spec note:_
_Mike: "I don't see any explanation for any of these three enums.
A one/two-liner comment on top of each enum would be good"_

## `ScrollPresenter` enumeration

```csharp
enum Microsoft.UI.Xaml.Controls.Primitives.ScrollSnapPointsAlignment
{
    Near = 0,
    Center = 1,
    Far = 2,
};
```

## Shared method argument classes between `ScrollView` and `ScrollPresenter`

```csharp
unsealed runtimeclass Microsoft.UI.Xaml.Controls.ScrollingScrollOptions
{
    ScrollingScrollOptions(ScrollingAnimationMode animationMode);
    ScrollingScrollOptions(ScrollingAnimationMode animationMode, ScrollingSnapPointsMode snapPointsMode);

    ScrollingAnimationMode AnimationMode { get; set; };
    ScrollingSnapPointsMode SnapPointsMode { get; set; };
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.ScrollingZoomOptions
{
    ScrollingZoomOptions(ScrollingAnimationMode animationMode);
    ScrollingZoomOptions(ScrollingAnimationMode animationMode, ScrollingSnapPointsMode snapPointsMode);

    ScrollingAnimationMode AnimationMode { get; set; };
    ScrollingSnapPointsMode SnapPointsMode { get; set; };
}
```

## Shared event argument classes between `ScrollView` and `ScrollPresenter`

```csharp
runtimeclass Microsoft.UI.Xaml.Controls.ScrollingScrollAnimationStartingEventArgs
{
    Microsoft.UI.Composition.CompositionAnimation Animation { get; set; };
    Windows.Foundation.Numerics.Vector2 StartPosition { get; };
    Windows.Foundation.Numerics.Vector2 EndPosition { get; };
    Int32 CorrelationId { get; };
}

runtimeclass Microsoft.UI.Xaml.Controls.ScrollingZoomAnimationStartingEventArgs
{
    Windows.Foundation.Numerics.Vector2 CenterPoint { get; };
    Single StartZoomFactor { get; };
    Single EndZoomFactor { get; };
    Microsoft.UI.Composition.CompositionAnimation Animation { get; set; };
    Int32 CorrelationId { get; };
}

runtimeclass Microsoft.UI.Xaml.Controls.ScrollingScrollCompletedEventArgs
{
    Int32 CorrelationId { get; };
}

runtimeclass Microsoft.UI.Xaml.Controls.ScrollingZoomCompletedEventArgs
{
    Int32 CorrelationId { get; };
}

runtimeclass Microsoft.UI.Xaml.Controls.ScrollingBringingIntoViewEventArgs
{
    ScrollingSnapPointsMode SnapPointsMode { get; set; };
    Microsoft.UI.Xaml.BringIntoViewRequestedEventArgs RequestEventArgs { get; };
    Double TargetHorizontalOffset { get; };
    Double TargetVerticalOffset { get; };
    Int32 CorrelationId { get; };
    Boolean Cancel { get; set; };
}

runtimeclass Microsoft.UI.Xaml.Controls.ScrollingAnchorRequestedEventArgs
{
    Windows.Foundation.Collections.IVector<Microsoft.UI.Xaml.UIElement> AnchorCandidates { get; };
    Microsoft.UI.Xaml.UIElement AnchorElement { get; set; };
}
```

_Spec note:_
_Mike: "ScrollingZoomAnimationStartingEventArgs.CenterPoint: Why Vector2 rather than Point?"_
_Mike: "BringingIntoView: Name this BringIntoViewRequested to match UIElement.BringIntoViewRequested?"_
_Mike: "ScrollingBringingIntoViewEventArgs: No explanation for this. Odd that it has a property of another args type."_

## Snap points related classes

```csharp
unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.SnapPointBase :
    Microsoft.UI.Xaml.DependencyObject
{
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollSnapPointBase
    : Microsoft.UI.Xaml.Controls.Primitives.SnapPointBase
{
    ScrollSnapPointsAlignment Alignment { get; };
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollSnapPoint
    : Microsoft.UI.Xaml.Controls.Primitives.ScrollSnapPointBase
{
    ScrollSnapPoint(
        Double snapPointValue,
        ScrollSnapPointsAlignment alignment);

    Double Value { get; };
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.RepeatedScrollSnapPoint
    : Microsoft.UI.Xaml.Controls.Primitives.ScrollSnapPointBase
{
    RepeatedScrollSnapPoint(
        Double offset,
        Double interval,
        Double start,
        Double end,
        ScrollSnapPointsAlignment alignment);

    Double Offset { get; };
    Double Interval { get; };
    Double Start { get; };
    Double End { get; };
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ZoomSnapPointBase
    : Microsoft.UI.Xaml.Controls.Primitives.SnapPointBase
{
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ZoomSnapPoint
    : Microsoft.UI.Xaml.Controls.Primitives.ZoomSnapPointBase
{
    ZoomSnapPoint(
        Double snapPointValue);

    Double Value { get; };
}

unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primitives.RepeatedZoomSnapPoint
    : Microsoft.UI.Xaml.Controls.Primitives.ZoomSnapPointBase
{
    RepeatedZoomSnapPoint(
        Double offset,
        Double interval,
        Double start,
        Double end);

    Double Offset { get; };
    Double Interval { get; };
    Double Start { get; };
    Double End { get; };
}
```

_Spec note:_
_Mike: "SnapPointBase: Why is this a DependencyObject?"_


## `IScrollController` interface and related classes

```csharp
interface Microsoft.UI.Xaml.Controls.Primitives.IScrollController
{
    Boolean AreInteractionsAllowed { get; };
    Boolean IsInteracting { get; };
    Boolean IsInteractionElementRailEnabled { get; };
    Microsoft.UI.Xaml.UIElement InteractionElement { get; };
    Microsoft.UI.Xaml.Controls.Orientation InteractionElementScrollOrientation { get; };

    void SetExpressionAnimationSources(
            Microsoft.UI.Composition.CompositionPropertySet propertySet,
            String minOffsetPropertyName,
            String maxOffsetPropertyName,
            String offsetPropertyName,
            String multiplierPropertyName);
    void SetScrollMode(
            Microsoft.UI.Xaml.Controls.ScrollingScrollMode scrollMode);
    void SetValues(
            Double minOffset,
            Double maxOffset,
            Double offset,
            Double viewport);
    Microsoft.UI.Composition.CompositionAnimation GetScrollAnimation(
            Int32 correlationId,
            Windows.Foundation.Numerics.Vector2 currentPosition,
            Microsoft.UI.Composition.CompositionAnimation defaultAnimation);
    void NotifyScrollCompleted(
            Int32 correlationId);

    event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerScrollToRequestedEventArgs> ScrollToRequested;
    event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerScrollByRequestedEventArgs> ScrollByRequested;
    event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerAddScrollVelocityRequestedEventArgs> AddScrollVelocityRequested;
    event Windows.Foundation.TypedEventHandler<IScrollController, ScrollControllerInteractionRequestedEventArgs> InteractionRequested;
    event Windows.Foundation.TypedEventHandler<IScrollController, Object> InteractionInfoChanged;
}

runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollControllerScrollToRequestedEventArgs
{
    ScrollControllerScrollToRequestedEventArgs(Double offset, Microsoft.UI.Xaml.Controls.ScrollingScrollOptions options);

    Double Offset { get; };
    Microsoft.UI.Xaml.Controls.ScrollingScrollOptions Options { get; };
    Int32 CorrelationId { get; set; };
}

runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollControllerScrollByRequestedEventArgs
{
    ScrollControllerScrollByRequestedEventArgs(Double offsetDelta, Microsoft.UI.Xaml.Controls.ScrollingScrollOptions options);

    Double OffsetDelta { get; };
    Microsoft.UI.Xaml.Controls.ScrollingScrollOptions Options { get; };
    Int32 CorrelationId { get; set; };
}

runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollControllerAddScrollVelocityRequestedEventArgs
{
    ScrollControllerAddScrollVelocityRequestedEventArgs(Single offsetVelocity, Windows.Foundation.IReference<Single> inertiaDecayRate);

    Single OffsetVelocity { get; };
    Windows.Foundation.IReference<Single> InertiaDecayRate { get; };
    Int32 CorrelationId { get; set; };
}

runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollControllerInteractionRequestedEventArgs
{
    ScrollControllerInteractionRequestedEventArgs(Microsoft.UI.Input.PointerPoint pointerPoint);

    Microsoft.UI.Input.PointerPoint PointerPoint { get; };
    Boolean Handled { get; set; };
}

runtimeclass Microsoft.UI.Xaml.Controls.Primitives.ScrollingViewChangeRequestedEventArgs
{
    Boolean IsAnimating { get; };
    Double TargetHorizontalOffset { get; };
    Double TargetVerticalOffset { get; };
    Single TargetZoomFactor { get; };
}
```

_Spec note:_
_Mike: "ScrollControllerScrollToRequestedEventArgs(Double offset, Microsoft.UI.Xaml.Controls.ScrollingScrollOptions options):
Why a constructor for the first two properties but not the CorrelationId? Is that not commonly used?
It might be easier to leave off the constructors; it's not that hard to set properties."_
_Mike: "Single OffsetVelocity { get; }: Is it valid for this to be negative?"_

## `ScrollPresenter` class

```csharp
[contentproperty("Content")]
unsealed runtimeclass Microsoft.UI.Xaml.Controls.Primittives.ScrollPresenter
    : Microsoft.UI.Xaml.FrameworkElement,
      Microsoft.UI.Xaml.Controls.IScrollAnchorProvider
{
    ScrollPresenter();

    Microsoft.UI.Xaml.Media.Brush Background { get; set; };
    Microsoft.UI.Xaml.UIElement Content { get; set; };
    Microsoft.UI.Composition.CompositionPropertySet ExpressionAnimationSources { get; };
    Double HorizontalOffset { get; };
    Double VerticalOffset { get; };
    Single ZoomFactor { get; };
    Double ExtentWidth { get; };
    Double ExtentHeight { get; };
    Double ViewportWidth { get; };
    Double ViewportHeight { get; };
    Double ScrollableWidth { get; };
    Double ScrollableHeight { get; };
    Microsoft.UI.Xaml.Controls.ScrollingContentOrientation ContentOrientation { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingChainMode HorizontalScrollChainMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingChainMode VerticalScrollChainMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingRailMode HorizontalScrollRailMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingRailMode VerticalScrollRailMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingScrollMode HorizontalScrollMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingScrollMode VerticalScrollMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingChainMode ZoomChainMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingZoomMode ZoomMode { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingInputKinds IgnoredInputKinds { get; set; };
    Double MinZoomFactor { get; set; };
    Double MaxZoomFactor { get; set; };
    Microsoft.UI.Xaml.Controls.ScrollingInteractionState State { get; };
    IScrollController HorizontalScrollController { get; set; };
    IScrollController VerticalScrollController { get; set; };
    Double HorizontalAnchorRatio { get; set; };
    Double VerticalAnchorRatio { get; set; };
    Windows.Foundation.Collections.IVector<ScrollSnapPointBase> HorizontalSnapPoints { get; };
    Windows.Foundation.Collections.IVector<ScrollSnapPointBase> VerticalSnapPoints { get; };
    Windows.Foundation.Collections.IVector<ZoomSnapPointBase> ZoomSnapPoints { get; };
    [method_name("ScrollTo")]
    Int32 ScrollTo(
        Double horizontalOffset,
        Double verticalOffset);
    [method_name("ScrollToWithOptions")]
    Int32 ScrollTo(
        Double horizontalOffset,
        Double verticalOffset,
        Microsoft.UI.Xaml.Controls.ScrollingScrollOptions options);
    [method_name("ScrollBy")]
    Int32 ScrollBy(
        Double horizontalOffsetDelta,
        Double verticalOffsetDelta);
    [method_name("ScrollByWithOptions")]
    Int32 ScrollBy(
        Double horizontalOffsetDelta,
        Double verticalOffsetDelta,
        Microsoft.UI.Xaml.Controls.ScrollingScrollOptions options);
    Int32 AddScrollVelocity(
        Windows.Foundation.Numerics.Vector2 offsetsVelocity,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> inertiaDecayRate);
    [method_name("ZoomTo")]
    Int32 ZoomTo(
        Single zoomFactor,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> centerPoint);
    [method_name("ZoomToWithOptions")]
    Int32 ZoomTo(
        Single zoomFactor,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> centerPoint,
        Microsoft.UI.Xaml.Controls.ScrollingZoomOptions options);
    [method_name("ZoomBy")]
    Int32 ZoomBy(
        Single zoomFactorDelta,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> centerPoint);
    [method_name("ZoomByWithOptions")]
    Int32 ZoomBy(
        Single zoomFactorDelta,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> centerPoint,
        Microsoft.UI.Xaml.Controls.ScrollingZoomOptions options);
    Int32 AddZoomVelocity(
        Single zoomFactorVelocity,
        Windows.Foundation.IReference<Windows.Foundation.Numerics.Vector2> centerPoint,
        Windows.Foundation.IReference<Single> inertiaDecayRate);

    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Object> ExtentChanged;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Object> StateChanged;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Object> ViewChanged;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingScrollAnimationStartingEventArgs> ScrollAnimationStarting;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingZoomAnimationStartingEventArgs> ZoomAnimationStarting;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingScrollCompletedEventArgs> ScrollCompleted;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingZoomCompletedEventArgs> ZoomCompleted;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingBringingIntoViewEventArgs> BringingIntoView;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, Microsoft.UI.Xaml.Controls.ScrollingAnchorRequestedEventArgs> AnchorRequested;
    event Windows.Foundation.TypedEventHandler<ScrollPresenter, MU_XCP_NAMESPACE.ScrollingViewChangeRequestedEventArgs> ViewChangeRequested;

    static Microsoft.UI.Xaml.DependencyProperty BackgroundProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty ContentProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty ContentOrientationProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty HorizontalScrollChainModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty VerticalScrollChainModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty HorizontalScrollRailModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty VerticalScrollRailModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty HorizontalScrollModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty VerticalScrollModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty ZoomChainModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty ZoomModeProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty IgnoredInputKindsProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty MinZoomFactorProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty MaxZoomFactorProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty HorizontalAnchorRatioProperty { get; };
    static Microsoft.UI.Xaml.DependencyProperty VerticalAnchorRatioProperty { get; };
}
```

_Spec note:_
_Mike: "Microsoft.UI.Composition.CompositionPropertySet ExpressionAnimationSources { get; }:
No explanation of what this is (it's fine to doc it as a comment)"_
_Mike: "Double ScrollableWidth { get; }: See
[ScrollViewer.ScrollableWidth](https://docs.microsoft.com/uwp/api/Windows.UI.Xaml.Controls.ScrollViewer.ScrollableWidth)"_
_Mike: "ScrollingInteractionState State { get; }: "State" is too ambiguous,
should be either ScrollingInterationState or InteractionState."_
_Mike: "ScrollCompleted, ZoomCompleted, BringingIntoView, AnchorRequested, ViewChangeRequested:
Is ScrollView going to listen to all of these events anyway? Would it be easier to make it a
callback interface? We usually prefer events to that, but if the use case is to listen to everything,
then it's more efficient."_

# Sample IScrollController implementations

_Spec note:_
_Mike: "These last samples are great, but long and I don't want reviewers to feel compelled to
provide feedback on this much content. Also I think this would go into the samples repo rather
than the docs. Could you keep them but put them in the appendix?"_

## IScrollController implementation without interaction element

The ScrollBarController class below is a sample implementation of the IScrollController interface
which uses a `ScrollBar` control internally. Its InteractionElement property does not return a UIElement,
so it does not support UI-thread-independent scrolling of the `ScrollPresenter`'s content.

```csharp
public class ScrollBarController : IScrollController
{
    private ScrollBar scrollBar = null;
    private ScrollingScrollMode scrollMode = ScrollingScrollMode.Disabled;
    private int lastOffsetChangeCorrelationIdForScrollTo = -1;
    private int lastOffsetChangeCorrelationIdForScrollBy = -1;
    private int lastOffsetChangeCorrelationIdForAddScrollVelocity = -1;
    private int operationsCount = 0;
    private double lastScrollBarValue = 0.0;
    private double lastOffset = 0.0;

    public event TypedEventHandler<IScrollController, ScrollControllerScrollToRequestedEventArgs> ScrollToRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerScrollByRequestedEventArgs> ScrollByRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerAddScrollVelocityRequestedEventArgs> AddScrollVelocityRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerInteractionRequestedEventArgs> InteractionRequested;
    public event TypedEventHandler<IScrollController, object> InteractionInfoChanged;

    public ScrollBarController(ScrollBar scrollBar)
    {
        this.scrollBar = scrollBar;

        scrollBar.SmallChange = 16.0;
        scrollBar.Scroll += ScrollBarScroll;
        scrollBar.RegisterPropertyChangedCallback(Control.IsEnabledProperty, new DependencyPropertyChangedCallback(ScrollBarPropertyChanged));
    }

    public bool AreInteractionsAllowed
    {
        get;
        private set;
    }

    public bool IsInteracting
    {
        get;
        private set;
    }

    public bool IsInteractionElementRailEnabled
    {
        get
        {
            // Unused because InteractionElement returns null.
            return false;
        }
    }

    public UIElement InteractionElement
    {
        get
        {
            // This IScrollController implementation has no touch-manipulatable element.
            return null;
        }
    }

    public Orientation InteractionElementScrollOrientation
    {
        get
        {
            return scrollBar.Orientation;
        }
    }

    public void SetExpressionAnimationSources(
        CompositionPropertySet propertySet,
        string minOffsetPropertyName,
        string maxOffsetPropertyName,
        string offsetPropertyName,
        string multiplierPropertyName)
    {
        // Unused because InteractionElement returns null.
    }

    public void SetScrollMode(ScrollingScrollMode scrollMode)
    {
        this.scrollMode = scrollMode;
        UpdateAreInteractionsAllowed();
    }

    public void SetValues(
        double minOffset,
        double maxOffset,
        double offset,
        double viewport)
    {
        if (maxOffset < minOffset)
        {
            throw new ArgumentOutOfRangeException("maxOffset cannot be smaller than minOffset.");
        }

        if (viewport < 0.0)
        {
            throw new ArgumentOutOfRangeException("viewport cannot be negative.");
        }

        offset = Math.Max(minOffset, offset);
        offset = Math.Min(maxOffset, offset);
        lastOffset = offset;

        if (minOffset < scrollBar.Minimum)
        {
            scrollBar.Minimum = minOffset;
        }

        if (maxOffset > scrollBar.Maximum)
        {
            scrollBar.Maximum = maxOffset;
        }

        if (minOffset != scrollBar.Minimum)
        {
            scrollBar.Minimum = minOffset;
        }

        if (maxOffset != scrollBar.Maximum)
        {
            scrollBar.Maximum = maxOffset;
        }

        // Default amount to scroll when hitting the SmallIncrement/SmallDecrement buttons: 1/8 of the viewport size.
        // This amount can be overridden by setting the ScrollBar.SmallChange property to something else than double.NaN.
        const double s_defaultViewportToSmallChangeRatio = 8.0;

        scrollBar.ViewportSize = viewport;
        scrollBar.LargeChange = viewport;
        scrollBar.SmallChange = Math.Max(1.0, viewport / s_defaultViewportToSmallChangeRatio);

        // The ScrollBar Value is only updated when there is no operation in progress.
        if (operationsCount == 0 || scrollBar.Value < minOffset || scrollBar.Value > maxOffset)
        {
            scrollBar.Value = offset;
            lastScrollBarValue = offset;
        }

        // Potentially changed ScrollBar.Minimum / ScrollBar.Maximum value(s) may have an effect
        // on the read-only IScrollController.AreInteractionsAllowed property.
        UpdateAreInteractionsAllowed();
    }

    public CompositionAnimation GetScrollAnimation(
        int correlationId,
        Vector2 currentPosition,
        CompositionAnimation defaultAnimation)
    {
        return null;
    }

    public void NotifyScrollCompleted(int correlationId)
    {
        operationsCount--;

        if (operationsCount == 0 && scrollBar.Value != lastOffset)
        {
            scrollBar.Value = lastOffset;
            lastScrollBarValue = lastOffset;
        }
    }

    private void ScrollBarScroll(object sender, ScrollEventArgs e)
    {
        ScrollEventType scrollEventType = e.ScrollEventType;

        if (scrollMode == ScrollingScrollMode.Disabled && scrollEventType != ScrollEventType.ThumbPosition)
        {
            // This ScrollBar is not interactive. Restore its previous Value.
            scrollBar.Value = lastScrollBarValue;
            return;
        }

        switch (scrollEventType)
        {
            case ScrollEventType.First:
            case ScrollEventType.Last:
                {
                    break;
                }
            case ScrollEventType.EndScroll:
                {
                    if (IsInteracting)
                    {
                        IsInteracting = false;
                        RaiseInteractionInfoChanged();
                    }
                    break;
                }
            case ScrollEventType.LargeDecrement:
            case ScrollEventType.LargeIncrement:
            case ScrollEventType.SmallDecrement:
            case ScrollEventType.SmallIncrement:
            case ScrollEventType.ThumbPosition:
            case ScrollEventType.ThumbTrack:
                {
                    if (scrollEventType == ScrollEventType.ThumbTrack)
                    {
                        if (!IsInteracting)
                        {
                            IsInteracting = true;
                            RaiseInteractionInfoChanged();
                        }
                    }

                    bool offsetChangeRequested = false;

                    if (scrollEventType == ScrollEventType.ThumbPosition ||
                        scrollEventType == ScrollEventType.ThumbTrack)
                    {
                        offsetChangeRequested = RaiseScrollToRequested(e.NewValue);
                    }
                    else
                    {
                        double offsetDelta = 0.0;

                        switch (scrollEventType)
                        {
                            case ScrollEventType.LargeDecrement:
                                offsetDelta = -Math.Min(lastScrollBarValue - scrollBar.Minimum, scrollBar.LargeChange);
                                break;
                            case ScrollEventType.LargeIncrement:
                                offsetDelta = Math.Min(scrollBar.Maximum - lastScrollBarValue, scrollBar.LargeChange);
                                break;
                            case ScrollEventType.SmallDecrement:
                                offsetDelta = -Math.Min(lastScrollBarValue - scrollBar.Minimum, scrollBar.SmallChange);
                                break;
                            case ScrollEventType.SmallIncrement:
                                offsetDelta = Math.Min(scrollBar.Maximum - lastScrollBarValue, scrollBar.SmallChange);
                                break;
                        }

                        const double s_minMaxEpsilon = 0.001;

                        // When the requested Value is near the Mininum or Maximum, include a little additional velocity
                        // to ensure the extreme value is reached.
                        if (e.NewValue - scrollBar.Minimum < s_minMaxEpsilon)
                        {
                            offsetDelta -= s_minMaxEpsilon;
                        }
                        else if (scrollBar.Maximum - e.NewValue < s_minMaxEpsilon)
                        {
                            offsetDelta += s_minMaxEpsilon;
                        }

                        if (new UISettings().AnimationsEnabled)
                        {
                            offsetChangeRequested = RaiseAddScrollVelocityRequested(offsetDelta);
                        }
                        else
                        {
                            offsetChangeRequested = RaiseScrollByRequested(offsetDelta);
                        }
                    }

                    if (!offsetChangeRequested)
                    {
                        // This request could not be requested, restore the previous Value.
                        scrollBar.Value = lastScrollBarValue;
                    }
                    break;
                }
        }

        lastScrollBarValue = scrollBar.Value;
    }

    private void ScrollBarPropertyChanged(DependencyObject sender, DependencyProperty e)
    {
        if (e == Control.IsEnabledProperty)
        {
            // Potentially changed ScrollBar.Minimum / ScrollBar.Maximum value(s) may have an effect
            // on the read-only IScrollController.AreInteractionsAllowed property.
            UpdateAreInteractionsAllowed();
        }
    }

    private void UpdateAreInteractionsAllowed()
    {
        bool oldAreInteractionsAllowed = AreInteractionsAllowed;

        AreInteractionsAllowed =
            scrollBar.IsEnabled &&
            scrollBar.Maximum > scrollBar.Minimum &&
            scrollMode != ScrollingScrollMode.Disabled;

        if (oldAreInteractionsAllowed != AreInteractionsAllowed)
        {
            RaiseInteractionInfoChanged();
        }
    }

    private void RaiseInteractionInfoChanged()
    {
        if (InteractionInfoChanged != null)
        {
            InteractionInfoChanged(this, null);
        }
    }

    private bool RaiseScrollToRequested(double offset)
    {
        if (ScrollToRequested == null)
        {
            return false;
        }

        ScrollingScrollOptions options = new ScrollingScrollOptions(ScrollingAnimationMode.Disabled, ScrollingSnapPointsMode.Ignore);
        ScrollControllerScrollToRequestedEventArgs scrollToRequestedEventArgs = new ScrollControllerScrollToRequestedEventArgs(offset, options);

        ScrollToRequested(this, scrollToRequestedEventArgs);

        int correlationId = scrollToRequestedEventArgs.CorrelationId;

        // Only increment operationsCount when the returned OffsetsChangeCorrelationId represents a new request that was not coalesced with a pending request.
        if correlationId != -1 && correlationId != lastOffsetChangeCorrelationIdForScrollTo)
        {
            lastOffsetChangeCorrelationIdForScrollTo = correlationId;
            operationsCount++;
            return true;
        }

        return false;
    }

    private bool RaiseScrollByRequested(double offsetDelta)
    {
        if (ScrollToRequested == null)
        {
            return false;
        }

        ScrollingScrollOptions options = new ScrollingScrollOptions(ScrollingAnimationMode.Disabled, ScrollingSnapPointsMode.Ignore);
        ScrollControllerScrollByRequestedEventArgs scrollByRequestedEventArgs = new ScrollControllerScrollByRequestedEventArgs(offsetDelta, options);

        ScrollByRequested(this, scrollByRequestedEventArgs);

        int correlationId = scrollByRequestedEventArgs.CorrelationId;

        // Only increment operationsCount when the returned OffsetsChangeCorrelationId represents a new request that was not coalesced with a pending request.
        if (correlationId != -1 && correlationId != lastOffsetChangeCorrelationIdForScrollBy)
        {
            lastOffsetChangeCorrelationIdForScrollBy = correlationId;
            operationsCount++;
            return true;
        }

        return false;
    }

    private bool RaiseAddScrollVelocityRequested(double offsetDelta)
    {
        if (AddScrollVelocityRequested == null)
        {
            return false;
        }

        // Minimum initial velocity required by InteractionTracker.TryUpdatePositionWithAdditionalVelocity to affect the Position.
        const double s_minimumVelocity = 30.0;

        // Inertia decay rate for SmallChange / LargeChange animated Value changes.
        const float s_inertiaDecayRate = 0.9995f;

        // Approximate additional velocity required with decay s_inertiaDecayRate to move offset by one pixel.
        const double s_velocityNeededPerPixel = 7.6;

        double offsetVelocity = operationsCount == 0 ? s_minimumVelocity : 0.0;

        if (offsetDelta < 0.0)
        {
            offsetVelocity *= -1;
        }
        offsetVelocity += offsetDelta * s_velocityNeededPerPixel;

        ScrollControllerAddScrollVelocityRequestedEventArgs addScrollVelocityRequestedEventArgs = new ScrollControllerAddScrollVelocityRequestedEventArgs((float)offsetVelocity, s_inertiaDecayRate);

        AddScrollVelocityRequested(this, addScrollVelocityRequestedEventArgs);

        int correlationId = addScrollVelocityRequestedEventArgs.CorrelationId;

        // Only increment operationsCount when the returned OffsetsChangeCorrelationId represents a new request that was not coalesced with a pending request.
        if (correlationId != -1 && correlationId != lastOffsetChangeCorrelationIdForAddScrollVelocity)
        {
            lastOffsetChangeCorrelationIdForAddScrollVelocity = correlationId;
            operationsCount++;
            return true;
        }

        return false;
    }
}
```

## IScrollController implementation with interaction element

The CompositionScrollController class below is a sample implementation of the IScrollController interface which
supports UI-thread-independent scrolling of the `ScrollPresenter`'s content by exposing a pannable thumb.

```csharp
public sealed class CompositionScrollController : Control, IScrollController
{
    private const float SmallChangeAdditionalVelocity = 144.0f;
    private const float SmallChangeInertiaDecayRate = 0.975f;

    private Dictionary<int, double> operations = new Dictionary<int, double>();
    private FrameworkElement interactionFrameworkElement = null;
    private UIElement horizontalGrid = null;
    private UIElement verticalGrid = null;
    private UIElement horizontalThumb = null;
    private UIElement verticalThumb = null;
    private RepeatButton horizontalDecrementRepeatButton = null;
    private RepeatButton verticalDecrementRepeatButton = null;
    private RepeatButton horizontalIncrementRepeatButton = null;
    private RepeatButton verticalIncrementRepeatButton = null;
    private Visual interactionVisual = null;
    private CompositionPropertySet expressionAnimationSources = null;
    private ExpressionAnimation thumbOffsetAnimation = null;
    private Orientation orientation = Orientation.Vertical;
    private ScrollingScrollMode scrollMode = ScrollingScrollMode.Disabled;
    private bool isThumbDragged = false;
    private double minOffset = 0.0;
    private double maxOffset = 0.0;
    private double offset = 0.0;
    private double offsetTarget = 0.0;
    private double viewport = 0.0;
    private double preManipulationThumbOffset = 0.0;
    private string minOffsetPropertyName;
    private string maxOffsetPropertyName;
    private string offsetPropertyName;
    private string multiplierPropertyName;

    public CompositionScrollController()
    {
        this.DefaultStyleKey = typeof(CompositionScrollController);
        OverriddenOffsetChangeDuration = TimeSpan.MinValue;
        IsEnabledChanged += CompositionScrollController_IsEnabledChanged;
        SizeChanged += CompositionScrollController_SizeChanged;
    }

    protected override void OnApplyTemplate()
    {
        UnhookHandlers();

        base.OnApplyTemplate();

        horizontalGrid = GetTemplateChild("HorizontalGrid") as UIElement;
        verticalGrid = GetTemplateChild("VerticalGrid") as UIElement;
        horizontalThumb = GetTemplateChild("HorizontalThumb") as UIElement;
        verticalThumb = GetTemplateChild("VerticalThumb") as UIElement;
        horizontalDecrementRepeatButton = GetTemplateChild("HorizontalDecrementRepeatButton") as RepeatButton;
        verticalDecrementRepeatButton = GetTemplateChild("VerticalDecrementRepeatButton") as RepeatButton;
        horizontalIncrementRepeatButton = GetTemplateChild("HorizontalIncrementRepeatButton") as RepeatButton;
        verticalIncrementRepeatButton = GetTemplateChild("VerticalIncrementRepeatButton") as RepeatButton;

        UpdateOrientation();
    }

    public TimeSpan OverriddenOffsetChangeDuration
    {
        get;
        set;
    }

    public Orientation Orientation
    {
        get
        {
            return orientation;
        }
        set
        {
            if (orientation != value)
            {
                UnhookHandlers();
                StopThumbAnimation(orientation);
                orientation = value;
                UpdateOrientation();
            }
        }
    }

    public void SetExpressionAnimationSources(
        CompositionPropertySet propertySet,
        string minOffsetPropertyName,
        string maxOffsetPropertyName,
        string offsetPropertyName,
        string multiplierPropertyName)
    {
        expressionAnimationSources = propertySet;
        if (expressionAnimationSources != null)
        {
            this.minOffsetPropertyName = minOffsetPropertyName.Trim();
            this.maxOffsetPropertyName = maxOffsetPropertyName.Trim();
            this.offsetPropertyName = offsetPropertyName.Trim();
            this.multiplierPropertyName = multiplierPropertyName.Trim();

            UpdateInteractionElementScrollMultiplier();

            if (thumbOffsetAnimation == null)
            {
                EnsureThumbAnimation();
                UpdateThumbExpression();
                StartThumbAnimation(Orientation);
            }
        }
        else
        {
            minOffsetPropertyName =
            maxOffsetPropertyName =
            offsetPropertyName =
            multiplierPropertyName = string.Empty;
            thumbOffsetAnimation = null;
            StopThumbAnimation(Orientation);
        }
    }

    public void SetScrollMode(ScrollingScrollMode scrollMode)
    {
        this.scrollMode = scrollMode;
        UpdateAreInteractionsAllowed();
    }

    public void SetValues(double minOffset, double maxOffset, double offset, double viewport)
    {
        if (maxOffset < minOffset)
        {
            throw new ArgumentOutOfRangeException("maxOffset");
        }

        if (viewport < 0.0)
        {
            throw new ArgumentOutOfRangeException("viewport");
        }

        offset = Math.Max(minOffset, offset);
        offset = Math.Min(maxOffset, offset);

        if (operations.Count == 0)
        {
            offsetTarget = offset;
        }
        else
        {
            offsetTarget = Math.Max(minOffset, offsetTarget);
            offsetTarget = Math.Min(maxOffset, offsetTarget);
        }

        bool updateInteractionFrameworkElementSize =
            this.minOffset != minOffset ||
            this.maxOffset != maxOffset ||
            this.viewport != viewport;

        this.minOffset = minOffset;
        this.offset = offset;
        this.maxOffset = maxOffset;
        this.viewport = viewport;

        if (updateInteractionFrameworkElementSize && !UpdateInteractionFrameworkElementSize())
        {
            UpdateInteractionElementScrollMultiplier();
        }
    }

    // Builds a custom Vector3KeyFrameAnimation animation that the ScrollPresenter applies when an animated offset change
    // is requested by the CompositionScrollController.
    public CompositionAnimation GetScrollAnimation(
        int correlationId,
        Vector2 currentPosition,
        CompositionAnimation defaultAnimation)
    {
        Vector3KeyFrameAnimation stockKeyFrameAnimation = defaultAnimation as Vector3KeyFrameAnimation;

        if (stockKeyFrameAnimation != null)
        {
            Vector3KeyFrameAnimation customKeyFrameAnimation = stockKeyFrameAnimation;
            float positionTarget = (float)operations[correlationId];
            float otherOrientationPosition = orientation == Orientation.Horizontal ? currentPosition.Y : currentPosition.X;

            customKeyFrameAnimation = stockKeyFrameAnimation.Compositor.CreateVector3KeyFrameAnimation();
            float deltaPosition = (float)(positionTarget - offset);

            CubicBezierEasingFunction cubicBezierStart = stockKeyFrameAnimation.Compositor.CreateCubicBezierEasingFunction(
                new Vector2(1.0f, 0.0f),
                new Vector2(1.0f, 0.0f));

            StepEasingFunction step = stockKeyFrameAnimation.Compositor.CreateStepEasingFunction(1);

            CubicBezierEasingFunction cubicBezierEnd = stockKeyFrameAnimation.Compositor.CreateCubicBezierEasingFunction(
                new Vector2(0.0f, 1.0f),
                new Vector2(0.0f, 1.0f));

            if (orientation == Orientation.Horizontal)
            {
                customKeyFrameAnimation.InsertKeyFrame(
                    0.499999f,
                    new Vector3(positionTarget - 0.9f * deltaPosition, otherOrientationPosition, 0.0f),
                    cubicBezierStart);
                customKeyFrameAnimation.InsertKeyFrame(
                    0.5f,
                    new Vector3(positionTarget - 0.1f * deltaPosition, otherOrientationPosition, 0.0f),
                    step);
                customKeyFrameAnimation.InsertKeyFrame(
                    1.0f,
                    new Vector3(positionTarget, otherOrientationPosition, 0.0f),
                    cubicBezierEnd);
            }
            else
            {
                customKeyFrameAnimation.InsertKeyFrame(
                    0.499999f,
                    new Vector3(otherOrientationPosition, positionTarget - 0.9f * deltaPosition, 0.0f),
                    cubicBezierStart);
                customKeyFrameAnimation.InsertKeyFrame(
                    0.5f,
                    new Vector3(otherOrientationPosition, positionTarget - 0.1f * deltaPosition, 0.0f),
                    step);
                customKeyFrameAnimation.InsertKeyFrame(
                    1.0f,
                    new Vector3(otherOrientationPosition, positionTarget, 0.0f),
                    cubicBezierEnd);
            }
            customKeyFrameAnimation.Duration = stockKeyFrameAnimation.Duration;

            if (OverriddenOffsetChangeDuration != TimeSpan.MinValue)
            {
                customKeyFrameAnimation.Duration = OverriddenOffsetChangeDuration;
            }

            return customKeyFrameAnimation;
        }

        return null;
    }

    public void NotifyScrollCompleted(int correlationId)
    {
        if (operations.ContainsKey(correlationId))
        {
            operations.Remove(correlationId);
        }
    }

    public bool AreInteractionsAllowed
    {
        get;
        private set;
    }

    public bool IsInteracting
    {
        get;
        private set;
    }

    public bool IsInteractionElementRailEnabled
    {
        get
        {
            return true;
        }
    }

    public UIElement InteractionElement
    {
        get
        {
            return (IsEnabled && interactionFrameworkElement != null && interactionFrameworkElement.Parent != null) ? interactionFrameworkElement.Parent as UIElement : null;
        }
    }

    public Orientation InteractionElementScrollOrientation
    {
        get
        {
            return Orientation;
        }
    }

    private float InteractionElementScrollMultiplier
    {
        get
        {
            if (interactionFrameworkElement != null)
            {
                interactionFrameworkElement.UpdateLayout();

                double parentDimension = 0.0;
                double interactionFrameworkElementDim = Orientation == Orientation.Horizontal ? interactionFrameworkElement.ActualWidth : interactionFrameworkElement.ActualHeight;
                FrameworkElement parent = interactionFrameworkElement.Parent as FrameworkElement;
                if (parent != null)
                {
                    parentDimension = Orientation == Orientation.Horizontal ? parent.ActualWidth : parent.ActualHeight;
                }
                if (parentDimension != interactionFrameworkElementDim)
                {
                    return (float)((maxOffset - minOffset) / (interactionFrameworkElementDim - parentDimension));
                }
            }

            return 0.0f;
        }
    }

    public event TypedEventHandler<IScrollController, ScrollControllerInteractionRequestedEventArgs> InteractionRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerScrollToRequestedEventArgs> ScrollToRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerScrollByRequestedEventArgs> ScrollByRequested;
    public event TypedEventHandler<IScrollController, ScrollControllerAddScrollVelocityRequestedEventArgs> AddScrollVelocityRequested;
    public event TypedEventHandler<IScrollController, Object> InteractionInfoChanged;

    public int ScrollTo(double offset, ScrollingAnimationMode animationMode)
    {
        return RaiseScrollToRequested(offset, animationMode);
    }

    public int ScrollBy(double offsetDelta, ScrollingAnimationMode animationMode)
    {
        return RaiseScrollByRequested(offsetDelta, animationMode);
    }

    public int AddScrollVelocity(float offsetVelocity, float? inertiaDecayRate)
    {
        return RaiseAddScrollVelocityRequested(offsetVelocity, inertiaDecayRate);
    }

    private void RaiseInteractionInfoChanged()
    {
        if (InteractionInfoChanged != null)
        {
            InteractionInfoChanged(this, null);
        }
    }

    private void RaiseInteractionRequested(PointerPoint pointerPoint)
    {
        if (InteractionRequested != null)
        {
            ScrollControllerInteractionRequestedEventArgs e = new ScrollControllerInteractionRequestedEventArgs(pointerPoint);
            InteractionRequested(this, e);
        }
    }

    private int RaiseScrollToRequested(double offset, ScrollingAnimationMode animationMode)
    {
        if (ScrollToRequested != null)
        {
            ScrollControllerScrollToRequestedEventArgs e =
                new ScrollControllerScrollToRequestedEventArgs(
                    offset,
                    new ScrollingScrollOptions(animationMode, ScrollingSnapPointsMode.Ignore));
            ScrollToRequested(this, e);
            return e.CorrelationId;
        }

        return -1;
    }

    private int RaiseScrollByRequested(double offsetDelta, ScrollingAnimationMode animationMode)
    {
        if (ScrollByRequested != null)
        {
            ScrollControllerScrollByRequestedEventArgs e =
                new ScrollControllerScrollByRequestedEventArgs(
                    offsetDelta,
                    new ScrollingScrollOptions(animationMode, ScrollingSnapPointsMode.Ignore));
            ScrollByRequested(this, e);
            return e.CorrelationId;
        }

        return -1;
    }

    private int RaiseAddScrollVelocityRequested(float offsetVelocity, float? inertiaDecayRate)
    {
        if (AddScrollVelocityRequested != null)
        {
            ScrollControllerAddScrollVelocityRequestedEventArgs e =
                new ScrollControllerAddScrollVelocityRequestedEventArgs(
                    offsetVelocity,
                    inertiaDecayRate);
            AddScrollVelocityRequested(this, e);
            return e.CorrelationId;
        }

        return -1;
    }

    private void InteractionFrameworkElement_PointerPressed(object sender, Microsoft.UI.Xaml.Input.PointerRoutedEventArgs e)
    {
        switch (e.Pointer.PointerDeviceType)
        {
            case Microsoft.UI.Input.PointerDeviceType.Touch:
            case Microsoft.UI.Input.PointerDeviceType.Pen:
                RaiseInteractionRequested(e.GetCurrentPoint(null));
                break;
            case Microsoft.UI.Input.PointerDeviceType.Mouse:
                isThumbDragged = true;
                if (!IsInteracting)
                {
                    IsInteracting = true;
                    RaiseInteractionInfoChanged();
                }
                break;
        }
    }

    private void InteractionFrameworkElement_ManipulationStarting(object sender, ManipulationStartingRoutedEventArgs e)
    {
        if (isThumbDragged)
        {
            preManipulationThumbOffset = Orientation == Orientation.Horizontal ? HorizontalThumbOffset : VerticalThumbOffset;
        }
    }

    private void InteractionFrameworkElement_ManipulationDelta(object sender, ManipulationDeltaRoutedEventArgs e)
    {
        if (isThumbDragged)
        {
            double targetThumbOffset = preManipulationThumbOffset + (Orientation == Orientation.Horizontal ? e.Cumulative.Translation.X : e.Cumulative.Translation.Y);
            double scrollPresenterOffset = ScrollPresenterOffsetFromThumbOffset(targetThumbOffset);

            int offsetChangeCorrelationId = RaiseScrollToRequested(
                scrollPresenterOffset, ScrollingAnimationMode.Disabled);
        }
    }

    private void InteractionFrameworkElement_ManipulationCompleted(object sender, ManipulationCompletedRoutedEventArgs e)
    {
        if (isThumbDragged)
        {
            isThumbDragged = false;
            if (IsInteracting)
            {
                IsInteracting = false;
                RaiseInteractionInfoChanged();
            }
        }
    }

    private void UnhookHandlers()
    {
        if (horizontalDecrementRepeatButton != null)
        {
            horizontalDecrementRepeatButton.Click -= DecrementRepeatButton_Click;
        }

        if (horizontalIncrementRepeatButton != null)
        {
            horizontalIncrementRepeatButton.Click -= IncrementRepeatButton_Click;
        }

        if (verticalDecrementRepeatButton != null)
        {
            verticalDecrementRepeatButton.Click -= DecrementRepeatButton_Click;
        }

        if (verticalIncrementRepeatButton != null)
        {
            verticalIncrementRepeatButton.Click -= IncrementRepeatButton_Click;
        }

        if (interactionFrameworkElement != null)
        {
            interactionFrameworkElement.PointerPressed -= InteractionFrameworkElement_PointerPressed;
            interactionFrameworkElement.ManipulationStarting -= InteractionFrameworkElement_ManipulationStarting;
            interactionFrameworkElement.ManipulationDelta -= InteractionFrameworkElement_ManipulationDelta;
            interactionFrameworkElement.ManipulationCompleted -= InteractionFrameworkElement_ManipulationCompleted;

            FrameworkElement parent = interactionFrameworkElement.Parent as FrameworkElement;
            if (parent != null)
            {
                parent.PointerPressed -= Parent_PointerPressed;
            }
        }
    }

    private void UpdateAreInteractionsAllowed()
    {
        bool oldAreInteractionsAllowed = AreInteractionsAllowed;

        AreInteractionsAllowed = scrollMode != ScrollingScrollMode.Disabled && IsEnabled;

        if (oldAreInteractionsAllowed != AreInteractionsAllowed)
        {
            RaiseInteractionInfoChanged();
        }
    }

    private void UpdateOrientation()
    {
        if (Orientation == Orientation.Horizontal)
        {
            if (horizontalGrid != null)
                horizontalGrid.Visibility = Visibility.Visible;
            if (verticalGrid != null)
                verticalGrid.Visibility = Visibility.Collapsed;
            interactionFrameworkElement = horizontalThumb as FrameworkElement;
            if (interactionFrameworkElement != null)
            {
                interactionFrameworkElement.ManipulationMode = ManipulationModes.TranslateX;
            }

            if (horizontalDecrementRepeatButton != null)
            {
                horizontalDecrementRepeatButton.Click += DecrementRepeatButton_Click;
            }

            if (horizontalIncrementRepeatButton != null)
            {
                horizontalIncrementRepeatButton.Click += IncrementRepeatButton_Click;
            }
        }
        else
        {
            if (verticalGrid != null)
                verticalGrid.Visibility = Visibility.Visible;
            if (horizontalGrid != null)
                horizontalGrid.Visibility = Visibility.Collapsed;
            interactionFrameworkElement = verticalThumb as FrameworkElement;
            if (interactionFrameworkElement != null)
            {
                interactionFrameworkElement.ManipulationMode = ManipulationModes.TranslateY;
            }

            if (verticalDecrementRepeatButton != null)
            {
                verticalDecrementRepeatButton.Click += DecrementRepeatButton_Click;
            }

            if (verticalIncrementRepeatButton != null)
            {
                verticalIncrementRepeatButton.Click += IncrementRepeatButton_Click;
            }
        }

        if (interactionFrameworkElement != null)
        {
            interactionVisual = ElementCompositionPreview.GetElementVisual(interactionFrameworkElement);
            ElementCompositionPreview.SetIsTranslationEnabled(interactionFrameworkElement, true);
            StartThumbAnimation(Orientation);

            interactionFrameworkElement.PointerPressed += InteractionFrameworkElement_PointerPressed;
            interactionFrameworkElement.ManipulationStarting += InteractionFrameworkElement_ManipulationStarting;
            interactionFrameworkElement.ManipulationDelta += InteractionFrameworkElement_ManipulationDelta;
            interactionFrameworkElement.ManipulationCompleted += InteractionFrameworkElement_ManipulationCompleted;

            FrameworkElement parent = interactionFrameworkElement.Parent as FrameworkElement;
            if (parent != null)
            {
                parent.IsTapEnabled = true;
                parent.PointerPressed += Parent_PointerPressed;
            }
        }
        else
        {
            interactionVisual = null;
        }

        RaiseInteractionInfoChanged();
    }

    private void UpdateInteractionElementScrollMultiplier()
    {
        if (expressionAnimationSources != null && !string.IsNullOrWhiteSpace(multiplierPropertyName))
        {
            float interactionVisualScrollMultiplier = InteractionElementScrollMultiplier;

            expressionAnimationSources.InsertScalar(multiplierPropertyName, interactionVisualScrollMultiplier);
        }
    }

    private bool UpdateInteractionFrameworkElementSize()
    {
        if (interactionFrameworkElement != null)
        {
            double parentWidth = 0.0;
            double parentHeight = 0.0;
            FrameworkElement parent = interactionFrameworkElement.Parent as FrameworkElement;

            if (parent != null)
            {
                parentWidth = parent.ActualWidth;
                parentHeight = parent.ActualHeight;
            }

            if (orientation == Orientation.Horizontal)
            {
                double newWidth;
                if (viewport == 0.0)
                {
                    newWidth = 40.0;
                }
                else
                {
                    newWidth = Math.Max(Math.Min(40.0, parentWidth), viewport / (maxOffset - minOffset + viewport) * parentWidth);
                }
                if (newWidth != interactionFrameworkElement.Width)
                {
                    interactionFrameworkElement.Width = newWidth;
                    var ignored = Dispatcher.RunAsync(Windows.UI.Core.CoreDispatcherPriority.Low, UpdateInteractionElementScrollMultiplier);
                    return true;
                }
            }
            else
            {
                double newHeight;
                if (viewport == 0.0)
                {
                    newHeight = 40.0;
                }
                else
                {
                    newHeight = Math.Max(Math.Min(40.0, parentHeight), viewport / (maxOffset - minOffset + viewport) * parentHeight);
                }
                if (newHeight != interactionFrameworkElement.Height)
                {
                    interactionFrameworkElement.Height = newHeight;
                    var ignored = Dispatcher.RunAsync(Windows.UI.Core.CoreDispatcherPriority.Low, UpdateInteractionElementScrollMultiplier);
                    return true;
                }
            }
        }
        return false;
    }

    private void EnsureThumbAnimation()
    {
        if (thumbOffsetAnimation == null && expressionAnimationSources != null &&
            !string.IsNullOrWhiteSpace(multiplierPropertyName) &&
            !string.IsNullOrWhiteSpace(offsetPropertyName) &&
            !string.IsNullOrWhiteSpace(minOffsetPropertyName) &&
            !string.IsNullOrWhiteSpace(maxOffsetPropertyName))
        {
            thumbOffsetAnimation = expressionAnimationSources.Compositor.CreateExpressionAnimation();
            thumbOffsetAnimation.SetReferenceParameter("sources", expressionAnimationSources);
        }
    }

    private void UpdateThumbExpression()
    {
        if (thumbOffsetAnimation != null)
        {
            thumbOffsetAnimation.Expression =
                "min(sources." + maxOffsetPropertyName + ",max(sources." + minOffsetPropertyName + ",sources." + offsetPropertyName + "))/(-sources." + multiplierPropertyName + ")";
        }
    }

    private void StartThumbAnimation(Orientation orientation)
    {
        if (interactionVisual != null && thumbOffsetAnimation != null)
        {
            if (orientation == Orienta