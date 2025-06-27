Directory structure:
└── microsoft-winui-gallery/
    ├── README.md
    ├── Directory.Build.props
    ├── LICENSE
    ├── nuget.config
    ├── SECURITY.md
    ├── standalone.props
    ├── WinUIGallery.DesktopWap.sln
    ├── WinUIGallery.sln
    ├── .editorconfig
    ├── docs/
    │   └── images/
    │       └── WinUIGalleryLanding.PNG
    ├── packagestore/
    │   └── readme.md
    ├── tests/
    │   ├── WinUIGallery.UITests/
    │   │   ├── README.md
    │   │   ├── AxeHelper.cs
    │   │   ├── SampleTestTemplate.cs
    │   │   ├── SessionManager.cs
    │   │   ├── TestBase.cs
    │   │   ├── WinUIGallery.UITests.csproj
    │   │   ├── Properties/
    │   │   │   ├── launchSettings.json
    │   │   │   └── PublishProfiles/
    │   │   │       ├── win-arm64.pubxml
    │   │   │       ├── win-arm64ec.pubxml
    │   │   │       ├── win-x64.pubxml
    │   │   │       └── win-x86.pubxml
    │   │   └── Tests/
    │   │       ├── AxeScanAllTests.cs
    │   │       ├── Button.cs
    │   │       ├── CheckBox.cs
    │   │       ├── ComboBox.cs
    │   │       ├── DatePicker.cs
    │   │       ├── MediaPlayerElement.cs
    │   │       ├── PersonPicture.cs
    │   │       ├── ProgressBar.cs
    │   │       ├── RadioButton.cs
    │   │       ├── SearchResults.cs
    │   │       ├── Slider.cs
    │   │       ├── TextBlock.cs
    │   │       ├── TextBox.cs
    │   │       ├── ToggleButton.cs
    │   │       └── ToggleSwitch.cs
    │   └── WinUIGallery.UnitTests/
    │       ├── app.manifest
    │       ├── Package.appxmanifest
    │       ├── UnitTestApp.xaml
    │       ├── UnitTestApp.xaml.cs
    │       ├── UnitTestAppWindow.xaml
    │       ├── UnitTestAppWindow.xaml.cs
    │       ├── UnitTests.cs
    │       ├── WinUIGallery.UnitTests.csproj
    │       └── Properties/
    │           ├── launchSettings.json
    │           └── PublishProfiles/
    │               ├── win-arm64.pubxml
    │               ├── win-arm64ec.pubxml
    │               ├── win-x64.pubxml
    │               └── win-x86.pubxml
    ├── Tools/
    │   ├── readme.md
    │   ├── Get-LatestAddedSamples.ps1
    │   └── Get-LatestUpdatedSamples.ps1
    ├── WinUIGallery/
    │   ├── app.manifest
    │   ├── App.xaml
    │   ├── App.xaml.cs
    │   ├── CollectionsInterop.cs
    │   ├── common.props
    │   ├── ContentIncludes.props
    │   ├── Directory.Build.props
    │   ├── Directory.Build.targets
    │   ├── GlobalSuppressions.cs
    │   ├── net7.override.targets
    │   ├── Package.appxmanifest
    │   ├── Package.Dev.appxmanifest
    │   ├── WinUIGallery.csproj
    │   ├── WinUIGallery.DesktopWap.Package.wapproj
    │   ├── Assets/
    │   │   ├── AnimatedVisuals/
    │   │   │   └── LottieLogo1.cs
    │   │   ├── SampleMedia/
    │   │   │   ├── Contacts.txt
    │   │   │   ├── fishes.wmv
    │   │   │   └── ladybug.wmv
    │   │   └── SceneNode/
    │   │       ├── DamagedHelmet1.bmp
    │   │       ├── DamagedHelmet2.bmp
    │   │       ├── DamagedHelmet3.bmp
    │   │       ├── DamagedHelmet4.bmp
    │   │       ├── DamagedHelmet5.bmp
    │   │       ├── DamagedHelmet6.bin
    │   │       ├── DamagedHelmet7.bin
    │   │       ├── DamagedHelmet8.bin
    │   │       └── DamagedHelmet9.bin
    │   ├── Behaviors/
    │   │   └── ImageScrollBehavior.cs
    │   ├── Controls/
    │   │   ├── ControlExample.xaml
    │   │   ├── ControlExample.xaml.cs
    │   │   ├── CopyButton.xaml
    │   │   ├── CopyButton.xaml.cs
    │   │   ├── HorizontalScrollContainer.xaml
    │   │   ├── HorizontalScrollContainer.xaml.cs
    │   │   ├── InlineColorPicker.xaml
    │   │   ├── InlineColorPicker.xaml.cs
    │   │   ├── OpacityMaskView.xaml
    │   │   ├── OpacityMaskView.xaml.cs
    │   │   ├── PageHeader.xaml
    │   │   ├── PageHeader.xaml.cs
    │   │   ├── SampleCodePresenter.xaml
    │   │   ├── SampleCodePresenter.xaml.cs
    │   │   ├── SampleThemeListener.xaml
    │   │   ├── SampleThemeListener.xaml.cs
    │   │   ├── DesignGuidance/
    │   │   │   ├── ColorPageExample.xaml
    │   │   │   ├── ColorPageExample.xaml.cs
    │   │   │   ├── ColorTile.xaml
    │   │   │   ├── ColorTile.xaml.cs
    │   │   │   ├── TypographyControl.xaml
    │   │   │   ├── TypographyControl.xaml.cs
    │   │   │   └── ColorSections/
    │   │   │       ├── BackgroundSection.xaml
    │   │   │       ├── BackgroundSection.xaml.cs
    │   │   │       ├── FillSection.xaml
    │   │   │       ├── FillSection.xaml.cs
    │   │   │       ├── HighContrastSection.xaml
    │   │   │       ├── HighContrastSection.xaml.cs
    │   │   │       ├── SignalSection.xaml
    │   │   │       ├── SignalSection.xaml.cs
    │   │   │       ├── StrokeSection.xaml
    │   │   │       ├── StrokeSection.xaml.cs
    │   │   │       ├── TextSection.xaml
    │   │   │       └── TextSection.xaml.cs
    │   │   └── HomePage/
    │   │       ├── HomePageHeader.xaml
    │   │       ├── HomePageHeader.xaml.cs
    │   │       ├── Tile.xaml
    │   │       └── Tile.xaml.cs
    │   ├── Converters/
    │   │   ├── BooleanToInvertedVisibilityConverter.cs
    │   │   ├── BooleanToValueConverter.cs
    │   │   ├── DoubleToThicknessConverter.cs
    │   │   ├── EmptyStringToVisibilityConverter.cs
    │   │   ├── MenuItemTemplateSelector.cs
    │   │   ├── NullableBooleanToBooleanConverter.cs
    │   │   └── NullToVisibilityConverter.cs
    │   ├── Helpers/
    │   │   ├── ControlInfoDataSource.cs
    │   │   ├── EnumHelper.cs
    │   │   ├── FileLoader.cs
    │   │   ├── IconsDataSource.cs
    │   │   ├── IdleSynchronizer.cs
    │   │   ├── LanguageList.cs
    │   │   ├── NativeHelper.cs
    │   │   ├── NavigationHelper.cs
    │   │   ├── NavigationOrientationHelper.cs
    │   │   ├── PageScrollBehaviorHelper.cs
    │   │   ├── ProtocolActivationClipboardHelper.cs
    │   │   ├── SettingsHelper.cs
    │   │   ├── SuspensionManager.cs
    │   │   ├── TabViewHelper.cs
    │   │   ├── ThemeHelper.cs
    │   │   ├── TitleBarHelper.cs
    │   │   ├── UIHelper.cs
    │   │   ├── VersionHelper.cs
    │   │   ├── Win32.cs
    │   │   ├── Win32WindowHelper.cs
    │   │   ├── WindowHelper.cs
    │   │   ├── WindowsSystemDispatcherQueueHelper.cs
    │   │   └── ColorCode.internal/
    │   │       ├── ExtensionMethods.cs
    │   │       └── RichTextBlockFormatter.cs
    │   ├── Layouts/
    │   │   ├── ActivityFeedLayout.cs
    │   │   ├── VariedImageSizeLayout.cs
    │   │   └── WrapPanel.cs
    │   ├── Models/
    │   │   ├── Category.cs
    │   │   ├── ControlInfoData.cs
    │   │   └── IconData.cs
    │   ├── Pages/
    │   │   ├── AllControlsPage.xaml
    │   │   ├── AllControlsPage.xaml.cs
    │   │   ├── HomePage.xaml
    │   │   ├── HomePage.xaml.cs
    │   │   ├── ItemPage.xaml
    │   │   ├── ItemPage.xaml.cs
    │   │   ├── ItemsPageBase.cs
    │   │   ├── NavigationRootPage.xaml
    │   │   ├── NavigationRootPage.xaml.cs
    │   │   ├── SearchResultsPage.xaml
    │   │   ├── SearchResultsPage.xaml.cs
    │   │   ├── SectionPage.xaml
    │   │   ├── SectionPage.xaml.cs
    │   │   ├── SettingsPage.xaml
    │   │   └── SettingsPage.xaml.cs
    │   ├── Properties/
    │   │   ├── AssemblyInfo.cs
    │   │   ├── launchSettings.json
    │   │   └── PublishProfiles/
    │   │       ├── win-arm64.pubxml
    │   │       ├── win-arm64ec.pubxml
    │   │       ├── win-x64.pubxml
    │   │       └── win-x86.pubxml
    │   ├── Samples/
    │   │   ├── ControlPages/
    │   │   │   ├── AcrylicPage.xaml
    │   │   │   ├── AcrylicPage.xaml.cs
    │   │   │   ├── AnimatedIconPage.xaml
    │   │   │   ├── AnimatedIconPage.xaml.cs
    │   │   │   ├── AnimatedVisualPlayerPage.xaml
    │   │   │   ├── AnimatedVisualPlayerPage.xaml.cs
    │   │   │   ├── AnnotatedScrollBarPage.xaml
    │   │   │   ├── AnnotatedScrollBarPage.xaml.cs
    │   │   │   ├── AppBarButtonPage.xaml
    │   │   │   ├── AppBarButtonPage.xaml.cs
    │   │   │   ├── AppBarSeparatorPage.xaml
    │   │   │   ├── AppBarSeparatorPage.xaml.cs
    │   │   │   ├── AppBarToggleButtonPage.xaml
    │   │   │   ├── AppBarToggleButtonPage.xaml.cs
    │   │   │   ├── AppNotificationPage.xaml
    │   │   │   ├── AppNotificationPage.xaml.cs
    │   │   │   ├── AppWindowPage.xaml
    │   │   │   ├── AppWindowPage.xaml.cs
    │   │   │   ├── AutoSuggestBoxPage.xaml
    │   │   │   ├── AutoSuggestBoxPage.xaml.cs
    │   │   │   ├── BadgeNotificationManagerPage.xaml
    │   │   │   ├── BadgeNotificationManagerPage.xaml.cs
    │   │   │   ├── BorderPage.xaml
    │   │   │   ├── BorderPage.xaml.cs
    │   │   │   ├── BreadcrumbBarPage.xaml
    │   │   │   ├── BreadcrumbBarPage.xaml.cs
    │   │   │   ├── ButtonPage.xaml
    │   │   │   ├── ButtonPage.xaml.cs
    │   │   │   ├── CalendarDatePickerPage.xaml
    │   │   │   ├── CalendarDatePickerPage.xaml.cs
    │   │   │   ├── CalendarViewPage.xaml
    │   │   │   ├── CalendarViewPage.xaml.cs
    │   │   │   ├── CanvasPage.xaml
    │   │   │   ├── CanvasPage.xaml.cs
    │   │   │   ├── CaptureElementPreviewPage.xaml
    │   │   │   ├── CaptureElementPreviewPage.xaml.cs
    │   │   │   ├── CheckBoxPage.xaml
    │   │   │   ├── CheckBoxPage.xaml.cs
    │   │   │   ├── ClipboardPage.xaml
    │   │   │   ├── ClipboardPage.xaml.cs
    │   │   │   ├── ColorPickerPage.xaml
    │   │   │   ├── ColorPickerPage.xaml.cs
    │   │   │   ├── ComboBoxPage.xaml
    │   │   │   ├── ComboBoxPage.xaml.cs
    │   │   │   ├── CommandBarFlyoutPage.xaml
    │   │   │   ├── CommandBarFlyoutPage.xaml.cs
    │   │   │   ├── CommandBarPage.xaml
    │   │   │   ├── CommandBarPage.xaml.cs
    │   │   │   ├── CompactSizingPage.xaml
    │   │   │   ├── CompactSizingPage.xaml.cs
    │   │   │   ├── ConnectedAnimationPage.xaml
    │   │   │   ├── ConnectedAnimationPage.xaml.cs
    │   │   │   ├── ContentDialogContent.xaml
    │   │   │   ├── ContentDialogContent.xaml.cs
    │   │   │   ├── ContentDialogExample.xaml
    │   │   │   ├── ContentDialogExample.xaml.cs
    │   │   │   ├── ContentDialogPage.xaml
    │   │   │   ├── ContentDialogPage.xaml.cs
    │   │   │   ├── ContentIslandPage.xaml
    │   │   │   ├── ContentIslandPage.xaml.cs
    │   │   │   ├── CreateMultipleWindowsPage.xaml
    │   │   │   ├── CreateMultipleWindowsPage.xaml.cs
    │   │   │   ├── DatePickerPage.xaml
    │   │   │   ├── DatePickerPage.xaml.cs
    │   │   │   ├── DropDownButtonPage.xaml
    │   │   │   ├── DropDownButtonPage.xaml.cs
    │   │   │   ├── EasingFunctionPage.xaml
    │   │   │   ├── EasingFunctionPage.xaml.cs
    │   │   │   ├── ExpanderPage.xaml
    │   │   │   ├── ExpanderPage.xaml.cs
    │   │   │   ├── FilePickerPage.xaml
    │   │   │   ├── FilePickerPage.xaml.cs
    │   │   │   ├── FlipViewPage.xaml
    │   │   │   ├── FlipViewPage.xaml.cs
    │   │   │   ├── FlyoutPage.xaml
    │   │   │   ├── FlyoutPage.xaml.cs
    │   │   │   ├── GridPage.xaml
    │   │   │   ├── GridPage.xaml.cs
    │   │   │   ├── GridViewPage.xaml
    │   │   │   ├── GridViewPage.xaml.cs
    │   │   │   ├── HyperlinkButtonPage.xaml
    │   │   │   ├── HyperlinkButtonPage.xaml.cs
    │   │   │   ├── IconElementPage.xaml
    │   │   │   ├── IconElementPage.xaml.cs
    │   │   │   ├── ImagePage.xaml
    │   │   │   ├── ImagePage.xaml.cs
    │   │   │   ├── ImplicitTransitionPage.xaml
    │   │   │   ├── ImplicitTransitionPage.xaml.cs
    │   │   │   ├── InfoBadgePage.xaml
    │   │   │   ├── InfoBadgePage.xaml.cs
    │   │   │   ├── InfoBarPage.xaml
    │   │   │   ├── InfoBarPage.xaml.cs
    │   │   │   ├── ItemsRepeaterPage.xaml
    │   │   │   ├── ItemsRepeaterPage.xaml.cs
    │   │   │   ├── ItemsViewPage.xaml
    │   │   │   ├── ItemsViewPage.xaml.cs
    │   │   │   ├── LinePage.xaml
    │   │   │   ├── LinePage.xaml.cs
    │   │   │   ├── ListBoxPage.xaml
    │   │   │   ├── ListBoxPage.xaml.cs
    │   │   │   ├── ListViewPage.xaml
    │   │   │   ├── ListViewPage.xaml.cs
    │   │   │   ├── MapControlPage.xaml
    │   │   │   ├── MapControlPage.xaml.cs
    │   │   │   ├── MediaPlayerElementPage.xaml
    │   │   │   ├── MediaPlayerElementPage.xaml.cs
    │   │   │   ├── MenuBarPage.xaml
    │   │   │   ├── MenuBarPage.xaml.cs
    │   │   │   ├── MenuFlyoutPage.xaml
    │   │   │   ├── MenuFlyoutPage.xaml.cs
    │   │   │   ├── NavigationViewPage.xaml
    │   │   │   ├── NavigationViewPage.xaml.cs
    │   │   │   ├── NumberBoxPage.xaml
    │   │   │   ├── NumberBoxPage.xaml.cs
    │   │   │   ├── PageTransitionPage.xaml
    │   │   │   ├── PageTransitionPage.xaml.cs
    │   │   │   ├── ParallaxViewPage.xaml
    │   │   │   ├── ParallaxViewPage.xaml.cs
    │   │   │   ├── PasswordBoxPage.xaml
    │   │   │   ├── PasswordBoxPage.xaml.cs
    │   │   │   ├── PersonPicturePage.xaml
    │   │   │   ├── PersonPicturePage.xaml.cs
    │   │   │   ├── PipsPagerPage.xaml
    │   │   │   ├── PipsPagerPage.xaml.cs
    │   │   │   ├── PivotPage.xaml
    │   │   │   ├── PivotPage.xaml.cs
    │   │   │   ├── PopupPage.xaml
    │   │   │   ├── PopupPage.xaml.cs
    │   │   │   ├── ProgressBarPage.xaml
    │   │   │   ├── ProgressBarPage.xaml.cs
    │   │   │   ├── ProgressRingPage.xaml
    │   │   │   ├── ProgressRingPage.xaml.cs
    │   │   │   ├── PullToRefreshPage.xaml
    │   │   │   ├── PullToRefreshPage.xaml.cs
    │   │   │   ├── RadialGradientBrushPage.xaml
    │   │   │   ├── RadialGradientBrushPage.xaml.cs
    │   │   │   ├── RadioButtonPage.xaml
    │   │   │   ├── RadioButtonPage.xaml.cs
    │   │   │   ├── RadioButtonsPage.xaml
    │   │   │   ├── RadioButtonsPage.xaml.cs
    │   │   │   ├── RatingControlPage.xaml
    │   │   │   ├── RatingControlPage.xaml.cs
    │   │   │   ├── RelativePanelPage.xaml
    │   │   │   ├── RelativePanelPage.xaml.cs
    │   │   │   ├── RepeatButtonPage.xaml
    │   │   │   ├── RepeatButtonPage.xaml.cs
    │   │   │   ├── RichEditBoxPage.xaml
    │   │   │   ├── RichEditBoxPage.xaml.cs
    │   │   │   ├── RichTextBlockPage.xaml
    │   │   │   ├── RichTextBlockPage.xaml.cs
    │   │   │   ├── ScrollViewerPage.xaml
    │   │   │   ├── ScrollViewerPage.xaml.cs
    │   │   │   ├── ScrollViewPage.xaml
    │   │   │   ├── ScrollViewPage.xaml.cs
    │   │   │   ├── SelectorBarPage.xaml
    │   │   │   ├── SelectorBarPage.xaml.cs
    │   │   │   ├── SemanticZoomPage.xaml
    │   │   │   ├── SemanticZoomPage.xaml.cs
    │   │   │   ├── ShapePage.xaml
    │   │   │   ├── ShapePage.xaml.cs
    │   │   │   ├── SliderPage.xaml
    │   │   │   ├── SliderPage.xaml.cs
    │   │   │   ├── SoundPage.xaml
    │   │   │   ├── SoundPage.xaml.cs
    │   │   │   ├── SplitButtonPage.xaml
    │   │   │   ├── SplitButtonPage.xaml.cs
    │   │   │   ├── SplitViewPage.xaml
    │   │   │   ├── SplitViewPage.xaml.cs
    │   │   │   ├── StackPanelPage.xaml
    │   │   │   ├── StackPanelPage.xaml.cs
    │   │   │   ├── StandardUICommandPage.xaml
    │   │   │   ├── StandardUICommandPage.xaml.cs
    │   │   │   ├── SwipeControlPage.xaml
    │   │   │   ├── SwipeControlPage.xaml.cs
    │   │   │   ├── SystemBackdropsPage.xaml
    │   │   │   ├── SystemBackdropsPage.xaml.cs
    │   │   │   ├── TabViewPage.xaml
    │   │   │   ├── TabViewPage.xaml.cs
    │   │   │   ├── TeachingTipPage.xaml
    │   │   │   ├── TeachingTipPage.xaml.cs
    │   │   │   ├── TextBlockPage.xaml
    │   │   │   ├── TextBlockPage.xaml.cs
    │   │   │   ├── TextBoxPage.xaml
    │   │   │   ├── TextBoxPage.xaml.cs
    │   │   │   ├── ThemeTransitionPage.xaml
    │   │   │   ├── ThemeTransitionPage.xaml.cs
    │   │   │   ├── TimePickerPage.xaml
    │   │   │   ├── TimePickerPage.xaml.cs
    │   │   │   ├── TitleBarPage.xaml
    │   │   │   ├── TitleBarPage.xaml.cs
    │   │   │   ├── ToggleButtonPage.xaml
    │   │   │   ├── ToggleButtonPage.xaml.cs
    │   │   │   ├── ToggleSplitButtonPage.xaml
    │   │   │   ├── ToggleSplitButtonPage.xaml.cs
    │   │   │   ├── ToggleSwitchPage.xaml
    │   │   │   ├── ToggleSwitchPage.xaml.cs
    │   │   │   ├── ToolTipPage.xaml
    │   │   │   ├── ToolTipPage.xaml.cs
    │   │   │   ├── TreeViewPage.xaml
    │   │   │   ├── TreeViewPage.xaml.cs
    │   │   │   ├── VariableSizedWrapGridPage.xaml
    │   │   │   ├── VariableSizedWrapGridPage.xaml.cs
    │   │   │   ├── ViewboxPage.xaml
    │   │   │   ├── ViewboxPage.xaml.cs
    │   │   │   ├── WebView2Page.xaml
    │   │   │   ├── WebView2Page.xaml.cs
    │   │   │   ├── XamlCompInteropPage.xaml
    │   │   │   ├── XamlCompInteropPage.xaml.cs
    │   │   │   ├── XamlUICommandPage.xaml
    │   │   │   ├── XamlUICommandPage.xaml.cs
    │   │   │   ├── Accessibility/
    │   │   │   │   ├── AccessibilityColorContrastPage.xaml
    │   │   │   │   ├── AccessibilityColorContrastPage.xaml.cs
    │   │   │   │   ├── AccessibilityKeyboardPage.xaml
    │   │   │   │   ├── AccessibilityKeyboardPage.xaml.cs
    │   │   │   │   ├── AccessibilityScreenReaderPage.xaml
    │   │   │   │   └── AccessibilityScreenReaderPage.xaml.cs
    │   │   │   ├── Design/
    │   │   │   │   ├── ColorPage.xaml
    │   │   │   │   ├── ColorPage.xaml.cs
    │   │   │   │   ├── GeometryPage.xaml
    │   │   │   │   ├── GeometryPage.xaml.cs
    │   │   │   │   ├── IconographyPage.xaml
    │   │   │   │   ├── IconographyPage.xaml.cs
    │   │   │   │   ├── SpacingPage.xaml
    │   │   │   │   ├── SpacingPage.xaml.cs
    │   │   │   │   ├── TypographyPage.xaml
    │   │   │   │   └── TypographyPage.xaml.cs
    │   │   │   └── Fundamentals/
    │   │   │       ├── BindingPage.xaml
    │   │   │       ├── BindingPage.xaml.cs
    │   │   │       ├── CustomUserControlsPage.xaml
    │   │   │       ├── CustomUserControlsPage.xaml.cs
    │   │   │       ├── ScratchPadPage.xaml
    │   │   │       ├── ScratchPadPage.xaml.cs
    │   │   │       ├── TemplatesPage.xaml
    │   │   │       ├── TemplatesPage.xaml.cs
    │   │   │       ├── XamlResourcesPage.xaml
    │   │   │       ├── XamlResourcesPage.xaml.cs
    │   │   │       ├── XamlStylesPage.xaml
    │   │   │       ├── XamlStylesPage.xaml.cs
    │   │   │       └── Controls/
    │   │   │           ├── CounterControl.cs
    │   │   │           ├── CounterControl.xaml
    │   │   │           ├── TemperatureConverterControl.xaml
    │   │   │           ├── TemperatureConverterControl.xaml.cs
    │   │   │           ├── ValidatedPasswordBox.cs
    │   │   │           └── ValidatedPasswordBox.xaml
    │   │   ├── Data/
    │   │   │   ├── ControlInfoData.json
    │   │   │   ├── ControlInfoDataSchema.json
    │   │   │   ├── IconsData.json
    │   │   │   └── IconsDataSchema.json
    │   │   ├── SampleCode/
    │   │   │   ├── AppWindow/
    │   │   │   │   ├── AppWindowSample1_xaml.txt
    │   │   │   │   ├── AppWindowSample2_cs.txt
    │   │   │   │   ├── AppWindowSample2_xaml.txt
    │   │   │   │   ├── AppWindowSample3_xaml.txt
    │   │   │   │   ├── AppWindowSample5_cs.txt
    │   │   │   │   ├── AppWindowSample5_xaml.txt
    │   │   │   │   ├── AppWindowSample6_cs.txt
    │   │   │   │   ├── AppWindowSample6_xaml.txt
    │   │   │   │   └── AppWindowSample7_xaml.txt
    │   │   │   ├── Binding/
    │   │   │   │   ├── BindingSample1_xaml.txt
    │   │   │   │   ├── BindingSample3_csharp.txt
    │   │   │   │   ├── BindingSample3_xaml.txt
    │   │   │   │   ├── BindingSample4_csharp.txt
    │   │   │   │   ├── BindingSample4_xaml.txt
    │   │   │   │   └── BindingSample5_csharp.txt
    │   │   │   ├── Brushes/
    │   │   │   │   └── RadialGradientBrushSample_xaml.txt
    │   │   │   ├── Buttons/
    │   │   │   │   ├── Button/
    │   │   │   │   │   └── CustomButtonStyle.txt
    │   │   │   │   ├── DropDown/
    │   │   │   │   │   ├── DropDownButton_Icon.txt
    │   │   │   │   │   ├── DropDownButton_RevealStyle.txt
    │   │   │   │   │   └── DropDownButton_Simple.txt
    │   │   │   │   ├── SplitButton/
    │   │   │   │   │   ├── SplitButtonSample1.txt
    │   │   │   │   │   └── SplitButtonSample2.txt
    │   │   │   │   └── ToggleSplitButton/
    │   │   │   │       └── ToggleSplitButtonSample1.txt
    │   │   │   ├── CommandBarFlyout/
    │   │   │   │   ├── CommandBarFlyoutSample1_cs.txt
    │   │   │   │   └── CommandBarFlyoutSample1_xaml.txt
    │   │   │   ├── ContentDialog/
    │   │   │   │   ├── ContentDialogSample1_cs.txt
    │   │   │   │   └── ContentDialogSample1_xaml.txt
    │   │   │   ├── CustomUserControls/
    │   │   │   │   ├── CustomUserControlsSample1_cs.txt
    │   │   │   │   ├── CustomUserControlsSample1_xaml.txt
    │   │   │   │   ├── CustomUserControlsSample2_cs.txt
    │   │   │   │   ├── CustomUserControlsSample2_xaml.txt
    │   │   │   │   ├── CustomUserControlsSample3_cs.txt
    │   │   │   │   ├── CustomUserControlsSample3_xaml.txt
    │   │   │   │   ├── CustomUserControlsSample4_cs.txt
    │   │   │   │   └── CustomUserControlsSample4_xaml.txt
    │   │   │   ├── Geometry/
    │   │   │   │   └── GeometrySample_xaml.txt
    │   │   │   ├── GridView/
    │   │   │   │   ├── GridViewSample1_cs.txt
    │   │   │   │   └── GridViewSample1_xaml.txt
    │   │   │   ├── Icons/
    │   │   │   │   ├── AnimatedIconSample1_cs.txt
    │   │   │   │   ├── AnimatedIconSample1_xaml.txt
    │   │   │   │   ├── AnimatedIconSample2_xaml.txt
    │   │   │   │   ├── FontIconSample1_xaml.txt
    │   │   │   │   ├── FontIconSample2_xaml.txt
    │   │   │   │   ├── ImageIconSample1_xaml.txt
    │   │   │   │   ├── ImageIconSample2_xaml.txt
    │   │   │   │   ├── PathIconSample1_xaml.txt
    │   │   │   │   ├── SymbolIconSample1_xaml.txt
    │   │   │   │   └── SymbolIconSample_1_xaml.txt
    │   │   │   ├── ItemsRepeater/
    │   │   │   │   ├── ItemsRepeaterNestedSample_xaml.txt
    │   │   │   │   ├── ItemsRepeaterSample1_cs.txt
    │   │   │   │   ├── ItemsRepeaterSample1_xaml.txt
    │   │   │   │   ├── ItemsRepeaterSample2_cs.txt
    │   │   │   │   ├── ItemsRepeaterSample2_xaml.txt
    │   │   │   │   ├── ItemsRepeaterSample3_cs.txt
    │   │   │   │   ├── ItemsRepeaterSample3_xaml.txt
    │   │   │   │   ├── ItemsRepeaterSample4_cs.txt
    │   │   │   │   └── ItemsRepeaterSample4_xaml.txt
    │   │   │   ├── ListView/
    │   │   │   │   ├── ListViewGroupedHeaderSample_xaml.txt
    │   │   │   │   ├── ListViewSample1_cs.txt
    │   │   │   │   ├── ListViewSample1_xaml.txt
    │   │   │   │   ├── ListViewSample2_cs.txt
    │   │   │   │   ├── ListViewSample2_xaml.txt
    │   │   │   │   ├── ListViewSample3_xaml.txt
    │   │   │   │   ├── ListViewSample4_cs.txt
    │   │   │   │   ├── ListViewSample4_xaml.txt
    │   │   │   │   └── ListViewStickyHeaderSample_xaml.txt
    │   │   │   ├── MapControl/
    │   │   │   │   └── MapControlSample_cs.txt
    │   │   │   ├── Media/
    │   │   │   │   ├── CaptureElementPreviewSample_cs.txt
    │   │   │   │   └── CaptureElementPreviewSample_xaml.txt
    │   │   │   ├── MenuBar/
    │   │   │   │   ├── MenuBarSample1.txt
    │   │   │   │   ├── MenuBarSample2.txt
    │   │   │   │   └── MenuBarSample3.txt
    │   │   │   ├── Motion/
    │   │   │   │   ├── AnimationInterop/
    │   │   │   │   │   ├── AnimationInteropSample1_cs.txt
    │   │   │   │   │   ├── AnimationInteropSample2_cs.txt
    │   │   │   │   │   ├── AnimationInteropSample2_xaml.txt
    │   │   │   │   │   ├── AnimationInteropSample3_cs.txt
    │   │   │   │   │   ├── AnimationInteropSample4_cs.txt
    │   │   │   │   │   ├── AnimationInteropSample5_cs.txt
    │   │   │   │   │   └── AnimationInteropSample5_xaml.txt
    │   │   │   │   └── ConnectedAnimation/
    │   │   │   │       ├── ConnectedAnimationSample1_cs.txt
    │   │   │   │       ├── ConnectedAnimationSample1_xaml.txt
    │   │   │   │       ├── ConnectedAnimationSample2_cs.txt
    │   │   │   │       ├── ConnectedAnimationSample2_xaml.txt
    │   │   │   │       └── ConnectedAnimationSample3_cs.txt
    │   │   │   ├── NavigationView/
    │   │   │   │   ├── NavigationViewSample1.txt
    │   │   │   │   ├── NavigationViewSample2.txt
    │   │   │   │   ├── NavigationViewSample3.txt
    │   │   │   │   ├── NavigationViewSample4.txt
    │   │   │   │   ├── NavigationViewSample4_cs.txt
    │   │   │   │   ├── NavigationViewSample4_xaml.txt
    │   │   │   │   ├── NavigationViewSample5.txt
    │   │   │   │   ├── NavigationViewSample5_cs.txt
    │   │   │   │   ├── NavigationViewSample5_xaml.txt
    │   │   │   │   ├── NavigationViewSample6.txt
    │   │   │   │   ├── NavigationViewSample8_xaml.txt
    │   │   │   │   └── NavigationViewSample9_xaml.txt
    │   │   │   ├── NumberBox/
    │   │   │   │   ├── NumberBoxSample3_cs.txt
    │   │   │   │   └── NumberBoxSample3_xaml.txt
    │   │   │   ├── ScrollView/
    │   │   │   │   ├── ScrollViewSample3_AccordionAnimation_cs.txt
    │   │   │   │   ├── ScrollViewSample3_DefaultAnimation_cs.txt
    │   │   │   │   └── ScrollViewSample3_TeleportationAnimation_cs.txt
    │   │   │   ├── StandardUICommand/
    │   │   │   │   ├── StandardUICommandSample1_cs.txt
    │   │   │   │   └── StandardUICommandSample1_xaml.txt
    │   │   │   ├── System/
    │   │   │   │   ├── FilePickerSample1_cs.txt
    │   │   │   │   ├── FilePickerSample1_xaml.txt
    │   │   │   │   ├── FilePickerSample2_cs.txt
    │   │   │   │   ├── FilePickerSample2_xaml.txt
    │   │   │   │   ├── FilePickerSample3_cs.txt
    │   │   │   │   ├── FilePickerSample3_xaml.txt
    │   │   │   │   ├── FilePickerSample4_cs.txt
    │   │   │   │   ├── FilePickerSample4_xaml.txt
    │   │   │   │   ├── FilePickerSample5_cs.txt
    │   │   │   │   ├── FilePickerSample5_xaml.txt
    │   │   │   │   └── Window.txt
    │   │   │   ├── SystemBackdrops/
    │   │   │   │   ├── SystemBackdropsEnsureSystemDQC.txt
    │   │   │   │   ├── SystemBackdropsSampleBackdropTypes_cs.txt
    │   │   │   │   ├── SystemBackdropsSampleBackdropTypes_xaml.txt
    │   │   │   │   ├── SystemBackdropsSampleDesktopAcrylicController.txt
    │   │   │   │   └── SystemBackdropsSampleMicaController.txt
    │   │   │   ├── TabView/
    │   │   │   │   ├── TabViewBasicSample_cs.txt
    │   │   │   │   └── TabViewKeyboardAcceleratorSample_cs.txt
    │   │   │   ├── TeachingTip/
    │   │   │   │   ├── TeachingTipSample1_cs.txt
    │   │   │   │   ├── TeachingTipSample1_xaml.txt
    │   │   │   │   ├── TeachingTipSample2_cs.txt
    │   │   │   │   ├── TeachingTipSample2_xaml.txt
    │   │   │   │   ├── TeachingTipSample3_cs.txt
    │   │   │   │   └── TeachingTipSample3_xaml.txt
    │   │   │   ├── Templates/
    │   │   │   │   ├── TemplatesSample1_xaml.txt
    │   │   │   │   ├── TemplatesSample2_xaml.txt
    │   │   │   │   ├── TemplatesSample3_StackPanel_xaml.txt
    │   │   │   │   └── TemplatesSample3_WrapGrid_xaml.txt
    │   │   │   ├── Text/
    │   │   │   │   └── RichEditBox/
    │   │   │   │       ├── RichEditBoxSample3_cs.txt
    │   │   │   │       ├── RichEditBoxSample3_xaml.txt
    │   │   │   │       ├── RichEditBoxSample4_cs.txt
    │   │   │   │       ├── RichEditBoxSample4_xaml.txt
    │   │   │   │       └── RichEditBoxSample6_cs.txt
    │   │   │   ├── TreeView/
    │   │   │   │   ├── TreeViewDataBindingSample_cs.txt
    │   │   │   │   ├── TreeViewDataBindingSample_xaml.txt
    │   │   │   │   ├── TreeViewSample1_cs.txt
    │   │   │   │   ├── TreeViewTemplateSelectorSample_cs.txt
    │   │   │   │   └── TreeViewTemplateSelectorSample_xaml.txt
    │   │   │   ├── Typography/
    │   │   │   │   └── TypographySample_xaml.txt
    │   │   │   ├── Window/
    │   │   │   │   ├── CreateWindowSample1.txt
    │   │   │   │   └── TitleBar/
    │   │   │   │       ├── TitleBarSample1.txt
    │   │   │   │       ├── TitleBarSample2.txt
    │   │   │   │       └── TitleBarSample3.txt
    │   │   │   ├── XamlResources/
    │   │   │   │   ├── XamlResourcesSample1_csharp.txt
    │   │   │   │   ├── XamlResourcesSample1_xaml.txt
    │   │   │   │   ├── XamlResourcesSample2_xaml.txt
    │   │   │   │   └── XamlResourcesSample3_xaml.txt
    │   │   │   ├── XamlStyles/
    │   │   │   │   ├── XamlStylesSample1_xaml.txt
    │   │   │   │   ├── XamlStylesSample2_xaml.txt
    │   │   │   │   ├── XamlStylesSample3_xaml.txt
    │   │   │   │   └── XamlStylesSample4_csharp.txt
    │   │   │   └── XamlUICommand/
    │   │   │       ├── XamlUICommandSample1_cs.txt
    │   │   │       └── XamlUICommandSample1_xaml.txt
    │   │   ├── SampleHelpers/
    │   │   │   └── SceneNode/
    │   │   │       ├── HelmetScenario.cs
    │   │   │       └── SceneNodeCommon.cs
    │   │   └── SamplePages/
    │   │       ├── CardPage.xaml
    │   │       ├── CardPage.xaml.cs
    │   │       ├── CollectionPage.xaml
    │   │       ├── CollectionPage.xaml.cs
    │   │       ├── DetailedInfoPage.xaml
    │   │       ├── DetailedInfoPage.xaml.cs
    │   │       ├── ModalWindow.xaml
    │   │       ├── ModalWindow.xaml.cs
    │   │       ├── SampleBuiltInSystemBackdropsWindow.xaml
    │   │       ├── SampleBuiltInSystemBackdropsWindow.xaml.cs
    │   │       ├── SampleCompactSizingPage.xaml
    │   │       ├── SampleCompactSizingPage.xaml.cs
    │   │       ├── SamplePage1.xaml
    │   │       ├── SamplePage1.xaml.cs
    │   │       ├── SamplePage2.xaml
    │   │       ├── SamplePage2.xaml.cs
    │   │       ├── SamplePage3.xaml
    │   │       ├── SamplePage3.xaml.cs
    │   │       ├── SamplePage4.xaml
    │   │       ├── SamplePage4.xaml.cs
    │   │       ├── SamplePage5.xaml
    │   │       ├── SamplePage5.xaml.cs
    │   │       ├── SamplePage6.xaml
    │   │       ├── SamplePage6.xaml.cs
    │   │       ├── SamplePage7.xaml
    │   │       ├── SamplePage7.xaml.cs
    │   │       ├── SampleSettingsPage.xaml
    │   │       ├── SampleSettingsPage.xaml.cs
    │   │       ├── SampleStandardSizingPage.xaml
    │   │       ├── SampleStandardSizingPage.xaml.cs
    │   │       ├── SampleSystemBackdropsWindow.xaml
    │   │       ├── SampleSystemBackdropsWindow.xaml.cs
    │   │       ├── SampleWindow1.xaml
    │   │       ├── SampleWindow1.xaml.cs
    │   │       ├── SampleWindow2.xaml
    │   │       ├── SampleWindow2.xaml.cs
    │   │       ├── SampleWindow3.xaml
    │   │       ├── SampleWindow3.xaml.cs
    │   │       ├── SampleWindow4.xaml
    │   │       ├── SampleWindow4.xaml.cs
    │   │       ├── SampleWindow6.xaml
    │   │       ├── SampleWindow6.xaml.cs
    │   │       ├── SampleWindow7.xaml
    │   │       ├── SampleWindow7.xaml.cs
    │   │       ├── TabContentSampleControl.xaml
    │   │       ├── TabContentSampleControl.xaml.cs
    │   │       ├── TabViewWindowingSamplePage.xaml
    │   │       └── TabViewWindowingSamplePage.xaml.cs
    │   └── Styles/
    │       ├── Button.xaml
    │       ├── Grid.xaml
    │       ├── GridViewItem.xaml
    │       ├── ItemTemplates.xaml
    │       ├── ItemTemplates.xaml.cs
    │       ├── SelectorBar.xaml
    │       └── TextBlock.xaml
    ├── .github/
    │   ├── CONTRIBUTING.md
    │   ├── PULL_REQUEST_TEMPLATE.md
    │   └── ISSUE_TEMPLATE/
    │       ├── bug_report.yaml
    │       └── feature_request.yaml
    └── .pipelines/
        ├── azure-pipelines.yml
        ├── WinUI-Gallery-OneBranch-Official.yml
        └── WinUI-Gallery-SyncMirror.yml


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
![WinUI Gallery hero image](docs/images/WinUIGalleryLanding.PNG)

<h1 align="center">
    WinUI 3 Gallery
</h1>

[![Build Status](https://dev.azure.com/ms/microsoft-ui-xaml/_apis/build/status%2Fmicrosoft.WinUI-Gallery?branchName=main)](https://dev.azure.com/ms/microsoft-ui-xaml/_build/latest?definitionId=612&branchName=main) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/your/your-project/blob/master/LICENSE)

### Accompanying Sample App for [WinAppSDK](https://github.com/microsoft/WindowsAppSDK)

This app demonstrates all of the WinUI 3 controls and styles available to make a modern Windows app with the [Windows App SDK](https://github.com/microsoft/WindowsAppSDK). It is the interactive companion to the [Fluent Design Guidelines](https://docs.microsoft.com/windows/apps/design/basics/) and shows the usage of the [WinUI](https://docs.microsoft.com/windows/apps/winui/) APIs.

<p align="center">
<img src="docs/images/winui-gallery.png" alt="WinUI 3 Gallery" width="400"/>
</p>
<p align="center">
<a href="https://apps.microsoft.com/detail/WinUI%203%20Gallery/9P3JFPWWDZRC?launch=true
	&mode=mini">
	<img alt="Store badge" src="docs/images/storeBadge.png" width="200"/>
</a>
</p>

## ⭐ Features

- **WinUI controls samples:** each control page shows the markup and codebehind used to create each example.

- **Use the Microsoft.UI.Xaml (WinUI) library:** the app includes the latest WinUI NuGet package and shows how to use the [WinUI](https://docs.microsoft.com/windows/apps/winui/) controls like NavigationView, SwipeControl, and more.

- **Adaptive UI:** in addition to showing how each control responds to different form factors, the app itself is responsive and shows various methods for achieving adaptive UI.

- **Design & accessibility guidance**: design and accessibility pages help make the gallery a useful developer companion app.



## 👏 Contribute to WinUI Gallery

Any samples or docs improvements you'd like to see? We're always looking for a helping hand. Feel free to file an issue to start the discussion, or even better, create a PR with the change you'd like to see!

Check out these [help wanted](https://github.com/microsoft/WinUI-Gallery/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) issues if you don't know where to start.

You can also learn more about current happenings with WinUI Gallery in the [project board](https://github.com/orgs/microsoft/projects/368).

## 🚀 Getting started

Quick start guide to building the WinUI 3 Gallery:


### 1. Set up the environment

> [!NOTE]
> The WinUI Gallery requires [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later to build and Windows 10 or later to execute. If you're building an app with WinUI and Windows App SDK for the first time, follow these [installation instructions](https://learn.microsoft.com/windows/apps/get-started/start-here).

**Required [Visual Studio components](https://learn.microsoft.com/windows/apps/get-started/start-here?tabs=vs-2022-17-10#required-workloads-and-components):**
- Windows application development

### 2. Clone the Repository

```shell
git clone https://github.com/microsoft/WinUI-Gallery.git
```

### 3. Open WinUIGallery.sln with Visual Studio and build!

Ensure that the `WinUIGallery` project is set as the startup project in Visual Studio.

> [!WARNING]
> Try deleting [`nuget.config`](nuget.config) and building again if you get the following build error:
> > Assets file 'C:\Users\\...\source\repos\WinUI-Gallery\WinUIGallery\obj\WinUIGallery\project.assets.json' not found. Run a NuGet package restore to generate this file.
>
> See [issue #1659: Broken repo build](https://github.com/microsoft/WinUI-Gallery/issues/1659).

## ➡️ Further information

To learn more about Windows app development, go to the [Windows Dev Center](https://developer.microsoft.com/windows).


### Related topics


- [Get started with WinUI](https://learn.microsoft.com/windows/apps/get-started/start-here)
- [About WinUI](https://aka.ms/windev)
- [WinUI repository](https://github.com/microsoft/microsoft-ui-xaml)
- [WindowsAppSDK repository](https://github.com/microsoft/WindowsAppSDK)
- [WindowsAppSDK samples](https://github.com/microsoft/WindowsAppSDK-Samples)

## 🏆 Contributors
Thanks to our amazing contributors!

[![WinUI 3 Gallery Contributors](https://contrib.rocks/image?repo=microsoft/WinUI-Gallery)](https://github.com/microsoft/WinUI-Gallery/graphs/contributors)

Made with [contrib.rocks](https://contrib.rocks).



================================================
FILE: Directory.Build.props
================================================
<Project>
  <Import Project="$([MSBuild]::GetPathOfFileAbove('Directory.Build.props', '$(MSBuildThisFileDirectory)../'))" Condition="Exists($([MSBuild]::GetPathOfFileAbove('Directory.Build.props', '$(MSBuildThisFileDirectory)../')))" />

  <!-- Building both in the WinUI repo and standalone, WinUIGallery's dependencies now require latest SDKs -->
  <PropertyGroup>
    <SamplesTargetFrameworkMoniker>net8.0-windows10.0.22621.0</SamplesTargetFrameworkMoniker>
    <WindowsSdkTargetPlatformVersion>10.0.22621.756</WindowsSdkTargetPlatformVersion>
    <WindowsAppSdkTargetPlatformVersion>10.0.17763.0</WindowsAppSdkTargetPlatformVersion>
    <MicrosoftWindowsSDKBuildToolsNugetPackageVersion>10.0.22621.756</MicrosoftWindowsSDKBuildToolsNugetPackageVersion>
  </PropertyGroup>

  <!-- If we aren't building in the WinUI repo, import the necessary missing props we'd normally pick up from its Directory.Build.props hierarchy -->
  <!-- The UseStandalone property allows this to be overridden, in order to buildSamples to build without changing the entire repo -->
  <Import Project="Standalone.props" Condition="'$(IsInWinUIRepo)' != 'true' OR '$(UseStandalone)' == 'true'"/>

  <!-- Temporary workaround until WinAppSDK 1.5.2 provides fix -->
  <Target Name="RemoveConflictingDepsJsonFiles" AfterTargets="GetPackagingOutputs">
    <!-- If conflicting build and publish deps.json files exist in this or referenced projects,
        use only the publish deps.json files, and remove the corresponding build deps.json files. -->
    <ItemGroup>
      <_PublishPackagingOutputs Include="@(PackagingOutputs->HasMetadata('CopyToPublishDirectory'))"/>
      <_PublishDepsJsonFiles Include="@(_PublishPackagingOutputs)"
        Condition="'@(_PublishPackagingOutputs)' != '' and $([System.String]::Copy(%(FileName)%(Extension)).EndsWith('.deps.json'))" />
      <PackagingOutputs Remove="@(_PublishDepsJsonFiles)" MatchOnMetadata="TargetPath"/>
      <PackagingOutputs Include="@(_PublishDepsJsonFiles)"/>
    </ItemGroup>
  </Target>

</Project>


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
FILE: nuget.config
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <config>
    <add key="repositoryPath" value="$\..\packages" />
  </config>
  <disabledPackageSources>
    <clear />
  </disabledPackageSources>
  <packageSources>
    <clear />
    <add key="MUX-Dependencies" value="https://pkgs.dev.azure.com/shine-oss/microsoft-ui-xaml/_packaging/MUX-Dependencies/nuget/v3/index.json" />

    <!-- a local directory to allow testing nupkg files without pushing to a remote feed -->
    <add key="packagestore" value="packagestore" />
  </packageSources>
  <activePackageSource>
    <add key="All" value="(Aggregate source)" />
  </activePackageSource>
</configuration>



================================================
FILE: SECURITY.md
================================================
<!-- BEGIN MICROSOFT SECURITY.MD V0.0.7 BLOCK -->

## Security

Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/Microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [our GitHub organizations](https://opensource.microsoft.com/).

If you believe you have found a security vulnerability in any Microsoft-owned repository that meets [Microsoft's definition of a security vulnerability](https://aka.ms/opensource/security/definition), please report it to us as described below.

## Reporting Security Issues

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them to the Microsoft Security Response Center (MSRC) at [https://msrc.microsoft.com/create-report](https://aka.ms/opensource/security/create-report).

If you prefer to submit without logging in, send email to [secure@microsoft.com](mailto:secure@microsoft.com).  If possible, encrypt your message with our PGP key; please download it from the [Microsoft Security Response Center PGP Key page](https://aka.ms/opensource/security/pgpkey).

You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your original message. Additional information can be found at [microsoft.com/msrc](https://aka.ms/opensource/security/msrc).

Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:

  * Type of issue (e.g. buffer overflow, SQL injection, cross-site scripting, etc.)
  * Full paths of source file(s) related to the manifestation of the issue
  * The location of the affected source code (tag/branch/commit or direct URL)
  * Any special configuration required to reproduce the issue
  * Step-by-step instructions to reproduce the issue
  * Proof-of-concept or exploit code (if possible)
  * Impact of the issue, including how an attacker might exploit the issue

This information will help us triage your report more quickly.

If you are reporting for a bug bounty, more complete reports can contribute to a higher bounty award. Please visit our [Microsoft Bug Bounty Program](https://aka.ms/opensource/security/bounty) page for more details about our active programs.

## Preferred Languages

We prefer all communications to be in English.

## Policy

Microsoft follows the principle of [Coordinated Vulnerability Disclosure](https://aka.ms/opensource/security/cvd).

<!-- END MICROSOFT SECURITY.MD BLOCK -->



================================================
FILE: standalone.props
================================================
<Project>
  <PropertyGroup>
    <!-- The NuGet versions of dependencies to build against. -->
    <WindowsSdkPackageVersion>10.0.22621.42</WindowsSdkPackageVersion>
    <WindowsAppSdkPackageVersion>1.7.250513003</WindowsAppSdkPackageVersion>
    <MicrosoftNETCoreUniversalWindowsPlatformVersion>6.2.11</MicrosoftNETCoreUniversalWindowsPlatformVersion>
    <GraphicsWin2DVersion>1.3.2</GraphicsWin2DVersion>
    <ColorCodeVersion>2.0.15</ColorCodeVersion>
    <CommunityToolkitWinUIVersion>8.2.250402</CommunityToolkitWinUIVersion>
    <MicrosoftCsWinRTPackageVersion>2.2.0</MicrosoftCsWinRTPackageVersion>
    <!-- We have multiple projects in the same directory, which means we need to separate their output paths-->
    <BaseIntermediateOutputPath>obj\$(MSBuildProjectName)\</BaseIntermediateOutputPath>
    <BaseOutputPath>bin\$(MSBuildProjectName)\</BaseOutputPath>
    <!--
         For Desktop, the .NET SDK automatically includes every .cs file in the project directory.  It normally
         also excludes items under the obj/bin folders based on the value of BaseIntermediateOutputPath/BaseOutputPath.
         However, because we overwrite those to output to subdirectories, the outputs of the UWP WinUI Gallery
         are erroneously included.  Explicitly exclude them here
    -->
    <DefaultItemExcludes>obj\**;bin\**;$(DefaultItemExcludes)</DefaultItemExcludes>
    <!-- Where to place the files generated from CSWinRT from WinUIGallery.Desktop.-->
    <GeneratedFilesDir>obj\generated</GeneratedFilesDir>
  </PropertyGroup>
</Project>


================================================
FILE: WinUIGallery.DesktopWap.sln
================================================
﻿
Microsoft Visual Studio Solution File, Format Version 12.00
# Visual Studio Version 17
VisualStudioVersion = 17.1.32319.34
MinimumVisualStudioVersion = 10.0.40219.1
Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "Solution Items", "Solution Items", "{A98961E3-CB85-4AFC-990C-FD9F57043E7D}"
	ProjectSection(SolutionItems) = preProject
		..\Directory.Build.props = ..\Directory.Build.props
	EndProjectSection
EndProject
Project("{C7167F0D-BC9F-4E6E-AFE1-012C56B48DB5}") = "WinUIGallery.DesktopWap.Package", "WinUIGallery\WinUIGallery.DesktopWap.Package.wapproj", "{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "WinUIGallery", "WinUIGallery\WinUIGallery.csproj", "{D78F3B56-340D-44F0-9AF1-320D473BA611}"
EndProject
Global
	GlobalSection(SolutionConfigurationPlatforms) = preSolution
		Debug|ARM64 = Debug|ARM64
		Debug|x64 = Debug|x64
		Debug|x86 = Debug|x86
		Release|ARM64 = Release|ARM64
		Release|x64 = Release|x64
		Release|x86 = Release|x86
	EndGlobalSection
	GlobalSection(ProjectConfigurationPlatforms) = postSolution
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|ARM64.Build.0 = Debug|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|ARM64.Deploy.0 = Debug|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x64.ActiveCfg = Debug|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x64.Build.0 = Debug|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x64.Deploy.0 = Debug|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x86.ActiveCfg = Debug|x86
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x86.Build.0 = Debug|x86
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Debug|x86.Deploy.0 = Debug|x86
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|ARM64.ActiveCfg = Release|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|ARM64.Build.0 = Release|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|ARM64.Deploy.0 = Release|ARM64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x64.ActiveCfg = Release|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x64.Build.0 = Release|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x64.Deploy.0 = Release|x64
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x86.ActiveCfg = Release|x86
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x86.Build.0 = Release|x86
		{4C7B20D7-5F5C-440E-8DA3-B19A328CC8BD}.Release|x86.Deploy.0 = Release|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64.Build.0 = Debug|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x64.ActiveCfg = Debug|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x64.Build.0 = Debug|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x86.ActiveCfg = Debug|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x86.Build.0 = Debug|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64.ActiveCfg = Release|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64.Build.0 = Release|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x64.ActiveCfg = Release|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x64.Build.0 = Release|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x86.ActiveCfg = Release|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x86.Build.0 = Release|x86
	EndGlobalSection
	GlobalSection(SolutionProperties) = preSolution
		HideSolutionNode = FALSE
	EndGlobalSection
	GlobalSection(ExtensibilityGlobals) = postSolution
		SolutionGuid = {5B033CDA-6491-405C-A05B-CEE6AC4060B9}
	EndGlobalSection
EndGlobal



================================================
FILE: WinUIGallery.sln
================================================
﻿
Microsoft Visual Studio Solution File, Format Version 12.00
# Visual Studio Version 17
VisualStudioVersion = 17.1.32319.34
MinimumVisualStudioVersion = 10.0.40219.1
Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "Solution Items", "Solution Items", "{A98961E3-CB85-4AFC-990C-FD9F57043E7D}"
	ProjectSection(SolutionItems) = preProject
		..\Directory.Build.props = ..\Directory.Build.props
	EndProjectSection
EndProject
Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "tests", "tests", "{DDB4EF12-CC4E-5E88-E6FC-71A802F4DE97}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "WinUIGallery", "WinUIGallery\WinUIGallery.csproj", "{D78F3B56-340D-44F0-9AF1-320D473BA611}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "WinUIGallery.UnitTests", "tests\WinUIGallery.UnitTests\WinUIGallery.UnitTests.csproj", "{94B9B3F5-AF8E-4401-876B-115C44986161}"
EndProject
Project("{FAE04EC0-301F-11D3-BF4B-00C04F79EFBC}") = "WinUIGallery.UITests", "tests\WinUIGallery.UITests\WinUIGallery.UITests.csproj", "{8ED42919-1635-44E4-A670-9329B07F1398}"
EndProject
Global
	GlobalSection(SolutionConfigurationPlatforms) = preSolution
		Debug|ARM64 = Debug|ARM64
		Debug|ARM64EC = Debug|ARM64EC
		Debug|x64 = Debug|x64
		Debug|x86 = Debug|x86
		Debug-Unpackaged|ARM64 = Debug-Unpackaged|ARM64
		Debug-Unpackaged|ARM64EC = Debug-Unpackaged|ARM64EC
		Debug-Unpackaged|x64 = Debug-Unpackaged|x64
		Debug-Unpackaged|x86 = Debug-Unpackaged|x86
		Preview|ARM64 = Preview|ARM64
		Preview|ARM64EC = Preview|ARM64EC
		Preview|x64 = Preview|x64
		Preview|x86 = Preview|x86
		Release|ARM64 = Release|ARM64
		Release|ARM64EC = Release|ARM64EC
		Release|x64 = Release|x64
		Release|x86 = Release|x86
		Release-Unpackaged|ARM64 = Release-Unpackaged|ARM64
		Release-Unpackaged|ARM64EC = Release-Unpackaged|ARM64EC
		Release-Unpackaged|x64 = Release-Unpackaged|x64
		Release-Unpackaged|x86 = Release-Unpackaged|x86
		Sideload|ARM64 = Sideload|ARM64
		Sideload|ARM64EC = Sideload|ARM64EC
		Sideload|x64 = Sideload|x64
		Sideload|x86 = Sideload|x86
		Stable|ARM64 = Stable|ARM64
		Stable|ARM64EC = Stable|ARM64EC
		Stable|x64 = Stable|x64
		Stable|x86 = Stable|x86
		Store|ARM64 = Store|ARM64
		Store|ARM64EC = Store|ARM64EC
		Store|x64 = Store|x64
		Store|x86 = Store|x86
	EndGlobalSection
	GlobalSection(ProjectConfigurationPlatforms) = postSolution
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64.Build.0 = Debug|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64.Deploy.0 = Debug|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64EC.ActiveCfg = Debug|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64EC.Build.0 = Debug|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|ARM64EC.Deploy.0 = Debug|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x64.ActiveCfg = Debug|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x64.Build.0 = Debug|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x64.Deploy.0 = Debug|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x86.ActiveCfg = Debug|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x86.Build.0 = Debug|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug|x86.Deploy.0 = Debug|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|ARM64.ActiveCfg = Debug-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|ARM64.Build.0 = Debug-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|ARM64EC.ActiveCfg = Debug-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|ARM64EC.Build.0 = Debug-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|ARM64EC.Deploy.0 = Debug-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|x64.ActiveCfg = Debug-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|x64.Build.0 = Debug-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|x86.ActiveCfg = Debug-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Debug-Unpackaged|x86.Build.0 = Debug-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|ARM64.ActiveCfg = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|ARM64.Build.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|ARM64.Deploy.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|ARM64EC.ActiveCfg = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|ARM64EC.Build.0 = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x64.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x64.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x64.Deploy.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x86.ActiveCfg = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x86.Build.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Preview|x86.Deploy.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64.ActiveCfg = Release|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64.Build.0 = Release|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64.Deploy.0 = Release|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64EC.ActiveCfg = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64EC.Build.0 = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|ARM64EC.Deploy.0 = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x64.ActiveCfg = Release|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x64.Build.0 = Release|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x64.Deploy.0 = Release|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x86.ActiveCfg = Release|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x86.Build.0 = Release|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release|x86.Deploy.0 = Release|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|ARM64.ActiveCfg = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|ARM64.Build.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|ARM64EC.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|ARM64EC.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|ARM64EC.Deploy.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|x64.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|x64.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|x86.ActiveCfg = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Release-Unpackaged|x86.Build.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|ARM64.ActiveCfg = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|ARM64.Build.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|ARM64.Deploy.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|ARM64EC.ActiveCfg = Debug|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|ARM64EC.Build.0 = Debug|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x64.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x64.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x64.Deploy.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x86.ActiveCfg = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x86.Build.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Sideload|x86.Deploy.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|ARM64.ActiveCfg = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|ARM64.Build.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|ARM64.Deploy.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|ARM64EC.ActiveCfg = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|ARM64EC.Build.0 = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x64.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x64.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x64.Deploy.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x86.ActiveCfg = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x86.Build.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Stable|x86.Deploy.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|ARM64.ActiveCfg = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|ARM64.Build.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|ARM64.Deploy.0 = Release-Unpackaged|ARM64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|ARM64EC.ActiveCfg = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|ARM64EC.Build.0 = Release|ARM64EC
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x64.ActiveCfg = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x64.Build.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x64.Deploy.0 = Release-Unpackaged|x64
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x86.ActiveCfg = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x86.Build.0 = Release-Unpackaged|x86
		{D78F3B56-340D-44F0-9AF1-320D473BA611}.Store|x86.Deploy.0 = Release-Unpackaged|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64.Build.0 = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64.Deploy.0 = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64EC.ActiveCfg = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64EC.Build.0 = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|ARM64EC.Deploy.0 = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x64.ActiveCfg = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x64.Build.0 = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x64.Deploy.0 = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x86.ActiveCfg = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x86.Build.0 = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug|x86.Deploy.0 = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|ARM64.ActiveCfg = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|ARM64.Build.0 = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|ARM64.Deploy.0 = Debug|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|ARM64EC.ActiveCfg = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|ARM64EC.Build.0 = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x64.ActiveCfg = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x64.Build.0 = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x64.Deploy.0 = Debug|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x86.ActiveCfg = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x86.Build.0 = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Debug-Unpackaged|x86.Deploy.0 = Debug|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|ARM64EC.ActiveCfg = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|ARM64EC.Build.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Preview|x86.Deploy.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64EC.ActiveCfg = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64EC.Build.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|ARM64EC.Deploy.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release|x86.Deploy.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|ARM64EC.ActiveCfg = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|ARM64EC.Build.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Release-Unpackaged|x86.Deploy.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|ARM64EC.ActiveCfg = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|ARM64EC.Build.0 = Debug|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Sideload|x86.Deploy.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|ARM64EC.ActiveCfg = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|ARM64EC.Build.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Stable|x86.Deploy.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|ARM64.ActiveCfg = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|ARM64.Build.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|ARM64.Deploy.0 = Release|ARM64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|ARM64EC.ActiveCfg = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|ARM64EC.Build.0 = Release|ARM64EC
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x64.ActiveCfg = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x64.Build.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x64.Deploy.0 = Release|x64
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x86.ActiveCfg = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x86.Build.0 = Release|x86
		{94B9B3F5-AF8E-4401-876B-115C44986161}.Store|x86.Deploy.0 = Release|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|ARM64.ActiveCfg = Debug|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|ARM64.Build.0 = Debug|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|ARM64EC.ActiveCfg = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|ARM64EC.Build.0 = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|x64.ActiveCfg = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|x64.Build.0 = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|x86.ActiveCfg = Debug|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug|x86.Build.0 = Debug|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|ARM64.ActiveCfg = Debug|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|ARM64.Build.0 = Debug|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|ARM64EC.ActiveCfg = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|ARM64EC.Build.0 = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|x64.ActiveCfg = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|x64.Build.0 = Debug|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|x86.ActiveCfg = Debug|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Debug-Unpackaged|x86.Build.0 = Debug|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|ARM64.ActiveCfg = Preview|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|ARM64.Build.0 = Preview|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|ARM64EC.ActiveCfg = Preview|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|ARM64EC.Build.0 = Preview|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|x64.ActiveCfg = Preview|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|x64.Build.0 = Preview|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|x86.ActiveCfg = Preview|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Preview|x86.Build.0 = Preview|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|ARM64.ActiveCfg = Release|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|ARM64.Build.0 = Release|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|ARM64EC.ActiveCfg = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|ARM64EC.Build.0 = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|x64.ActiveCfg = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|x64.Build.0 = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|x86.ActiveCfg = Release|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release|x86.Build.0 = Release|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|ARM64.ActiveCfg = Release|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|ARM64.Build.0 = Release|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|ARM64EC.ActiveCfg = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|ARM64EC.Build.0 = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|x64.ActiveCfg = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|x64.Build.0 = Release|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|x86.ActiveCfg = Release|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Release-Unpackaged|x86.Build.0 = Release|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|ARM64.ActiveCfg = Sideload|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|ARM64.Build.0 = Sideload|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|ARM64EC.ActiveCfg = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|ARM64EC.Build.0 = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|x64.ActiveCfg = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|x64.Build.0 = Sideload|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|x86.ActiveCfg = Sideload|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Sideload|x86.Build.0 = Sideload|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|ARM64.ActiveCfg = Stable|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|ARM64.Build.0 = Stable|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|ARM64EC.ActiveCfg = Stable|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|ARM64EC.Build.0 = Stable|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|x64.ActiveCfg = Stable|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|x64.Build.0 = Stable|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|x86.ActiveCfg = Stable|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Stable|x86.Build.0 = Stable|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|ARM64.ActiveCfg = Store|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|ARM64.Build.0 = Store|ARM64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|ARM64EC.ActiveCfg = Store|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|ARM64EC.Build.0 = Store|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|x64.ActiveCfg = Store|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|x64.Build.0 = Store|x64
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|x86.ActiveCfg = Store|x86
		{8ED42919-1635-44E4-A670-9329B07F1398}.Store|x86.Build.0 = Store|x86
	EndGlobalSection
	GlobalSection(SolutionProperties) = preSolution
		HideSolutionNode = FALSE
	EndGlobalSection
	GlobalSection(NestedProjects) = preSolution
		{94B9B3F5-AF8E-4401-876B-115C44986161} = {DDB4EF12-CC4E-5E88-E6FC-71A802F4DE97}
		{8ED42919-1635-44E4-A670-9329B07F1398} = {DDB4EF12-CC4E-5E88-E6FC-71A802F4DE97}
	EndGlobalSection
	GlobalSection(ExtensibilityGlobals) = postSolution
		SolutionGuid = {5B033CDA-6491-405C-A05B-CEE6AC4060B9}
	EndGlobalSection
EndGlobal



================================================
FILE: .editorconfig
================================================
# Remove the line below if you want to inherit .editorconfig settings from higher directories
root = true

# C# files
[*.cs]

#### Core EditorConfig Options ####

# Indentation and spacing
indent_size = 4
indent_style = space
tab_width = 4

# New line preferences
end_of_line = crlf
insert_final_newline = false

#### .NET Coding Conventions ####

# Organize usings
dotnet_separate_import_directive_groups = false
dotnet_sort_system_directives_first = false
file_header_template = Copyright (c) Microsoft Corporation. All rights reserved.\nLicensed under the MIT License.
dotnet_diagnostic.IDE0073.severity = warning
dotnet_diagnostic.IDE0005.severity = warning
dotnet_diagnostic.IDE0008.severity = none

dotnet_diagnostic.IDE0160.severity = none

# Closing parenthesis should be spaced correctly: "foo()!"
dotnet_diagnostic.SA1009.severity = none

# Hide warnings when using the new() expression from C# 9.
dotnet_diagnostic.SA1000.severity = none

dotnet_diagnostic.SA1010.severity = none
dotnet_diagnostic.SA1011.severity = none
dotnet_diagnostic.SA1101.severity = none

# Hide warnings when accessing properties without "this".
dotnet_diagnostic.SA1101.severity = none
dotnet_diagnostic.SA1118.severity = none
dotnet_diagnostic.SA1200.severity = none
dotnet_diagnostic.SA1201.severity = none
dotnet_diagnostic.SA1202.severity = none
dotnet_diagnostic.SA1204.severity = none
dotnet_diagnostic.SA1206.severity = none
dotnet_diagnostic.SA1309.severity = none
dotnet_diagnostic.SA1310.severity = none

# Hide warnings for record parameters.
dotnet_diagnostic.SA1313.severity = none

# TypeParameterNamesMustBeginWithT: We do have a few templates that don't start with T. We need to double check that changing this is not a breaking change. If not, we can re-enable this.
dotnet_diagnostic.SA1314.severity = none

# UseTrailingCommasInMultiLineInitializers: This would also mean a lot of changes at the end of all multiline initializers. It's also debatable if we want this or not.
dotnet_diagnostic.SA1413.severity = none

dotnet_diagnostic.SA1407.severity = none
dotnet_diagnostic.SA1402.severity = none

dotnet_diagnostic.SA1600.severity = none
dotnet_diagnostic.SA1601.severity = none
dotnet_diagnostic.SA1602.severity = none
dotnet_diagnostic.SA1611.severity = none

# DocumentationTextMustEndWithAPeriod: Let's enable this rule back when we shift to WinUI3 (v8.x). If we do it now, it would mean more than 400 file changes.
dotnet_diagnostic.SA1629.severity = none

dotnet_diagnostic.SA1633.severity = none
dotnet_diagnostic.SA1634.severity = none
dotnet_diagnostic.SA1652.severity = none
dotnet_diagnostic.SA1649.severity = none

dotnet_diagnostic.SA1210.severity = warning
dotnet_diagnostic.SA1208.severity = warning
dotnet_diagnostic.SA1516.severity = none

dotnet_diagnostic.CA1711.severity = none
dotnet_diagnostic.CA1852.severity = none
dotnet_diagnostic.CA1822.severity = none

# TODO: review this 2 rules
dotnet_diagnostic.CA1001.severity = none
dotnet_diagnostic.CA1816.severity = none

dotnet_diagnostic.CA2000.severity = warning

# RS2008: Enable analyzer release tracking
dotnet_diagnostic.RS2008.severity = none

# this. and Me. preferences
dotnet_style_qualification_for_event = false
dotnet_style_qualification_for_field = false
dotnet_style_qualification_for_method = false
dotnet_style_qualification_for_property = false

# Language keywords vs BCL types preferences
dotnet_style_predefined_type_for_locals_parameters_members = true
dotnet_style_predefined_type_for_member_access = true

# Parentheses preferences
dotnet_style_parentheses_in_arithmetic_binary_operators = always_for_clarity
dotnet_style_parentheses_in_other_binary_operators = always_for_clarity
dotnet_style_parentheses_in_other_operators = never_if_unnecessary
dotnet_style_parentheses_in_relational_binary_operators = always_for_clarity

# Modifier preferences
dotnet_style_require_accessibility_modifiers = for_non_interface_members

# Expression-level preferences
dotnet_style_coalesce_expression = true
dotnet_style_collection_initializer = true
dotnet_style_explicit_tuple_names = true
dotnet_style_namespace_match_folder = true
dotnet_style_null_propagation = true
dotnet_style_object_initializer = true
dotnet_style_operator_placement_when_wrapping = beginning_of_line
dotnet_style_prefer_auto_properties = true
dotnet_style_prefer_collection_expression = when_types_loosely_match
dotnet_style_prefer_compound_assignment = true
dotnet_style_prefer_conditional_expression_over_assignment = true
dotnet_style_prefer_conditional_expression_over_return = true
dotnet_style_prefer_foreach_explicit_cast_in_source = when_strongly_typed
dotnet_style_prefer_inferred_anonymous_type_member_names = true
dotnet_style_prefer_inferred_tuple_names = true
dotnet_style_prefer_is_null_check_over_reference_equality_method = true
dotnet_style_prefer_simplified_boolean_expressions = true
dotnet_style_prefer_simplified_interpolation = true

# Field preferences
dotnet_style_readonly_field = true

# Parameter preferences
dotnet_code_quality_unused_parameters = all

# Suppression preferences
dotnet_remove_unnecessary_suppression_exclusions = none

# New line preferences
dotnet_style_allow_multiple_blank_lines_experimental = true
dotnet_style_allow_statement_immediately_after_block_experimental = true

#### C# Coding Conventions ####

# var preferences
csharp_style_var_elsewhere = false
csharp_style_var_for_built_in_types = false
csharp_style_var_when_type_is_apparent = false

# Expression-bodied members
csharp_style_expression_bodied_accessors = true:silent
csharp_style_expression_bodied_constructors = false:silent
csharp_style_expression_bodied_indexers = true:silent
csharp_style_expression_bodied_lambdas = true:silent
csharp_style_expression_bodied_local_functions = false:silent
csharp_style_expression_bodied_methods = false:silent
csharp_style_expression_bodied_operators = false:silent
csharp_style_expression_bodied_properties = true:silent

# Pattern matching preferences
csharp_style_pattern_matching_over_as_with_null_check = true
csharp_style_pattern_matching_over_is_with_cast_check = true
csharp_style_prefer_extended_property_pattern = true
csharp_style_prefer_not_pattern = true
csharp_style_prefer_pattern_matching = true
csharp_style_prefer_switch_expression = true

# Null-checking preferences
csharp_style_conditional_delegate_call = true

# Modifier preferences
csharp_prefer_static_local_function = true
csharp_preferred_modifier_order = public,private,protected,internal,file,static,extern,new,virtual,abstract,sealed,override,readonly,unsafe,required,volatile,async
csharp_style_prefer_readonly_struct = true
csharp_style_prefer_readonly_struct_member = true

# Code-block preferences
csharp_prefer_braces = true:silent
csharp_prefer_simple_using_statement = true:suggestion
csharp_style_namespace_declarations = file_scoped:warning
csharp_style_prefer_method_group_conversion = true:silent
csharp_style_prefer_primary_constructors = true:suggestion
csharp_style_prefer_top_level_statements = true:silent

# Expression-level preferences
csharp_prefer_simple_default_expression = true
csharp_style_deconstructed_variable_declaration = true
csharp_style_implicit_object_creation_when_type_is_apparent = true
csharp_style_inlined_variable_declaration = true
csharp_style_prefer_index_operator = true
csharp_style_prefer_local_over_anonymous_function = true
csharp_style_prefer_null_check_over_type_check = true
csharp_style_prefer_range_operator = true
csharp_style_prefer_tuple_swap = true
csharp_style_prefer_utf8_string_literals = true
csharp_style_throw_expression = true
csharp_style_unused_value_assignment_preference = discard_variable
csharp_style_unused_value_expression_statement_preference = discard_variable

# 'using' directive preferences
csharp_using_directive_placement = outside_namespace:silent

# New line preferences
csharp_style_allow_blank_line_after_colon_in_constructor_initializer_experimental = true
csharp_style_allow_blank_line_after_token_in_arrow_expression_clause_experimental = true
csharp_style_allow_blank_line_after_token_in_conditional_expression_experimental = true
csharp_style_allow_blank_lines_between_consecutive_braces_experimental = true
csharp_style_allow_embedded_statements_on_same_line_experimental = true

#### C# Formatting Rules ####

# New line preferences
csharp_new_line_before_catch = true
csharp_new_line_before_else = true
csharp_new_line_before_finally = true
csharp_new_line_before_members_in_anonymous_types = true
csharp_new_line_before_members_in_object_initializers = true
csharp_new_line_before_open_brace = all
csharp_new_line_between_query_expression_clauses = true

# Indentation preferences
csharp_indent_block_contents = true
csharp_indent_braces = false
csharp_indent_case_contents = true
csharp_indent_case_contents_when_block = true
csharp_indent_labels = one_less_than_current
csharp_indent_switch_labels = true

# Space preferences
csharp_space_after_cast = false
csharp_space_after_colon_in_inheritance_clause = true
csharp_space_after_comma = true
csharp_space_after_dot = false
csharp_space_after_keywords_in_control_flow_statements = true
csharp_space_after_semicolon_in_for_statement = true
csharp_space_around_binary_operators = before_and_after
csharp_space_around_declaration_statements = false
csharp_space_before_colon_in_inheritance_clause = true
csharp_space_before_comma = false
csharp_space_before_dot = false
csharp_space_before_open_square_brackets = false
csharp_space_before_semicolon_in_for_statement = false
csharp_space_between_empty_square_brackets = false
csharp_space_between_method_call_empty_parameter_list_parentheses = false
csharp_space_between_method_call_name_and_opening_parenthesis = false
csharp_space_between_method_call_parameter_list_parentheses = false
csharp_space_between_method_declaration_empty_parameter_list_parentheses = false
csharp_space_between_method_declaration_name_and_open_parenthesis = false
csharp_space_between_method_declaration_parameter_list_parentheses = false
csharp_space_between_parentheses = false
csharp_space_between_square_brackets = false

# Wrapping preferences
csharp_preserve_single_line_blocks = true
csharp_preserve_single_line_statements = true

#### Naming styles ####

# Naming rules

dotnet_naming_rule.interface_should_be_begins_with_i.severity = suggestion
dotnet_naming_rule.interface_should_be_begins_with_i.symbols = interface
dotnet_naming_rule.interface_should_be_begins_with_i.style = begins_with_i

dotnet_naming_rule.types_should_be_pascal_case.severity = suggestion
dotnet_naming_rule.types_should_be_pascal_case.symbols = types
dotnet_naming_rule.types_should_be_pascal_case.style = pascal_case

dotnet_naming_rule.non_field_members_should_be_pascal_case.severity = suggestion
dotnet_naming_rule.non_field_members_should_be_pascal_case.symbols = non_field_members
dotnet_naming_rule.non_field_members_should_be_pascal_case.style = pascal_case

# Symbol specifications

dotnet_naming_symbols.interface.applicable_kinds = interface
dotnet_naming_symbols.interface.applicable_accessibilities = public, internal, private, protected, protected_internal, private_protected
dotnet_naming_symbols.interface.required_modifiers =

dotnet_naming_symbols.types.applicable_kinds = class, struct, interface, enum
dotnet_naming_symbols.types.applicable_accessibilities = public, internal, private, protected, protected_internal, private_protected
dotnet_naming_symbols.types.required_modifiers =

dotnet_naming_symbols.non_field_members.applicable_kinds = property, event, method
dotnet_naming_symbols.non_field_members.applicable_accessibilities = public, internal, private, protected, protected_internal, private_protected
dotnet_naming_symbols.non_field_members.required_modifiers =

# Naming styles

dotnet_naming_style.pascal_case.required_prefix =
dotnet_naming_style.pascal_case.required_suffix =
dotnet_naming_style.pascal_case.word_separator =
dotnet_naming_style.pascal_case.capitalization = pascal_case

dotnet_naming_style.begins_with_i.required_prefix = I
dotnet_naming_style.begins_with_i.required_suffix =
dotnet_naming_style.begins_with_i.word_separator =
dotnet_naming_style.begins_with_i.capitalization = pascal_case

# CA1859: Use concrete types when possible for improved performance
dotnet_diagnostic.CA1859.severity = suggestion

[*.{cs,vb}]
dotnet_style_operator_placement_when_wrapping = beginning_of_line
tab_width = 4
indent_size = 4
end_of_line = crlf
dotnet_style_coalesce_expression = true:suggestion
dotnet_style_null_propagation = true:suggestion
dotnet_style_prefer_is_null_check_over_reference_equality_method = true:suggestion
dotnet_style_prefer_auto_properties = true:silent
dotnet_style_object_initializer = true:suggestion
dotnet_style_collection_initializer = true:suggestion
dotnet_style_prefer_simplified_boolean_expressions = true:suggestion
dotnet_style_prefer_conditional_expression_over_assignment = true:suggestion
dotnet_style_prefer_conditional_expression_over_return = true:suggestion
dotnet_style_explicit_tuple_names = true:suggestion
dotnet_style_prefer_inferred_tuple_names = true:suggestion
dotnet_style_prefer_inferred_anonymous_type_member_names = true:suggestion
dotnet_style_prefer_compound_assignment = true:suggestion
dotnet_style_prefer_simplified_interpolation = true:suggestion
dotnet_style_prefer_collection_expression = when_types_loosely_match:suggestion
dotnet_style_namespace_match_folder = true:suggestion

# IDE0046: Convert to conditional expression
dotnet_diagnostic.IDE0046.severity = suggestion

# IDE0045: Convert to conditional expression
dotnet_diagnostic.IDE0045.severity = suggestion

# Trimmer settings
dotnet_diagnostic.IL2059.severity = suggestion


================================================
FILE: docs/images/WinUIGalleryLanding.PNG
================================================
[Non-text file]


================================================
FILE: packagestore/readme.md
================================================
Local source for packages. Places nupkg files in this directory to test them out before uploading.


================================================
FILE: tests/WinUIGallery.UITests/README.md
================================================
# UI Tests with WinAppDriver

The UI Test repository is a collection of WinAppDriver-based test scenarios that cover basic interactions with WinUI 3 controls. See the [Windows Platform controls reference](https://learn.microsoft.com/windows/apps/design/controls/) for more information on available controls.

The test scenarios are written to test the controls in the WinUI 3 Gallery app. The procedure below outlines the steps needed to build and deploy WinUI 3 Gallery and WinAppDriver to run the UI Tests. These steps mirror what azure-pipelines.yml does in pipeline runs.

## Deploy WinUI 3 Gallery

The easiest way to deploy the WinUI 3 Gallery for unit test execution is to simply build WinUIGallery.sln and F5 deploy it from within Visual Studio.  Alternatively, the following commands can be used for automation.

1. Generate the test signing certificate:

```shell
    PS> .\build\GenerateTestPfx.ps1
```

1. Build and publish the WinUI 3 Gallery from the command line, e.g.:

```shell
    >dotnet.exe publish WinUIGallery.sln /p:AppxPackageDir=AppxPackages\ /p:platform=x64 /p:PublishProfile=./WinUIGallery/Properties/PublishProfiles/win-x64.pubxml
```

1. Locate the WinUI 3 Gallery package output folder from above and deploy for testing:

```shell
    PS> .\WinUIGallery\AppxPackages\WinUIGallery.Desktop_Test\Install.ps1
```

## Run WinAppDriver

The test runner (vstest.console.exe and VS Test Explorer) should automatically launch WinAppDriver. Alternatively, it can be launched manually to observe diagnostic output as follows:

1. Download and install the latest version of WinAppDriver from [here](https://github.com/microsoft/WinAppDriver/releases)

1. Run WinAppDriver:

```shell
    >C:\Program Files (x86)\Windows Application Driver\WinAppDriver.exe
```

## Build and run/debug Tests

The easiest way to run/debug the UI tests is with Visual Studio, as follows:

   * Open `WinUIGallery.sln` in Visual Studio
   * Select **Test** > **Windows** > **Test Explorer**
   * Select **Run All** on the test pane or through menu **Test** > **Run** > **All Tests**

Once the project is successfully built, you can use the **Test Explorer** to choose  test scenarios to run/debug

Alternatively, the following commands can be used for automation:

1. Build UITests:

```shell
    >dotnet build WinUIGallery.sln
    --or--
    >msbuild WinUIGallery.sln
```

1. Run test cases built above on command line:

```shell
    >dotnet test .\WinUIGallery\WinUIGallery.UITests.csproj
    --or--
    >vstest.console.exe .\WinUIGallery.UITests\bin\x64\Debug\net7.0\WinUIGallery.UITests.dll
```

## Test output

In either scenario above (cmdline or VS), if the tests run successfully, you should see:

* The WinUI 3 Gallery launch and run with automated UI interactions
* vstest.console.exe spew or Test Explorer indications of test case status
* Optionally, WinAppDriver console spew indicating successful launch of the test app

## Adding/Updating Test Scenarios

Please follow the guidelines below to maintain test reliability and reduce test execution time:

1. Provide a complete set of interactions (if applicable) for each new control
1. Aim for simple and reliable scenario using the least amount of test steps



================================================
FILE: tests/WinUIGallery.UITests/AxeHelper.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Axe.Windows.Automation;
using Axe.Windows.Core.Enums;
using Microsoft.VisualStudio.TestTools.UnitTesting;
using System.Diagnostics;
using System.Linq;

namespace WinUIGallery.UITests;

public class AxeHelper
{
    public static IScanner AccessibilityScanner;

    internal static void InitializeAxe()
    {
        var processes = Process.GetProcessesByName("WinUIGallery");
        Assert.IsTrue(processes.Length > 0);

        var config = Config.Builder.ForProcessId(processes[0].Id).Build();

        AccessibilityScanner = ScannerFactory.CreateScanner(config);
    }

    public static void AssertNoAccessibilityErrors()
    {
        // Bug 1474: Disabling Rules NameReasonableLength and BoundingRectangleNotNull temporarily
        var testResult = AccessibilityScanner.Scan(null).WindowScanOutputs.SelectMany(output => output.Errors)
            .Where(rule => rule.Rule.ID != RuleId.NameIsInformative)
            .Where(rule => rule.Rule.ID != RuleId.NameExcludesControlType)
            .Where(rule => rule.Rule.ID != RuleId.NameExcludesLocalizedControlType)
            .Where(rule => rule.Rule.ID != RuleId.SiblingUniqueAndFocusable)
            .Where(rule => rule.Rule.ID != RuleId.NameReasonableLength)
            .Where(rule => rule.Rule.ID != RuleId.BoundingRectangleNotNull)
            .Where(rule => rule.Rule.ID != RuleId.BoundingRectangleNotNullListViewXAML)
            .Where(rule => rule.Rule.ID != RuleId.BoundingRectangleNotNullTextBlockXAML)
            .Where(rule => rule.Rule.ID != RuleId.NameNotNull)
            .Where(rule => rule.Rule.ID != RuleId.ChromiumComponentsShouldUseWebScanner);

        if (testResult.Any())
        {
            var mappedResult = testResult.Select(result =>
            "Element " + result.Element.Properties["ControlType"] + " violated rule '" + result.Rule.Description + "'.");
            Assert.Fail("Failed with the following accessibility errors \r\n" + string.Join("\r\n", mappedResult));
        }
    }
}



================================================
FILE: tests/WinUIGallery.UITests/SampleTestTemplate.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using System.Threading;
using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests;

[TestClass]
public class SampleTestTemplate : TestBase
{

    private static WindowsElement element1 = null;
    private static WindowsElement element2 = null;

    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("MyControlPage");
        Thread.Sleep(1000);
        element1 = Session.FindElementByAccessibilityId("Element Locator");
        Assert.IsNotNull(element1);
        element2 = Session.FindElementByAccessibilityId("Element Locator");
        Assert.IsNotNull(element2);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/SessionManager.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using Microsoft.VisualStudio.TestTools.UnitTesting.Logging;
using OpenQA.Selenium.Appium;
using OpenQA.Selenium.Appium.Windows;
using System;
using System.Diagnostics;
using System.IO;
using System.Threading;

namespace WinUIGallery.UITests;

[TestClass]
public class SessionManager
{
    private const string WindowsApplicationDriverUrl = "http://127.0.0.1:4723";
    private static readonly string[] WinUIGalleryAppIDs = [
        // WinUI 3 Gallery apps built in the lab
        "Microsoft.WinUI3ControlsGallery.Debug_grv3cx5qrw0gp!App",
        "Microsoft.WinUI3ControlsGallery_grv3cx5qrw0gp!App",
        // WinUI 3 Gallery apps built locally
        "Microsoft.WinUI3ControlsGallery.Debug_8wekyb3d8bbwe!App",
        "Microsoft.WinUI3ControlsGallery_8wekyb3d8bbwe!App"
    ];

    private static uint appIdIndex = 0;

    private static WindowsDriver<WindowsElement> _session;
    public static WindowsDriver<WindowsElement> Session
    {
        get
        {
            if (_session is null)
            {
                Setup(null);
            }
            return _session;
        }
    }

    public static TestContext TestContext { get; set; }

    private static string screenshotDirectory;

    [AssemblyInitialize]
    public static void Setup(TestContext context)
    {
        TestContext = context;

        string outputDirectory;

        if (context.Properties.Contains("ArtifactStagingDirectory"))
        {
            outputDirectory = context.Properties["ArtifactStagingDirectory"].ToString();
        }
        else
        {
            outputDirectory = context.TestRunResultsDirectory;
        }

        screenshotDirectory = Path.Combine(outputDirectory, "Screenshots");

        if (_session is null)
        {
            int timeoutCount = 50;

            TryInitializeSession();
            if (_session is null)
            {
                // WinAppDriver is probably not running, so lets start it!
                string winAppDriverX64Path = Path.Join(Environment.GetEnvironmentVariable("ProgramFiles"), "Windows Application Driver", "WinAppDriver.exe");
                string winAppDriverX86Path = Path.Join(Environment.GetEnvironmentVariable("ProgramFiles(x86)"), "Windows Application Driver", "WinAppDriver.exe");

                if (File.Exists(winAppDriverX64Path))
                {
                    Process.Start(winAppDriverX64Path);
                }
                else if (File.Exists(winAppDriverX86Path))
                {
                    Process.Start(winAppDriverX86Path);
                }
                else
                {
                    throw new Exception("Unable to start WinAppDriver since no suitable location was found.");
                }

                Thread.Sleep(10000);
                TryInitializeSession();
            }

            while (_session is null && timeoutCount < 1000 * 4)
            {
                TryInitializeSession();
                Thread.Sleep(timeoutCount);
                timeoutCount *= 2;
            }

            Thread.Sleep(3000);
            Assert.IsNotNull(_session);
            Assert.IsNotNull(_session.SessionId);
            AxeHelper.InitializeAxe();

            // Dismiss the disclaimer window that may pop up on the very first application launch
            // If the disclaimer is not found, this throws an exception, so lets catch that
            try
            {
                _session.FindElementByName("Disclaimer").FindElementByName("Accept").Click();
            }
            catch (OpenQA.Selenium.WebDriverException) { }

            // Wait if something is still animating in the visual tree
            _session.Manage().Timeouts().ImplicitWait = TimeSpan.FromSeconds(3);
            _session.Manage().Window.Maximize();
        }
    }

    [AssemblyCleanup()]
    public static void TestRunTearDown()
    {
        TearDown();
    }

    public static void TearDown()
    {
        if (_session is not null)
        {
            _session.CloseApp();
            _session.Quit();
            _session = null;
        }
    }

    public static void TakeScreenshot(string fileName)
    {
        Directory.CreateDirectory(screenshotDirectory);
        _session.GetScreenshot().SaveAsFile(Path.Join(screenshotDirectory, $"{fileName}.png"));
    }

    public static void DumpTree()
    {
        Logger.LogMessage("=================");
        Logger.LogMessage("Begin visual tree");
        Logger.LogMessage("=================");

        foreach (WindowsElement element in _session.FindElementsByXPath("/*"))
        {
            DumpTreeHelper(element, 0);
        }

        Logger.LogMessage("===============");
        Logger.LogMessage("End visual tree");
        Logger.LogMessage("===============");
    }

    private static void DumpTreeHelper(WindowsElement root, int depth)
    {
        string indent = string.Empty;

        for (int i = 0; i < depth; i++)
        {
            indent += "|";

            if (i == depth - 1)
            {
                indent += "-";
            }
            else
            {
                indent += " ";
            }
        }

        if (root.Displayed && !string.IsNullOrEmpty(root.TagName))
        {
            string message;

            if (string.IsNullOrEmpty(root.Text))
            {
                message = $"{indent}{root.TagName}";
            }
            else
            {
                message = $"{indent}{root.TagName} [{root.Text}]";
            }

            Logger.LogMessage(message.Replace("{", "{{").Replace("}", "}}"));
        }

        foreach (WindowsElement child in root.FindElementsByXPath("*/*"))
        {
            DumpTreeHelper(child, root.Displayed ? depth + 1 : depth);
        }
    }

    private static void TryInitializeSession()
    {
        AppiumOptions appiumOptions = new();
        appiumOptions.AddAdditionalCapability("app", WinUIGalleryAppIDs[appIdIndex]);
        appiumOptions.AddAdditionalCapability("deviceName", "WindowsPC");
        try
        {
            _session = new WindowsDriver<WindowsElement>(new Uri(WindowsApplicationDriverUrl), appiumOptions);
        }
        catch (OpenQA.Selenium.WebDriverException exc)
        {
            // Use next app ID since the current one was failing
            if (exc.Message.Contains("Package was not found"))
            {
                appIdIndex++;
            }
            else
            {
                Console.WriteLine("Failed to update start driver, got exception:" + exc.Message);
            }
        }
    }
}



================================================
FILE: tests/WinUIGallery.UITests/TestBase.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;
using OpenQA.Selenium.Interactions;
using System.Threading;

namespace WinUIGallery.UITests;

public class TestBase
{
    public static WindowsDriver<WindowsElement> Session => SessionManager.Session;

    public static void OpenControlPage(string name)
    {
        var search = Session.FindElementByName("Search");
        search.Clear();

        search.SendKeys(name);
        GetElementByName(name).Click();

        Assert.IsNotNull(WaitForPageHeader(name), "Failed to find matching page header for page: " + name);
    }

    public static WindowsElement GetElementByName(string name)
    {
        for (int i = 0; i < 100; i++)
        {
            Thread.Sleep(50);
            var element = Session.FindElementByName(name);
            if (element != null)
            {
                return element;
            }
        }
        return null;
    }

    private static WindowsElement WaitForPageHeader(string name)
    {
        for (int i = 0; i < 100; i++)
        {
            var header = Session.FindElementByAccessibilityId("PageHeader");
            if (header != null && header.Text == name)
            {
                return header;
            }
            Thread.Sleep(50);
        }
        return null;
    }

    public static void TypeText(string text)
    {
        var actions = new Actions(Session);
        actions.SendKeys(text).Perform();
    }
}



================================================
FILE: tests/WinUIGallery.UITests/WinUIGallery.UITests.csproj
================================================
﻿<!--  Copyright (c) Microsoft Corporation. Licensed under the MIT License.  -->
<Project Sdk="Microsoft.NET.Sdk">

    <PropertyGroup>
        <TargetFramework>net8.0</TargetFramework>
        <RootNamespace>WinUIGallery.UITests</RootNamespace>
        <IsPackable>false</IsPackable>
        <Configurations>Debug;Release;Sideload;Stable;Preview;Store</Configurations>
        <Platforms>x86;x64;ARM64</Platforms>
        <RuntimeIdentifiers>win-x86;win-x64;win-arm64</RuntimeIdentifiers>
        <PublishProfile>win-$(Platform).pubxml</PublishProfile>
    </PropertyGroup>

    <ItemGroup>
        <PackageReference Include="Appium.WebDriver" Version="4.4.0" />
        <PackageReference Include="Axe.Windows" Version="2.4.1" />
        <PackageReference Include="Microsoft.NET.Test.Sdk" Version="17.5.0" />
        <PackageReference Include="MSTest.TestAdapter" Version="3.0.2" />
        <PackageReference Include="MSTest.TestFramework" Version="3.0.2" />
    </ItemGroup>

    <ItemGroup>
        <None Include="$(MSBuildThisFileDirectory)..\..\WinUIGallery\Samples\Data\ControlInfoData.json">
            <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
        </None>
    </ItemGroup>

</Project>



================================================
FILE: tests/WinUIGallery.UITests/Properties/launchSettings.json
================================================
{
  "profiles": {
    "WinUIGallery.UITests (Package)": {
      "commandName": "MsixPackage"
    },
    "WinUIGallery.UITests (Unpackaged)": {
      "commandName": "Project"
    }
  }
}


================================================
FILE: tests/WinUIGallery.UITests/Properties/PublishProfiles/win-arm64.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>ARM64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-arm64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-arm64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UITests/Properties/PublishProfiles/win-arm64ec.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UITests/Properties/PublishProfiles/win-x64.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UITests/Properties/PublishProfiles/win-x86.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x86</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x86</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x86</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UITests/Tests/AxeScanAllTests.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;
using System;
using System.Linq;
using System.Text.Json;
using System.Collections.Generic;
using System.Reflection;
using Newtonsoft.Json;
using Microsoft.VisualStudio.TestTools.UnitTesting.Logging;
using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class AxeScanAll : TestBase
{
    public static readonly string jsonUri = "ControlInfoData.json";
    public static new WindowsDriver<WindowsElement> Session => SessionManager.Session;

    public static string[] ExclusionList =
    [
        "WebView2", // 46668961: Web contents from WebView2 are throwing null BoundingRectangle errors.
        "Icons", // https://github.com/CommunityToolkit/Windows/issues/240 External toolkit SettingsExpander does not pass Axe testing
        // https://github.com/microsoft/axe-windows/issues/662
        // AxeWindowsAutomationException: Failed to get the root element(s) of the specified process error for following pages:
        "PersonPicture",
        "MapControl",
        "TabView"
    ];

    public class ControlInfoData
    {
        public List<Group> Groups { get; set; }
    }

    public class Group
    {
        [JsonProperty("UniqueId")]
        public string UniqueId { get; set; }

        [JsonProperty("Items")]
        public List<Item> Items { get; set; }
    }

    public class Item
    {
        [JsonProperty("UniqueId")]
        public string UniqueId { get; set; }
    }

    private static IEnumerable<object[]> TestData()
    {
        var testCases = new List<object[]>();

        string jsonContent = System.IO.File.ReadAllText(jsonUri);
        var controlInfoData = JsonConvert.DeserializeObject<ControlInfoData>(jsonContent);

        foreach (var group in controlInfoData.Groups)
        {
            var sectionName = group.UniqueId;

            // Select all row names within the current table
            var items = group.Items;

            foreach (var item in items)
            {
                var pageName = item.UniqueId;

                // Skip pages in the exclusion list.
                if (ExclusionList.Contains(pageName))
                {
                    continue;
                }
                testCases.Add([sectionName, pageName]);
            }
        }

        return testCases;
    }

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
    }

    [TestMethod]
    [DynamicData(nameof(TestData), DynamicDataSourceType.Method, DynamicDataDisplayName = nameof(GetCustomDynamicDataDisplayName))]
    [TestProperty("Description", "Scan pages in the WinUIGallery for accessibility issues.")]
    public void ValidatePageAccessibilityWithAxe(string sectionName, string pageName)
    {
        try
        {
            Logger.LogMessage($"Opening page \"{pageName}\".");

            // Click into page and check for accessibility issues.
            var page = Session.FindElementByAccessibilityId(pageName);
            page.Click();

            AxeHelper.AssertNoAccessibilityErrors();
        }
        catch (OpenQA.Selenium.WebDriverException exc)
        {
            if (exc.Message.Contains("element could not be located"))
            {
                try
                {
                    Logger.LogMessage($"Page not found. Opening section \"{sectionName}\" first.");

                    // If element is not found, expand tree view as it is nested.
                    var section = Session.FindElementByAccessibilityId(sectionName);
                    section.Click();

                    // wait for tree to expand
                    Thread.Sleep(1000);

                    // Click into page and check for accessibility issues.
                    var page = Session.FindElementByAccessibilityId(pageName);
                    page.Click();

                    AxeHelper.AssertNoAccessibilityErrors();
                }
                catch (OpenQA.Selenium.WebDriverException exc2)
                {
                    Logger.LogMessage($"Section \"{sectionName}\" not found either.");
                    Logger.LogMessage(exc2.Message);

                    SessionManager.DumpTree();
                    SessionManager.TakeScreenshot($"{sectionName}.{pageName}");

                    throw;
                }
            }
            else if (exc.Message.Contains("Currently selected window has been closed"))
            {
                Logger.LogMessage("Window closed. Reinitializing session.");
                SessionManager.TakeScreenshot($"{sectionName}.{pageName}");
                SessionManager.Setup(null);
            }
            else
            {
                Logger.LogMessage(exc.Message);
                SessionManager.TakeScreenshot($"{sectionName}.{pageName}");
            }

        }
    }

    public static string GetCustomDynamicDataDisplayName(MethodInfo methodInfo, object[] data)
    {
        return string.Format("Validate{0}PageAccessibility", data[1]);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/Button.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class Button : TestBase
{
    private static WindowsElement buttonElement = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("Button");
        buttonElement = Session.FindElementByAccessibilityId("Button1");
        Assert.IsNotNull(buttonElement);
    }

    [TestMethod]
    public void Button_Click()
    {

        var buttonEventOutput = Session.FindElementByAccessibilityId("Control1Output");
        Assert.AreEqual(string.Empty, buttonEventOutput.Text);

        buttonElement.Click();

        Assert.AreEqual("You clicked: Button1", buttonEventOutput.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(buttonElement.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        var disableButtonCheckbox = Session.FindElementByAccessibilityId("DisableButton1");
        Assert.IsTrue(buttonElement.Enabled);
        disableButtonCheckbox.Click();
        Assert.IsFalse(buttonElement.Enabled);
        disableButtonCheckbox.Click();
        Assert.IsTrue(buttonElement.Enabled);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Button", buttonElement.TagName);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(buttonElement.Size.Width > 0);
        Assert.IsTrue(buttonElement.Size.Height > 0);
    }

    [TestMethod]
    public void Text()
    {
        Assert.AreEqual("Standard XAML", buttonElement.Text);
    }
}


================================================
FILE: tests/WinUIGallery.UITests/Tests/CheckBox.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class CheckBox : TestBase
{
    private static WindowsElement checkBoxElement1 = null;
    private static WindowsElement checkBoxElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("CheckBox");
        checkBoxElement1 = Session.FindElementByName("Two-state");
        checkBoxElement2 = Session.FindElementByName("Three-state");
        Assert.IsNotNull(checkBoxElement2);
    }

    [TestMethod]
    public void Click()
    {
        var checkBoxEventOutput = Session.FindElementByAccessibilityId("Control2Output");
        Assert.AreEqual(string.Empty, checkBoxEventOutput.Text);

        checkBoxElement2.Click();
        Assert.AreEqual("CheckBox is checked.", checkBoxEventOutput.Text);

        checkBoxElement2.Click();
        Assert.AreEqual("CheckBox state is indeterminate.", checkBoxEventOutput.Text);

        checkBoxElement2.Click();
        Assert.AreEqual("CheckBox is unchecked.", checkBoxEventOutput.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(checkBoxElement1.Displayed);
        Assert.IsTrue(checkBoxElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(checkBoxElement1.Enabled);
        Assert.IsTrue(checkBoxElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(checkBoxElement2.Location.X >= checkBoxElement1.Location.X);
        Assert.IsTrue(checkBoxElement2.Location.Y >= checkBoxElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(checkBoxElement2.LocationOnScreenOnceScrolledIntoView.X >= checkBoxElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(checkBoxElement2.LocationOnScreenOnceScrolledIntoView.Y >= checkBoxElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.CheckBox", checkBoxElement1.TagName);
        Assert.AreEqual("ControlType.CheckBox", checkBoxElement2.TagName);
    }

    [TestMethod]
    public void Selected()
    {
        var originalState = checkBoxElement1.Selected;
        checkBoxElement1.Click();
        Assert.AreNotEqual(originalState, checkBoxElement1.Selected);
        checkBoxElement1.Click();
        Assert.AreEqual(originalState, checkBoxElement1.Selected);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(checkBoxElement1.Size.Width > 0);
        Assert.IsTrue(checkBoxElement1.Size.Height > 0);
        Assert.IsTrue(checkBoxElement1.Size.Width <= checkBoxElement2.Size.Width);
        Assert.AreEqual(checkBoxElement1.Size.Height, checkBoxElement2.Size.Height);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/ComboBox.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class ComboBox : TestBase
{
    private static WindowsElement comboBoxElement1 = null;
    private static WindowsElement comboBoxElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("ComboBox");
        comboBoxElement1 = Session.FindElementByAccessibilityId("Combo1");
        Assert.IsNotNull(comboBoxElement1);
        comboBoxElement2 = Session.FindElementByAccessibilityId("Combo2");
        Assert.IsNotNull(comboBoxElement2);
    }

    [TestMethod]
    public void Click()
    {
        // Click comboBoxElement1 to show the list and simply dismiss it
        var originalSelectedItem = comboBoxElement1.Text;
        comboBoxElement1.Click();
        comboBoxElement1.FindElementByAccessibilityId("Light Dismiss").Click();
        Assert.AreEqual(originalSelectedItem, comboBoxElement1.Text);

        // Click comboBoxElement1 to show the list and select an entry
        comboBoxElement1.Click();
        comboBoxElement1.FindElementByName("Yellow").Click();
        Assert.AreEqual("Yellow", comboBoxElement1.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(comboBoxElement1.Displayed);
        Assert.IsTrue(comboBoxElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(comboBoxElement1.Enabled);
        Assert.IsTrue(comboBoxElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(comboBoxElement2.Location.X >= comboBoxElement1.Location.X);
        Assert.IsTrue(comboBoxElement2.Location.Y >= comboBoxElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(comboBoxElement2.LocationOnScreenOnceScrolledIntoView.X >= comboBoxElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(comboBoxElement2.LocationOnScreenOnceScrolledIntoView.Y >= comboBoxElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.ComboBox", comboBoxElement1.TagName);
        Assert.AreEqual("ControlType.ComboBox", comboBoxElement2.TagName);
    }

    [TestMethod]
    public void SendKeys()
    {
        // Use the cursor key to scroll through the entries in the combo box
        comboBoxElement1.SendKeys(Keys.Down + Keys.Up + Keys.Up + Keys.Up); // Ensure top entry is selected
        Assert.AreEqual("Blue", comboBoxElement1.Text);
        comboBoxElement1.SendKeys(Keys.Down);
        Assert.AreEqual("Green", comboBoxElement1.Text);
        comboBoxElement1.SendKeys(Keys.Up);
        Assert.AreEqual("Blue", comboBoxElement1.Text);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(comboBoxElement1.Size.Width > 0);
        Assert.IsTrue(comboBoxElement1.Size.Height > 0);
        Assert.IsTrue(comboBoxElement2.Size.Width >= comboBoxElement1.Size.Width);
        Assert.IsTrue(comboBoxElement2.Size.Height >= comboBoxElement1.Size.Height);
    }

    [TestMethod]
    public void Text()
    {
        comboBoxElement1.SendKeys(Keys.Down + Keys.Up + Keys.Up + Keys.Up); // Ensure top entry is selected
        Assert.AreEqual("Blue", comboBoxElement1.Text);
        Assert.AreEqual("Courier New", comboBoxElement2.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/DatePicker.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class DatePicker : TestBase
{
    private static WindowsElement datePickerElement1 = null;
    private static WindowsElement datePickerElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("DatePicker");
        datePickerElement1 = Session.FindElementByName("Pick a date");
        Assert.IsNotNull(datePickerElement1);
        datePickerElement2 = Session.FindElementByAccessibilityId("Control2");
        Assert.IsNotNull(datePickerElement2);
    }

    [TestMethod]
    public void Click()
    {
        // Click datePickerElement1 to show the picker and simply dismiss it
        datePickerElement1.Click();
        var datePickerFlyout = Session.FindElementByAccessibilityId("FlyoutButton");
        Assert.IsNotNull(datePickerFlyout);
        Assert.IsTrue(datePickerFlyout.Displayed);
        Session.FindElementByAccessibilityId("DatePickerFlyoutPresenter").FindElementByAccessibilityId("DismissButton").Click();
        Thread.Sleep(1000);

        // Click datePickerElement1 to show the picker and set the year to 2000
        datePickerElement1.Click();
        datePickerFlyout = Session.FindElementByAccessibilityId("DatePickerFlyoutPresenter");
        Assert.IsNotNull(datePickerFlyout);
        var yearLoopingSelector = datePickerFlyout.FindElementByAccessibilityId("YearLoopingSelector");
        Assert.IsNotNull(yearLoopingSelector);
        var currentYear = yearLoopingSelector.Text;
        yearLoopingSelector.FindElementByName("2000").Click();
        Thread.Sleep(1000);
        Assert.AreNotEqual(currentYear, yearLoopingSelector.Text);
        datePickerFlyout.FindElementByAccessibilityId("AcceptButton").Click();
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(datePickerElement1.Displayed);
        Assert.IsTrue(datePickerElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(datePickerElement1.Enabled);
        Assert.IsTrue(datePickerElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(datePickerElement2.Location.X >= datePickerElement1.Location.X);
        Assert.IsTrue(datePickerElement2.Location.Y >= datePickerElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(datePickerElement2.LocationOnScreenOnceScrolledIntoView.X >= datePickerElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(datePickerElement2.LocationOnScreenOnceScrolledIntoView.Y >= datePickerElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Group", datePickerElement1.TagName);
        Assert.AreEqual("ControlType.Group", datePickerElement2.TagName);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(datePickerElement1.Size.Width > 0);
        Assert.IsTrue(datePickerElement1.Size.Height > 0);
        Assert.IsTrue(datePickerElement2.Size.Width >= datePickerElement1.Size.Width);
        Assert.IsTrue(datePickerElement2.Size.Height <= datePickerElement1.Size.Height);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/MediaPlayerElement.cs
================================================
// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;
using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class MediaPlayerElement : TestBase
{

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        // Doing this manually due to keyboard layout issues surrounding y and z
        var search = Session.FindElementByName("Search");
        search.Clear();
        Thread.Sleep(1_000);
        search.SendKeys("MediaPla");
        GetElementByName("MediaPlayerElement").Click();
    }

    [TestMethod]
    public void PlayMedia()
    {
        WindowsElement play = Session.FindElementByAccessibilityId("PlayPauseButton");
        Assert.IsNotNull(play);
        Assert.IsNotNull(Session.FindElementByAccessibilityId("svPanel"));

        // Play the video
        play.Click();
        Thread.Sleep(1000);

        // Pause the video
        play.Click();
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/PersonPicture.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class PersonPicture : TestBase
{
    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("PersonPicture");
    }

    [TestMethod]
    public void SwitchOptions()
    {
        GetElementByName("Profile Image").Click();
        GetElementByName("Display Name").Click();
        GetElementByName("Initials").Click();
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/ProgressBar.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class ProgressBar : TestBase
{
    private static WindowsElement progressBarElement = null;
    private static WindowsElement clickAndHoldButton = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("ProgressBar");
        progressBarElement = Session.FindElementByAccessibilityId("ProgressBar2");
        Assert.IsNotNull(progressBarElement);
        // Numberbox is a spinner, thus "Increase" is the button we need
        clickAndHoldButton = Session.FindElementByName("Increase");
        Assert.IsNotNull(clickAndHoldButton);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(progressBarElement.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(progressBarElement.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(clickAndHoldButton.Location.X >= progressBarElement.Location.X);
        Assert.IsTrue(clickAndHoldButton.Location.Y <= progressBarElement.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(clickAndHoldButton.LocationOnScreenOnceScrolledIntoView.X >= progressBarElement.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(clickAndHoldButton.LocationOnScreenOnceScrolledIntoView.Y <= progressBarElement.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.ProgressBar", progressBarElement.TagName);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(progressBarElement.Size.Width > 0);
        Assert.IsTrue(progressBarElement.Size.Height > 0);
    }

    [TestMethod]
    public void Text()
    {
        var originalValue = int.Parse(progressBarElement.Text);
        Assert.IsTrue(originalValue >= 0);
        clickAndHoldButton.Click();
        Assert.AreEqual(originalValue + 1, int.Parse(progressBarElement.Text));
        clickAndHoldButton.Click();
        Assert.AreEqual(originalValue + 2, int.Parse(progressBarElement.Text));
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/RadioButton.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class RadioButton : TestBase
{
    private static WindowsElement radioButtonElement1 = null;
    private static WindowsElement radioButtonElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("RadioButton");
        radioButtonElement1 = Session.FindElementByAccessibilityId("Option1RadioButton");
        Assert.IsNotNull(radioButtonElement1);
        radioButtonElement2 = Session.FindElementByAccessibilityId("Option2RadioButton");
        Assert.IsNotNull(radioButtonElement2);
    }

    [TestMethod]
    public void Click()
    {
        var radioButtonEventOutput = Session.FindElementByAccessibilityId("Control1Output");

        radioButtonElement1.Click();
        Assert.AreEqual("You selected Option 1", radioButtonEventOutput.Text);

        radioButtonElement2.Click();
        Assert.AreEqual("You selected Option 2", radioButtonEventOutput.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(radioButtonElement1.Displayed);
        Assert.IsTrue(radioButtonElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(radioButtonElement1.Enabled);
        Assert.IsTrue(radioButtonElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(radioButtonElement2.Location.X >= radioButtonElement1.Location.X);
        Assert.IsTrue(radioButtonElement2.Location.Y >= radioButtonElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(radioButtonElement2.LocationOnScreenOnceScrolledIntoView.X >= radioButtonElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(radioButtonElement2.LocationOnScreenOnceScrolledIntoView.Y >= radioButtonElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.RadioButton", radioButtonElement1.TagName);
        Assert.AreEqual("ControlType.RadioButton", radioButtonElement2.TagName);
    }

    [TestMethod]
    public void Selected()
    {
        radioButtonElement1.Click();
        Assert.IsTrue(radioButtonElement1.Selected);
        Assert.IsFalse(radioButtonElement2.Selected);

        radioButtonElement2.Click();
        Assert.IsTrue(radioButtonElement2.Selected);
        Assert.IsFalse(radioButtonElement1.Selected);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(radioButtonElement1.Size.Width > 0);
        Assert.IsTrue(radioButtonElement1.Size.Height > 0);
        Assert.AreEqual(radioButtonElement1.Size.Width, radioButtonElement2.Size.Width);
        Assert.AreEqual(radioButtonElement1.Size.Height, radioButtonElement2.Size.Height);
    }

    [TestMethod]
    public void Text()
    {
        Assert.AreEqual("Option 1", radioButtonElement1.Text);
        Assert.AreEqual("Option 2", radioButtonElement2.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/SearchResults.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium;
using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class SearchResults : TestBase
{
    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
    }

    [TestMethod]
    [DataRow("a")]  // "a" should return results for all groups.
    [TestProperty("Description", "Validate the accessibility of the search results page.")]
    public void ValidateSearchResultsPageAccessibility(string searchText)
    {
        var search = Session.FindElementByName("Search");
        search.Clear();

        search.SendKeys(searchText);
        search.SendKeys(Keys.Enter);

        Thread.Sleep(100);

        var resultsNavView = Session.FindElementByAccessibilityId("resultsNavView");
        var resultItems = resultsNavView.FindElements(By.ClassName("Microsoft.UI.Xaml.Controls.NavigationViewItem"));

        foreach (var menuItem in resultItems)
        {
            Thread.Sleep(1000);
            menuItem.Click();
            AxeHelper.AssertNoAccessibilityErrors();
        }
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/Slider.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class Slider : TestBase
{
    private static WindowsElement sliderElement1 = null;
    private static WindowsElement sliderElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("Slider");
        sliderElement1 = Session.FindElementByAccessibilityId("Slider1");
        Assert.IsNotNull(sliderElement1);
        sliderElement2 = Session.FindElementByAccessibilityId("Slider2");
        Assert.IsNotNull(sliderElement2);
    }

    [TestMethod]
    public void Click()
    {
        sliderElement1.Click();
        Assert.IsTrue(int.Parse(sliderElement1.Text) > 45); // The value of the slider when the center is clicked should be greater than 45 and close to 50

        sliderElement2.Click();
        Assert.AreEqual("750", sliderElement2.Text);  // The value of the slider when the center is clicked
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(sliderElement1.Displayed);
        Assert.IsTrue(sliderElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(sliderElement1.Enabled);
        Assert.IsTrue(sliderElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(sliderElement1.Location.X >= sliderElement1.Location.X);
        Assert.IsTrue(sliderElement1.Location.Y >= sliderElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(sliderElement2.LocationOnScreenOnceScrolledIntoView.X >= sliderElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(sliderElement2.LocationOnScreenOnceScrolledIntoView.Y >= sliderElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Slider", sliderElement1.TagName);
        Assert.AreEqual("ControlType.Slider", sliderElement2.TagName);
    }

    [TestMethod]
    public void SendKeys()
    {
        var originalValue = sliderElement1.Text;
        // Pressing right arrow will move the slider right and the value should increase by 1
        sliderElement1.SendKeys(Keys.Right);
        Assert.AreEqual(int.Parse(originalValue) + 1, int.Parse(sliderElement1.Text));
        // Pressing left arrow will move the slider back to the original value
        sliderElement1.SendKeys(Keys.Left);
        Assert.AreEqual(originalValue, sliderElement1.Text);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(sliderElement1.Size.Width > 0);
        Assert.IsTrue(sliderElement1.Size.Height > 0);
    }

    [TestMethod]
    public void Text()
    {
        sliderElement1.Click();
        Assert.IsTrue(int.Parse(sliderElement1.Text) > 45); // The value of the slider when the center is clicked should be greater than 45 and close to 50

        sliderElement2.Click();
        Assert.AreEqual(750, int.Parse(sliderElement2.Text)); // The value of the slider when the center is clicked should be 750
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/TextBlock.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class TextBlock : TestBase
{
    private static WindowsElement textBlockElement1 = null;
    private static WindowsElement textBlockElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("TextBlock");
        textBlockElement1 = Session.FindElementByName("I am a TextBlock.");
        Assert.IsNotNull(textBlockElement1);
        textBlockElement2 = Session.FindElementByName("I am a styled TextBlock.");
        Assert.IsNotNull(textBlockElement2);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(textBlockElement1.Displayed);
        Assert.IsTrue(textBlockElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(textBlockElement1.Enabled);
        Assert.IsTrue(textBlockElement1.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(textBlockElement2.Location.X >= textBlockElement1.Location.X);
        Assert.IsTrue(textBlockElement2.Location.Y >= textBlockElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(textBlockElement2.LocationOnScreenOnceScrolledIntoView.X >= textBlockElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(textBlockElement2.LocationOnScreenOnceScrolledIntoView.Y >= textBlockElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Text", textBlockElement1.TagName);
        Assert.AreEqual("ControlType.Text", textBlockElement2.TagName);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(textBlockElement1.Size.Width > 0);
        Assert.IsTrue(textBlockElement1.Size.Height > 0);
        Assert.IsTrue(textBlockElement2.Size.Width >= textBlockElement1.Size.Width);
        Assert.IsTrue(textBlockElement2.Size.Height >= textBlockElement1.Size.Height);
    }

    [TestMethod]
    public void Text()
    {
        Assert.AreEqual("I am a TextBlock.", textBlockElement1.Text);
        Assert.AreEqual("I am a styled TextBlock.", textBlockElement2.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/TextBox.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium;
using OpenQA.Selenium.Appium.Windows;

using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class TextBox : TestBase
{
    private static WindowsElement textBoxElement1 = null;
    private static WindowsElement textBoxElement2 = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("TextBox");
        textBoxElement1 = Session.FindElementByName("simple TextBox");
        textBoxElement2 = Session.FindElementByName("Enter your name:");
        Assert.IsNotNull(textBoxElement1);
        Assert.IsNotNull(textBoxElement2);
    }

    [TestMethod]
    public void Clear()
    {
        textBoxElement1.Clear();
        Assert.AreEqual(string.Empty, textBoxElement1.Text);
        textBoxElement1.SendKeys("F");
        Assert.AreEqual("F", textBoxElement1.Text);
        textBoxElement1.Clear();
        Assert.AreEqual(string.Empty, textBoxElement1.Text);
    }

    [TestMethod]
    public void Click()
    {
        // Click textBoxElement1 to set focus and arbitrarily type
        textBoxElement1.Clear();
        Assert.AreEqual(string.Empty, textBoxElement1.Text);
        textBoxElement1.Click();
        Thread.Sleep(1_000);
        TypeText("1");
        Assert.AreEqual("1", textBoxElement1.Text);

        // Click textBoxElement2 to set focus and arbitrarily type
        textBoxElement2.Clear();
        Assert.AreEqual(string.Empty, textBoxElement2.Text);
        textBoxElement2.Click();
        Thread.Sleep(1_000);
        TypeText("1");
        Assert.AreEqual("1", textBoxElement2.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(textBoxElement1.Displayed);
        Assert.IsTrue(textBoxElement2.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(textBoxElement1.Enabled);
        Assert.IsTrue(textBoxElement2.Enabled);
    }

    [TestMethod]
    public void Location()
    {
        Assert.IsTrue(textBoxElement2.Location.X >= textBoxElement1.Location.X);
        Assert.IsTrue(textBoxElement2.Location.Y >= textBoxElement1.Location.Y);
    }

    [TestMethod]
    public void LocationInView()
    {
        Assert.IsTrue(textBoxElement2.LocationOnScreenOnceScrolledIntoView.X >= textBoxElement1.LocationOnScreenOnceScrolledIntoView.X);
        Assert.IsTrue(textBoxElement2.LocationOnScreenOnceScrolledIntoView.Y >= textBoxElement1.LocationOnScreenOnceScrolledIntoView.Y);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Edit", textBoxElement1.TagName);
        Assert.AreEqual("ControlType.Edit", textBoxElement2.TagName);
    }

    [TestMethod]
    public void SendKeys()
    {
        textBoxElement1.Clear();
        Assert.AreEqual(string.Empty, textBoxElement1.Text);
        textBoxElement1.SendKeys("A");
        Assert.AreEqual("A", textBoxElement1.Text);

        // Use Ctrl + A to select all text and backspace to clear the box
        textBoxElement1.SendKeys(Keys.Control + "a" + Keys.Control + Keys.Backspace);
        Assert.AreEqual(string.Empty, textBoxElement1.Text);

        textBoxElement2.Clear();
        Assert.AreEqual(string.Empty, textBoxElement2.Text);
        textBoxElement2.SendKeys("E");
        Assert.AreEqual("E", textBoxElement2.Text);
    }

    [TestMethod]
    public void Text()
    {
        textBoxElement1.Clear();
        Assert.AreEqual(string.Empty, textBoxElement1.Text);
        textBoxElement1.SendKeys("A");
        Assert.AreEqual("A", textBoxElement1.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/ToggleButton.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class ToggleButton : TestBase
{
    private static WindowsElement toggleButtonElement = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("ToggleButton");
        toggleButtonElement = Session.FindElementByAccessibilityId("Toggle1");
        Assert.IsNotNull(toggleButtonElement);
    }

    [TestMethod]
    public void Click()
    {
        var buttonEventOutput = Session.FindElementByAccessibilityId("Control1Output");
        Assert.AreEqual("Off", buttonEventOutput.Text);

        toggleButtonElement.Click();
        Assert.AreEqual("On", buttonEventOutput.Text);
        toggleButtonElement.Click();
        Assert.AreEqual("Off", buttonEventOutput.Text);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(toggleButtonElement.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        var disableButtonCheckbox = Session.FindElementByAccessibilityId("DisableToggle1");
        Assert.IsTrue(toggleButtonElement.Enabled);

        disableButtonCheckbox.Click();
        Assert.IsFalse(toggleButtonElement.Enabled);

        disableButtonCheckbox.Click();
        Assert.IsTrue(toggleButtonElement.Enabled);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Button", toggleButtonElement.TagName);
    }

    [TestMethod]
    public void Selected()
    {
        toggleButtonElement.Click();
        Assert.IsTrue(toggleButtonElement.Selected);

        toggleButtonElement.Click();
        Assert.IsFalse(toggleButtonElement.Selected);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(toggleButtonElement.Size.Width > 0);
        Assert.IsTrue(toggleButtonElement.Size.Height > 0);
    }

    [TestMethod]
    public void Text()
    {
        Assert.AreEqual("ToggleButton", toggleButtonElement.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UITests/Tests/ToggleSwitch.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.VisualStudio.TestTools.UnitTesting;
using OpenQA.Selenium.Appium.Windows;
using System.Threading;

namespace WinUIGallery.UITests.Tests;

[TestClass]
public class ToggleSwitch : TestBase
{
    private static WindowsElement toggleSwitchElement = null;

    [ClassInitialize]
    public static void ClassInitialize(TestContext context)
    {
        OpenControlPage("ToggleSwitch");
        toggleSwitchElement = Session.FindElementByAccessibilityId("ToggleSwitch2");
        Assert.IsNotNull(toggleSwitchElement);
    }

    [TestMethod]
    public void Click()
    {
        var originalState = toggleSwitchElement.Selected;
        toggleSwitchElement.Click();
        Assert.AreNotEqual(originalState, toggleSwitchElement.Selected);

        Thread.Sleep(1000);
        toggleSwitchElement.Click();
        Assert.AreEqual(originalState, toggleSwitchElement.Selected);
    }

    [TestMethod]
    public void Displayed()
    {
        Assert.IsTrue(toggleSwitchElement.Displayed);
    }

    [TestMethod]
    public void Enabled()
    {
        Assert.IsTrue(toggleSwitchElement.Enabled);
    }

    [TestMethod]
    public void Name()
    {
        Assert.AreEqual("ControlType.Button", toggleSwitchElement.TagName);
    }

    [TestMethod]
    public void Selected()
    {
        var originalState = toggleSwitchElement.Selected;
        toggleSwitchElement.Click();
        Assert.AreNotEqual(originalState, toggleSwitchElement.Selected);

        Thread.Sleep(1000);
        toggleSwitchElement.Click();
        Assert.AreEqual(originalState, toggleSwitchElement.Selected);
    }

    [TestMethod]
    public void Size()
    {
        Assert.IsTrue(toggleSwitchElement.Size.Width > 0);
        Assert.IsTrue(toggleSwitchElement.Size.Height > 0);
    }

    [TestMethod]
    public void Text()
    {
        Assert.AreEqual("Toggle work Working", toggleSwitchElement.Text);
    }
}



================================================
FILE: tests/WinUIGallery.UnitTests/app.manifest
================================================
<?xml version="1.0" encoding="utf-8"?>
<assembly manifestVersion="1.0" xmlns="urn:schemas-microsoft-com:asm.v1">
    <assemblyIdentity version="1.0.0.0" name="WinUIGallery.UnitTests.app"/>

    <compatibility xmlns="urn:schemas-microsoft-com:compatibility.v1">
        <application>

            <!--
                The ID below informs the system that this application is compatible with OS features first introduced in Windows 10.
                It is necessary to support features in unpackaged applications, for example the custom titlebar implementation.
                For more info see https://docs.microsoft.com/windows/apps/windows-app-sdk/use-windows-app-sdk-run-time#declare-os-compatibility-in-your-application-manifest
            -->

            <supportedOS Id="{8e0f7a12-bfb3-4fe8-b9a5-48fd50a15a9a}" />
        </application>
    </compatibility>

    <application xmlns="urn:schemas-microsoft-com:asm.v3">
        <windowsSettings>
            <dpiAwareness xmlns="http://schemas.microsoft.com/SMI/2016/WindowsSettings">PerMonitorV2</dpiAwareness>
        </windowsSettings>
    </application>

</assembly>



================================================
FILE: tests/WinUIGallery.UnitTests/Package.appxmanifest
================================================
﻿<!--  Copyright (c) Microsoft Corporation. Licensed under the MIT License.  -->
<Package
    xmlns="http://schemas.microsoft.com/appx/manifest/foundation/windows10"
    xmlns:mp="http://schemas.microsoft.com/appx/2014/phone/manifest"
    xmlns:uap="http://schemas.microsoft.com/appx/manifest/uap/windows10"
    xmlns:rescap="http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities"
    IgnorableNamespaces="uap rescap">

    <Identity
        Name="WinUIGallery.UnitTests"
        Publisher="CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US"
        Version="1.0.0.0" />

    <mp:PhoneIdentity PhoneProductId="3a75d49b-f769-4a7b-91ae-850b7cd79d2d" PhonePublisherId="00000000-0000-0000-0000-000000000000"/>

    <Properties>
        <DisplayName>WinUIGallery.UnitTests</DisplayName>
        <PublisherDisplayName>kmahone</PublisherDisplayName>
        <Logo>Assets\StoreLogo.png</Logo>
    </Properties>

    <Dependencies>
        <TargetDeviceFamily Name="Windows.Universal" MinVersion="10.0.17763.0" MaxVersionTested="10.0.19041.0" />
        <TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.17763.0" MaxVersionTested="10.0.19041.0" />
    </Dependencies>

    <Resources>
        <Resource Language="x-generate"/>
    </Resources>

    <Applications>
        <Application Id="App"
            Executable="$targetnametoken$.exe"
            EntryPoint="$targetentrypoint$">
            <uap:VisualElements
                DisplayName="WinUIGallery.UnitTests"
                Description="WinUIGallery.UnitTests"
                BackgroundColor="transparent"
                Square150x150Logo="Assets\Square150x150Logo.png"
                Square44x44Logo="Assets\Square44x44Logo.png">
                <uap:DefaultTile Wide310x150Logo="Assets\Wide310x150Logo.png" />
                <uap:SplashScreen Image="Assets\SplashScreen.png" />
            </uap:VisualElements>
        </Application>
    </Applications>

    <Capabilities>
        <rescap:Capability Name="runFullTrust" />
    </Capabilities>

</Package>



================================================
FILE: tests/WinUIGallery.UnitTests/UnitTestApp.xaml
================================================
<!--  Copyright (c) Microsoft Corporation. Licensed under the MIT License.  -->
<Application
    x:Class="WinUIGallery.UnitTests.UnitTestApp"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:local="using:WinUIGallery.UnitTests">

    <Application.Resources>
        <ResourceDictionary>
            <ResourceDictionary.MergedDictionaries>
                <XamlControlsResources xmlns="using:Microsoft.UI.Xaml.Controls" />
                <!--  Other merged dictionaries here  -->
            </ResourceDictionary.MergedDictionaries>
        </ResourceDictionary>
    </Application.Resources>

</Application>



================================================
FILE: tests/WinUIGallery.UnitTests/UnitTestApp.xaml.cs
================================================
﻿// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.UI.Xaml;
using Microsoft.VisualStudio.TestTools.UnitTesting.AppContainer;
using System;

namespace WinUIGallery.UnitTests;

public partial class UnitTestApp : Application
{
    public UnitTestApp()
    {
        InitializeComponent();
    }

    protected override void OnLaunched(LaunchActivatedEventArgs args)
    {
        Microsoft.VisualStudio.TestPlatform.TestExecutor.UnitTestClient.CreateDefaultUI();

        s_window = new UnitTestAppWindow();
        s_window.Activate();

        UITestMethodAttribute.DispatcherQueue = s_window.DispatcherQueue;

        Microsoft.VisualStudio.TestPlatform.TestExecutor.UnitTestClient.Run(Environment.CommandLine);
    }

    private static UnitTestAppWindow s_window;

    public static UnitTestAppWindow UnitTestAppWindow
    {
        get { return s_window; }
    }
}



================================================
FILE: tests/WinUIGallery.UnitTests/UnitTestAppWindow.xaml
================================================
<!--  Copyright (c) Microsoft Corporation. Licensed under the MIT License.  -->
<Window
    x:Class="WinUIGallery.UnitTests.UnitTestAppWindow"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
    xmlns:local="using:WinUIGallery.UnitTests"
    xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
    mc:Ignorable="d">

    <Grid x:Name="rootGrid" />

</Window>



================================================
FILE: tests/WinUIGallery.UnitTests/UnitTestAppWindow.xaml.cs
================================================
// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.UI.Xaml;
using Microsoft.UI.Xaml.Controls;

namespace WinUIGallery.UnitTests;

public sealed partial class UnitTestAppWindow : Window
{
    public UnitTestAppWindow()
    {
        InitializeComponent();
    }

    public Grid RootGrid
    {
        get
        {
            return rootGrid;
        }
    }

    public void AddToVisualTree(UIElement element)
    {
        RootGrid.Children.Add(element);
    }

    public void CleanupVisualTree()
    {
        RootGrid.Children.Clear();
    }
}



================================================
FILE: tests/WinUIGallery.UnitTests/UnitTests.cs
================================================
// Copyright (c) Microsoft Corporation.
// Licensed under the MIT License.

using Microsoft.UI;
using Microsoft.UI.Dispatching;
using Microsoft.UI.Xaml;
using Microsoft.UI.Xaml.Controls;
using Microsoft.UI.Xaml.Controls.Primitives;
using Microsoft.UI.Xaml.Media;
using Microsoft.UI.Xaml.Shapes;
using Microsoft.VisualStudio.TestTools.UnitTesting;
using Microsoft.VisualStudio.TestTools.UnitTesting.AppContainer;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading;
using System.Threading.Tasks;
using Windows.Foundation;
using WinUIGallery.Helpers;

namespace WinUIGallery.UnitTests;

[TestClass]
public class UnitTests
{
    [TestMethod]
    public async Task TestControlInfoDataSource()
    {
        var groups = await ControlInfoDataSource.Instance.GetGroupsAsync();
        var groupsList = groups.ToList();

        var expectedGroups = new List<string>
        {
            "Fundamentals",
            "Design",
            "Accessibility",
            "Menus & toolbars",
            "Collections",
            "Date & time",
            "Basic input",
            "Status & info",
            "Dialogs & flyouts",
            "Scrolling",
            "Layout",
            "Navigation",
            "Media",
            "Styles",
            "Text",
            "Motion",
            "Windowing",
            "System"
        };

        Assert.AreEqual(expectedGroups.Count, groupsList.Count);

        int groupCount = expectedGroups.Count;
        for(int i = 0; i < groupCount; i++)
        {
            var actualTitle = groupsList[i].Title;
            Assert.AreEqual(expectedGroups[i], actualTitle);
        }
    }

    // Use the UITestMethod attribute for tests that need to run on the UI thread.
    [UITestMethod]
    public void TestWrapGrid()
    {
        Layouts.WrapPanel wrapPanel = new()
        {
            Width = 250,
            Height = 250
        };
        for (int i = 0; i < 4; i++)
        {
            wrapPanel.Children.Add(new Button()
            {
                Width = 120,
                Height = 80,
                Content = $"Button {i}"
            });
        }

        UnitTestApp.UnitTestAppWindow.AddToVisualTree(wrapPanel);
        wrapPanel.UpdateLayout();

        List<Rect> expectedLayouts =
        [
            new Rect(0,    0, 120,  80),
            new Rect(120,  0, 120,  80),
            new Rect(0,   80, 120,  80),
            new Rect(120, 80, 120,  80)
        ];
        for (int i = 0; i < 4; i++)
        {
            var actualLayout = LayoutInformation.GetLayoutSlot(wrapPanel.Children[i] as FrameworkElement);
            Assert.AreEqual(expectedLayouts[i], actualLayout);
        }
    }

    // This test demonstrates executing test code both on and off the UI thread.
    // We use the ExecuteOnUIThread method to run code on the UI thread.
    [TestMethod]
    public void MultiThreadTest()
    {
        Border border = null;
        AutoResetEvent borderSizeChanged = new(false);

        ExecuteOnUIThread(() =>
        {
            Grid grid = new()
            {
                Width = 200,
            };

            border = new Border
            {
                Background = new SolidColorBrush(Colors.Green),
                HorizontalAlignment = HorizontalAlignment.Stretch,
                Child = new Rectangle
                {
                    Fill = new SolidColorBrush(Colors.Red),
                    Width = 100,
                }
            };

            border.SizeChanged += (s, e) =>
            {
                borderSizeChanged.Set();
            };

            grid.Children.Add(border);

            UnitTestApp.UnitTestAppWindow.AddToVisualTree(grid);
        });
        Assert.IsTrue(borderSizeChanged.WaitOne());

        ExecuteOnUIThread(() =>
        {
            Assert.AreEqual(200, border.ActualWidth);

            border.HorizontalAlignment = HorizontalAlignment.Left;
        });

        Assert.IsTrue(borderSizeChanged.WaitOne());

        ExecuteOnUIThread(() =>
        {
            Assert.AreEqual(100, border.ActualWidth);
        });
    }

    private void ExecuteOnUIThread(Action action)
    {
        AutoResetEvent done = new(false);
        DispatcherQueue dispatcherQueue = UnitTestApp.UnitTestAppWindow.DispatcherQueue;
        if (dispatcherQueue.HasThreadAccess)
        {
            action();
        }
        else
        {
            Exception exception = null;
            var success = dispatcherQueue.TryEnqueue(() =>
            {
                try
                {
                    action();
                }
                catch (Exception ex)
                {
                    exception = ex;
                }
                finally
                {
                    done.Set();
                }
            });
            Assert.IsTrue(success);
            Assert.IsTrue(done.WaitOne());
            if(exception != null)
            {
                Assert.Fail(exception.ToString());
            }
        }
    }

    [TestCleanup]
    public void Cleanup()
    {
        ExecuteOnUIThread(() =>
        {
            UnitTestApp.UnitTestAppWindow.CleanupVisualTree();
        });
    }
}



================================================
FILE: tests/WinUIGallery.UnitTests/WinUIGallery.UnitTests.csproj
================================================
<!--  Copyright (c) Microsoft Corporation. Licensed under the MIT License.  -->
<Project Sdk="Microsoft.NET.Sdk">

    <PropertyGroup>
        <OutputType>WinExe</OutputType>
        <TargetFramework>$(SamplesTargetFrameworkMoniker)</TargetFramework>
        <TargetPlatformVersion>$(WindowsSdkTargetPlatformVersion)</TargetPlatformVersion>
        <TargetPlatformMinVersion>$(WindowsAppSdkTargetPlatformVersion)</TargetPlatformMinVersion>
        <RootNamespace>WinUIGallery.UnitTests</RootNamespace>
        <ApplicationManifest>app.manifest</ApplicationManifest>
        <Platforms>x86;x64;ARM64</Platforms>
        <RuntimeIdentifiers>win-x86;win-x64;win-arm64</RuntimeIdentifiers>
        <PublishProfile>win-$(Platform).pubxml</PublishProfile>
        <UseWinUI>true</UseWinUI>
        <EnableMsixTooling>true</EnableMsixTooling>
        <ErrorOnDuplicatePublishOutputFiles>false</ErrorOnDuplicatePublishOutputFiles>
        <SelfContained>true</SelfContained>
    </PropertyGroup>

    <ItemGroup>
        <Page Remove="UnitTestApp.xaml" />
        <ApplicationDefinition Include="UnitTestApp.xaml" />
        <ProjectCapability Include="TestContainer" />
        <Content Include="Assets\*.png" />
    </ItemGroup>

    <ItemGroup>
        <ProjectReference Include="..\..\WinUIGallery\WinUIGallery.csproj" />
    </ItemGroup>

    <ItemGroup>
        <PackageReference Include="Microsoft.WindowsAppSDK" Version="$(WindowsAppSdkPackageVersion)" />
        <PackageReference Include="Microsoft.Windows.SDK.BuildTools" Version="10.0.22621.756" />
        <PackageReference Include="MSTest.TestAdapter" Version="3.1.1" />
        <PackageReference Include="MSTest.TestFramework" Version="3.1.1" />
        <PackageReference Include="Microsoft.TestPlatform.TestHost" Version="17.7.2" ExcludeAssets="build" />
        <Manifest Include="$(ApplicationManifest)" />
    </ItemGroup>

    <ItemGroup Condition="'$(DisableMsixProjectCapabilityAddedByProject)'!='true' and '$(EnableMsixTooling)'=='true'">
        <ProjectCapability Include="Msix" />
    </ItemGroup>
    <PropertyGroup Condition="'$(DisableHasPackageAndPublishMenuAddedByProject)'!='true' and '$(EnableMsixTooling)'=='true'">
        <HasPackageAndPublishMenu>true</HasPackageAndPublishMenu>
    </PropertyGroup>

</Project>



================================================
FILE: tests/WinUIGallery.UnitTests/Properties/launchSettings.json
================================================
{
  "profiles": {
    "WinUIGallery.UnitTests (Package)": {
      "commandName": "MsixPackage"
    },
    "WinUIGallery.UnitTests (Unpackaged)": {
      "commandName": "Project"
    }
  }
}


================================================
FILE: tests/WinUIGallery.UnitTests/Properties/PublishProfiles/win-arm64.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>ARM64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-arm64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-arm64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UnitTests/Properties/PublishProfiles/win-arm64ec.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UnitTests/Properties/PublishProfiles/win-x64.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x64</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x64</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x64</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: tests/WinUIGallery.UnitTests/Properties/PublishProfiles/win-x86.pubxml
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<!--
https://go.microsoft.com/fwlink/?LinkID=208121.
-->
<Project ToolsVersion="4.0" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <PublishProtocol>FileSystem</PublishProtocol>
    <Platform>x86</Platform>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) >= 8">win-x86</RuntimeIdentifier>
    <RuntimeIdentifier Condition="$([MSBuild]::GetTargetFrameworkVersion('$(TargetFramework)')) &lt; 8">win10-x86</RuntimeIdentifier>
    <PublishDir>bin\$(Configuration)\$(TargetFramework)\$(RuntimeIdentifier)\publish\</PublishDir>
    <SelfContained>true</SelfContained>
    <PublishSingleFile>False</PublishSingleFile>
    <PublishReadyToRun Condition="'$(Configuration)' == 'Debug'">False</PublishReadyToRun>
    <PublishReadyToRun Condition="'$(Configuration)' != 'Debug'">True</PublishReadyToRun>
    <PublishTrimmed Condition="'$(Configuration)' == 'Debug'">False</PublishTrimmed>
    <PublishTrimmed Condition="'$(Configuration)' != 'Debug'">True</PublishTrimmed>
  </PropertyGroup>
</Project>


================================================
FILE: Tools/readme.md
================================================
# Tools Folder

The Tools folder contains a set of tools and utilities that are repeatedly used by developers to assist in managing and developing the WinUI Gallery. These tools streamline various development tasks, providing functionality to track, manage, and organize files within the repository.

> **Note**: Before running any PowerShell script, you must set the execution policy to allow locally created scripts to run. Use the following command to set the policy:
>
> ```powershell
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```
> This ensures that PowerShell scripts downloaded from the internet are not run unless they are signed by a trusted publisher, while locally created scripts are allowed to run.


## Running scripts

#### 1st Way: From File Explorer
- Step 1: Navigate to the `Tools` folder.
- Step 2: Right-click the `Get-LatestAddedSamples.ps1` script and select **Run with PowerShell**.
- Step 3: The script will output a list of newly added files along with their first commit dates.

#### 2nd Way: From Visual Studio
- Step 1: Open `WinUIGallery` project in Visual Studio.
- Step 2: Navigate to the **Tools** menu and select **Open PowerShell Window**.
- Step 3: In the PowerShell window, type the following command:
  ```powershell
  ..\Tools\Get-LatestAddedSamples.ps1
  ```
- Step 4: The script will output the list of added files.

## Scripts

### Get-LatestAddedSamples tool

The goal of the `Get-LatestAddedSamples.ps1` script is to assist developers in identifying newly added files in the `ControlPages` directory, along with the date of their first commit. This helps in tracking the progress of new additions to the project and identifying which samples should be included on the home page, ensuring that the most recent content is always showcased.

### Get-LatestUpdatedSamples tool

The goal of the `Get-LatestUpdatedSamples.ps1` script is to help developers quickly identify files in the `ControlPages` directory that have been updated, along with their last commit dates. This information is useful for tracking changes made to the project, ensuring that developers can monitor updates to existing samples, and identifying which updated samples might need to be showcased on the home page.


================================================
FILE: Tools/Get-LatestAddedSamples.ps1
================================================
# Define the folder containing the WinUIGallery Samples relative to the script location
$SamplesFolder = Join-Path -Path $PSScriptRoot -ChildPath "..\WinUIGallery\Samples"

# Change directory to the WinUIGallery folder
Set-Location -Path $SamplesFolder

# Define the folder containing the control pages
$currentFolder = "ControlPages"

# Retrieve the list of files in the folder with their details
$filesWithDetails = git ls-tree -r HEAD --name-only $currentFolder | ForEach-Object {
    $file = $_  # Current file path from the git tree

    # Check if the file is directly under the $currentFolder and not in subdirectories
    if ($file -match "^$currentFolder/[^/]+$") {
        # Get the date of the first commit where the file was added (diff-filter A means "added")
        $firstAddCommit = git log --diff-filter=A --reverse --format="%ai" -- $file | Select-Object -First 1

        # If the file has an add commit (i.e., it's not a new file)
        if ($firstAddCommit) {
            # Create a custom object with file name and its first added commit date
            [PSCustomObject]@{
                File = $file.Substring($currentFolder.Length + 1)  # Remove the folder path to get the file name
                FirstAddCommitDate = $firstAddCommit  # Date of the first commit where the file was added
            }
        }
    }
}
# Sort the files by their first add commit date in descending order (most recent first)
$sortedFiles = $filesWithDetails | Sort-Object FirstAddCommitDate -Descending
# Create a hashtable to cache processed file base names to avoid duplicates
$cachedBaseNames = @{ }
# Initialize the output string for the latest added samples
$LatestAddeddSamples = "Latest Added Samples:`n"
# Process the sorted files
$sortedFiles | ForEach-Object {
    # Remove file extensions and standardize the file name
    $fileName = $_.File -replace '\.xaml\.cs$', '' -replace '\.xaml$', ''
    $fileName = $fileName -replace 'Page$', ''
    $date = $_.FirstAddCommitDate

    # Add the file to the output if it hasn't been cached yet (to avoid duplicates)
    if (-not $cachedBaseNames.Contains($fileName)) {
        $cachedBaseNames[$fileName] = $true  # Mark the file name as cached
        $LatestAddeddSamples += $fileName + " (" + $date + ")`n" # Append the file name to the output list
    }
}

# Output the list of the latest added samples
Write-Output $LatestAddeddSamples
# Wait for the user to press Enter before closing the PowerShell window
Read-Host -Prompt "Press Enter to exit"


================================================
FILE: Tools/Get-LatestUpdatedSamples.ps1
================================================
# Define the folder containing the WinUIGallery Samples relative to the script location
$SamplesFolder = Join-Path -Path $PSScriptRoot -ChildPath "..\WinUIGallery\Samples"

# Change directory to the WinUIGallery folder
Set-Location -Path $SamplesFolder

# Define the folder containing the control pages
$currentFolder = "ControlPages"

# Retrieve the list of files in the folder with their details
$filesWithDetails = git ls-tree -r HEAD --name-only $currentFolder | ForEach-Object {
    $file = $_  # Current file path from the git tree

    # Check if the file is directly under the $currentFolder and not in subdirectories
    if ($file -match "^$currentFolder/[^/]+$") {
        # Get the last commit date for the file
        $lastCommitDate = git log -1 --format="%ai" -- $file

        # Get the commit status for the file (checks if it was modified in the last commit)
        $commitStatus = git log -1 --name-status -- $file | Select-String -Pattern "^M" | ForEach-Object { $_.Line.Split()[0] }
        # If the file was modified ("M"), create a custom object with file details
        if ($commitStatus -eq "M") {
            [PSCustomObject]@{
                File = $file.Substring($currentFolder.Length + 1)  # Trim the folder path to get the file name
                LastCommitDate = $lastCommitDate  # Last commit date for the file
            }
        }
    }
}
# Sort the files by the last commit date in descending order
$sortedFiles = $filesWithDetails | Sort-Object LastCommitDate -Descending
# Create a hashtable to cache processed file base names to avoid duplicates
$cachedBaseNames = @{ }
# Initialize the output string for the latest updated samples
$LatestUpdatedSamples = "Latest Updated Samples:`n"
# Process the sorted files
$sortedFiles | ForEach-Object {
    # Remove file extensions and standardize the file name
    $fileName = $_.File -replace '\.xaml\.cs$', '' -replace '\.xaml$', ''
    $fileName = $fileName -replace 'Page$', ''
    $date = $_.LastCommitDate

    # Add the file to the output if it hasn't been cached yet
    if (-not $cachedBaseNames.Contains($fileName)) {
        $cachedBaseNames[$fileName] = $true  # Mark the file name as cached
        $LatestUpdatedSamples += $fileName + " (" + $date + ")`n" # Append the file name to the output
    }
}

# Output the list of latest updated samples
Write-Output $LatestUpdatedSamples
# Wait for the user to press Enter before closing the PowerShell window
Read-Host -Prompt "Press Enter to exit"


================================================
FILE: WinUIGallery/app.manifest
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<assembly manifestVersion="1.0" xmlns="urn:schemas-microsoft-com:asm.v1">
  <assemblyIdentity version="1.0.0.0" name="WinUIGallery.Desktop.app"/>

  <application xmlns="urn:schemas-microsoft-com:asm.v3">
    <windowsSettings>
      <dpiAware xmlns="http://schemas.microsoft.com/SMI/2005/WindowsSettings">true/PM</dpiAware>
      <dpiAwareness xmlns="http://schemas.microsoft.com/SMI/2016/WindowsSettings">PerMonitorV2, PerMonitor</dpiAwareness>
    </windowsSettings>
  </application>

  <compatibility xmlns="urn:schemas-microsoft-com:compatibility.v1">
    <application>
      <!-- Windows 10 -->
      <supportedOS Id="{8e0f7a12-bfb3-4fe8-b9a5-48fd50a15a9a}" />
    </application>
  </compatibility>
</assembly>



================================================
FILE: WinUIGallery/App.xaml
================================================
<!--
    //*********************************************************
    //
    // Copyright (c) Microsoft. All rights reserved.
    // THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF
    // ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY
    // IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR
    // PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.
    //
    //*********************************************************
-->
<Application
    x:Class="WinUIGallery.App"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:converters="using:WinUIGallery.Converters"
    xmlns:local="using:WinUIGallery">
    <Application.Resources>
        <ResourceDictionary>
            <ResourceDictionary.MergedDictionaries>
                <XamlControlsResources xmlns="using:Microsoft.UI.Xaml.Controls" />
                <local:ItemTemplates />
                <ResourceDictionary Source="ms-appx:///Controls/CopyButton.xaml" />
                <ResourceDictionary Source="ms-appx:///Controls/OpacityMaskView.xaml" />
                <ResourceDictionary Source="ms-appx:///Styles/Button.xaml" />
                <ResourceDictionary Source="ms-appx:///Styles/Grid.xaml" />
                <ResourceDictionary Source="ms-appx:///Styles/GridViewItem.xaml" />
                <ResourceDictionary Source="ms-appx:///Styles/TextBlock.xaml" />
                <ResourceDictionary Source="ms-appx:///Styles/SelectorBar.xaml" />
                <ResourceDictionary Source="ms-appx:///Samples/ControlPages/Fundamentals/Controls/CounterControl.xaml" />
                <ResourceDictionary Source="ms-appx:///Samples/ControlPages/Fundamentals/Controls/ValidatedPasswordBox.xaml" />
            </ResourceDictionary.MergedDictionaries>

            <ResourceDictionary.ThemeDictionaries>
                <ResourceDictionary x:Key="Light">
                    <SolidColorBrush x:Key="HomePageBackgroundBrush" Color="Transparent" />
                    <StaticResource x:Key="GalleryBackgroundBrush" ResourceKey="SolidBackgroundFillColorBaseBrush" />
                    <StaticResource x:Key="GalleryBorderBrush" ResourceKey="CardStrokeColorDefaultBrush" />
                </ResourceDictionary>
                <ResourceDictionary x:Key="Dark">
                    <SolidColorBrush x:Key="HomePageBackgroundBrush" Color="Transparent" />
                    <StaticResource x:Key="GalleryBackgroundBrush" ResourceKey="SolidBackgroundFillColorBaseBrush" />
                    <StaticResource x:Key="GalleryBorderBrush" ResourceKey="CardStrokeColorDefaultBrush" />
                </ResourceDictionary>
                <ResourceDictionary x:Key="HighContrast">
                    <SolidColorBrush x:Key="HomePageBackgroundBrush" Color="{ThemeResource SystemColorWindowColor}" />
                    <SolidColorBrush x:Key="GalleryBackgroundBrush" Color="{ThemeResource SystemColorWindowColor}" />
                    <SolidColorBrush x:Key="GalleryBorderBrush" Color="{ThemeResource SystemColorWindowColor}" />
                </ResourceDictionary>
            </ResourceDictionary.ThemeDictionaries>

            <!--  Application-specific resources  -->
            <x:String x:Key="ControlsName">All</x:String>
            <x:String x:Key="AppTitleName">WinUI 3 Gallery</x:String>
            <x:String x:Key="GitHubIconPath">M48.854 0C21.839 0 0 22 0 49.217c0 21.756 13.993 40.172 33.405 46.69 2.427.49 3.316-1.059 3.316-2.362 0-1.141-.08-5.052-.08-9.127-13.59 2.934-16.42-5.867-16.42-5.867-2.184-5.704-5.42-7.17-5.42-7.17-4.448-3.015.324-3.015.324-3.015 4.934.326 7.523 5.052 7.523 5.052 4.367 7.496 11.404 5.378 14.235 4.074.404-3.178 1.699-5.378 3.074-6.6-10.839-1.141-22.243-5.378-22.243-24.283 0-5.378 1.94-9.778 5.014-13.2-.485-1.222-2.184-6.275.486-13.038 0 0 4.125-1.304 13.426 5.052a46.97 46.97 0 0 1 12.214-1.63c4.125 0 8.33.571 12.213 1.63 9.302-6.356 13.427-5.052 13.427-5.052 2.67 6.763.97 11.816.485 13.038 3.155 3.422 5.015 7.822 5.015 13.2 0 18.905-11.404 23.06-22.324 24.283 1.78 1.548 3.316 4.481 3.316 9.126 0 6.6-.08 11.897-.08 13.526 0 1.304.89 2.853 3.316 2.364 19.412-6.52 33.405-24.935 33.405-46.691C97.707 22 75.788 0 48.854 0z</x:String>
            <x:String x:Key="TemplateStudioIconPath">M39,30l-15,7.5-5-2.5v-9l-4-2v9l-3-1.5v-14.944l12,5.944,15.034-7.447L24,3.831,9,15.027v14.973L0,34.5l24,12,24-12-9-4.5ZM24,7.575v11.577l-9.323-4.618,9.323-6.959Z</x:String>
            <x:Double x:Key="Breakpoint640Plus">641</x:Double>
            <x:Double x:Key="ColorSectionSpacing">4</x:Double>

            <!--  Style Overrides  -->
            <SolidColorBrush x:Key="GridViewHeaderItemDividerStroke" Color="Transparent" />
            <x:Double x:Key="TeachingTipMinWidth">48</x:Double>

            <!--  Converters  -->
            <converters:NullableBooleanToBooleanConverter x:Key="nullableBooleanToBooleanConverter" />
            <converters:NullToVisibilityConverter x:Key="nullToVisibilityConverter" />
            <converters:EmptyStringToVisibilityConverter x:Key="emptyStringToVisibilityConverter" />
            <converters:NullToVisibilityConverter
                x:Key="inverseNullToVisibilityConverter"
                NonNullValue="Collapsed"
                NullValue="Visible" />
            <converters:BooleanToValueConverter x:Key="booleanToValueConverter" />
            <converters:DoubleToThicknessConverter x:Key="doubleToThicknessConverter" />
        </ResourceDictionary>
    </Application.Resources>
</Application>



================================================
FILE: WinUIGallery/App.xaml.cs
================================================
//*********************************************************
//
// Copyright (c) Microsoft. All rights reserved.
// THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF
// ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY
// IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR
// PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.
//
//*********************************************************
using System;
using System.Diagnostics;
using System.Linq;
using Microsoft.UI.Xaml;
using Microsoft.UI.Xaml.Controls;
using Microsoft.UI.Xaml.Navigation;
using Microsoft.Windows.AppLifecycle;
using Microsoft.Windows.AppNotifications;
using Microsoft.Windows.AppNotifications.Builder;
using Microsoft.Windows.BadgeNotifications;
using Windows.ApplicationModel.Activation;
using WinUIGallery.Helpers;
using WinUIGallery.Pages;
using static WinUIGallery.Helpers.Win32;

namespace WinUIGallery;

/// <summary>
/// Provides application-specific behavior to supplement the default Application class.
/// </summary>
sealed partial class App : Application
{
    private static Window startupWindow;
    private static Win32WindowHelper win32WindowHelper;
    private static int registeredKeyPressedHook = 0;
    private HookProc keyEventHook;

    /// <summary>
    /// Get the initial window created for this app.
    /// </summary>
    public static Window StartupWindow
    {
        get => startupWindow;
    }

    /// <summary>
    /// Initializes the singleton Application object. This is the first line of authored code
    /// executed, and as such is the logical equivalent of main() or WinMain().
    /// </summary>
    public App()
    {
        InitializeComponent();
        UnhandledException += HandleExceptions;
    }

    /// <summary>
    /// Invoked when the application is launched normally by the end user.  Other entry points
    /// will be used such as when the application is launched to open a specific file.
    /// </summary>
    /// <param name="e">Details about the launch request and process.</param>
    protected override void OnLaunched(Microsoft.UI.Xaml.LaunchActivatedEventArgs args)
    {
        IdleSynchronizer.Init();

        startupWindow = WindowHelper.CreateWindow();
        startupWindow.ExtendsContentIntoTitleBar = true;

        win32WindowHelper = new Win32WindowHelper(startupWindow);
        win32WindowHelper.SetWindowMinMaxSize(new Win32WindowHelper.POINT() { x = 532, y = 500 });

#if DEBUG
        if (Debugger.IsAttached)
        {
            DebugSettings.BindingFailed += DebugSettings_BindingFailed;
        }
#endif

        keyEventHook = KeyEventHook;
        registeredKeyPressedHook = SetWindowKeyHook(keyEventHook);

        EnsureWindow();

        startupWindow.Closed += (s, e) =>
        {
            BadgeNotificationManager.Current.ClearBadge();
        };
    }

    private int KeyEventHook(int nCode, IntPtr wParam, IntPtr lParam)
    {
        if (nCode >= 0 && IsKeyDownHook(lParam))
        {
            RootFrameNavigationHelper.RaiseKeyPressed((uint)wParam);
        }

        return CallNextHookEx(registeredKeyPressedHook, nCode, wParam, lParam);
    }

    private void DebugSettings_BindingFailed(object sender, BindingFailedEventArgs e)
    {
        // Ignore the exception from NonExistentProperty in BindingPage.xaml,
        // as the sample code intentionally includes a binding failure.
        if (e.Message.Contains("NonExistentProperty"))
        {
            return;
        }

        throw new Exception($"A debug binding failed: " + e.Message);
    }

    private async void EnsureWindow()
    {
        await ControlInfoDataSource.Instance.GetGroupsAsync();
        await IconsDataSource.Instance.LoadIcons();

        Frame rootFrame = GetRootFrame();

        ThemeHelper.Initialize();

        var targetPageType = typeof(HomePage);
        var targetPageArguments = string.Empty;

        AppActivationArguments eventArgs = AppInstance.GetCurrent().GetActivatedEventArgs();
        if (eventArgs != null && eventArgs.Kind == ExtendedActivationKind.Protocol && eventArgs.Data is ProtocolActivatedEventArgs)
        {
            var ProtocolArgs = eventArgs.Data as ProtocolActivatedEventArgs;
            string uri = ProtocolArgs.Uri.LocalPath.Replace("/", "");
            targetPageArguments = uri;

            if (uri == "AllControls")
            {
                targetPageType = typeof(AllControlsPage);
            }
            else if (uri == "NewControls")
            {
                targetPageType = typeof(HomePage);
            }
            else if (ControlInfoDataSource.Instance.Groups.Any(g => g.UniqueId == uri))
            {
                targetPageType = typeof(SectionPage);
            }
            else if (ControlInfoDataSource.Instance.Groups.Any(g => g.Items.Any(i => i.UniqueId == uri)))
            {
                targetPageType = typeof(ItemPage);
            }
        }

        var rootPage = StartupWindow.Content as NavigationRootPage;
        rootPage.Navigate(targetPageType, targetPageArguments);

        if (targetPageType == typeof(HomePage))
        {
            var navItem = (NavigationViewItem)rootPage.NavigationView.MenuItems[0];
            navItem.IsSelected = true;
        }

        // Activate the startup window.
        StartupWindow.Activate();
    }

    /// <summary>
    /// Gets the frame of the StartupWindow.
    /// </summary>
    /// <returns>The frame of the StartupWindow.</returns>
    /// <exception cref="Exception">Thrown if the window doesn't have a frame with the name "rootFrame".</exception>
    public Frame GetRootFrame()
    {
        Frame rootFrame;
        if (StartupWindow.Content is NavigationRootPage rootPage)
        {
            rootFrame = (Frame)rootPage.FindName("rootFrame");
        }
        else
        {
            rootPage = new NavigationRootPage();
            rootFrame = (Frame)rootPage.FindName("rootFrame");
            if (rootFrame == null)
            {
                throw new Exception("Root frame not found");
            }
            SuspensionManager.RegisterFrame(rootFrame, "AppFrame");
            rootFrame.Language = Windows.Globalization.ApplicationLanguages.Languages[0];
            rootFrame.NavigationFailed += OnNavigationFailed;

            StartupWindow.Content = rootPage;
        }

        return rootFrame;
    }

    /// <summary>
    /// Invoked when Navigation to a certain page fails
    /// </summary>
    /// <param name="sender">The Frame which failed navigation</param>
    /// <param name="e">Details about the navigation failure</param>
    void OnNavigationFailed(object sender, NavigationFailedEventArgs e)
    {
        throw new Exception("Failed to load Page " + e.SourcePageType.FullName);
    }

    /// <summary>
    /// Prevents the app from crashing when a exception gets thrown and notifies the user.
    /// </summary>
    /// <param name="sender">The app as an object.</param>
    /// <param name="e">Details about the exception.</param>
    private void HandleExceptions(object sender, Microsoft.UI.Xaml.UnhandledExceptionEventArgs e)
    {
        e.Handled = true; //Don't crash the app.

        //Create the notification.
        var notification = new AppNotificationBuilder()
            .AddText("An exception was thrown.")
            .AddText($"Type: {e.Exception.GetType()}")
            .AddText($"Message: {e.Message}\r\n" +
                     $"HResult: {e.Exception.HResult}")
            .BuildNotification();

        //Show the notification
        AppNotificationManager.Default.Show(notification);
    }
}



================================================
FILE: WinUIGallery/CollectionsInterop.cs
================================================
﻿using Microsoft.UI.Xaml.Data;
using Microsoft.UI.Xaml.Interop;
using System;
using System.Collections;
using System.Collections.Generic;
using System.Collections.ObjectModel;
using System.Collections.Specialized;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

using NotifyCollectionChangedAction = Microsoft.UI.Xaml.Interop.NotifyCollectionChangedAction;

namespace WinUIGallery;

// .NET collection types are tightly coupled with WUX types - e.g., ObservableCollection<T>
// maps to WUX.INotifyCollectionChanged, and creates WUX.NotifyCollectionChangedEventArgs
// when raising its INCC event.  This is a problem because we've switched everything else over
// to use MUX types, such that creating WUX types raises an RPC_E_WRONG_THREAD error
// due to DXamlCore not being initialized.  For the purposes of our tests, we're providing
// our own implementation of ObservableCollection<T> that implements MUX.INotifyCollectionChanged.
public class ObservableCollection<T> : Collection<T>, Microsoft.UI.Xaml.Interop.INotifyCollectionChanged, INotifyPropertyChanged
{
    private ReentrancyGuard reentrancyGuard = null;

    private class ReentrancyGuard : IDisposable
    {
        private ObservableCollection<T> owningCollection;

        public ReentrancyGuard(ObservableCollection<T> owningCollection)
        {
            owningCollection.CheckReentrancy();
            owningCollection.reentrancyGuard = this;
            this.owningCollection = owningCollection;
        }

        public void Dispose()
        {
            owningCollection.reentrancyGuard = null;
        }
    }

    public ObservableCollection() : base() { }
    public ObservableCollection(IList<T> list) : base(list.ToList()) { }
    public ObservableCollection(IEnumerable<T> collection) : base(collection.ToList()) { }

    public event Microsoft.UI.Xaml.Interop.NotifyCollectionChangedEventHandler CollectionChanged;

    public void Move(int oldIndex, int newIndex)
    {
        MoveItem(oldIndex, newIndex);
    }

    protected IDisposable BlockReentrancy()
    {
        return new ReentrancyGuard(this);
    }

    protected void CheckReentrancy()
    {
        if (reentrancyGuard != null)
        {
            throw new InvalidOperationException("Collection cannot be modified in a collection changed handler.");
        }
    }

    protected override void ClearItems()
    {
        CheckReentrancy();

        TestBindableVector<T> oldItems = new TestBindableVector<T>(this);

        base.ClearItems();
        OnCollectionChanged(
            NotifyCollectionChangedAction.Reset,
            null, oldItems, 0, 0);
    }

    protected override void InsertItem(int index, T item)
    {
        CheckReentrancy();

        TestBindableVector<T> newItem = new TestBindableVector<T>();
        newItem.Add(item);

        base.InsertItem(index, item);
        OnCollectionChanged(
            NotifyCollectionChangedAction.Add,
            newItem, null, index, 0);
    }

    protected virtual void MoveItem(int oldIndex, int newIndex)
    {
        CheckReentrancy();

        TestBindableVector<T> oldItem = new TestBindableVector<T>();
        oldItem.Add(this[oldIndex]);
        TestBindableVector<T> newItem = new TestBindableVector<T>(oldItem);

        T item = this[oldIndex];
        base.RemoveAt(oldIndex);
        base.InsertItem(newIndex, item);
        OnCollectionChanged(
            NotifyCollectionChangedAction.Move,
            newItem, oldItem, newIndex, oldIndex);
    }

    protected override void RemoveItem(int index)
    {
        CheckReentrancy();

        TestBindableVector<T> oldItem = new TestBindableVector<T>();
        oldItem.Add(this[index]);

        base.RemoveItem(index);
        OnCollectionChanged(
            NotifyCollectionChangedAction.Remove,
            null, oldItem, 0, index);
    }

    protected override void SetItem(int index, T item)
    {
        CheckReentrancy();

        TestBindableVector<T> oldItem = new TestBindableVector<T>();
        oldItem.Add(this[index]);
        TestBindableVector<T> newItem = new TestBindableVector<T>();
        newItem.Add(item);

        base.SetItem(index, item);
        OnCollectionChanged(
            NotifyCollectionChangedAction.Replace,
            newItem, oldItem, index, index);
    }

    protected virtual void OnCollectionChanged(
        NotifyCollectionChangedAction action,
        IBindableVector newItems,
        IBindableVector oldItems,
        int newIndex,
        int oldIndex)
    {
        OnCollectionChanged(new Microsoft.UI.Xaml.Interop.NotifyCollectionChangedEventArgs(action, newItems, oldItems, newIndex, oldIndex));
    }

    protected virtual void OnCollectionChanged(Microsoft.UI.Xaml.Interop.NotifyCollectionChangedEventArgs e)
    {
        using (BlockReentrancy())
        {
            CollectionChanged?.Invoke(this, e);
        }
    }

#pragma warning disable 0067 // PropertyChanged is never used, raising a warning, but it's needed to implement INotifyPropertyChanged.
    public event PropertyChangedEventHandler PropertyChanged;
#pragma warning restore 0067
}

public class TestBindableVector<T> : IList<T>, IBindableVector
{
    IList<T> implementation;

    public TestBindableVector() { implementation = new List<T>(); }
    public TestBindableVector(IList<T> list) { implementation = new List<T>(list); }

    public T this[int index] { get => implementation[index]; set => implementation[index] = value; }

    public int Count => implementation.Count;

    public virtual bool IsReadOnly => implementation.IsReadOnly;

    public void Add(T item)
    {
        implementation.Add(item);
    }

    public void Clear()
    {
        implementation.Clear();
    }

    public bool Contains(T item)
    {
        return implementation.Contains(item);
    }

    public void CopyTo(T[] array, int arrayIndex)
    {
        implementation.CopyTo(array, arrayIndex);
    }

    public IEnumerator<T> GetEnumerator()
    {
        return implementation.GetEnumerator();
    }

    public int IndexOf(T item)
    {
        return implementation.IndexOf(item);
    }

    public void Insert(int index, T item)
    {
        implementation.Insert(index, item);
    }

    public bool Remove(T item)
    {
        return implementation.Remove(item);
    }

    public void RemoveAt(int index)
    {
        implementation.RemoveAt(index);
    }

    IEnumerator IEnumerable.GetEnumerator()
    {
        return implementation.GetEnumerator();
    }

    public object GetAt(uint index)
    {
        return implementation[(int)index];
    }

    public IBindableVectorView GetView()
    {
        return new TestBindableVectorView<T>(implementation);
    }

    public bool IndexOf(object value, out uint index)
    {
        int indexOf = implementation.IndexOf((T)value);

        if (indexOf >= 0)
        {
            index = (uint)indexOf;
            return true;
        }
        else
        {
            index = 0;
            return false;
        }
    }

    public void SetAt(uint index, object value)
    {
        implementation[(int)index] = (T)value;
    }

    public void InsertAt(uint index, object value)
    {
        implementation.Insert((int)index, (T)value);
    }

    public void RemoveAt(uint index)
    {
        implementation.RemoveAt((int)index);
    }

    public void Append(object value)
    {
        implementation.Add((T)value);
    }

    public void RemoveAtEnd()
    {
        implementation.RemoveAt(implementation.Count - 1);
    }

    public uint Size => (uint)implementation.Count;

    public IBindableIterator First()
    {
        return new TestBindableIterator<T>(implementation);
    }
}

public class TestBindableVectorView<T> : TestBindableVector<T>, IBindableVectorView
{
    public TestBindableVectorView(IList<T> list) : base(list) { }

    public override bool IsReadOnly => true;
}

public class TestBindableIterator<T> : IBindableIterator
{
    private readonly IEnumerator<T> enumerator;

    public TestBindableIterator(IEnumerable<T> enumerable) { enumerator = enumerable.GetEnumerator(); }

    public bool MoveNext()
    {
        return enumerator.MoveNext();
    }

    public object Current => enumerator.Current;

    public bool HasCurrent => enumerator.Current != null;
}



================================================
FILE: WinUIGallery/common.props
================================================
<Project>
    <!-- This file is similar to Directory.Build.props, in that it contains properties common to all WinUI Gallery projects.
         However, this props file is imported directly in the projects themselves,
         since Directory.Build.props is imported before some key MSBuild properties are set which we need here.  In general, common properties
         should go in Directory.Build.props instead of here, this just contains special cases. -->

    <!-- When building outside the WinUI repo, configure the NugetPackageDirectory property it normally sets.  This value is based
         off of the NuGetPackageRoot property set in the auto-generated NuGet props.  Unfortunately, the auto-generated props
         are imported after Directory.Build.props, so we can't assign it there -->
    <PropertyGroup Condition="'$(NugetPackageDirectory)' == '' AND '$(IsInWinUIRepo)' != 'true' ">
        <NugetPackageDirectory>$(NuGetPackageRoot)</NugetPackageDirectory>
    </PropertyGroup>
</Project>


================================================
FILE: WinUIGallery/ContentIncludes.props
================================================
<Project>
  <ItemGroup>
    <Content Include="Assets\SampleMedia\CoffeeCup.png" />
    <Content Include="Assets\SampleMedia\Contacts.txt" />
    <Content Include="Assets\CopyLinkTeachingTip.png" />
    <Content Include="Assets\SampleMedia\folder.png" />
    <Content Include="Assets\SampleMedia\SunBlack.png" />
    <Content Include="Assets\SampleMedia\SunWhite.png" />
    <Content Include="Assets\SampleMedia\Slices.png" />
    <Content Include="Assets\SampleMedia\Slices2.png" />
    <Content Include="Assets\ControlImages\Acrylic.png" />
    <Content Include="Assets\ControlImages\AnimatedIcon.png" />
    <Content Include="Assets\ControlImages\AnimatedVisualPlayer.png" />
    <Content Include="Assets\ControlImages\AnimationInterop.png" />
    <Content Include="Assets\ControlImages\AnnotatedScrollBar.png" />
    <Content Include="Assets\ControlImages\AppBarButton.png" />
    <Content Include="Assets\ControlImages\AppBarSeparator.png" />
    <Content Include="Assets\ControlImages\AppBarToggleButton.png" />
    <Content Include="Assets\ControlImages\AutoSuggestBox.png" />
    <Content Include="Assets\ControlImages\Border.png" />
    <Content Include="Assets\ControlImages\BreadcrumbBar.png" />
    <Content Include="Assets\ControlImages\Button.png" />
    <Content Include="Assets\ControlImages\CalendarDatePicker.png" />
    <Content Include="Assets\ControlImages\CalendarView.png" />
    <Content Include="Assets\ControlImages\CaptureElement.png" />
    <Content Include="Assets\ControlImages\Canvas.png" />
    <Content Include="Assets\ControlImages\Checkbox.png" />
    <Content Include="Assets\ControlImages\Clipboard.png" />
    <Content Include="Assets\ControlImages\ColorPaletteResources.png" />
    <Content Include="Assets\ControlImages\ColorPicker.png" />
    <Content Include="Assets\ControlImages\ComboBox.png" />
    <Content Include="Assets\ControlImages\CommandBar.png" />
    <Content Include="Assets\ControlImages\CommandBarFlyout.png" />
    <Content Include="Assets\ControlImages\CompactSizing.png" />
    <Content Include="Assets\ControlImages\ConnectedAnimation.png" />
    <Content Include="Assets\ControlImages\ContentDialog.png" />
    <Content Include="Assets\ControlImages\CreateMultipleWindows.png" />
    <Content Include="Assets\ControlImages\DatePicker.png" />
    <Content Include="Assets\ControlImages\DropDownButton.png" />
    <Content Include="Assets\ControlImages\EasingFunction.png" />
    <Content Include="Assets\ControlImages\Expander.png" />
    <Content Include="Assets\ControlImages\FilePicker.png" />
    <Content Include="Assets\ControlImages\FlipView.png" />
    <Content Include="Assets\ControlImages\Flyout.png" />
    <Content Include="Assets\ControlImages\Grid.png" />
    <Content Include="Assets\ControlImages\GridView.png" />
    <Content Include="Assets\ControlImages\HyperlinkButton.png" />
    <Content Include="Assets\ControlImages\IconElement.png" />
    <Content Include="Assets\ControlImages\Image.png" />
    <Content Include="Assets\ControlImages\ImplicitTransition.png" />
    <Content Include="Assets\ControlImages\InfoBadge.png" />
    <Content Include="Assets\ControlImages\InfoBar.png" />
    <Content Include="Assets\ControlImages\ItemsRepeater.png" />
    <Content Include="Assets\ControlImages\ItemsView.png" />
    <Content Include="Assets\ControlImages\Line.png" />
    <Content Include="Assets\ControlImages\ListBox.png" />
    <Content Include="Assets\ControlImages\ListView.png" />
    <Content Include="Assets\ControlImages\MapControl.png" />
    <Content Include="Assets\ControlImages\MediaPlayerElement.png" />
    <Content Include="Assets\ControlImages\MenuBar.png" />
    <Content Include="Assets\ControlImages\MenuFlyout.png" />
    <Content Include="Assets\ControlImages\NavigationView.png" />
    <Content Include="Assets\ControlImages\NumberBox.png" />
    <Content Include="Assets\ControlImages\PageTransition.png" />
    <Content Include="Assets\ControlImages\ParallaxView.png" />
    <Content Include="Assets\ControlImages\PasswordBox.png" />
    <Content Include="Assets\ControlImages\PersonPicture.png" />
    <Content Include="Assets\ControlImages\PipsPager.png" />
    <Content Include="Assets\ControlImages\Pivot.png" />
    <Content Include="Assets\ControlImages\Placeholder.png" />
    <Content Include="Assets\ControlImages\ProgressBar.png" />
    <Content Include="Assets\ControlImages\ProgressRing.png" />
    <Content Include="Assets\ControlImages\PullToRefresh.png" />
    <Content Include="Assets\ControlImages\RadialGradientBrush.png" />
    <Content Include="Assets\ControlImages\RadioButton.png" />
    <Content Include="Assets\ControlImages\RadioButtons.png" />
    <Content Include="Assets\ControlImages\RatingControl.png" />
    <Content Include="Assets\ControlImages\RelativePanel.png" />
    <Content Include="Assets\ControlImages\RepeatButton.png" />
    <Content Include="Assets\ControlImages\RichEditBox.png" />
    <Content Include="Assets\ControlImages\RichTextBlock.png" />
    <Content Include="Assets\ControlImages\ScratchPad.png" />
    <Content Include="Assets\ControlImages\ScrollView.png" />
    <Content Include="Assets\ControlImages\ScrollViewer.png" />
    <Content Include="Assets\ControlImages\SemanticZoom.png" />
    <Content Include="Assets\ControlImages\Shape.png" />
    <Content Include="Assets\ControlImages\Slider.png" />
    <Content Include="Assets\ControlImages\Sound.png" />
    <Content Include="Assets\ControlImages\SplitButton.png" />
    <Content Include="Assets\ControlImages\SplitView.png" />
    <Content Include="Assets\ControlImages\StackPanel.png" />
    <Content Include="Assets\ControlImages\StandardUICommand.png" />
    <Content Include="Assets\ControlImages\SwipeControl.png" />
    <Content Include="Assets\ControlImages\TabView.png" />
    <Content Include="Assets\ControlImages\TeachingTip.png" />
    <Content Include="Assets\ControlImages\TextBlock.png" />
    <Content Include="Assets\ControlImages\TextBox.png" />
    <Content Include="Assets\ControlImages\ThemeTransition.png" />
    <Content Include="Assets\ControlImages\TimePicker.png" />
    <Content Include="Assets\ControlImages\TitleBar.png" />
    <Content Include="Assets\ControlImages\ToggleButton.png" />
    <Content Include="Assets\ControlImages\ToggleSplitButton.png" />
    <Content Include="Assets\ControlImages\ToggleSwitch.png" />
    <Content Include="Assets\ControlImages\ToolTip.png" />
    <Content Include="Assets\ControlImages\TreeView.png" />
    <Content Include="Assets\ControlImages\VariableSizedWrapGrid.png" />
    <Content Include="Assets\ControlImages\Viewbox.png" />
    <Content Include="Assets\ControlImages\WebView.png" />
    <Content Include="Assets\ControlImages\XamlUICommand.png" />
    <Content Include="Assets\SampleMedia\MirrorPCConsent.svg" />
    <Content Include="Assets\SampleMedia\cliff.jpg" />
    <Content Include="Assets\SampleMedia\fishes.wmv" />
    <Content Include="Assets\SampleMedia\grapes.jpg" />
    <Content Include="Assets\SampleMedia\ladybug.wmv" />
    <Content Include="Assets\SampleMedia\LandscapeImage1.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage2.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage3.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage4.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage5.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage6.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage7.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage8.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage9.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage10.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage11.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage12.jpg" />
    <Content Include="Assets\SampleMedia\LandscapeImage13.jpg" />
    <Content Include="Assets\SampleMedia\rainier.jpg" />
    <Content Include="Assets\SampleMedia\sunset.jpg" />
    <Content Include="Assets\SampleMedia\treetops.jpg" />
    <Content Include="Assets\SampleMedia\valley.jpg" />
    <Content Include="Assets\SampleMedia\MapExample.png" />
    <Content Include="Assets\SampleMedia\cmd.png" />
    <Content Include="Assets\SampleMedia\linux.png" />
    <Content Include="Assets\SampleMedia\powershell.png" />
    <Content Include="Assets\Tiles\LargeTile.scale-100.png" />
    <Content Include="Assets\Tiles\LargeTile.scale-125.png" />
    <Content Include="Assets\Tiles\LargeTile.scale-150.png" />
    <Content Include="Assets\Tiles\LargeTile.scale-200.png" />
    <Content Include="Assets\Tiles\LargeTile.scale-400.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-100.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-125.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-150.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-200.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-400.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-100.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-125.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-150.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-200.png" />
    <Content Include="Assets\Tiles\SmallTile.scale-400.png" />
    <Content Include="Assets\Tiles\SplashScreen.scale-100.png" />
    <Content Include="Assets\Tiles\SplashScreen.scale-125.png" />
    <Content Include="Assets\Tiles\SplashScreen.scale-150.png" />
    <Content Include="Assets\Tiles\SplashScreen.scale-200.png" />
    <Content Include="Assets\Tiles\SplashScreen.scale-400.png" />
    <Content Include="Assets\Tiles\MedTile.scale-100.png" />
    <Content Include="Assets\Tiles\MedTile.scale-125.png" />
    <Content Include="Assets\Tiles\MedTile.scale-150.png" />
    <Content Include="Assets\Tiles\MedTile.scale-200.png" />
    <Content Include="Assets\Tiles\MedTile.scale-400.png" />
    <Content Include="Assets\Tiles\StoreLogo.scale-100.png" />
    <Content Include="Assets\Tiles\StoreLogo.scale-125.png" />
    <Content Include="Assets\Tiles\StoreLogo.scale-150.png" />
    <Content Include="Assets\Tiles\StoreLogo.scale-200.png" />
    <Content Include="Assets\Tiles\StoreLogo.scale-400.png" />
    <Content Include="Assets\Tiles\WideTile.scale-100.png" />
    <Content Include="Assets\Tiles\WideTile.scale-125.png" />
    <Content Include="Assets\Tiles\WideTile.scale-150.png" />
    <Content Include="Assets\Tiles\WideTile.scale-200.png" />
    <Content Include="Assets\Tiles\WideTile.scale-400.png" />
    <Content Include="Samples\SampleCode\Binding\BindingSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample3_csharp.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample4_csharp.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample5_csharp.txt" />
    <Content Include="Samples\SampleCode\Brushes\RadialGradientBrushSample_xaml.txt" />
    <Content Include="Samples\SampleCode\Buttons\Button\CustomButtonStyle.txt" />
    <Content Include="Samples\SampleCode\Buttons\DropDown\DropDownButton_Icon.txt" />
    <Content Include="Samples\SampleCode\Buttons\DropDown\DropDownButton_RevealStyle.txt" />
    <Content Include="Samples\SampleCode\Buttons\DropDown\DropDownButton_Simple.txt" />
    <Content Include="Samples\SampleCode\Buttons\SplitButton\SplitButtonSample1.txt" />
    <Content Include="Samples\SampleCode\Buttons\SplitButton\SplitButtonSample2.txt" />
    <Content Include="Samples\SampleCode\Buttons\ToggleSplitButton\ToggleSplitButtonSample1.txt" />
    <Content Include="Samples\SampleCode\ContentDialog\ContentDialogSample1_cs.txt" />
    <Content Include="Samples\SampleCode\ContentDialog\ContentDialogSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Geometry\GeometrySample_xaml.txt" />
    <Content Include="Samples\SampleCode\GridView\GridViewSample1_cs.txt" />
    <Content Include="Samples\SampleCode\GridView\GridViewSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\AnimatedIconSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\AnimatedIconSample1_cs.txt" />
    <Content Include="Samples\SampleCode\Icons\AnimatedIconSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\SymbolIconSample_1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\PathIconSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\ImageIconSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\ImageIconSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\FontIconSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Icons\FontIconSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterNestedSample_xaml.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample1_cs.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample2_cs.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample3_cs.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample4_cs.txt" />
    <Content Include="Samples\SampleCode\ItemsRepeater\ItemsRepeaterSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewGroupedHeaderSample_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample1_cs.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample2_cs.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample4_cs.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\ListView\ListViewStickyHeaderSample_xaml.txt" />
    <Content Include="Samples\SampleCode\MapControl\MapControlSample_cs.txt" />
    <Content Include="Samples\SampleCode\Media\CaptureElementPreviewSample_cs.txt" />
    <Content Include="Samples\SampleCode\Media\CaptureElementPreviewSample_xaml.txt" />
    <Content Include="Samples\SampleCode\MenuBar\MenuBarSample1.txt" />
    <Content Include="Samples\SampleCode\MenuBar\MenuBarSample2.txt" />
    <Content Include="Samples\SampleCode\MenuBar\MenuBarSample3.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample4_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample5_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample5_xaml.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample5_cs.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample5_xaml.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample1.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample2.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample3.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample4_cs.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample6.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample8_xaml.txt" />
    <Content Include="Samples\SampleCode\NavigationView\NavigationViewSample9_xaml.txt" />
    <Content Include="Samples\SampleCode\NumberBox\NumberBoxSample3_cs.txt" />
    <Content Include="Samples\SampleCode\NumberBox\NumberBoxSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample1_cs.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample2_cs.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample3_cs.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample4_cs.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample5_cs.txt" />
    <Content Include="Samples\SampleCode\System\FilePickerSample5_xaml.txt" />
    <Content Include="Samples\SampleCode\System\Window.txt" />
    <Content Include="Samples\SampleCode\SystemBackdrops\SystemBackdropsSampleBackdropTypes_cs.txt" />
    <Content Include="Samples\SampleCode\SystemBackdrops\SystemBackdropsSampleBackdropTypes_xaml.txt" />
    <Content Include="Samples\SampleCode\SystemBackdrops\SystemBackdropsSampleMicaController.txt" />
    <Content Include="Samples\SampleCode\SystemBackdrops\SystemBackdropsSampleDesktopAcrylicController.txt" />
    <Content Include="Samples\SampleCode\SystemBackdrops\SystemBackdropsEnsureSystemDQC.txt" />
    <Content Include="Samples\SampleCode\TabView\TabViewBasicSample_cs.txt" />
    <Content Include="Samples\SampleCode\TabView\TabViewKeyboardAcceleratorSample_cs.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample3_cs.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample2_cs.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample1_cs.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\TeachingTip\TeachingTipSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\Text\RichEditBox\RichEditBoxSample3_cs.txt" />
    <Content Include="Samples\SampleCode\Text\RichEditBox\RichEditBoxSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\Text\RichEditBox\RichEditBoxSample4_cs.txt" />
    <Content Include="Samples\SampleCode\Text\RichEditBox\RichEditBoxSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\TreeView\TreeViewDataBindingSample_xaml.txt" />
    <Content Include="Samples\SampleCode\TreeView\TreeViewTemplateSelectorSample_xaml.txt" />
    <Content Include="Samples\SampleCode\Typography\TypographySample_xaml.txt" />
    <Content Include="Samples\SampleCode\StandardUICommand\StandardUICommandSample1_cs.txt" />
    <Content Include="Samples\SampleCode\StandardUICommand\StandardUICommandSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\ScrollView\ScrollViewSample3_AccordionAnimation_cs.txt" />
    <Content Include="Samples\SampleCode\ScrollView\ScrollViewSample3_DefaultAnimation_cs.txt" />
    <Content Include="Samples\SampleCode\ScrollView\ScrollViewSample3_TeleportationAnimation_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample3_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample2_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\Motion\AnimationInterop\AnimationInteropSample1_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\ConnectedAnimation\ConnectedAnimationSample1_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\ConnectedAnimation\ConnectedAnimationSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Motion\ConnectedAnimation\ConnectedAnimationSample2_cs.txt" />
    <Content Include="Samples\SampleCode\Motion\ConnectedAnimation\ConnectedAnimationSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\Motion\ConnectedAnimation\ConnectedAnimationSample3_cs.txt" />
    <Content Include="Samples\SampleCode\CommandBarFlyout\CommandBarFlyoutSample1_cs.txt" />
    <Content Include="Samples\SampleCode\CommandBarFlyout\CommandBarFlyoutSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlUICommand\XamlUICommandSample1_cs.txt" />
    <Content Include="Samples\SampleCode\XamlUICommand\XamlUICommandSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Window\CreateWindowSample1.txt" />
    <Content Include="Samples\SampleCode\Window\TitleBar\TitleBarSample1.txt" />
    <Content Include="Samples\SampleCode\Window\TitleBar\TitleBarSample2.txt" />
    <Content Include="Samples\SampleCode\Window\TitleBar\TitleBarSample3.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample3_csharp.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample4_csharp.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample4_xaml.txt" />
    <Content Include="Samples\SampleCode\Binding\BindingSample5_csharp.txt" />
    <Content Include="Samples\SampleCode\TreeView\TreeViewDataBindingSample_cs.txt" />
    <Content Include="Samples\SampleCode\TreeView\TreeViewSample1_cs.txt" />
    <Content Include="Samples\SampleCode\TreeView\TreeViewTemplateSelectorSample_cs.txt" />
    <Content Include="Samples\SampleCode\Templates\TemplatesSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\Templates\TemplatesSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\Templates\TemplatesSample3_StackPanel_xaml.txt" />
    <Content Include="Samples\SampleCode\Templates\TemplatesSample3_WrapGrid_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlResources\XamlResourcesSample1_csharp.txt" />
    <Content Include="Samples\SampleCode\XamlResources\XamlResourcesSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlResources\XamlResourcesSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlResources\XamlResourcesSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlStyles\XamlStylesSample1_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlStyles\XamlStylesSample2_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlStyles\XamlStylesSample3_xaml.txt" />
    <Content Include="Samples\SampleCode\XamlStyles\XamlStylesSample4_csharp.txt" />
    <Content Include="Samples\Data\ControlInfoData.json" />
    <Content Include="Samples\Data\IconsData.json" />
  </ItemGroup>
</Project>



================================================
FILE: WinUIGallery/Directory.Build.props
================================================
<?xml version="1.0" encoding="utf-8"?>
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <!-- We have two projects in the same directory here, so we'll add a differentiator folder to output directories. -->
    <GenerateProjectSpecificOutputFolder>true</GenerateProjectSpecificOutputFolder>
  </PropertyGroup>

  <Import Project="$([MSBuild]::GetPathOfFileAbove('Directory.Build.props', '$(MSBuildThisFileDirectory)../'))" Condition="Exists($([MSBuild]::GetPathOfFileAbove('Directory.Build.props', '$(MSBuildThisFileDirectory)../')))" />

  <!-- When building standalone, WinUI Gallery needs to do some extra things that are done implicitly in the WinUI repo.-->
  <PropertyGroup Condition="'$(IsInWinUIRepo)' == 'true'">
    <!-- We want to binplace the WinUI Gallery pdb to a subdirectory of Symbols\Test so that the UWP and Desktop versions don't
         overwrite each other. -->
    <BinplaceSymbolsToSubdir>true</BinplaceSymbolsToSubdir>
  </PropertyGroup>

    <!--
         When building in the WinUI repo, we likely only have one current flavor built, either x86 or x64, and won't have locally built bits to support both.
         In that case, we only build an appx for the current flavor.  If we're not in the WinUI repo or specify we have all flavors built with BuildAllAppFlavors,
         we will build both the x86 and x64 flavors into the same appx.
    -->
  <PropertyGroup Condition="'$(IsInWinUIRepo)' != 'true' AND '$(BuildAllAppFlavors)' == ''">
    <BuildAllAppFlavors>true</BuildAllAppFlavors>
  </PropertyGroup>
</Project>


================================================
FILE: WinUIGallery/Directory.Build.targets
================================================
<?xml version="1.0" encoding="utf-8"?>
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <Import Project="$([MSBuild]::GetPathOfFileAbove('Directory.Build.targets', '$(MSBuildThisFileDirectory)../'))" Condition="Exists($([MSBuild]::GetPathOfFileAbove('Directory.Build.targets', '$(MSBuildThisFileDirectory)../')))"/>
  <PropertyGroup Condition="'$(WindowsPackageType)' == 'MSIX'">
    <!-- These are set in Directory.Build.targets because we need to import the publish profile first -->
    <AppxPackageName>WinUIGallery.Desktop</AppxPackageName>
  </PropertyGroup>

  <Import Project="net7.override.targets" Condition="'$(MSBuildRuntimeType)' == 'Core'" />

</Project>


================================================
FILE: WinUIGallery/GlobalSuppressions.cs
================================================
﻿// This file is used by Code Analysis to maintain SuppressMessage
// attributes that are applied to this project.
// Project-level suppressions either have no target or are given
// a specific target and scoped to a namespace, type, member, etc.

using System.Diagnostics.CodeAnalysis;

[assembly: SuppressMessage("Interoperability", "CA1416:Validate platform compatibility", Justification = "<Pending>")]



================================================
FILE: WinUIGallery/net7.override.targets
================================================
<Project>
<!-- Hack to get around issues with missing tasks in .net core -->
  <Target Name="GetInstalledSDKLocations"
      Condition="'@(SDKReference)' != ''"
      DependsOnTargets="$(GetInstalledSDKLocationsDependsOn)"
      Returns="@(InstalledSDKLocations)">
    <ItemGroup>
    </ItemGroup>
  </Target>
  <Target
      Name="ResolveSDKReferences"
      Returns="@(ResolvedSDKReference)"
      DependsOnTargets="$(ResolveSDKReferencesDependsOn)">
    <ItemGroup>
    </ItemGroup>
  </Target>
</Project>


================================================
FILE: WinUIGallery/Package.appxmanifest
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<Package
    xmlns="http://schemas.microsoft.com/appx/manifest/foundation/windows10"
    xmlns:mp="http://schemas.microsoft.com/appx/2014/phone/manifest"
    xmlns:uap="http://schemas.microsoft.com/appx/manifest/uap/windows10"
    xmlns:uap3="http://schemas.microsoft.com/appx/manifest/uap/windows10/3"
    xmlns:rescap="http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities"
    IgnorableNamespaces="uap mp uap3">
  <!--Note: package version and assembly version must be kept in sync-->
  <Identity Name="Microsoft.WinUI3ControlsGallery" Publisher="CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US" Version="2.6.0.0" />
  <mp:PhoneIdentity PhoneProductId="863667e0-667a-4bb4-ac52-c59656c7333a" PhonePublisherId="00000000-0000-0000-0000-000000000000" />
  <Properties>
    <DisplayName>WinUI 3 Gallery</DisplayName>
    <PublisherDisplayName>Microsoft Corporation</PublisherDisplayName>
    <Logo>Assets\Tiles\StoreLogo.png</Logo>
    <uap:SupportedUsers>multiple</uap:SupportedUsers>
  </Properties>
  <Dependencies>
      <TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.17763.0" MaxVersionTested="10.0.19041.0" />
  </Dependencies>
  <Resources>
    <Resource Language="x-generate" />
  </Resources>
  <Applications>
    <Application Id="App" Executable="$targetnametoken$.exe" EntryPoint="$targetentrypoint$">
      <uap:VisualElements DisplayName="WinUI 3 Gallery" Square150x150Logo="Assets\Tiles\MedTile.png" Square44x44Logo="Assets\Tiles\AppList.png" Description="WinUI 3 Gallery" BackgroundColor="transparent">
        <uap:DefaultTile Square310x310Logo="Assets\Tiles\LargeTile.png" Wide310x150Logo="Assets\Tiles\WideTile.png" Square71x71Logo="Assets\Tiles\SmallTile.png">
          <uap:ShowNameOnTiles>
            <uap:ShowOn Tile="square150x150Logo" />
            <uap:ShowOn Tile="wide310x150Logo" />
            <uap:ShowOn Tile="square310x310Logo" />
          </uap:ShowNameOnTiles>
        </uap:DefaultTile>
        <uap:SplashScreen Image="Assets\Tiles\SplashScreen.png"/>
      </uap:VisualElements>
      <Extensions>
        <uap3:Extension Category="windows.appUriHandler">
          <uap3:AppUriHandler>
            <uap3:Host Name="winuigallery.com" />
            <uap3:Host Name="xamlcontrolsgallery.com" />
          </uap3:AppUriHandler>
        </uap3:Extension>
        <uap:Extension Category="windows.protocol">
          <uap:Protocol Name="winui3gallery">
            <uap:DisplayName>WinUI 3 Gallery</uap:DisplayName>
          </uap:Protocol>
        </uap:Extension>
      </Extensions>
    </Application>
  </Applications>
  <Capabilities>
    <rescap:Capability Name="runFullTrust" />
  </Capabilities>
</Package>


================================================
FILE: WinUIGallery/Package.Dev.appxmanifest
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<Package
    xmlns="http://schemas.microsoft.com/appx/manifest/foundation/windows10"
    xmlns:mp="http://schemas.microsoft.com/appx/2014/phone/manifest"
    xmlns:uap="http://schemas.microsoft.com/appx/manifest/uap/windows10"
    xmlns:uap3="http://schemas.microsoft.com/appx/manifest/uap/windows10/3"
    xmlns:rescap="http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities"
    IgnorableNamespaces="uap mp uap3">
  <!--Note: package version and assembly version must be kept in sync-->
  <Identity Name="Microsoft.WinUI3ControlsGallery.Debug" Publisher="CN=Microsoft Corporation, O=Microsoft Corporation, L=Redmond, S=Washington, C=US" Version="2.6.0.0" />
  <mp:PhoneIdentity PhoneProductId="863667e0-667a-4bb4-ac52-c59656c7333a" PhonePublisherId="00000000-0000-0000-0000-000000000000" />
  <Properties>
    <DisplayName>WinUI 3 Gallery Dev</DisplayName>
    <PublisherDisplayName>Microsoft Corporation</PublisherDisplayName>
    <Logo>Assets\Tiles\StoreLogo.png</Logo>
    <uap:SupportedUsers>multiple</uap:SupportedUsers>
  </Properties>
  <Dependencies>
      <TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.17763.0" MaxVersionTested="10.0.19041.0" />
  </Dependencies>
  <Resources>
    <Resource Language="x-generate" />
  </Resources>
  <Applications>
    <Application Id="App" Executable="$targetnametoken$.exe" EntryPoint="$targetentrypoint$">
      <uap:VisualElements DisplayName="WinUI 3 Gallery Dev" Square150x150Logo="Assets\Tiles\MedTile.png" Square44x44Logo="Assets\Tiles\AppList.png" Description="WinUI 3 Gallery Debug" BackgroundColor="transparent">
        <uap:DefaultTile Square310x310Logo="Assets\Tiles\LargeTile.png" Wide310x150Logo="Assets\Tiles\WideTile.png" Square71x71Logo="Assets\Tiles\SmallTile.png">
          <uap:ShowNameOnTiles>
            <uap:ShowOn Tile="square150x150Logo" />
            <uap:ShowOn Tile="wide310x150Logo" />
            <uap:ShowOn Tile="square310x310Logo" />
          </uap:ShowNameOnTiles>
        </uap:DefaultTile>
        <uap:SplashScreen Image="Assets\Tiles\SplashScreen.png" BackgroundColor="transparent" />
      </uap:VisualElements>
      <Extensions>
        <uap3:Extension Category="windows.appUriHandler">
          <uap3:AppUriHandler>
            <uap3:Host Name="winuigallery.com" />
            <uap3:Host Name="xamlcontrolsgallery.com" />
          </uap3:AppUriHandler>
        </uap3:Extension>
        <uap:Extension Category="windows.protocol">
          <uap:Protocol Name="winui3gallerydev">
            <uap:DisplayName>WinUI 3 Gallery Dev</uap:DisplayName>
          </uap:Protocol>
        </uap:Extension>
      </Extensions>
    </Application>
  </Applications>
  <Capabilities>
    <rescap:Capability Name="runFullTrust" />
  </Capabilities>
</Package>


================================================
FILE: WinUIGallery/WinUIGallery.csproj
================================================
﻿<Project Sdk="Microsoft.NET.Sdk">
    <Sdk Name="Microsoft.Build.CentralPackageVersions" Version="2.0.1" />
    <PropertyGroup>
        <OutputType>WinExe</OutputType>
        <TargetFramework>$(SamplesTargetFrameworkMoniker)</TargetFramework>
        <TargetPlatformVersion>$(WindowsSdkTargetPlatformVersion)</TargetPlatformVersion>
        <TargetPlatformMinVersion>$(WindowsAppSdkTargetPlatformVersion)</TargetPlatformMinVersion>
        <UseWinUI>true</UseWinUI>
        <ApplicationManifest>app.manifest</ApplicationManifest>
        <Platforms>x86;x64;ARM64</Platforms>
        <NoWarn>8305</NoWarn>
        <GenerateAssemblyInfo>false</GenerateAssemblyInfo>
        <RuntimeIdentifiers>win-x86;win-x64;win-arm64</RuntimeIdentifiers>
        <NoWarn>
            0108;   <!-- 'x' hides inherited member 'y'. Use the new keyword if hiding was intended. -->
            8305    <!-- 'x' is for evaluation purposes only and is subject to change or removal in future updates. -->
        </NoWarn>
        <MSBuildWarningsAsMessages>
            WMC1501 <!-- x is for evaluation purposes only and is subject to change or removal in future updates. -->
        </MSBuildWarningsAsMessages>
        <ErrorOnDuplicatePublishOutputFiles>false</ErrorOnDuplicatePublishOutputFiles>
        <Configurations>Debug;Release;Debug-Unpackaged;Release-Unpackaged</Configurations>
        <Release>true</Release>
        <Release Condition="'$(Configuration)' == 'Debug' Or '$(Configuration)' == 'Debug-Unpackaged'">false</Release>
        <Packaged>true</Packaged>
        <Packaged Condition="'$(Configuration)' == 'Debug-Unpackaged' Or '$(Configuration)' == 'Release-Unpackaged'">false</Packaged>
        <Optimized>true</Optimized>
        <Optimized Condition="'$(Configuration)' == 'Debug-Unpackaged' Or '$(Configuration)' == 'Debug'">false</Optimized>
        <!-- In .NET 8, serialization is prohibited by default - we can safely use it since we're not dealing with UDTs. -->
        <JsonSerializerIsReflectionEnabledByDefault>true</JsonSerializerIsReflectionEnabledByDefault>
        <SingleProject>true</SingleProject>
        <SingleProject Condition="'$(SolutionName)' == 'WinUIGallery.DesktopWap'">false</SingleProject>
        <WindowsAppSdkIncludeVersionInfo>true</WindowsAppSdkIncludeVersionInfo>
        <PublishProfile>win-$(Platform).pubxml</PublishProfile>
        <PublishAot>false</PublishAot>
        <PublishSingleFile Condition="'$(PublishSingleFile)' == '' and '$(Packaged)' != 'true'">true</PublishSingleFile>
        <WindowsAppSdkSelfContained Condition="'$(WindowsAppSdkSelfContained)' == '' and '$(PublishSingleFile)' == 'true'">true</WindowsAppSdkSelfContained>
        <!-- Enable ExplicitlyIncludeVersionInfo workaround by setting WindowsAppSdkSelfContained earlier than the mock package would -->
        <WindowsAppSdkSelfContained Condition="'$(IsInWinUIRepo)' == 'true' and '$(WindowsAppSdkSelfContained)'==''">true</WindowsAppSdkSelfContained>
        <ApplicationIcon>Assets\Tiles\GalleryIcon.ico</ApplicationIcon>
    </PropertyGroup>

    <PropertyGroup Condition="'$(Packaged)' != 'true' and '$(SingleProject)'=='true'">
        <EnableMsixTooling>false</EnableMsixTooling>
        <EnableMsixTooling Condition="'$(PublishSingleFile)'=='true'">true</EnableMsixTooling>
        <WindowsPackageType>None</WindowsPackageType>
    </PropertyGroup>

    <PropertyGroup Condition="'$(Packaged)' == 'true' and '$(SingleProject)'=='true'">
        <WindowsPackageType>MSIX</WindowsPackageType>
        <AppxBundleNameForOutput>WinUIGallery</AppxBundleNameForOutput>
        <EnableMsixTooling>true</EnableMsixTooling>
        <SDKIdentifier>Windows</SDKIdentifier>
        <DefaultLanguage>en-US</DefaultLanguage>
        <AppxPackage>true</AppxPackage>
        <AppxPackageSigningEnabled>True</AppxPackageSigningEnabled>
        <GenerateAppInstallerFile>False</GenerateAppInstallerFile>
        <AssetTargetFallback>net5.0-windows$(TargetPlatformVersion);net6.0-windows$(TargetPlatformVersion);$(AssetTargetFallback)</AssetTargetFallback>
        <AppxPackageSigningTimestampDigestAlgorithm>SHA256</AppxPackageSigningTimestampDigestAlgorithm>
        <AppxAutoIncrementPackageRevision>False</AppxAutoIncrementPackageRevision>
        <GenerateTestArtifacts>True</GenerateTestArtifacts>
        <AppxBundlePlatforms>$(Platform)</AppxBundlePlatforms>
        <AppxBundlePlatforms Condition="'$(BuildAllAppFlavors)' == 'true'">x86|x64|ARM64</AppxBundlePlatforms>
        <AppxBundle>Always</AppxBundle>
        <HoursBetweenUpdateChecks>0</HoursBetweenUpdateChecks>
        <SDKVersion>10.0</SDKVersion>
        <PfxFile>$(MSBuildProjectDirectory)\..\build\WinUI-Gallery-Test.pfx</PfxFile>
        <PackageCertificateKeyFile Condition="Exists('$(PfxFile)')">$(PfxFile)</PackageCertificateKeyFile>
    </PropertyGroup>

    <ItemGroup Condition="'$(Packaged)' == 'true' and '$(SingleProject)'=='true'">
        <AppxManifest Include="Package.appxmanifest" Condition="'$(Release)' == 'true'">
            <SubType>Designer</SubType>
        </AppxManifest>
        <AppxManifest Include="Package.Dev.appxmanifest" Condition="'$(Release)' == 'false'">
            <SubType>Designer</SubType>
        </AppxManifest>
    </ItemGroup>

    <PropertyGroup Condition="'$(IsInWinUIRepo)' == 'true'">
        <GenerateAppInstallerFile>true</GenerateAppInstallerFile>
        <!-- URI must be absolute so this is really only useful for testing a locally produced AppInstaller. -->
        <AppInstallerUri>$(AppxPackageDir)</AppInstallerUri>
        <!-- False until https://task.ms/31482969 is implemented -->
        <AppxBundle>Never</AppxBundle>
    </PropertyGroup>

    <Import Project="Common.props" />

    <ItemGroup>
      <Compile Remove="Assets\ControlIcons\**" />
      <Compile Remove="Samples\SampleCode\**" />
      <Content Remove="Assets\ControlIcons\**" />
      <EmbeddedResource Remove="Assets\ControlIcons\**" />
      <EmbeddedResource Remove="Samples\SampleCode\**" />
      <None Remove="Assets\ControlIcons\**" />
      <None Remove="Samples\SampleCode\**" />
      <Page Remove="Assets\ControlIcons\**" />
      <Page Remove="Samples\SampleCode\**" />
      <PRIResource Remove="Assets\ControlIcons\**" />
    </ItemGroup>

    <!-- In the WinUI repo, package reference versions are controlled centrally by a Packages.props.  We will
            just add versionless PackageReferences here.  They will be updated to their actual versions by either the Packages.props file
            in the WinUI repo, or the next ItemGroup below when standalone. -->
    <ItemGroup>
        <PackageReference Include="Microsoft.WindowsAppSDK" />
        <PackageReference Include="ColorCode.Core" />
        <PackageReference Include="Microsoft.Graphics.Win2D" />
        <PackageReference Include="Microsoft.Windows.CsWinRT" />
        <PackageReference Include="CommunityToolkit.WinUI.Controls.SettingsControls" />
        <PackageReference Include="CommunityToolkit.WinUI.Converters" />
        <PackageReference Include="CommunityToolkit.WinUI.Animations" />
        <PackageReference Include="CommunityToolkit.WinUI.Controls.Primitives" />
        <Manifest Include="$(ApplicationManifest)" />
        <!-- System.Private.Uri is pulled in transitively through ColorCode.Core and contains vulnerabilities
          CVE-2019-0657, CVE-2019-0980, and CVE-2019-0981. Since no meta-package depends on version 4.3.2, which
          addresses those vulnerabilites, we need to pull it in ourselves. -->
        <PackageReference Include="System.Private.Uri" />
    </ItemGroup>

    <ItemGroup Condition="'$(IsInWinUIRepo)' != 'true'">
        <PackageReference Update="Microsoft.WindowsAppSDK" Version="$(WindowsAppSdkPackageVersion)" />
        <PackageReference Remove="ColorCode.Core" />
        <PackageReference Include="ColorCode.WinUI" Version="$(ColorCodeVersion)" />
        <PackageReference Update="CommunityToolkit.WinUI.Controls.SettingsControls" Version="$(CommunityToolkitWinUIVersion)" />
        <PackageReference Update="CommunityToolkit.WinUI.Converters" Version="$(CommunityToolkitWinUIVersion)" />
        <PackageReference Update="CommunityToolkit.WinUI.Animations" Version="$(CommunityToolkitWinUIVersion)" />
        <PackageReference Update="CommunityToolkit.WinUI.Controls.Primitives" Version="$(CommunityToolkitWinUIVersion)" />
        <PackageReference Update="Microsoft.Graphics.Win2D" Version="$(GraphicsWin2DVersion)" />
        <!-- Get latest WinRT.Runtime.dll from C#/WinRT -->
        <PackageReference Update="Microsoft.Windows.CsWinRT" Version="$(MicrosoftCsWinRTPackageVersion)" />
        <PackageReference Update="System.Private.Uri" Version="4.3.2" />
    </ItemGroup>

    <ItemGroup>
        <Compile Remove="CollectionsInterop.cs" />
        <Compile Remove="Behaviors\ImageScrollBehavior.cs" />
        <!-- RichTextBlockFormatter is defined in ColorCode.WinUI outside the WinUI repo -->
        <Compile Remove="Helpers\ColorCode.internal\RichTextBlockFormatter.cs" Condition="'$(IsInWinUIRepo)' != 'true'" />
        <Compile Remove="Helpers\ColorCode.internal\ExtensionMethods.cs" Condition="'$(IsInWinUIRepo)' != 'true'" />
        <Content Remove="@(Content)" />
    </ItemGroup>

    <ItemGroup>
        <None Remove="Assets\ControlImages\AppNotification.png" />
        <None Remove="Assets\ControlImages\AppWindow.png" />
        <None Remove="Assets\ControlImages\BadgeNotification.png" />
        <None Remove="Assets\ControlImages\CodeTagIcon.png" />
        <None Remove="Assets\ControlImages\Accessibility.png" />
        <None Remove="Assets\ControlImages\ContentIsland.png" />
        <None Remove="Assets\ControlImages\Popup.png" />
        <None Remove="Assets\Design\Cards.dark.png" />
        <None Remove="Assets\Design\Cards.light.png" />
        <None Remove="Assets\Design\Dialog.dark.png" />
        <None Remove="Assets\Design\Dialog.light.png" />
        <None Remove="Assets\ninegrid.gif" />
        <None Remove="Assets\SampleMedia\folder.png" />
        <None Remove="Assets\Geometry.dark.png" />
        <None Remove="Assets\Geometry.light.png" />
        <None Remove="Assets\HomeHeaderTiles\Header-WinUI.png" />
        <None Remove="Assets\SampleMedia\Dark_Image.png" />
        <None Remove="Assets\SampleMedia\Light_Image.png" />
        <None Remove="Assets\SceneNode\DamagedHelmet1.bmp" />
        <None Remove="Assets\SceneNode\DamagedHelmet2.bmp" />
        <None Remove="Assets\SceneNode\DamagedHelmet3.bmp" />
        <None Remove="Assets\SceneNode\DamagedHelmet4.bmp" />
        <None Remove="Assets\SceneNode\DamagedHelmet5.bmp" />
        <None Remove="Assets\SceneNode\DamagedHelmet6.bin" />
        <None Remove="Assets\SceneNode\DamagedHelmet7.bin" />
        <None Remove="Assets\SceneNode\DamagedHelmet8.bin" />
        <None Remove="Assets\SceneNode\DamagedHelmet9.bin" />
        <None Remove="Assets\Tiles\AppList.scale-100.png" />
        <None Remove="Assets\Tiles\AppList.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\AppList.scale-125.png" />
        <None Remove="Assets\Tiles\AppList.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\AppList.scale-150.png" />
        <None Remove="Assets\Tiles\AppList.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\AppList.scale-200.png" />
        <None Remove="Assets\Tiles\AppList.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\AppList.scale-400.png" />
        <None Remove="Assets\Tiles\AppList.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-16.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-16_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-16_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-20.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-20_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-20_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-24.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-24_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-24_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-256.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-256_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-256_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-30.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-30_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-30_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-32.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-32_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-32_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-36.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-36_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-36_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-40.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-40_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-40_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-48.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-48_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-48_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-56.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-56_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-56_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-60.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-60_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-60_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-64.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-64_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-64_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-72.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-72_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-72_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-80.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-80_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-80_altform-unplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-96.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-96_altform-lightunplated.png" />
        <None Remove="Assets\Tiles\AppList.targetsize-96_altform-unplated.png" />
        <None Remove="Assets\Tiles\BadgeLogo.scale-100.png" />
        <None Remove="Assets\Tiles\BadgeLogo.scale-125.png" />
        <None Remove="Assets\Tiles\BadgeLogo.scale-150.png" />
        <None Remove="Assets\Tiles\BadgeLogo.scale-200.png" />
        <None Remove="Assets\Tiles\BadgeLogo.scale-400.png" />
        <None Remove="Assets\Tiles\GalleryIcon.ico" />
        <None Remove="Assets\Tiles\LargeTile.scale-100.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-125.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-150.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-200.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-400.png" />
        <None Remove="Assets\Tiles\LargeTile.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\MedTile.scale-100.png" />
        <None Remove="Assets\Tiles\MedTile.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\MedTile.scale-125.png" />
        <None Remove="Assets\Tiles\MedTile.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\MedTile.scale-150.png" />
        <None Remove="Assets\Tiles\MedTile.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\MedTile.scale-200.png" />
        <None Remove="Assets\Tiles\MedTile.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\MedTile.scale-400.png" />
        <None Remove="Assets\Tiles\MedTile.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-100.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-125.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-150.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-200.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-400.png" />
        <None Remove="Assets\Tiles\SmallTile.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-100.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-100_altform-colorful_theme-dark.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-125.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-125_altform-colorful_theme-dark.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-150.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-150_altform-colorful_theme-dark.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-200.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-200_altform-colorful_theme-dark.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-400.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-400_altform-colorful_theme-dark.png" />
        <None Remove="Assets\Tiles\SplashScreen.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\StoreDisplay-150.png" />
        <None Remove="Assets\Tiles\StoreDisplay-300.png" />
        <None Remove="Assets\Tiles\StoreDisplay-71.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-100.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-125.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-150.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-200.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-400.png" />
        <None Remove="Assets\Tiles\StoreLogo.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\WideTile.scale-100.png" />
        <None Remove="Assets\Tiles\WideTile.scale-100_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\WideTile.scale-125.png" />
        <None Remove="Assets\Tiles\WideTile.scale-125_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\WideTile.scale-150.png" />
        <None Remove="Assets\Tiles\WideTile.scale-150_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\WideTile.scale-200.png" />
        <None Remove="Assets\Tiles\WideTile.scale-200_altform-colorful_theme-light.png" />
        <None Remove="Assets\Tiles\WideTile.scale-400.png" />
        <None Remove="Assets\Tiles\WideTile.scale-400_altform-colorful_theme-light.png" />
        <None Remove="Controls\CopyButton\CopyButton.xaml" />
        <None Remove="Controls\DesignGuidance\ColorPageExample.xaml" />
        <None Remove="Controls\DesignGuidance\ColorSections\HighContrastSection.xaml" />
        <None Remove="Controls\DesignGuidance\ColorSections\SignalSection.xaml" />
        <None Remove="Controls\DesignGuidance\ColorSections\TextSection.xaml" />
        <None Remove="Controls\DesignGuidance\ColorTile.xaml" />
        <None Remove="Controls\DesignGuidance\TypographyControl.xaml" />
        <None Remove="Controls\HorizontalScrollContainer.xaml" />
        <None Remove="Controls\OpacityMaskView.xaml" />
        <None Remove="Controls\PageHeader.xaml" />
        <None Remove="Controls\SampleThemeListener.xaml" />
        <None Remove="Samples\ControlPages\AppNotificationPage.xaml" />
        <None Remove="Samples\ControlPages\BadgeNotificationManagerPage.xaml" />
        <None Remove="Samples\ControlPages\Fundamentals\Controls\CounterControl.xaml" />
        <None Remove="Samples\ControlPages\Fundamentals\Controls\ValidatedPasswordBox.xaml" />
        <None Remove="Samples\ControlPages\Fundamentals\CustomUserControlsPage.xaml" />
        <None Remove="Samples\ControlPages\AppWindowPage.xaml" />
        <None Remove="Samples\Data\IconsData.json" />
        <None Remove="SamplePages\SampleBuiltInSystemBackdropsWindow.xaml" />
        <None Remove="Samples\SamplePages\SampleWindow2.xaml" />
        <None Remove="Styles\Button.xaml" />
        <None Remove="Styles\Grid.xaml" />
        <None Remove="Styles\GridViewItem.xaml" />
        <None Remove="Styles\ItemTemplates.xaml" />
        <None Remove="Styles\SelectorBar.xaml" />
        <None Remove="Styles\TextBlock.xaml" />
    </ItemGroup>

    <ItemGroup>
        <Content Include="Assets\ControlImages\AppNotification.png" />
        <Content Include="Assets\ControlImages\AppWindow.png" />
        <Content Include="Assets\ControlImages\BadgeNotification.png" />
        <Content Include="Assets\ControlImages\CodeTagIcon.png" />
        <Content Include="Assets\ControlImages\Accessibility.png" />
        <Content Include="Assets\ControlImages\ContentIsland.png" />
        <Content Include="Assets\ControlImages\CustomControls.png" />
        <Content Include="Assets\ControlImages\Popup.png" />
        <Content Include="Assets\Design\Cards.dark.png" />
        <Content Include="Assets\Design\Cards.light.png" />
        <Content Include="Assets\Design\Dialog.dark.png" />
        <Content Include="Assets\Design\Dialog.light.png" />
        <Content Include="Assets\SampleMedia\ninegrid.gif" />
        <Content Include="Assets\SampleMedia\folder.png" />
        <Content Include="Assets\GalleryHeaderImage.png" />
        <Content Include="Assets\Design\Geometry.dark.png" />
        <Content Include="Assets\Design\Geometry.light.png" />
        <Content Include="Assets\HomeHeaderTiles\Header-Store.dark.png" />
        <Content Include="Assets\HomeHeaderTiles\Header-Store.light.png" />
        <Content Include="Assets\HomeHeaderTiles\Header-Toolkit.png" />
        <Content Include="Assets\HomeHeaderTiles\Header-WindowsDesign.png" />
        <Content Include="Assets\HomeHeaderTiles\Header-WinUI.png" />
        <Content Include="Assets\SampleMedia\Dark_Image.png" />
        <Content Include="Assets\SampleMedia\Light_Image.png" />
        <Content Include="Assets\SceneNode\DamagedHelmet1.bmp" />
        <Content Include="Assets\SceneNode\DamagedHelmet2.bmp" />
        <Content Include="Assets\SceneNode\DamagedHelmet3.bmp" />
        <Content Include="Assets\SceneNode\DamagedHelmet4.bmp" />
        <Content Include="Assets\SceneNode\DamagedHelmet5.bmp" />
        <Content Include="Assets\SceneNode\DamagedHelmet6.bin" />
        <Content Include="Assets\SceneNode\DamagedHelmet7.bin" />
        <Content Include="Assets\SceneNode\DamagedHelmet8.bin" />
        <Content Include="Assets\SceneNode\DamagedHelmet9.bin" />
        <Content Include="Assets\Tiles\AppList.scale-100.png" />
        <Content Include="Assets\Tiles\AppList.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\AppList.scale-125.png" />
        <Content Include="Assets\Tiles\AppList.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\AppList.scale-150.png" />
        <Content Include="Assets\Tiles\AppList.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\AppList.scale-200.png" />
        <Content Include="Assets\Tiles\AppList.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\AppList.scale-400.png" />
        <Content Include="Assets\Tiles\AppList.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-16.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-16_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-16_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-20.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-20_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-20_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-24.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-24_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-24_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-256.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-256_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-256_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-30.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-30_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-30_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-32.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-32_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-32_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-36.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-36_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-36_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-40.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-40_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-40_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-48.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-48_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-48_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-56.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-56_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-56_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-60.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-60_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-60_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-64.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-64_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-64_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-72.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-72_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-72_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-80.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-80_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-80_altform-unplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-96.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-96_altform-lightunplated.png" />
        <Content Include="Assets\Tiles\AppList.targetsize-96_altform-unplated.png" />
        <Content Include="Assets\Tiles\BadgeLogo.scale-100.png" />
        <Content Include="Assets\Tiles\BadgeLogo.scale-125.png" />
        <Content Include="Assets\Tiles\BadgeLogo.scale-150.png" />
        <Content Include="Assets\Tiles\BadgeLogo.scale-200.png" />
        <Content Include="Assets\Tiles\BadgeLogo.scale-400.png" />
        <Content Include="Assets\Design\Typography.dark.png" />
        <Content Include="Assets\Design\Typography.light.png" />
        <Content Include="Assets\Tiles\GalleryIcon.ico" />
        <Content Include="Assets\Tiles\LargeTile.scale-100.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-125.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-150.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-200.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-400.png" />
        <Content Include="Assets\Tiles\LargeTile.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\MedTile.scale-100.png" />
        <Content Include="Assets\Tiles\MedTile.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\MedTile.scale-125.png" />
        <Content Include="Assets\Tiles\MedTile.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\MedTile.scale-150.png" />
        <Content Include="Assets\Tiles\MedTile.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\MedTile.scale-200.png" />
        <Content Include="Assets\Tiles\MedTile.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\MedTile.scale-400.png" />
        <Content Include="Assets\Tiles\MedTile.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-100.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-125.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-150.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-200.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-400.png" />
        <Content Include="Assets\Tiles\SmallTile.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-100.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-100_altform-colorful_theme-dark.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-125.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-125_altform-colorful_theme-dark.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-150.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-150_altform-colorful_theme-dark.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-200.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-200_altform-colorful_theme-dark.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-400.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-400_altform-colorful_theme-dark.png" />
        <Content Include="Assets\Tiles\SplashScreen.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\StoreDisplay-150.png" />
        <Content Include="Assets\Tiles\StoreDisplay-300.png" />
        <Content Include="Assets\Tiles\StoreDisplay-71.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-100.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-125.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-150.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-200.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-400.png" />
        <Content Include="Assets\Tiles\StoreLogo.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\WideTile.scale-100.png" />
        <Content Include="Assets\Tiles\WideTile.scale-100_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\WideTile.scale-125.png" />
        <Content Include="Assets\Tiles\WideTile.scale-125_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\WideTile.scale-150.png" />
        <Content Include="Assets\Tiles\WideTile.scale-150_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\WideTile.scale-200.png" />
        <Content Include="Assets\Tiles\WideTile.scale-200_altform-colorful_theme-light.png" />
        <Content Include="Assets\Tiles\WideTile.scale-400.png" />
        <Content Include="Assets\Tiles\WideTile.scale-400_altform-colorful_theme-light.png" />
        <Content Include="Samples\Data\IconsData.json" />
        <Content Include="Samples\Data\ControlInfoData.json" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample1_xaml.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample2_cs.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample2_xaml.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample3_xaml.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample5_cs.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample5_xaml.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample6_cs.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample6_xaml.txt" />
        <Content Include="Samples\SampleCode\AppWindow\AppWindowSample7_xaml.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample1_cs.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample1_xaml.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample2_cs.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample2_xaml.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample3_cs.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample3_xaml.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample4_cs.txt" />
        <Content Include="Samples\SampleCode\CustomUserControls\CustomUserControlsSample4_xaml.txt" />
        <Content Include="Samples\SampleCode\Text\RichEditBox\RichEditBoxSample6_cs.txt" />
    </ItemGroup>

    <ItemGroup>
      <Page Update="Controls\OpacityMaskView.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>

    <ItemGroup>
      <Page Update="Styles\SelectorBar.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>

    <ItemGroup>
      <Page Update="Controls\HorizontalScrollContainer.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>

    <ItemGroup>
      <Page Update="Samples\ControlPages\BadgeNotificationManagerPage.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>

    <ItemGroup>
      <Page Update="Samples\ControlPages\AppNotificationPage.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>

    <ItemGroup>
      <Page Update="Samples\ControlPages\Fundamentals\Controls\ValidatedPasswordBox.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\SampleWindow7.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\ControlPages\Fundamentals\Controls\CounterControl.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\SampleWindow6.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\ControlPages\Fundamentals\CustomUserControlsPage.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\SampleWindow2.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\ModalWindow.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\SampleWindow3.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\SamplePages\SampleWindow1.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Samples\ControlPages\AppWindowPage.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
        <Page Update="Controls\CopyButton\CopyButton.xaml">
            <Generator>MSBuild:Compile</Generator>
        </Page>
    </ItemGroup>
    <ItemGroup>
        <Page Update="ControlPages\InfoBadgePage.xaml">
            <Generator>MSBuild:Compile</Generator>
        </Page>
    </ItemGroup>
    <ItemGroup>
        <Page Update="Controls\SampleThemeListener.xaml">
            <Generator>MSBuild:Compile</Generator>
        </Page>
    </ItemGroup>
    <ItemGroup>
        <Page Update="Controls\PageHeader.xaml">
            <Generator>MSBuild:Compile</Generator>
        </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Styles\TextBlock.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Styles\ItemTemplates.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Styles\GridViewItem.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Styles\Grid.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Styles\Button.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <ItemGroup>
      <Page Update="Controls\HomePage\HomePageHeader.xaml">
        <Generator>MSBuild:Compile</Generator>
      </Page>
    </ItemGroup>
    <Import Project="ContentIncludes.props" />
    <!--Per comment in Microsoft.Common.CurrentVersion.targets, the default GetCopyToPublishDirectoryItems
        just returns GetCopyToOutputDirectoryItems, which automatically includes the ContentWithTargetPath
        and _NoneWithTargetPath items in the MSIX package.  The .NET GetCopyToPublishDirectoryItems
        overrides this and drops all these items unless they're specifically set to copy to the output
        directory.  The default behavior is easier, so we'll mimic that here.-->
    <Target Name="AddCopyToPublishDirectoryItems" Condition="'$(PublishSingleFile)'=='true'" BeforeTargets="GetCopyToPublishDirectoryItems" DependsOnTargets="AssignTargetPaths">
        <ItemGroup>
            <CurrentContentWithTargetPath Include="@(ContentWithTargetPath)" />
            <ContentWithTargetPath Remove="@(CurrentContentWithTargetPath )" />
            <ContentWithTargetPath Include="@(CurrentContentWithTargetPath )">
                <CopyToPublishDirectory>PreserveNewest</CopyToPublishDirectory>
            </ContentWithTargetPath>
            <CurrentNoneWithTargetPath Include="@(_NoneWithTargetPath)" />
            <_NoneWithTargetPath Remove="@(CurrentNoneWithTargetPath )" />
            <_NoneWithTargetPath Include="@(CurrentNoneWithTargetPath )">
                <CopyToPublishDirectory>PreserveNewest</CopyToPublishDirectory>
            </_NoneWithTargetPath>
        </ItemGroup>
    </Target>
</Project>



================================================
FILE: WinUIGallery/WinUIGallery.DesktopWap.Package.wapproj
================================================
<?xml version="1.0" encoding="utf-8"?>
<Project ToolsVersion="15.0" DefaultTargets="Build" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup Condition="'$(VisualStudioVersion)' == '' or '$(VisualStudioVersion)' &lt; '15.0'">
    <VisualStudioVersion>15.0</VisualStudioVersion>
  </PropertyGroup>
  <ItemGroup Label="ProjectConfigurations">
    <ProjectConfiguration Include="Debug|x86">
      <Configuration>Debug</Configuration>
      <Platform>x86</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|x86">
      <Configuration>Release</Configuration>
      <Platform>x86</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Debug|x64">
      <Configuration>Debug</Configuration>
      <Platform>x64</Platform>
    </ProjectConfiguration>
    <ProjectConfiguration Include="Release|x64">
      <Configuration>Release</Configuration>
      <Platform>x64</Platform>
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
  <PropertyGroup>
    <WapProjPath Condition="'$(WapProjPath)'==''">$(MSBuildExtensionsPath)\Microsoft\DesktopBridge\</WapProjPath>
    <SDKIdentifier>Windows</SDKIdentifier>
    <SDKVersion>10.0</SDKVersion>
  </PropertyGroup>
  <Import Project="$(WapProjPath)\Microsoft.DesktopBridge.props" />
  <Import Project="common.props" />
  <PropertyGroup>
    <ProjectGuid>4c7b20d7-5f5c-440e-8da3-b19a328cc8bd</ProjectGuid>
    <TargetPlatformVersion>10.0.22621.0</TargetPlatformVersion>
    <TargetPlatformMinVersion>10.0.17763.0</TargetPlatformMinVersion>
    <DefaultLanguage>en-US</DefaultLanguage>
    <AppxPackageSigningEnabled>True</AppxPackageSigningEnabled>
    <EntryPointProjectUniqueName>WinUIGallery.csproj</EntryPointProjectUniqueName>
    <AppxBundleNameForOutput>WinUIGallery.DesktopWap</AppxBundleNameForOutput>
  </PropertyGroup>
  <PropertyGroup Condition="'$(IsInWinUIRepo)' == 'true'">
    <PackageCertificateKeyFile>$(ProjectRoot)build\MSTest.pfx</PackageCertificateKeyFile>
  </PropertyGroup>
  <PropertyGroup Condition="'$(IsInWinUIRepo)' != 'true'">
    <PackageCertificateKeyFile Condition="'$(PackageCertificateKeyFile)'==''">$(SolutionDir)..\build\WinUI-Gallery-Test.pfx</PackageCertificateKeyFile>
  </PropertyGroup>
  <PropertyGroup>
    <GenerateAppInstallerFile>False</GenerateAppInstallerFile>
    <AppxPackageSigningTimestampDigestAlgorithm>SHA256</AppxPackageSigningTimestampDigestAlgorithm>
    <AppxAutoIncrementPackageRevision>False</AppxAutoIncrementPackageRevision>
    <GenerateTestArtifacts>True</GenerateTestArtifacts>
    <AppxBundlePlatforms>x86|x64|arm64</AppxBundlePlatforms>
    <AppxBundlePlatforms Condition="'$(BuildAllAppFlavors)' == 'true'">x86|x64|ARM64</AppxBundlePlatforms>
    <HoursBetweenUpdateChecks>0</HoursBetweenUpdateChecks>
    <AssetTargetFallback>net5.0-windows$(TargetPlatformVersion);net6.0-windows$(TargetPlatformVersion);$(AssetTargetFallback)</AssetTargetFallback>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x86'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|ARM64'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x86'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|ARM64'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <AppxBundle>Always</AppxBundle>
  </PropertyGroup>
  <ItemGroup>
    <AppxManifest Include="Package.appxmanifest" Condition="!('$(Configuration)' == 'Debug')">
      <SubType>Designer</SubType>
    </AppxManifest>
    <AppxManifest Include="Package.Dev.appxmanifest" Condition="'$(Configuration)' == 'Debug'">
      <SubType>Designer</SubType>
    </AppxManifest>
  </ItemGroup>
  <ItemGroup>
    <ProjectReference Include="WinUIGallery.csproj">
      <SkipGetTargetFrameworkProperties>True</SkipGetTargetFrameworkProperties>
      <PublishProfile>Properties\PublishProfiles\win-$(Platform).pubxml</PublishProfile>
    </ProjectReference>
  </ItemGroup>
  <ItemGroup Condition="'$(WindowsAppSdkPackageVersion)' != ''">
    <PackageReference Include="Microsoft.WindowsAppSDK" Version="[$(WindowsAppSdkPackageVersion)]" GeneratePathProperty="true">
      <IncludeAssets>build</IncludeAssets>
    </PackageReference>
    <PackageReference Include="Microsoft.Windows.SDK.BuildTools" Version="[$(MicrosoftWindowsSDKBuildToolsNugetPackageVersion)]">
      <IncludeAssets>build</IncludeAssets>
    </PackageReference>
  </ItemGroup>
  <Import Project="$(WapProjPath)\Microsoft.DesktopBridge.targets" />
</Project>


================================================
FILE: WinUIGallery/Assets/AnimatedVisuals/LottieLogo1.cs
================================================
//------------------------------------------------------------------------------
// <auto-generated>
//     This code was generated by a tool.
//
//     Changes to this file may cause incorrect behavior and will be lost if
//     the code is regenerated.
// </auto-generated>
//------------------------------------------------------------------------------
using System;
using System.Numerics;
using Microsoft.Graphics.Canvas.Geometry;
using Microsoft.UI.Composition;
using Microsoft.UI.Xaml.Controls;

namespace AnimatedVisuals;

sealed class LottieLogo1 : IAnimatedVisualSource
{
    public IAnimatedVisual TryCreateAnimatedVisual(Compositor compositor, out object diagnostics)
    {
        diagnostics = null;
        return new AnimatedVisual(compositor);
    }

    sealed class AnimatedVisual : IAnimatedVisual
    {
        const long c_durationTicks = 59670000;
        readonly Compositor _c;
        readonly ExpressionAnimation _reusableExpressionAnimation;
        CompositionColorBrush _colorBrush_AlmostTeal_FF007A87;
        CompositionColorBrush _colorBrush_White;
        CompositionPath _compositionPath_00;
        CompositionPath _compositionPath_01;
        CompositionPath _compositionPath_02;
        CompositionPath _compositionPath_03;
        CompositionPath _compositionPath_04;
        CompositionPath _compositionPath_05;
        CompositionPath _compositionPath_06;
        CompositionPath _compositionPath_07;
        CompositionPath _compositionPath_08;
        CubicBezierEasingFunction _cubicBezierEasingFunction_02;
        CubicBezierEasingFunction _cubicBezierEasingFunction_03;
        CubicBezierEasingFunction _cubicBezierEasingFunction_04;
        CubicBezierEasingFunction _cubicBezierEasingFunction_05;
        CubicBezierEasingFunction _cubicBezierEasingFunction_07;
        CubicBezierEasingFunction _cubicBezierEasingFunction_08;
        CubicBezierEasingFunction _cubicBezierEasingFunction_11;
        CubicBezierEasingFunction _cubicBezierEasingFunction_12;
        CubicBezierEasingFunction _cubicBezierEasingFunction_15;
        CubicBezierEasingFunction _cubicBezierEasingFunction_16;
        CubicBezierEasingFunction _cubicBezierEasingFunction_23;
        CompositionEllipseGeometry _ellipse_4p7;
        StepEasingFunction _holdThenStepEasingFunction;
        LinearEasingFunction _linearEasingFunction;
        ContainerVisual _root;
        ScalarKeyFrameAnimation _scalarAnimation_0_to_0p249;
        ScalarKeyFrameAnimation _scalarAnimation_0_to_1_2;
        ScalarKeyFrameAnimation _scalarAnimation_0p87_to_0_02;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_10;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_12;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_13;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_14;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_15;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_18;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_19;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_27;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_28;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_30;
        ScalarKeyFrameAnimation _scalarAnimation_1_to_0_31;
        ScalarKeyFrameAnimation _scalarAnimation_to_1_02;
        ScalarKeyFrameAnimation _scalarAnimation_to_1_06;
        ExpressionAnimation _scalarExpressionAnimation;
        StepEasingFunction _stepThenHoldEasingFunction;
        Vector2KeyFrameAnimation _vector2Animation_02;
        Vector2KeyFrameAnimation _vector2Animation_03;
        Vector2KeyFrameAnimation _vector2Animation_04;
        Vector2KeyFrameAnimation _vector2Animation_05;
        Vector2KeyFrameAnimation _vector2Animation_06;
        Vector2KeyFrameAnimation _vector2Animation_07;

        // Rectangle Path 1
        CompositionColorBrush ColorBrush_AlmostDarkTurquoise_FF00D1C1()
        {
            return _c.CreateColorBrush(Microsoft.UI.ColorHelper.FromArgb(0xFF, 0x00, 0xD1, 0xC1));
        }

        CompositionColorBrush ColorBrush_AlmostTeal_FF007A87()
        {
            return _colorBrush_AlmostTeal_FF007A87 = _c.CreateColorBrush(Microsoft.UI.ColorHelper.FromArgb(0xFF, 0x00, 0x7A, 0x87));
        }

        CompositionColorBrush ColorBrush_White()
        {
            return _colorBrush_White = _c.CreateColorBrush(Microsoft.UI.ColorHelper.FromArgb(0xFF, 0xFF, 0xFF, 0xFF));
        }

        CompositionPath CompositionPath_00()
        {
            var result = _compositionPath_00 = new CompositionPath(Geometry_00());
            return result;
        }

        CompositionPath CompositionPath_01()
        {
            var result = _compositionPath_01 = new CompositionPath(Geometry_01());
            return result;
        }

        CompositionPath CompositionPath_02()
        {
            var result = _compositionPath_02 = new CompositionPath(Geometry_02());
            return result;
        }

        CompositionPath CompositionPath_03()
        {
            var result = _compositionPath_03 = new CompositionPath(Geometry_03());
            return result;
        }

        CompositionPath CompositionPath_04()
        {
            var result = _compositionPath_04 = new CompositionPath(Geometry_04());
            return result;
        }

        CompositionPath CompositionPath_05()
        {
            var result = _compositionPath_05 = new CompositionPath(Geometry_05());
            return result;
        }

        CompositionPath CompositionPath_06()
        {
            var result = _compositionPath_06 = new CompositionPath(Geometry_06());
            return result;
        }

        CompositionPath CompositionPath_07()
        {
            var result = _compositionPath_07 = new CompositionPath(Geometry_07());
            return result;
        }

        CompositionPath CompositionPath_08()
        {
            var result = _compositionPath_08 = new CompositionPath(Geometry_08());
            return result;
        }

        // Layer (Shape): Dot-Y
        CompositionContainerShape ContainerShape_00()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_01());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_00());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): Dot-Y
        CompositionContainerShape ContainerShape_01()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_02());
            return result;
        }

        // Transforms for Bncr
        CompositionContainerShape ContainerShape_02()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(164.781998F, 57.4729996F));
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_03());
            result.StartAnimation("Position", Vector2Animation_01());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(60,60)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Transforms for Dot-Y
        CompositionContainerShape ContainerShape_03()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(43.2630005F, 59.75F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_01());
            result.StartAnimation("Position", Vector2Animation_00());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", ScalarExpressionAnimation());
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(196.791,266.504)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E3-Y
        CompositionContainerShape ContainerShape_04()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_05());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_00());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E3-Y
        CompositionContainerShape ContainerShape_05()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_06());
            return result;
        }

        // Transforms for E3-Y
        CompositionContainerShape ContainerShape_06()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(119.167F, 57.4790001F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_02());
            result.StartAnimation("Position", Vector2Animation_02());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(345.124,261.801)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E3-B
        CompositionContainerShape ContainerShape_07()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_08());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_01());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E3-B
        CompositionContainerShape ContainerShape_08()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_09());
            return result;
        }

        // Transforms for E3-Y
        CompositionContainerShape ContainerShape_09()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(119.167F, 57.4790001F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_03());
            result.StartAnimation("Position", _vector2Animation_02);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(345.124,261.801)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): I-Y
        CompositionContainerShape ContainerShape_10()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_11());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_01());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): I-Y
        CompositionContainerShape ContainerShape_11()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_12());
            return result;
        }

        // Transforms for I-Y
        CompositionContainerShape ContainerShape_12()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(93.5940018F, 62.8610001F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_04());
            result.StartAnimation("Position", Vector2Animation_03());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(303.802,282.182)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): I-B
        CompositionContainerShape ContainerShape_13()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_14());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_02());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): I-B
        CompositionContainerShape ContainerShape_14()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_15());
            return result;
        }

        // Transforms for I-Y
        CompositionContainerShape ContainerShape_15()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(93.5940018F, 62.8610001F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_05());
            result.StartAnimation("Position", _vector2Animation_03);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(303.802,282.182)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E2-Y
        CompositionContainerShape ContainerShape_16()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_17());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_02());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E2-Y
        CompositionContainerShape ContainerShape_17()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_18());
            return result;
        }

        // Transforms for E2-Y
        CompositionContainerShape ContainerShape_18()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(109.092003F, 33.6100006F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_06());
            result.StartAnimation("Position", Vector2Animation_04());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(332.05,237.932)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E2-B
        CompositionContainerShape ContainerShape_19()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_20());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_03());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E2-B
        CompositionContainerShape ContainerShape_20()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_21());
            return result;
        }

        // Transforms for E2-Y
        CompositionContainerShape ContainerShape_21()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(109.092003F, 33.6100006F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_07());
            result.StartAnimation("Position", _vector2Animation_04);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(332.05,237.932)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E1-Y
        CompositionContainerShape ContainerShape_22()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_23());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_03());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E1-Y
        CompositionContainerShape ContainerShape_23()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_24());
            return result;
        }

        // Transforms for E1-Y
        CompositionContainerShape ContainerShape_24()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(113.714996F, 9.14599991F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_08());
            result.StartAnimation("Position", Vector2Animation_05());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(344.672,214.842)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E1-B
        CompositionContainerShape ContainerShape_25()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_26());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_04());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): E1-B
        CompositionContainerShape ContainerShape_26()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_27());
            return result;
        }

        // Transforms for E1-Y
        CompositionContainerShape ContainerShape_27()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(113.714996F, 9.14599991F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_09());
            result.StartAnimation("Position", _vector2Animation_05);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(344.672,214.842)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-Y
        CompositionContainerShape ContainerShape_28()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_29());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_04());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-Y
        CompositionContainerShape ContainerShape_29()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_30());
            return result;
        }

        // Transforms for T1a-Y
        CompositionContainerShape ContainerShape_30()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(39.0429993F, 48.6780014F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_10());
            result.StartAnimation("Position", Vector2Animation_06());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(250,250)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T2b-Y
        CompositionContainerShape ContainerShape_31()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_11());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_05());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T2a-Y
        CompositionContainerShape ContainerShape_32()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_12());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_06());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T2b-B
        CompositionContainerShape ContainerShape_33()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_13());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_05());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1b-Y
        CompositionContainerShape ContainerShape_34()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_14());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_07());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1b-B
        CompositionContainerShape ContainerShape_35()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_15());
            result.StartAnimation("TransformMatrix._11", _scalarAnimation_to_1_02);
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): O-Y
        CompositionContainerShape ContainerShape_36()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_37());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_06());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): O-Y
        CompositionContainerShape ContainerShape_37()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_38());
            return result;
        }

        // Transforms for O-Y
        CompositionContainerShape ContainerShape_38()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(-62.7919998F, 73.0569992F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_16());
            result.StartAnimation("Position", Vector2Animation_08());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(196.791,266.504)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): O-B
        CompositionContainerShape ContainerShape_39()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_40());
            result.StartAnimation("TransformMatrix._11", _scalarAnimation_to_1_06);
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): O-B
        CompositionContainerShape ContainerShape_40()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_41());
            return result;
        }

        // Transforms for O-B
        CompositionContainerShape ContainerShape_41()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(-62.7919998F, 73.0569992F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_17());
            result.StartAnimation("Position", Vector2Animation_09());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(196.791,266.504)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-Y 2
        CompositionContainerShape ContainerShape_42()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_43());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_07());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-Y 2
        CompositionContainerShape ContainerShape_43()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_44());
            return result;
        }

        // Transforms for T1a-Y 2
        CompositionContainerShape ContainerShape_44()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(39.0429993F, 48.6780014F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_18());
            result.StartAnimation("Position", _vector2Animation_06);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(250,250)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T2a-B
        CompositionContainerShape ContainerShape_45()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_19());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_08());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-B
        CompositionContainerShape ContainerShape_46()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_47());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_09());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): T1a-B
        CompositionContainerShape ContainerShape_47()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_48());
            return result;
        }

        // Transforms for T1a-Y
        CompositionContainerShape ContainerShape_48()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(39.0429993F, 48.6780014F));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_20());
            result.StartAnimation("Position", _vector2Animation_06);
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(250,250)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): Dot-Y
        CompositionContainerShape ContainerShape_49()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_50());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_1_to_0_08());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): Dot-Y
        CompositionContainerShape ContainerShape_50()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(1, 0, 0, 1, 154.457001F, 287.821991F);
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_51());
            return result;
        }

        // Transforms for N
        CompositionContainerShape ContainerShape_51()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(-33.6669998F, 8.18200016F));
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_52());
            result.StartAnimation("Position", Vector2Animation_11());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(60,60)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Transforms for Dot-Y
        CompositionContainerShape ContainerShape_52()
        {
            var result = _c.CreateContainerShape();
            var propertySet = result.Properties;
            propertySet.InsertVector2("Position", new Vector2(39.875F, 60));
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_21());
            result.StartAnimation("Position", Vector2Animation_10());
            var controller = result.TryGetAnimationController("Position");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.Position - Vector2(196.791,266.504)";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("Offset", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): L-Y
        CompositionContainerShape ContainerShape_53()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_22());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_10());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): L-B
        CompositionContainerShape ContainerShape_54()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Matrix3x2(0, 0, 0, 0, 0, 0);
            var shapes = result.Shapes;
            shapes.Add(SpriteShape_23());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_1_11());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): Dot1
        CompositionContainerShape ContainerShape_55()
        {
            var result = _c.CreateContainerShape();
            var shapes = result.Shapes;
            shapes.Add(ContainerShape_56());
            result.StartAnimation("TransformMatrix._11", ScalarAnimation_to_0());
            var controller = result.TryGetAnimationController("TransformMatrix._11");
            controller.Pause();
            controller.StartAnimation("Progress", _scalarExpressionAnimation);
            _reusableExpressionAnimation.ClearAllParameters();
            _reusableExpressionAnimation.Expression = "my.TransformMatrix._11";
            _reusableExpressionAnimation.SetReferenceParameter("my", result);
            result.StartAnimation("TransformMatrix._22", _reusableExpressionAnimation);
            return result;
        }

        // Layer (Shape): Dot1
        CompositionContainerShape ContainerShape_56()
        {
            var result = _c.CreateContainerShape();
            result.TransformMatrix = new Mat