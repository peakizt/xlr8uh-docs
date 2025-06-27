Directory structure:
└── microsoftdocs-windows-dev-docs/
    ├── README.md
    ├── auto-publish.yml
    ├── CONTRIBUTING.md
    ├── LICENSE
    ├── LICENSE-CODE
    ├── master-branch-inf.txt
    ├── SECURITY.md
    ├── ThirdPartyNotices
    ├── .localization-config
    ├── .openpublishing.publish.config.json
    ├── .openpublishing.redirection.json
    ├── .whatsnew.json
    ├── hub/
    │   ├── delbranch.bash
    │   ├── docfx.json
    │   ├── index.yml
    │   ├── advanced-settings/
    │   │   ├── fe-version-control.md
    │   │   ├── index.md
    │   │   └── sudo/
    │   │       └── index.md
    │   ├── android/
    │   │   ├── emulator.md
    │   │   ├── native-android.md
    │   │   ├── overview.md
    │   │   ├── pwa.md
    │   │   └── wsa/
    │   │       ├── index.md
    │   │       └── release-notes.md
    │   ├── apps/
    │   │   ├── index.yml
    │   │   ├── toc.yml
    │   │   ├── zone-pivot-groups.yml
    │   │   ├── api-reference/
    │   │   │   ├── index.md
    │   │   │   ├── bootstrapper-cpp-api/
    │   │   │   │   ├── bootstrapper-cpp-api-constants.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── microsoft.windows.applicationmodel/
    │   │   │   │   │   ├── microsoft.windows.applicationmodel.md
    │   │   │   │   │   └── microsoft.windows.applicationmodel.packageversion.md
    │   │   │   │   └── microsoft.windows.applicationmodel.dynamicdependency.bootstrap/
    │   │   │   │       ├── microsoft.windows.applicationmodel.dynamicdependency.bootstrap.initialize.md
    │   │   │   │       ├── microsoft.windows.applicationmodel.dynamicdependency.bootstrap.initializefailfast.md
    │   │   │   │       ├── microsoft.windows.applicationmodel.dynamicdependency.bootstrap.initializenothrow.md
    │   │   │   │       └── microsoft.windows.applicationmodel.dynamicdependency.bootstrap.md
    │   │   │   ├── cs-bootstrapper-apis/
    │   │   │   │   ├── cs-bootstrapper-apis-constants.md
    │   │   │   │   ├── index.md
    │   │   │   │   └── microsoft.windows.applicationmodel.dynamicdependency/
    │   │   │   │       ├── microsoft.windows.applicationmodel.dynamicdependency.bootstrap.md
    │   │   │   │       ├── microsoft.windows.applicationmodel.dynamicdependency.md
    │   │   │   │       └── microsoft.windows.applicationmodel.dynamicdependency.packageversion.md
    │   │   │   ├── cs-interop-apis/
    │   │   │   │   ├── index.md
    │   │   │   │   └── microsoft.ui/
    │   │   │   │       ├── microsoft.ui.md
    │   │   │   │       ├── microsoft.ui.win32interop.getdisplayidfrommonitor.md
    │   │   │   │       ├── microsoft.ui.win32interop.geticonfromiconid.md
    │   │   │   │       ├── microsoft.ui.win32interop.geticonidfromicon.md
    │   │   │   │       ├── microsoft.ui.win32interop.getmonitorfromdisplayid.md
    │   │   │   │       ├── microsoft.ui.win32interop.getwindowfromwindowid.md
    │   │   │   │       ├── microsoft.ui.win32interop.getwindowidfromwindow.md
    │   │   │   │       └── microsoft.ui.win32interop.md
    │   │   │   └── interface-members/
    │   │   │       ├── iaccesskeymanagerstaticsdisplaymode-enterdisplaymode.md
    │   │   │       └── ixamlsourcetransparency-isbackgroundtransparent.md
    │   │   ├── design/
    │   │   │   ├── index.md
    │   │   │   ├── toc.yml
    │   │   │   ├── accessibility/
    │   │   │   │   ├── accessibility-checklist.md
    │   │   │   │   ├── accessibility-in-the-store.md
    │   │   │   │   ├── accessibility-overview.md
    │   │   │   │   ├── accessibility-testing.md
    │   │   │   │   ├── accessibility.md
    │   │   │   │   ├── accessible-text-requirements.md
    │   │   │   │   ├── basic-accessibility-information.md
    │   │   │   │   ├── control-patterns-and-interfaces.md
    │   │   │   │   ├── custom-automation-peers.md
    │   │   │   │   ├── designing-inclusive-software.md
    │   │   │   │   ├── developing-inclusive-windows-apps.md
    │   │   │   │   ├── high-contrast-themes.md
    │   │   │   │   ├── keyboard-accessibility.md
    │   │   │   │   ├── landmarks-and-headings.md
    │   │   │   │   ├── practices-to-avoid.md
    │   │   │   │   ├── system-button-narration.md
    │   │   │   │   └── images/
    │   │   │   │       ├── high-contrast-list1.psd
    │   │   │   │       ├── high-contrast-list2.psd
    │   │   │   │       ├── high-contrast-list3.psd
    │   │   │   │       ├── high-contrast-list4.psd
    │   │   │   │       └── high-contrast-resources.psd
    │   │   │   ├── app-settings/
    │   │   │   │   ├── guidelines-for-app-settings.md
    │   │   │   │   ├── store-and-retrieve-app-data.md
    │   │   │   │   └── images/
    │   │   │   │       ├── appsettings-nav-settings.PNG
    │   │   │   │       ├── entertainment-29-settings.psd
    │   │   │   │       └── js-settingstab.psd
    │   │   │   ├── basics/
    │   │   │   │   ├── app-silhouette.md
    │   │   │   │   ├── commanding-basics.md
    │   │   │   │   ├── content-basics.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── navigate-between-two-pages.md
    │   │   │   │   ├── navigation-basics.md
    │   │   │   │   ├── navigation-history-and-backwards-navigation.md
    │   │   │   │   ├── titlebar-design.md
    │   │   │   │   └── images/
    │   │   │   │       ├── food-truck-finder/
    │   │   │   │       │   ├── uap-foodtruck-desktop-home-700.psd
    │   │   │   │       │   └── uap-foodtruck-phone-bottomtabs-320.psd
    │   │   │   │       ├── news-reader/
    │   │   │   │       │   └── .ds-store
    │   │   │   │       ├── photo-editor/
    │   │   │   │       │   └── uap-photo-pc-phone.psd
    │   │   │   │       ├── subway/
    │   │   │   │       │   └── uap-subway-pc-phone.psd
    │   │   │   │       └── xaml-basics/
    │   │   │   │           ├── adaptive-layout-small-after.PNG
    │   │   │   │           └── adaptive-layout-small-before.PNG
    │   │   │   ├── controls/
    │   │   │   │   ├── animated-icon.md
    │   │   │   │   ├── annotated-scrollbar.md
    │   │   │   │   ├── auto-suggest-box.md
    │   │   │   │   ├── breadcrumbbar.md
    │   │   │   │   ├── buttons.md
    │   │   │   │   ├── calendar-date-picker.md
    │   │   │   │   ├── calendar-view.md
    │   │   │   │   ├── checkbox.md
    │   │   │   │   ├── collection-commanding.md
    │   │   │   │   ├── color-picker.md
    │   │   │   │   ├── combo-box.md
    │   │   │   │   ├── command-bar-flyout.md
    │   │   │   │   ├── command-bar.md
    │   │   │   │   ├── commanding.md
    │   │   │   │   ├── contact-card.md
    │   │   │   │   ├── content-links.md
    │   │   │   │   ├── controls-and-events-intro.md
    │   │   │   │   ├── custom-transport-controls.md
    │   │   │   │   ├── data-template-selector.md
    │   │   │   │   ├── date-and-time.md
    │   │   │   │   ├── date-picker.md
    │   │   │   │   ├── expander.md
    │   │   │   │   ├── flipview.md
    │   │   │   │   ├── forms.md
    │   │   │   │   ├── hyperlinks.md
    │   │   │   │   ├── images-imagebrushes.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── info-badge.md
    │   │   │   │   ├── infobar.md
    │   │   │   │   ├── inking-controls.md
    │   │   │   │   ├── inverted-lists.md
    │   │   │   │   ├── item-containers-templates.md
    │   │   │   │   ├── item-templates-gridview.md
    │   │   │   │   ├── item-templates-listview.md
    │   │   │   │   ├── items-repeater.md
    │   │   │   │   ├── itemsview.md
    │   │   │   │   ├── labels.md
    │   │   │   │   ├── list-details.md
    │   │   │   │   ├── lists.md
    │   │   │   │   ├── listview-and-gridview.md
    │   │   │   │   ├── listview-filtering.md
    │   │   │   │   ├── media-playback.md
    │   │   │   │   ├── menus-and-context-menus.md
    │   │   │   │   ├── menus.md
    │   │   │   │   ├── navigationview.md
    │   │   │   │   ├── nested-ui.md
    │   │   │   │   ├── number-box.md
    │   │   │   │   ├── password-box.md
    │   │   │   │   ├── person-picture.md
    │   │   │   │   ├── pipspager.md
    │   │   │   │   ├── pivot.md
    │   │   │   │   ├── progress-controls.md
    │   │   │   │   ├── pull-to-refresh.md
    │   │   │   │   ├── radio-button.md
    │   │   │   │   ├── rating.md
    │   │   │   │   ├── rich-edit-box.md
    │   │   │   │   ├── rich-text-block.md
    │   │   │   │   ├── scroll-controls.md
    │   │   │   │   ├── selection-modes.md
    │   │   │   │   ├── selector-bar.md
    │   │   │   │   ├── semantic-zoom.md
    │   │   │   │   ├── shapes.md
    │   │   │   │   ├── slider.md
    │   │   │   │   ├── split-view.md
    │   │   │   │   ├── swipe.md
    │   │   │   │   ├── tab-view.md
    │   │   │   │   ├── text-block.md
    │   │   │   │   ├── text-box.md
    │   │   │   │   ├── text-controls.md
    │   │   │   │   ├── text-handwriting-view.md
    │   │   │   │   ├── time-picker.md
    │   │   │   │   ├── title-bar.md
    │   │   │   │   ├── toggles.md
    │   │   │   │   ├── tooltips.md
    │   │   │   │   ├── tree-view.md
    │   │   │   │   ├── two-pane-view.md
    │   │   │   │   ├── web-view.md
    │   │   │   │   ├── dialogs-and-flyouts/
    │   │   │   │   │   ├── dialogs.md
    │   │   │   │   │   ├── flyouts.md
    │   │   │   │   │   ├── index.md
    │   │   │   │   │   └── teaching-tip.md
    │   │   │   │   └── images/
    │   │   │   │       ├── button-dialog-example.PNG
    │   │   │   │       ├── checkbox.psd
    │   │   │   │       ├── combo-box-no-selection.PNG
    │   │   │   │       ├── flyout-lightdismiss.PNG
    │   │   │   │       ├── listview-basic-code-example2.PNG
    │   │   │   │       ├── navigation-view-left-style.PNG
    │   │   │   │       ├── navigation-view-top-style.PNG
    │   │   │   │       ├── news_and_weather_patterns_16_progress_bar.psd
    │   │   │   │       ├── patterns_md_splitview_parts.PNG
    │   │   │   │       ├── productivity_6_list_layout_new.psd
    │   │   │   │       ├── progress_changing.psd
    │   │   │   │       ├── ProgressBar.psd
    │   │   │   │       ├── radiobuttons.PNG
    │   │   │   │       ├── scrollbar-panning-1.PNG
    │   │   │   │       ├── scrollbar-panning.PNG
    │   │   │   │       ├── scrollbar-standard-1.PNG
    │   │   │   │       ├── scrollbar-traditional.PNG
    │   │   │   │       ├── Scrollbar.psd
    │   │   │   │       ├── search-app-canvas.PNG
    │   │   │   │       ├── search-icon-expanded-maps.PNG
    │   │   │   │       ├── slider-ticks.PNG
    │   │   │   │       ├── Slider.psd
    │   │   │   │       ├── spellcheck.psd
    │   │   │   │       ├── spicyoptions2.PNG
    │   │   │   │       ├── TextButtons.psd
    │   │   │   │       ├── TextInput.psd
    │   │   │   │       ├── toggle-switch-off.PNG
    │   │   │   │       ├── toggle-switch-on.PNG
    │   │   │   │       ├── ToggleSwitch.psd
    │   │   │   │       ├── uap-photo-pc-phone.psd
    │   │   │   │       ├── uap_foodtruck_desktop_home_700.psd
    │   │   │   │       ├── uap_foodtruck_phone_bottomtabs_320.psd
    │   │   │   │       ├── uap_photo_pc_phone.psd
    │   │   │   │       ├── uap_subway_pc_phone.psd
    │   │   │   │       └── ListItems/
    │   │   │   │           ├── doublelineexample.PNG
    │   │   │   │           ├── doublelineicon.PNG
    │   │   │   │           ├── icontext.PNG
    │   │   │   │           ├── icontext2.PNG
    │   │   │   │           ├── imageandtext2.PNG
    │   │   │   │           ├── singlelineexample.PNG
    │   │   │   │           └── triplelineexample.PNG
    │   │   │   ├── devices/
    │   │   │   │   ├── designing-for-MR.md
    │   │   │   │   ├── designing-for-tv.md
    │   │   │   │   ├── index.md
    │   │   │   │   └── images/
    │   │   │   │       └── input-patterns/
    │   │   │   │           ├── input-keyboard.psd
    │   │   │   │           ├── input-mouse.psd
    │   │   │   │           ├── input-pen.psd
    │   │   │   │           ├── input-touch.psd
    │   │   │   │           └── input-touchpad.psd
    │   │   │   ├── downloads/
    │   │   │   │   └── index.md
    │   │   │   ├── globalizing/
    │   │   │   │   ├── adjust-layout-and-fonts--and-support-rtl.md
    │   │   │   │   ├── design-for-bidi-text.md
    │   │   │   │   ├── glob-numeralsystem-values.md
    │   │   │   │   ├── globalizing-portal.md
    │   │   │   │   ├── guidelines-and-checklist-for-globalizing-your-app.md
    │   │   │   │   ├── japanese-era-change.md
    │   │   │   │   ├── loc-international-fonts.md
    │   │   │   │   ├── manage-language-and-region.md
    │   │   │   │   ├── mat-announcements.md
    │   │   │   │   ├── mat-faq-troubleshooting.yml
    │   │   │   │   ├── multilingual-app-toolkit-editor-downloads.md
    │   │   │   │   ├── prepare-your-app-for-localization.md
    │   │   │   │   ├── use-global-ready-formats.md
    │   │   │   │   ├── use-mat.md
    │   │   │   │   ├── use-patterns-to-format-dates-and-times.md
    │   │   │   │   ├── use-utf8-code-page.md
    │   │   │   │   └── images/
    │   │   │   │       ├── 56283_BIDI_01_startscreen.xml
    │   │   │   │       ├── 56283_BIDI_01_startscreen_resized.xml
    │   │   │   │       ├── 56283_BIDI_02_startscreen_charm.xml
    │   │   │   │       ├── 56283_BIDI_02_startscreen_charm_resized.xml
    │   │   │   │       ├── 56284_BIDI_03_tile_callouts_en-us.xml
    │   │   │   │       ├── 56284_BIDI_03_tile_callouts_withKey.xml
    │   │   │   │       ├── 56285_BIDI_04_bidirectional_tiles_white.xml
    │   │   │   │       ├── 56286_BIDI_05_search_flyout.xml
    │   │   │   │       ├── 56286_BIDI_05_search_flyout_resized.xml
    │   │   │   │       ├── 56286_BIDI_06_print_flyout.xml
    │   │   │   │       ├── 56286_BIDI_06_print_flyout_resized.xml
    │   │   │   │       ├── 56286_BIDI_07_settings_flyout.xml
    │   │   │   │       ├── 56286_BIDI_07_settings_flyout_resized.xml
    │   │   │   │       ├── 56286_BIDI_08_app_bars.xml
    │   │   │   │       ├── 56286_BIDI_08_app_bars_resized.xml
    │   │   │   │       ├── 56287_BIDI_09_keyboard_layout.xml
    │   │   │   │       ├── 56287_BIDI_09_keyboard_layout_resized.xml
    │   │   │   │       ├── 56288_BIDI_10_english_app.xml
    │   │   │   │       ├── 56288_BIDI_10_english_app_resized.xml
    │   │   │   │       ├── 56289_BIDI_11_parentheses.xml
    │   │   │   │       ├── 56289_BIDI_11_parentheses_resized.xml
    │   │   │   │       ├── 56289_BIDI_12_parentheses_fixed.xml
    │   │   │   │       ├── 56289_BIDI_12_parentheses_fixed_resized.xml
    │   │   │   │       ├── 56290_BIDI_13_start_screen_segoe.xml
    │   │   │   │       ├── 56290_BIDI_13_start_screen_segoe_arabic.xml
    │   │   │   │       ├── 56291_BIDI_1415_music_player_layouts_left-withcallouts.xml
    │   │   │   │       ├── 56291_BIDI_1415_music_player_layouts_right-withcallouts.xml
    │   │   │   │       ├── 56292_BIDI_16_app_layout_callouts.xml
    │   │   │   │       ├── 56292_bidi_16_app_layout_callouts_resized.xml
    │   │   │   │       ├── 56292_BIDI_17_app_layout_callouts.xml
    │   │   │   │       ├── 56292_bidi_17_app_layout_callouts_resized.xml
    │   │   │   │       ├── 56292_BIDI_18_app_layout_callouts.xml
    │   │   │   │       ├── 56292_bidi_18_app_layout_callouts_resized.xml
    │   │   │   │       ├── 56293_BIDI_19_icon_realignment_cropped.xml
    │   │   │   │       ├── 56293_BIDI_19_icon_realignment_cropped_resized.xml
    │   │   │   │       ├── 56294_BIDI_20_email_orientation_email.xml
    │   │   │   │       ├── 56294_BIDI_20_email_orientation_email_resized.xml
    │   │   │   │       ├── 56294_BIDI_21_email_orientation_LtR.xml
    │   │   │   │       ├── 56294_BIDI_21_email_orientation_LtR_resized.xml
    │   │   │   │       ├── 56294_BIDI_22_email_orientation_RtL.xml
    │   │   │   │       └── 56294_BIDI_22_email_orientation_RtL_resized.xml
    │   │   │   ├── in-app-help/
    │   │   │   │   ├── external-help.md
    │   │   │   │   ├── guidelines-for-app-help.md
    │   │   │   │   ├── in-app-help.md
    │   │   │   │   └── instructional-ui.md
    │   │   │   ├── input/
    │   │   │   │   ├── access-keys.md
    │   │   │   │   ├── convert-ink-to-text.md
    │   │   │   │   ├── cortana-deep-link-into-your-app.md
    │   │   │   │   ├── cortana-design-guidelines.md
    │   │   │   │   ├── cortana-dynamically-modify-voice-command-definition-vcd-phrase-lists.md
    │   │   │   │   ├── cortana-interact-with-a-background-app.md
    │   │   │   │   ├── cortana-interactions.md
    │   │   │   │   ├── cortana-launch-a-background-app-with-voice-commands.md
    │   │   │   │   ├── cortana-launch-a-foreground-app-with-voice-commands.md
    │   │   │   │   ├── cortana-support-natural-language-voice-commands.md
    │   │   │   │   ├── custom-text-input.md
    │   │   │   │   ├── define-custom-recognition-constraints.md
    │   │   │   │   ├── drag-and-drop.md
    │   │   │   │   ├── enable-continuous-dictation.md
    │   │   │   │   ├── focus-navigation-programmatic.md
    │   │   │   │   ├── focus-navigation.md
    │   │   │   │   ├── gamepad-and-remote-interactions.md
    │   │   │   │   ├── gaze-interactions.md
    │   │   │   │   ├── guidelines-for-cross-slide.md
    │   │   │   │   ├── guidelines-for-optical-zoom.md
    │   │   │   │   ├── guidelines-for-panning.md
    │   │   │   │   ├── guidelines-for-rotation.md
    │   │   │   │   ├── guidelines-for-targeting.md
    │   │   │   │   ├── guidelines-for-textselection.md
    │   │   │   │   ├── guidelines-for-visualfeedback.md
    │   │   │   │   ├── handle-pointer-input.md
    │   │   │   │   ├── identify-input-devices.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── ink-toolbar.md
    │   │   │   │   ├── ink-walkthrough.md
    │   │   │   │   ├── input-injection.md
    │   │   │   │   ├── input-method-editor-requirements.md
    │   │   │   │   ├── input-method-editors.md
    │   │   │   │   ├── input-primer.md
    │   │   │   │   ├── keyboard-accelerators.md
    │   │   │   │   ├── keyboard-events.md
    │   │   │   │   ├── keyboard-interactions.md
    │   │   │   │   ├── manage-issues-with-audio-input.md
    │   │   │   │   ├── mouse-interactions.md
    │   │   │   │   ├── multiple-input-design-guidelines.md
    │   │   │   │   ├── pen-and-stylus-interactions.md
    │   │   │   │   ├── pen-haptics.md
    │   │   │   │   ├── radialcontroller-walkthrough.md
    │   │   │   │   ├── respond-to-the-presence-of-the-touch-keyboard.md
    │   │   │   │   ├── save-and-load-ink.md
    │   │   │   │   ├── set-speech-recognition-timeouts.md
    │   │   │   │   ├── specify-the-speech-recognizer-language.md
    │   │   │   │   ├── speech-interactions.md
    │   │   │   │   ├── speech-recognition.md
    │   │   │   │   ├── text-scaling.md
    │   │   │   │   ├── touch-developer-guide.md
    │   │   │   │   ├── touch-interactions.md
    │   │   │   │   ├── touchpad-interactions.md
    │   │   │   │   ├── use-input-scope-to-change-the-touch-keyboard.md
    │   │   │   │   ├── windows-wheel-interactions.md
    │   │   │   │   ├── code/
    │   │   │   │   │   ├── dev_app_to_app.sln
    │   │   │   │   │   ├── copy_paste/
    │   │   │   │   │   │   └── cs/
    │   │   │   │   │   │       ├── App.xaml
    │   │   │   │   │   │       ├── App.xaml.cs
    │   │   │   │   │   │       ├── copy_paste.csproj
    │   │   │   │   │   │       ├── MainPage.xaml
    │   │   │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │   │   │       ├── Package.appxmanifest
    │   │   │   │   │   │       ├── Properties/
    │   │   │   │   │   │       │   ├── AssemblyInfo.cs
    │   │   │   │   │   │       │   └── Default.rd.xml
    │   │   │   │   │   │       └── Service References/
    │   │   │   │   │   │           └── Application Insights/
    │   │   │   │   │   │               └── ConnectedService.json
    │   │   │   │   │   ├── drag_drop/
    │   │   │   │   │   │   └── cs/
    │   │   │   │   │   │       ├── App.xaml
    │   │   │   │   │   │       ├── App.xaml.cs
    │   │   │   │   │   │       ├── drag_drop.csproj
    │   │   │   │   │   │       ├── MainPage.xaml
    │   │   │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │   │   │       ├── Package.appxmanifest
    │   │   │   │   │   │       ├── Properties/
    │   │   │   │   │   │       │   ├── AssemblyInfo.cs
    │   │   │   │   │   │       │   └── Default.rd.xml
    │   │   │   │   │   │       └── Service References/
    │   │   │   │   │   │           └── Application Insights/
    │   │   │   │   │   │               └── ConnectedService.json
    │   │   │   │   │   ├── receive_data/
    │   │   │   │   │   │   └── cs/
    │   │   │   │   │   │       ├── App.xaml
    │   │   │   │   │   │       ├── App.xaml.cs
    │   │   │   │   │   │       ├── MainPage.xaml
    │   │   │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │   │   │       ├── Package.appxmanifest
    │   │   │   │   │   │       ├── receive_data.csproj
    │   │   │   │   │   │       └── Properties/
    │   │   │   │   │   │           ├── AssemblyInfo.cs
    │   │   │   │   │   │           └── Default.rd.xml
    │   │   │   │   │   └── share_data/
    │   │   │   │   │       └── cs/
    │   │   │   │   │           ├── App.xaml
    │   │   │   │   │           ├── App.xaml.cs
    │   │   │   │   │           ├── MainPage.xaml
    │   │   │   │   │           ├── MainPage.xaml.cs
    │   │   │   │   │           ├── Package.appxmanifest
    │   │   │   │   │           ├── share_data.csproj
    │   │   │   │   │           ├── ShareData.csproj
    │   │   │   │   │           ├── Properties/
    │   │   │   │   │           │   ├── AssemblyInfo.cs
    │   │   │   │   │           │   └── Default.rd.xml
    │   │   │   │   │           └── Service References/
    │   │   │   │   │               └── Application Insights/
    │   │   │   │   │                   └── ConnectedService.json
    │   │   │   │   └── images/
    │   │   │   │       └── input-patterns/
    │   │   │   │           ├── input-keyboard.psd
    │   │   │   │           ├── input-mouse.psd
    │   │   │   │           ├── input-pen.psd
    │   │   │   │           ├── input-touch.psd
    │   │   │   │           └── input-touchpad.psd
    │   │   │   ├── layout/
    │   │   │   │   ├── alignment-margin-padding.md
    │   │   │   │   ├── attached-layouts.md
    │   │   │   │   ├── boxpanel-example-custom-panel.md
    │   │   │   │   ├── custom-panels-overview.md
    │   │   │   │   ├── depth-shadow.md
    │   │   │   │   ├── grid-tutorial.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── layout-panels.md
    │   │   │   │   ├── layouts-with-xaml.md
    │   │   │   │   ├── responsive-design.md
    │   │   │   │   ├── screen-sizes-and-breakpoints-for-responsive-design.md
    │   │   │   │   └── images/
    │   │   │   │       ├── grid-weather-1.PNG
    │   │   │   │       ├── grid-weather-2.PNG
    │   │   │   │       ├── grid-weather-3.PNG
    │   │   │   │       ├── partially-cloudy.PNG
    │   │   │   │       ├── food-truck-finder/
    │   │   │   │       │   ├── uap-foodtruck-desktop-home-700.psd
    │   │   │   │       │   └── uap-foodtruck-phone-bottomtabs-320.psd
    │   │   │   │       ├── news-reader/
    │   │   │   │       │   └── .ds-store
    │   │   │   │       ├── photo-editor/
    │   │   │   │       │   └── uap-photo-pc-phone.psd
    │   │   │   │       └── subway/
    │   │   │   │           └── uap-subway-pc-phone.psd
    │   │   │   ├── motion/
    │   │   │   │   ├── connected-animation.md
    │   │   │   │   ├── content-transition-animations.md
    │   │   │   │   ├── directionality-and-gravity.md
    │   │   │   │   ├── key-frame-and-easing-function-animations.md
    │   │   │   │   ├── motion-dragdrop.md
    │   │   │   │   ├── motion-edgebased.md
    │   │   │   │   ├── motion-fade.md
    │   │   │   │   ├── motion-in-practice.md
    │   │   │   │   ├── motion-list.md
    │   │   │   │   ├── motion-pointer.md
    │   │   │   │   ├── motion-popup-animations.md
    │   │   │   │   ├── motion-reposition.md
    │   │   │   │   ├── page-transitions.md
    │   │   │   │   ├── parallax.md
    │   │   │   │   ├── storyboarded-animations.md
    │   │   │   │   ├── timing-and-easing.md
    │   │   │   │   ├── xaml-animation.md
    │   │   │   │   ├── xaml-property-animations.md
    │   │   │   │   └── images/
    │   │   │   │       ├── alignment.psd
    │   │   │   │       ├── character-count.psd
    │   │   │   │       ├── clipping.psd
    │   │   │   │       ├── desktop.ini
    │   │   │   │       ├── feature.psd
    │   │   │   │       ├── hanging-text-alignment.psd
    │   │   │   │       ├── kerning-tracking.psd
    │   │   │   │       ├── line-endings.psd
    │   │   │   │       ├── line-height-stacking.psd
    │   │   │   │       ├── line-spacing.psd
    │   │   │   │       ├── news_and_weather_patterns_16_progress_bar.psd
    │   │   │   │       ├── paragraphs.psd
    │   │   │   │       ├── productivity_6_list_layout_new.psd
    │   │   │   │       ├── progress_changing.psd
    │   │   │   │       ├── ProgressBar.psd
    │   │   │   │       ├── RadioButton.psd
    │   │   │   │       ├── radiobutton_vs_dropdownlist.psd
    │   │   │   │       ├── Scrollbar.psd
    │   │   │   │       ├── segoe-sample.psd
    │   │   │   │       ├── shades.psd
    │   │   │   │       ├── Slider.psd
    │   │   │   │       ├── spellcheck.psd
    │   │   │   │       ├── TextButtons.psd
    │   │   │   │       ├── TextInput.psd
    │   │   │   │       ├── ToggleSwitch.psd
    │   │   │   │       ├── type-ramp.psd
    │   │   │   │       ├── weights.psd
    │   │   │   │       └── word-letter.psd
    │   │   │   ├── shell/
    │   │   │   │   ├── index.md
    │   │   │   │   ├── pin-to-taskbar.md
    │   │   │   │   └── tiles-and-notifications/
    │   │   │   │       ├── adaptive-interactive-toasts.md
    │   │   │   │       ├── badges.md
    │   │   │   │       ├── channel-types.md
    │   │   │   │       ├── choosing-a-notification-delivery-method.md
    │   │   │   │       ├── custom-audio-on-toasts.md
    │   │   │   │       ├── custom-timestamps-on-toasts.md
    │   │   │   │       ├── firewall-allowlist-config.md
    │   │   │   │       ├── notification-listener.md
    │   │   │   │       ├── notification-mirroring.md
    │   │   │   │       ├── notifications-visualizer.md
    │   │   │   │       ├── periodic-notification-overview.md
    │   │   │   │       ├── push-request-response-headers.md
    │   │   │   │       ├── quickstart-send-push-notification.md
    │   │   │   │       ├── raw-notification-overview.md
    │   │   │   │       ├── request-create-save-notification-channel.md
    │   │   │   │       ├── scheduled-toast.md
    │   │   │   │       ├── secondary-tiles-desktop-pinning.md
    │   │   │   │       ├── send-local-toast-cpp-uwp.md
    │   │   │   │       ├── send-local-toast-desktop-cpp-wrl.md
    │   │   │   │       ├── send-local-toast-other-apps.md
    │   │   │   │       ├── send-local-toast.md
    │   │   │   │       ├── the-code-generated-by-the-push-notification-wizard.md
    │   │   │   │       ├── toast-collections.md
    │   │   │   │       ├── toast-desktop-apps.md
    │   │   │   │       ├── toast-headers.md
    │   │   │   │       ├── toast-notifications-overview.md
    │   │   │   │       ├── toast-pending-update.md
    │   │   │   │       ├── toast-progress-bar.md
    │   │   │   │       ├── toast-schema.md
    │   │   │   │       ├── toast-ux-guidance.md
    │   │   │   │       ├── troubleshoot-notifications.md
    │   │   │   │       ├── universal-dismiss.md
    │   │   │   │       ├── windows-push-notification-services--wns--overview.md
    │   │   │   │       ├── WNS-Notification-Priorities.md
    │   │   │   │       └── includes/
    │   │   │   │           ├── desktop-toast-activation-code.md
    │   │   │   │           ├── desktop-toast-activation-sequence.md
    │   │   │   │           ├── images-note.md
    │   │   │   │           ├── nuget-package-dotnet-warnings.md
    │   │   │   │           ├── nuget-package.md
    │   │   │   │           ├── onlaunched-warning.md
    │   │   │   │           ├── send-toast-basic-toast-intro.md
    │   │   │   │           └── send-toast-intro.md
    │   │   │   ├── signature-experiences/
    │   │   │   │   ├── color.md
    │   │   │   │   ├── geometry.md
    │   │   │   │   ├── iconography.md
    │   │   │   │   ├── layering.md
    │   │   │   │   ├── materials.md
    │   │   │   │   ├── motion.md
    │   │   │   │   └── typography.md
    │   │   │   ├── style/
    │   │   │   │   ├── acrylic.md
    │   │   │   │   ├── balancing-style-and-consistency.md
    │   │   │   │   ├── icons.md
    │   │   │   │   ├── mica.md
    │   │   │   │   ├── rounded-corner.md
    │   │   │   │   ├── segoe-fluent-icons-font.md
    │   │   │   │   ├── segoe-ui-symbol-font.md
    │   │   │   │   ├── sound.md
    │   │   │   │   ├── spacing.md
    │   │   │   │   ├── writing-style.md
    │   │   │   │   ├── iconography/
    │   │   │   │   │   ├── app-icon-construction.md
    │   │   │   │   │   ├── app-icon-design.md
    │   │   │   │   │   ├── live-tile-icons.md
    │   │   │   │   │   ├── overview.md
    │   │   │   │   │   └── visual-studio-asset-generation.md
    │   │   │   │   └── images/
    │   │   │   │       ├── alignment.psd
    │   │   │   │       ├── character-count.psd
    │   │   │   │       ├── checkbox.psd
    │   │   │   │       ├── clipping.psd
    │   │   │   │       ├── desktop.ini
    │   │   │   │       ├── feature.psd
    │   │   │   │       ├── hanging-text-alignment.psd
    │   │   │   │       ├── kerning-tracking.psd
    │   │   │   │       ├── line-endings.psd
    │   │   │   │       ├── line-height-stacking.psd
    │   │   │   │       ├── line-spacing.psd
    │   │   │   │       ├── news_and_weather_patterns_16_progress_bar.psd
    │   │   │   │       ├── paragraphs.psd
    │   │   │   │       ├── productivity_6_list_layout_new.psd
    │   │   │   │       ├── progress_changing.psd
    │   │   │   │       ├── ProgressBar.psd
    │   │   │   │       ├── RadioButton.psd
    │   │   │   │       ├── radiobutton_vs_dropdownlist.psd
    │   │   │   │       ├── Scrollbar.psd
    │   │   │   │       ├── segoe-sample.psd
    │   │   │   │       ├── shades.psd
    │   │   │   │       ├── Slider.psd
    │   │   │   │       ├── spellcheck.psd
    │   │   │   │       ├── TextButtons.psd
    │   │   │   │       ├── TextInput.psd
    │   │   │   │       ├── ToggleSwitch.psd
    │   │   │   │       ├── type-ramp.psd
    │   │   │   │       ├── weights.psd
    │   │   │   │       ├── word-letter.psd
    │   │   │   │       ├── color/
    │   │   │   │       │   └── color-on-color.psd
    │   │   │   │       └── segoe-mdl/
    │   │   │   │           └── txt.txt
    │   │   │   ├── usability/
    │   │   │   │   └── index.md
    │   │   │   └── widgets/
    │   │   │       ├── index.md
    │   │   │       ├── widgets-create-a-template.md
    │   │   │       ├── widgets-design-fundamentals.md
    │   │   │       ├── widgets-interaction-design.md
    │   │   │       ├── widgets-picker-integration.md
    │   │   │       └── widgets-states-and-ui.md
    │   │   ├── desktop/
    │   │   │   ├── index.yml
    │   │   │   ├── visual-studio-templates.md
    │   │   │   ├── images/
    │   │   │   │   ├── desktop-app-projects-cpp.PNG
    │   │   │   │   ├── desktop-console-projects-cpp.PNG
    │   │   │   │   ├── desktop-library-projects-cpp.PNG
    │   │   │   │   ├── dotnet-projects-csharp.PNG
    │   │   │   │   ├── uwp-projects-cpp.PNG
    │   │   │   │   ├── uwp-projects-csharp.PNG
    │   │   │   │   ├── winui-items-csharp.PNG
    │   │   │   │   └── winui-projects-csharp.PNG
    │   │   │   └── modernize/
    │   │   │       ├── desktop-to-uwp-distribute.md
    │   │   │       ├── desktop-to-uwp-enhance.md
    │   │   │       ├── desktop-to-uwp-extend.md
    │   │   │       ├── desktop-to-uwp-extensions.md
    │   │   │       ├── desktop-to-uwp-supported-api.md
    │   │   │       ├── get-activation-info-for-packaged-apps.md
    │   │   │       ├── grant-identity-to-nonpackaged-apps-overview.md
    │   │   │       ├── grant-identity-to-nonpackaged-apps-visual-studio.md
    │   │   │       ├── grant-identity-to-nonpackaged-apps.md
    │   │   │       ├── index.md
    │   │   │       ├── integrate-packaged-app-with-file-explorer.md
    │   │   │       ├── modernize-packaged-apps.md
    │   │   │       ├── modernize-wpf-tutorial-1.md
    │   │   │       ├── modernize-wpf-tutorial-2.md
    │   │   │       ├── modernize-wpf-tutorial-3.md
    │   │   │       ├── modernize-wpf-tutorial-4.md
    │   │   │       ├── modernize-wpf-tutorial-5.md
    │   │   │       ├── modernize-wpf-tutorial.md
    │   │   │       ├── package-identity-overview.md
    │   │   │       ├── winrt-com-interop-csharp.md
    │   │   │       ├── framework-packages/
    │   │   │       │   ├── framework-packages-overview.md
    │   │   │       │   ├── index.md
    │   │   │       │   └── use-the-dynamic-dependency-api.md
    │   │   │       ├── ui/
    │   │   │       │   ├── apply-mica-win32.md
    │   │   │       │   ├── apply-rounded-corners.md
    │   │   │       │   ├── apply-snap-layout-menu.md
    │   │   │       │   ├── apply-windows-themes.md
    │   │   │       │   ├── using-the-visual-layer-with-win32.md
    │   │   │       │   ├── using-the-visual-layer-with-windows-forms.md
    │   │   │       │   ├── using-the-visual-layer-with-wpf.md
    │   │   │       │   └── visual-layer-in-desktop-apps.md
    │   │   │       └── xaml-islands/
    │   │   │           ├── advanced-scenarios-xaml-islands-cpp.md
    │   │   │           ├── host-custom-control-with-xaml-islands-cpp.md
    │   │   │           ├── host-custom-control-with-xaml-islands.md
    │   │   │           ├── host-standard-control-with-xaml-islands-cpp.md
    │   │   │           ├── host-standard-control-with-xaml-islands.md
    │   │   │           ├── using-the-xaml-hosting-api.md
    │   │   │           └── xaml-islands.md
    │   │   ├── develop/
    │   │   │   ├── accessibility.md
    │   │   │   ├── app-lifecycle-and-system-services.md
    │   │   │   ├── audio-video-camera.md
    │   │   │   ├── communication.md
    │   │   │   ├── data-and-files.md
    │   │   │   ├── devices-and-sensors.md
    │   │   │   ├── dispatcherqueue.md
    │   │   │   ├── graphics.md
    │   │   │   ├── index.md
    │   │   │   ├── speech.md
    │   │   │   ├── title-bar.md
    │   │   │   ├── user-interface.md
    │   │   │   ├── windows-app-restore.md
    │   │   │   ├── camera/
    │   │   │   │   ├── basic-photo-capture.md
    │   │   │   │   ├── camera-privacy-setting.md
    │   │   │   │   ├── camera-profiles.md
    │   │   │   │   ├── camera-quickstart-winui3.md
    │   │   │   │   ├── camera.md
    │   │   │   │   ├── cameracaptureui.md
    │   │   │   │   ├── capture-device-controls-for-photo-and-video-capture.md
    │   │   │   │   ├── capture-device-controls-for-video-capture.md
    │   │   │   │   ├── connect-to-remote-cameras.md
    │   │   │   │   ├── detect-audio-level-changes.md
    │   │   │   │   ├── effects-for-video-capture.md
    │   │   │   │   ├── hdr-low-light-photo-capture.md
    │   │   │   │   ├── launch-camera-settings.md
    │   │   │   │   ├── process-audio-frames-with-mediaframereader.md
    │   │   │   │   ├── process-media-frames-with-mediaframereader.md
    │   │   │   │   ├── scene-analysis-for-media-capture.md
    │   │   │   │   ├── set-media-encoding-properties.md
    │   │   │   │   └── variable-photo-sequence.md
    │   │   │   ├── data-access/
    │   │   │   │   ├── cosmos-db-data-access.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── mongodb-database.md
    │   │   │   │   ├── mysql-database.md
    │   │   │   │   ├── sql-server-database.md
    │   │   │   │   └── sqlite-data-access.md
    │   │   │   ├── data-binding/
    │   │   │   │   ├── bind-to-hierarchical-data-and-create-a-master-details-view.md
    │   │   │   │   ├── data-binding-and-mvvm.md
    │   │   │   │   ├── data-binding-in-depth.md
    │   │   │   │   ├── data-binding-overview.md
    │   │   │   │   ├── function-bindings.md
    │   │   │   │   └── index.md
    │   │   │   ├── devices-sensors/
    │   │   │   │   ├── customize-the-print-preview-ui.md
    │   │   │   │   ├── print-from-your-app.md
    │   │   │   │   ├── printing-and-scanning.md
    │   │   │   │   └── scan-from-your-app.md
    │   │   │   ├── feeds/
    │   │   │   │   ├── feed-provider-manifest.md
    │   │   │   │   ├── feed-providers.md
    │   │   │   │   ├── implement-feed-provider-cs.md
    │   │   │   │   └── implement-feed-provider-win32.md
    │   │   │   ├── files/
    │   │   │   │   ├── dotnet-files.md
    │   │   │   │   ├── index.md
    │   │   │   │   └── winrt-files.md
    │   │   │   ├── launch/
    │   │   │   │   ├── create-and-register-a-background-task.md
    │   │   │   │   ├── handle-file-activation.md
    │   │   │   │   ├── handle-uri-activation.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── launch-default-app.md
    │   │   │   │   ├── launch-default-apps-settings.md
    │   │   │   │   ├── launch-people-app.md
    │   │   │   │   ├── launch-screen-snipping.md
    │   │   │   │   ├── launch-settings-app.md
    │   │   │   │   ├── launch-snipping-tool.md
    │   │   │   │   ├── launch-store-app.md
    │   │   │   │   ├── launch-the-default-app-for-a-file.md
    │   │   │   │   ├── reserved-uri-scheme-names.md
    │   │   │   │   └── web-to-app-linking.md
    │   │   │   ├── platform/
    │   │   │   │   ├── csharp-winrt/
    │   │   │   │   │   ├── agile-objects.md
    │   │   │   │   │   ├── authoring-diagnostics.md
    │   │   │   │   │   ├── authoring.md
    │   │   │   │   │   ├── create-windows-runtime-component-cswinrt.md
    │   │   │   │   │   ├── create-winrt-component-winui-cswinrt.md
    │   │   │   │   │   ├── index.md
    │   │   │   │   │   ├── net-mappings-of-winrt-types.md
    │   │   │   │   │   ├── net-projection-from-cppwinrt-component.md
    │   │   │   │   │   └── images/
    │   │   │   │   │       ├── console-output.PNG
    │   │   │   │   │       └── projection-dependencies.PNG
    │   │   │   │   └── xaml/
    │   │   │   │       ├── 3-d-perspective-effects.md
    │   │   │   │       ├── brushes.md
    │   │   │   │       ├── transforms.md
    │   │   │   │       ├── xaml-control-templates.md
    │   │   │   │       ├── xaml-resource-dictionary.md
    │   │   │   │       ├── xaml-styles.md
    │   │   │   │       └── xaml-theme-resources.md
    │   │   │   ├── search/
    │   │   │   │   ├── cloud-search-integration.md
    │   │   │   │   ├── index.md
    │   │   │   │   └── search-providers.md
    │   │   │   ├── security/
    │   │   │   │   ├── credential-locker.md
    │   │   │   │   ├── design.md
    │   │   │   │   ├── fingerprint-biometrics.md
    │   │   │   │   ├── implement.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── intro.md
    │   │   │   │   ├── oauth2.md
    │   │   │   │   ├── reference.md
    │   │   │   │   ├── share-certificates.md
    │   │   │   │   ├── smart-cards.md
    │   │   │   │   ├── third-party.md
    │   │   │   │   ├── tools-libraries.md
    │   │   │   │   ├── use-cases.md
    │   │   │   │   ├── windows-hello-auth-service.md
    │   │   │   │   ├── windows-hello-login.md
    │   │   │   │   └── windows-hello.md
    │   │   │   ├── settings/
    │   │   │   │   ├── readclouddatasettings-exe.md
    │   │   │   │   ├── settings-common.md
    │   │   │   │   └── settings-windows-11.md
    │   │   │   ├── smart-app-control/
    │   │   │   │   ├── code-signing-for-smart-app-control.md
    │   │   │   │   ├── overview.md
    │   │   │   │   └── test-your-app-with-smart-app-control.md
    │   │   │   ├── ui-input/
    │   │   │   │   ├── display-ui-objects.md
    │   │   │   │   ├── retrieve-hwnd.md
    │   │   │   │   └── visual-tree.md
    │   │   │   ├── widgets/
    │   │   │   │   ├── implement-widget-provider-cs.md
    │   │   │   │   ├── implement-widget-provider-win32.md
    │   │   │   │   ├── web-widget-providers.md
    │   │   │   │   ├── widget-header-customization.md
    │   │   │   │   ├── widget-provider-activateapplication-protocol.md
    │   │   │   │   ├── widget-provider-manifest.md
    │   │   │   │   └── widget-providers.md
    │   │   │   ├── win2d/
    │   │   │   │   ├── avoiding-memory-leaks.md
    │   │   │   │   ├── bitmap-block-compression.md
    │   │   │   │   ├── choosing-control-resolution.md
    │   │   │   │   ├── custom-effects.md
    │   │   │   │   ├── dpi-and-dips.md
    │   │   │   │   ├── effect-precision-and-clamping.md
    │   │   │   │   ├── features.md
    │   │   │   │   ├── handling-device-lost.md
    │   │   │   │   ├── hellowin2dworld.md
    │   │   │   │   ├── in-a-core-app.md
    │   │   │   │   ├── index.md
    │   │   │   │   ├── interop.md
    │   │   │   │   ├── loading-resources-outside-of-createresources.md
    │   │   │   │   ├── offscreen-drawing.md
    │   │   │   │   ├── pixel-formats.md
    │   │   │   │   ├── premultiplied-alpha.md
    │   │   │   │   ├── quick-start.md
    │   │   │   │   └── using-win2d-without-built-in-controls.md
    │   │   │   └── windows-integration/
    │   │   │       ├── copilot-key-state.md
    │   │   │       ├── cross-device-people-api.md
    │   │   │       ├── index.md
    │   │   │       ├── integrate-sharesheet-overview.md
    │   │   │       ├── integrate-sharesheet-packaged.md
    │   │   │       ├── integrate-sharesheet-pwa.md
    │   │   │       ├── integrate-sharesheet-unpackaged.md
    │   │   │       └── microsoft-copliot-key-provider.md
    │   │   ├── distribute-through-store/
    │   │   │   ├── how-to-distribute-your-win32-app-through-microsoft-store.md
    │   │   │   ├── how-to-transition-users-from-your-web-unpackaged-app-to-store-packaged-app.md
    │   │   │   └── how-to-use-store-web-installer-for-distribution.md
    │   │   ├── get-started/
    │   │   │   ├── best-practices.md
    │   │   │   ├── developer-mode-features-and-debugging.md
    │   │   │   ├── enable-your-device-for-development.md
    │   │   │   ├── index.md
    │   │   │   ├── intro-pack-dep-proc.md
    │   │   │   ├── make-apps-great-for-windows.md
    │   │   │   ├── samples.md
    │   │   │   ├── sign-up.md
    │   │   │   ├── simple-photo-viewer-winui3.md
    │   │   │   ├── start-here.md
    │   │   │   ├── uno-simple-photo-viewer.md
    │   │   │   ├── windows-developer-faq.yml
    │   │   │   ├── windows-developer-glossary.md
    │   │   │   └── images/
    │   │   │       ├── devmode-pc-pinpair.PNG
    │   │   │       └── VisualStudio2017Hero_ImageXL-LG.PNG
    │   │   ├── how-tos/
    │   │   │   ├── chatgpt-openai-winui3.md
    │   │   │   ├── copilot-chat-winui3.md
    │   │   │   ├── dall-e-winui3.md
    │   │   │   ├── github-copilot-winui-vs.md
    │   │   │   ├── hello-world-winui3.md
    │   │   │   └── uno-multiplatform.md
    │   │   ├── package-and-deploy/
    │   │   │   ├── ci-for-winui3.md
    │   │   │   ├── deploy-overview.md
    │   │   │   ├── index.md
    │   │   │   ├── project-properties.md
    │   │   │   └── self-contained-deploy/
    │   │   │       └── deploy-self-contained-apps.md
    │   │   ├── performance/
    │   │   │   ├── choose-between-tools.md
    │   │   │   ├── disk-memory.md
    │   │   │   ├── index.md
    │   │   │   ├── introduction.md
    │   │   │   ├── power.md
    │   │   │   ├── responsive.md
    │   │   │   └── winui-perf.md
    │   │   ├── publish/
    │   │   │   ├── actionable-analytics-insights.md
    │   │   │   ├── app-management-and-services.md
    │   │   │   ├── app-marketing-guidelines.md
    │   │   │   ├── attract-customers-and-promote-your-apps.md
    │   │   │   ├── beta-testing-and-targeted-distribution.md
    │   │   │   ├── contact-us.md
    │   │   │   ├── create-a-custom-app-promotion-campaign.md
    │   │   │   ├── create-customer-groups.md
    │   │   │   ├── create-customer-segments.md
    │   │   │   ├── create-known-user-groups.md
    │   │   │   ├── distribute-lob-apps-to-enterprises.md
    │   │   │   ├── engage-with-your-customers.md
    │   │   │   ├── generate-preinstall-packages-for-oems.md
    │   │   │   ├── generate-promotional-codes.md
    │   │   │   ├── gradual-package-rollout.md
    │   │   │   ├── improved-health-report.md
    │   │   │   ├── index.md
    │   │   │   ├── last-update-date.md
    │   │   │   ├── link-to-your-app.md
    │   │   │   ├── make-your-app-easier-to-promote.md
    │   │   │   ├── microsoft-store-app-badge.md
    │   │   │   ├── organizational-licensing.md
    │   │   │   ├── package-flights.md
    │   │   │   ├── product-page-experiments.md
    │   │   │   ├── put-apps-and-add-ons-on-sale.md
    │   │   │   ├── respond-to-customer-feedback.md
    │   │   │   ├── respond-to-customer-reviews.md
    │   │   │   ├── send-push-notifications-to-your-apps-customers.md
    │   │   │   ├── store-app-quality.md
    │   │   │   ├── store-business-verification-reqs.md
    │   │   │   ├── store-developer-code-of-conduct.md
    │   │   │   ├── store-policies-and-code-of-conduct.md
    │   │   │   ├── store-policies-change-history.md
    │   │   │   ├── store-policies.md
    │   │   │   ├── store-submission-api.md
    │   │   │   ├── toc.yml
    │   │   │   ├── use-targeted-offers-to-maximize-engagement-and-conversions.md
    │   │   │   ├── view-app-identity-details.md
    │   │   │   ├── whats-new-msix-app-overview-page.md
    │   │   │   ├── analyze-app-performance/
    │   │   │   │   ├── gdk-xbox.md
    │   │   │   │   ├── msi-exe.md
    │   │   │   │   └── msix.md
    │   │   │   ├── analyze-msi-exe/
    │   │   │   │   ├── analyze-app-performance.md
    │   │   │   │   └── ratings-reviews-performance.md
    │   │   │   ├── msstore-dev-cli/
    │   │   │   │   ├── commands.md
    │   │   │   │   ├── flights-command.md
    │   │   │   │   ├── flights-create-command.md
    │   │   │   │   ├── flights-delete-command.md
    │   │   │   │   ├── flights-get-command.md
    │   │   │   │   ├── flights-list-command.md
    │   │   │   │   ├── flights-submission-command.md
    │   │   │   │   ├── flights-submission-delete-command.md
    │   │   │   │   ├── flights-submission-get-command.md
    │   │   │   │   ├── flights-submission-poll-command.md
    │   │   │   │   ├── flights-submission-publish-command.md
    │   │   │   │   ├── flights-submission-rollout-command.md
    │   │   │   │   ├── flights-submission-rollout-finalize-command.md
    │   │   │   │   ├── flights-submission-rollout-get-command.md
    │   │   │   │   ├── flights-submission-rollout-halt-command.md
    │   │   │   │   ├── flights-submission-rollout-update-command.md
    │   │   │   │   ├── flights-submission-status-command.md
    │   │   │   │   ├── flights-submission-update-command.md
    │   │   │   │   └── overview.md
    │   │   │   ├── partner-center/
    │   │   │   │   ├── account-types-locations-and-fees.md
    │   │   │   │   ├── assign-account-level-custom-permissions-to-account-users.md
    │   │   │   │   ├── assign-product-level-custom-permissions-to-account-users.md
    │   │   │   │   ├── assign-roles-to-account-users.md
    │   │   │   │   ├── associate-existing-azure-ad-tenant-with-partner-center-account.md
    │   │   │   │   ├── close-your-developer-account-in-partner-center.md
    │   │   │   │   ├── create-new-azure-ad-tenant.md
    │   │   │   │   ├── manage-account-users.md
    │   │   │   │   ├── manage-azure-ad-applications-in-partner-center.md
    │   │   │   │   ├── manage-groups-in-partner-center.md
    │   │   │   │   ├── manage-users-in-partner-center.md
    │   │   │   │   ├── open-a-developer-account.md
    │   │   │   │   ├── overview-of-custom-permissions-for-account-users.md
    │   │   │   │   ├── overview-of-roles-and-permissions-for-account-users.md
    │   │   │   │   ├── overview-users-groups-azure-ad-applications.md
    │   │   │   │   ├── partner-center-developer-account.md
    │   │   │   │   ├── partner-center-workspaces.md
    │   │   │   │   ├── remove-azure-ad-tenant-associations.md
    │   │   │   │   ├── trademark-and-copyright-protection.md
    │   │   │   │   ├── troubleshoot-app-creation.md
    │   │   │   │   ├── msi/
    │   │   │   │   │   └── manage-app-name-reservations.md
    │   │   │   │   ├── msix/
    │   │   │   │   │   └── manage-app-name-reservations.md
    │   │   │   │   └── pwa/
    │   │   │   │       └── manage-app-name-reservations.md
    │   │   │   ├── publish-your-app/
    │   │   │   │   ├── responsible-ai-faq-ai-generated-keywords.md
    │   │   │   │   ├── why-distribute-through-store.md
    │   │   │   │   ├── add-on/
    │   │   │   │   │   ├── add-and-edit-store-listing-info.md
    │   │   │   │   │   ├── app-certification-process.md
    │   │   │   │   │   ├── create-app-store-listing.md
    │   │   │   │   │   ├── create-app-submission.md
    │   │   │   │   │   ├── enter-app-properties.md
    │   │   │   │   │   ├── import-and-export-store-listings.md
    │   │   │   │   │   ├── manage-submission-options.md
    │   │   │   │   │   ├── market-selection.md
    │   │   │   │   │   ├── overview.md
    │   │   │   │   │   ├── price-and-availability.md
    │   │   │   │   │   ├── product-declarations.md
    │   │   │   │   │   ├── publish-update-to-your-app-on-store.md
    │   │   │   │   │   ├── reserve-your-apps-name.md
    │   │   │   │   │   ├── resolve-submission-errors.md
    │   │   │   │   │   ├── schedule-pricing-changes.md
    │   │   │   │   │   ├── support-info.md
    │   │   │   │   │   ├── visibility-options.md
    │   │   │   │   │   ├── what-are-add-ons.md
    │   │   │   │   │   └── write-great-app-description.md
    │   │   │   │   ├── msi/
    │   │   │   │   │   ├── add-additional-information.md
    │   │   │   │   │   ├── add-and-edit-store-listing-info.md
    │   │   │   │   │   ├── age-ratings.md
    │   │   │   │   │   ├── app-certification-process.md
    │   │   │   │   │   ├── app-package-management.md
    │   │   │   │   │   ├── app-package-requirements.md
    │   │   │   │   │   ├── app-submission-control.md
    │   │   │   │   │   ├── categories-and-subcategories.md
    │   │   │   │   │   ├── create-app-store-listing.md
    │   │   │   │   │   ├── create-app-submission.md
    │   │   │   │   │   ├── enter-app-properties.md
    │   │   │   │   │   ├── import-and-export-store-listings.md
    │   │   │   │   │   ├── manual-package-validation.md
    │   │   │   │   │   ├── market-selection.md
    │   │   │   │   │   ├── package-validation-pre-check.md
    │   │   │   │   │   ├── price-and-availability.md
    │   │   │   │   │   ├── product-declarations.md
    │   │   │   │   │   ├── publish-update-to-your-app-on-store.md
    │   │   │   │   │   ├── reserve-your-apps-name.md
    │   │   │   │   │   ├── screenshots-and-images.md
    │   │   │   │   │   ├── set-app-pricing.md
    │   │   │   │   │   ├── support-info.md
    │   │   │   │   │   ├── system-requirements.md
    │   │   │   │   │   ├── upload-app-packages.md
    │   │   │   │   │   ├── visibility-options.md
    │   │   │   │   │   └── write-great-app-description.md
    │   │   │   │   ├── msix/
    │   │   │   │   │   ├── add-additional-information.md
    │   │   │   │   │   ├── add-and-edit-store-listing-info.md
    │   │   │   │   │   ├── age-ratings.md
    │   │   │   │   │   ├── app-certification-process.md
    │   │   │   │   │   ├── app-package-management.md
    │   │   │   │   │   ├── app-package-requirements.md
    │   │   │   │   │   ├── categories-and-subcategories.md
    │   │   │   │   │   ├── create-app-store-listing.md
    │   │   │   │   │   ├── create-app-submission.md
    │   │   │   │   │   ├── enter-app-properties.md
    │   │   │   │   │   ├── import-and-export-store-listings.md
    │   │   │   │   │   ├── manage-submission-options.md
    │   │   │   │   │   ├── market-selection.md
    │   │   │   │   │   ├── price-and-availability.md
    │   │   │   │   │   ├── product-declarations.md
    │   │   │   │   │   ├── publish-update-to-your-app-on-store.md
    │   │   │   │   │   ├── reserve-your-apps-name.md
    │   │   │   │   │   ├── resolve-submission-errors.md
    │   │   │   │   │   ├── schedule-pricing-changes.md
    │   │   │   │   │   ├── screenshots-and-images.md
    │   │   │   │   │   ├── support-info.md
    │   │   │   │   │   ├── system-requirements.md
    │   │   │   │   │   ├── upload-app-packages.md
    │   │   │   │   │   ├── visibility-options.md
    │   │   │   │   │   └── write-great-app-description.md
    │   │   │   │   └── pwa/
    │   │   │   │       ├── add-additional-information.md
    │   │   │   │       ├── add-and-edit-store-listing-info.md
    │   │   │   │       ├── age-ratings.md
    │   │   │   │       ├── app-certification-process.md
    │   │   │   │       ├── app-package-management.md
    │   │   │   │       ├── app-package-requirements.md
    │   │   │   │       ├── categories-and-subcategories.md
    │   │   │   │       ├── create-app-store-listing.md
    │   │   │   │       ├── create-app-submission.md
    │   │   │   │       ├── enter-app-properties.md
    │   │   │   │       ├── import-and-export-store-listings.md
    │   │   │   │       ├── manage-submission-options.md
    │   │   │   │       ├── market-selection.md
    │   │   │   │       ├── price-and-availability.md
    │   │   │   │       ├── product-declarations.md
    │   │   │   │       ├── publish-update-to-your-app-on-store.md
    │   │   │   │       ├── reserve-your-apps-name.md
    │   │   │   │       ├── resolve-submission-errors.md
    │   │   │   │       ├── schedule-pricing-changes.md
    │   │   │   │       ├── screenshots-and-images.md
    │   │   │   │       ├── support-info.md
    │   │   │   │       ├── system-requirements.md
    │   │   │   │       ├── turn-your-website-pwa.md
    │   │   │   │       ├── upload-app-packages.md
    │   │   │   │       ├── visibility-options.md
    │   │   │   │       └── write-great-app-description.md
    │   │   │   └── store-policy-archive/
    │   │   │       ├── store-policy-7-11.md
    │   │   │       ├── store-policy-7-12.md
    │   │   │       ├── store-policy-7-13.md
    │   │   │       ├── store-policy-7-14.md
    │   │   │       ├── store-policy-7-15.md
    │   │   │       ├── store-policy-7-16-1.md
    │   │   │       ├── store-policy-7-16.md
    │   │   │       ├── store-policy-7-17.md
    │   │   │       ├── store-policy-7-6.md
    │   │   │       └── store-policy-7-7.md
    │   │   ├── trace-processing/
    │   │   │   ├── extensibility.md
    │   │   │   ├── index.yml
    │   │   │   ├── overview.md
    │   │   │   ├── quickstart.md
    │   │   │   ├── reference.md
    │   │   │   ├── streaming.md
    │   │   │   ├── symbols.md
    │   │   │   ├── TOC.yml
    │   │   │   └── tutorial.md
    │   │   ├── tutorials/
    │   │   │   └── winui-notes/
    │   │   │       ├── index.yml
    │   │   │       └── includes/
    │   │   │           ├── all-notes.md
    │   │   │           ├── intro.md
    │   │   │           ├── navigation.md
    │   │   │           ├── note.md
    │   │   │           ├── project.md
    │   │   │           └── view-model.md
    │   │   ├── whats-new/
    │   │   │   ├── community.md
    │   │   │   └── windows-11-build-22000.md
    │   │   ├── windows-app-sdk/
    │   │   │   ├── breaking-changes.md
    │   │   │   ├── check-windows-app-sdk-versions.md
    │   │   │   ├── composition.md
    │   │   │   ├── deploy-packaged-apps.md
    │   │   │   ├── deploy-unpackaged-apps.md
    │   │   │   ├── deployment-architecture.md
    │   │   │   ├── downloads-archive.md
    │   │   │   ├── downloads.md
    │   │   │   ├── dwritecore.md
    │   │   │   ├── experimental-channel.md
    │   │   │   ├── index.md
    │   │   │   ├── preview-channel.md
    │   │   │   ├── preview-experimental-create-winui3-app.md
    │   │   │   ├── preview-experimental-unpackaged-tutorial.md
    │   │   │   ├── release-channels.md
    │   │   │   ├── remove-windows-app-sdk-versions.md
    │   │   │   ├── set-up-your-development-environment.md
    │   │   │   ├── single-project-msix.md
    │   │   │   ├── stable-channel.md
    │   │   │   ├── support.md
    │   │   │   ├── system-backdrop-controller.md
    │   │   │   ├── system-requirements.md
    │   │   │   ├── tutorial-unpackaged-deployment.md
    │   │   │   ├── update-existing-projects-to-the-latest-release.md
    │   │   │   ├── use-windows-app-sdk-in-existing-project.md
    │   │   │   ├── use-windows-app-sdk-run-time.md
    │   │   │   ├── applifecycle/
    │   │   │   │   ├── applifecycle-instancing.md
    │   │   │   │   ├── applifecycle-power.md
    │   │   │   │   ├── applifecycle-restart.md
    │   │   │   │   ├── applifecycle-rich-activation.md
    │   │   │   │   ├── applifecycle-single-instance.md
    │   │   │   │   ├── applifecycle.md
    │   │   │   │   ├── background-tasks.md
    │   │   │   │   └── focus-session.md
    │   │   │   ├── includes/
    │   │   │   │   └── uwp-app-sdk-migration-pointer.md
    │   │   │   ├── migrate-to-windows-app-sdk/
    │   │   │   │   ├── api-mapping-table.md
    │   │   │   │   ├── case-study-1.md
    │   │   │   │   ├── case-study-2.md
    │   │   │   │   ├── feature-mapping-table.md
    │   │   │   │   ├── migrate-to-windows-app-sdk-ovw.md
    │   │   │   │   ├── misc-info.md
    │   │   │   │   ├── overall-migration-strategy.md
    │   │   │   │   ├── upgrade-assistant.md
    │   │   │   │   ├── what-is-supported.md
    │   │   │   │   ├── winforms-plus-winappsdk.md
    │   │   │   │   ├── wpf-plus-winappsdk.md
    │   │   │   │   └── guides/
    │   │   │   │       ├── applifecycle.md
    │   │   │   │       ├── background-task-migration-strategy.md
    │   │   │   │       ├── dwritecore.md
    │   │   │   │       ├── feature-area-guides-ovw.md
    │   │   │   │       ├── keyboard-events.md
    │   │   │   │       ├── mrtcore.md
    │   │   │   │       ├── notifications.md
    │   │   │   │       ├── threading.md
    │   │   │   │       ├── toast-notifications.md
    │   │   │   │       ├── windowing.md
    │   │   │   │       └── winui3.md
    │   │   │   ├── mrtcore/
    │   │   │   │   ├── images-tailored-for-scale-theme-contrast.md
    │   │   │   │   ├── localize-strings.md
    │   │   │   │   ├── mrtcore-overview.md
    │   │   │   │   ├── tailor-resources-lang-scale-contrast.md
    │   │   │   │   └── images/
    │   │   │   │       ├── add-quickstart-string.PNG
    │   │   │   │       ├── add-resw-file.PNG
    │   │   │   │       ├── add-resx-file.PNG
    │   │   │   │       ├── framework-update.PNG
    │   │   │   │       ├── framework.PNG
    │   │   │   │       └── new-winui-app.PNG
    │   │   │   ├── notifications/
    │   │   │   │   ├── app-notifications/
    │   │   │   │   │   ├── app-notifications-quickstart.md
    │   │   │   │   │   └── index.md
    │   │   │   │   └── push-notifications/
    │   │   │   │       ├── index.md
    │   │   │   │       ├── push-quickstart.md
    │   │   │   │       └── troubleshooting.md
    │   │   │   ├── release-notes-archive/
    │   │   │   │   ├── experimental-channel-0.8.md
    │   │   │   │   ├── experimental-channel-1.0.md
    │   │   │   │   ├── experimental-channel-1.2.md
    │   │   │   │   ├── experimental-channel-1.3.md
    │   │   │   │   ├── experimental-channel-1.4.md
    │   │   │   │   ├── experimental-channel-1.5.md
    │   │   │   │   ├── experimental-channel-1.6.md
    │   │   │   │   ├── experimental-channel-1.7.md
    │   │   │   │   ├── preview-channel-1.0.md
    │   │   │   │   ├── preview-channel-1.1.md
    │   │   │   │   ├── preview-channel-1.2.md
    │   │   │   │   ├── preview-channel-1.3.md
    │   │   │   │   ├── preview-channel-1.4.md
    │   │   │   │   ├── preview-channel-1.5.md
    │   │   │   │   ├── preview-channel-1.6.md
    │   │   │   │   ├── stable-channel-0.5.md
    │   │   │   │   ├── stable-channel-0.8.md
    │   │   │   │   ├── stable-channel-1.0.md
    │   │   │   │   ├── stable-channel-1.1.md
    │   │   │   │   ├── stable-channel-1.2.md
    │   │   │   │   ├── stable-channel-1.3.md
    │   │   │   │   ├── stable-channel-1.4.md
    │   │   │   │   ├── stable-channel-1.5.md
    │   │   │   │   └── stable-channel-1.6.md
    │   │   │   └── windowing/
    │   │   │       └── windowing-overview.md
    │   │   ├── windows-dotnet-maui/
    │   │   │   ├── index.md
    │   │   │   ├── tutorial-csharp-ui-maui-toolkit.md
    │   │   │   ├── tutorial-graph-api.md
    │   │   │   └── walkthrough-first-app.md
    │   │   └── winui/
    │   │       ├── index.md
    │   │       ├── winui2/
    │   │       │   └── license.md
    │   │       └── winui3/
    │   │           ├── create-your-first-winui3-app.md
    │   │           ├── desktop-winui3-app-with-basic-interop.md
    │   │           ├── index.md
    │   │           ├── localize-winui3-app.md
    │   │           ├── winui-project-templates-in-visual-studio.md
    │   │           ├── xaml-templated-controls-cppwinrt-winui-3.md
    │   │           ├── xaml-templated-controls-csharp-winui-3.md
    │   │           ├── images/
    │   │           │   ├── WinUI-cpp-appproject-1.0-later.PNG
    │   │           │   ├── WinUI-csharp-appproject-1.0-later.PNG
    │   │           │   ├── winui-items-csharp.PNG
    │   │           │   ├── winui-projects-csharp.PNG
    │   │           │   ├── WinUI3-cpp-newproject-1.0-later.PNG
    │   │           │   ├── WinUI3-csharp-newproject-1.0-later.PNG
    │   │           │   ├── WinUI3-csharp-newproject-1.0-later2.PNG
    │   │           │   └── WinUI3XamlControlsGalleryP3.PNG
    │   │           ├── release-notes/
    │   │           │   ├── release-notes-08-preview.md
    │   │           │   ├── winui3-project-reunion-0.5-preview.md
    │   │           │   └── winui3-project-reunion-0.5.md
    │   │           ├── samples/
    │   │           │   ├── window-titlebar/
    │   │           │   │   ├── window-titlebar.sln
    │   │           │   │   └── window-titlebar/
    │   │           │   │       ├── app.manifest
    │   │           │   │       ├── App.xaml
    │   │           │   │       ├── App.xaml.cs
    │   │           │   │       ├── MainWindow.xaml
    │   │           │   │       ├── MainWindow.xaml.cs
    │   │           │   │       ├── NativeMethods.txt
    │   │           │   │       ├── Package.appxmanifest
    │   │           │   │       ├── window-titlebar.csproj
    │   │           │   │       └── Properties/
    │   │           │   │           ├── launchSettings.json
    │   │           │   │           └── PublishProfiles/
    │   │           │   │               ├── win-arm64.pubxml
    │   │           │   │               ├── win-x64.pubxml
    │   │           │   │               └── win-x86.pubxml
    │   │           │   └── WinUI-3-basic-win32-interop/
    │   │           │       ├── WinUI-3-basic-win32-interop.sln
    │   │           │       └── WinUI-3-basic-win32-interop/
    │   │           │           ├── app.manifest
    │   │           │           ├── App.xaml
    │   │           │           ├── App.xaml.cs
    │   │           │           ├── MainWindow.xaml
    │   │           │           ├── MainWindow.xaml.cs
    │   │           │           ├── NativeMethods.txt
    │   │           │           ├── Package.appxmanifest
    │   │           │           ├── WinUI-3-basic-win32-interop.csproj
    │   │           │           └── Properties/
    │   │           │               ├── launchSettings.json
    │   │           │               └── PublishProfiles/
    │   │           │                   ├── win-arm64.pubxml
    │   │           │                   ├── win-x64.pubxml
    │   │           │                   └── win-x86.pubxml
    │   │           └── testing/
    │   │               ├── create-winui-unit-test-project.md
    │   │               └── index.md
    │   ├── breadcrumbs/
    │   │   └── toc.yml
    │   ├── cross-device/
    │   │   └── phonelink/
    │   │       ├── index.md
    │   │       └── toc.yml
    │   ├── dev-drive/
    │   │   ├── group-policy.md
    │   │   └── index.md
    │   ├── dev-environment/
    │   │   ├── dev-environment-context.yml
    │   │   ├── index.md
    │   │   ├── mac-to-windows.md
    │   │   ├── toc.yml
    │   │   ├── docker/
    │   │   │   └── overview.md
    │   │   ├── javascript/
    │   │   │   ├── gatsby-on-wsl.md
    │   │   │   ├── index.md
    │   │   │   ├── nextjs-on-wsl.md
    │   │   │   ├── nodejs-beginners-tutorial.md
    │   │   │   ├── nodejs-on-windows.md
    │   │   │   ├── nodejs-on-wsl.md
    │   │   │   ├── nodejs-overview.md
    │   │   │   ├── nuxtjs-on-wsl.md
    │   │   │   ├── react-beginners-tutorial.md
    │   │   │   ├── react-native-for-android.md
    │   │   │   ├── react-native-for-windows.md
    │   │   │   ├── react-on-windows.md
    │   │   │   ├── react-on-wsl.md
    │   │   │   ├── react-overview.md
    │   │   │   ├── vue-beginners-tutorial.md
    │   │   │   ├── vue-on-windows.md
    │   │   │   ├── vue-on-wsl.md
    │   │   │   └── vue-overview.md
    │   │   └── rust/
    │   │       ├── index.yml
    │   │       ├── overview.md
    │   │       ├── rss-reader-rust-for-windows.md
    │   │       ├── rust-for-windows.md
    │   │       └── setup.md
    │   ├── dev-home/
    │   │   ├── environments.md
    │   │   ├── extensions.md
    │   │   ├── index.md
    │   │   ├── setup.md
    │   │   ├── utilities.md
    │   │   └── windows-customization.md
    │   ├── includes/
    │   │   ├── install-and-run-mongo.md
    │   │   ├── install-and-run-postgres.md
    │   │   ├── install-powertoys.md
    │   │   ├── muxc-alias-note.md
    │   │   ├── postgres-v-mongo.md
    │   │   ├── profile-aliases.md
    │   │   ├── uno-setup.md
    │   │   ├── uwp-winui-2-note.md
    │   │   ├── winui-2-gallery.md
    │   │   └── winui-3-gallery.md
    │   ├── package-manager/
    │   │   ├── index.md
    │   │   ├── configuration/
    │   │   │   ├── check.md
    │   │   │   ├── create.md
    │   │   │   └── index.md
    │   │   ├── package/
    │   │   │   ├── index.md
    │   │   │   ├── manifest.md
    │   │   │   ├── repository.md
    │   │   │   └── windows-package-manager-policies.md
    │   │   └── winget/
    │   │       ├── configure.md
    │   │       ├── download.md
    │   │       ├── export.md
    │   │       ├── features.md
    │   │       ├── hash.md
    │   │       ├── help.md
    │   │       ├── import.md
    │   │       ├── index.md
    │   │       ├── info.md
    │   │       ├── install.md
    │   │       ├── list.md
    │   │       ├── pinning.md
    │   │       ├── search.md
    │   │       ├── settings.md
    │   │       ├── show.md
    │   │       ├── source.md
    │   │       ├── tab-completion.md
    │   │       ├── troubleshooting.md
    │   │       ├── uninstall.md
    │   │       ├── upgrade.md
    │   │       └── validate.md
    │   ├── powertoys/
    │   │   ├── administrator.md
    │   │   ├── advanced-paste.md
    │   │   ├── always-on-top.md
    │   │   ├── awake.md
    │   │   ├── cmd-not-found.md
    │   │   ├── color-picker.md
    │   │   ├── crop-and-lock.md
    │   │   ├── dsc-configure.md
    │   │   ├── environment-variables.md
    │   │   ├── fancyzones.md
    │   │   ├── file-explorer.md
    │   │   ├── file-locksmith.md
    │   │   ├── general.md
    │   │   ├── grouppolicy.md
    │   │   ├── hosts-file-editor.md
    │   │   ├── image-resizer.md
    │   │   ├── index.md
    │   │   ├── install.md
    │   │   ├── keyboard-manager.md
    │   │   ├── mouse-utilities.md
    │   │   ├── mouse-without-borders.md
    │   │   ├── newplus.md
    │   │   ├── peek.md
    │   │   ├── powerrename.md
    │   │   ├── quick-accent.md
    │   │   ├── registry-preview.md
    │   │   ├── run.md
    │   │   ├── screen-ruler.md
    │   │   ├── shortcut-guide.md
    │   │   ├── text-extractor.md
    │   │   ├── video-conference-mute.md
    │   │   ├── workspaces.md
    │   │   ├── zoomit.md
    │   │   └── command-palette/
    │   │       ├── add-top-level-commands-to-your-extension.md
    │   │       ├── adding-commands.md
    │   │       ├── command-results.md
    │   │       ├── creating-an-extension.md
    │   │       ├── extensibility-overview.md
    │   │       ├── overview.md
    │   │       ├── publish-extension.md
    │   │       ├── samples.md
    │   │       ├── sdk-namespaces.md
    │   │       ├── update-a-list-of-commands.md
    │   │       ├── using-form-pages.md
    │   │       ├── using-markdown-content.md
    │   │       ├── microsoft-commandpalette-extensions/
    │   │       │   ├── color.md
    │   │       │   ├── commandresultkind.md
    │   │       │   ├── icommand.md
    │   │       │   ├── icommandcontextitem.md
    │   │       │   ├── icommanditem.md
    │   │       │   ├── icommandprovider.md
    │   │       │   ├── icommandprovider_fallbackcommands.md
    │   │       │   ├── icommandprovider_getcommand.md
    │   │       │   ├── icommandprovider_initializewithhost.md
    │   │       │   ├── icommandprovider_toplevelcommands.md
    │   │       │   ├── icommandresult.md
    │   │       │   ├── icommandresultargs.md
    │   │       │   ├── icommandsettings.md
    │   │       │   ├── iconfirmationargs.md
    │   │       │   ├── icontent.md
    │   │       │   ├── icontentpage.md
    │   │       │   ├── icontentpage_getcontent.md
    │   │       │   ├── icontextitem.md
    │   │       │   ├── idetails.md
    │   │       │   ├── idetailscommand.md
    │   │       │   ├── idetailsdata.md
    │   │       │   ├── idetailselement.md
    │   │       │   ├── idetailslink.md
    │   │       │   ├── idetailsseparator.md
    │   │       │   ├── idetailstags.md
    │   │       │   ├── idynamiclistpage.md
    │   │       │   ├── iextension.md
    │   │       │   ├── iextension_dispose.md
    │   │       │   ├── iextension_getprovider.md
    │   │       │   ├── iextensionhost.md
    │   │       │   ├── iextensionhost_hidestatus.md
    │   │       │   ├── iextensionhost_logmessage.md
    │   │       │   ├── iextensionhost_showstatus.md
    │   │       │   ├── ifallbackcommanditem.md
    │   │       │   ├── ifallbackhandler.md
    │   │       │   ├── ifallbackhandler_updatequery.md
    │   │       │   ├── ifilter.md
    │   │       │   ├── ifilteritem.md
    │   │       │   ├── ifilters.md
    │   │       │   ├── ifilters_filters.md
    │   │       │   ├── iform.md
    │   │       │   ├── iform_datajson.md
    │   │       │   ├── iform_statejson.md
    │   │       │   ├── iform_submitform.md
    │   │       │   ├── iform_templatejson.md
    │   │       │   ├── iformcontent.md
    │   │       │   ├── iformcontent_submitform.md
    │   │       │   ├── iformpage.md
    │   │       │   ├── iformpage_forms.md
    │   │       │   ├── igotopageargs.md
    │   │       │   ├── igridproperties.md
    │   │       │   ├── iicondata.md
    │   │       │   ├── iiconinfo.md
    │   │       │   ├── iinvokablecommand.md
    │   │       │   ├── iinvokablecommand_invoke.md
    │   │       │   ├── iitemschangedeventargs.md
    │   │       │   ├── ilistitem.md
    │   │       │   ├── ilistpage.md
    │   │       │   ├── ilistpage_getitems.md
    │   │       │   ├── ilistpage_loadmore.md
    │   │       │   ├── ilogmessage.md
    │   │       │   ├── imarkdowncontent.md
    │   │       │   ├── imarkdownpage.md
    │   │       │   ├── imarkdownpage_bodies.md
    │   │       │   ├── imarkdownpage_details.md
    │   │       │   ├── inotifyitemschanged.md
    │   │       │   ├── inotifypropchanged.md
    │   │       │   ├── ipage.md
    │   │       │   ├── iprogressstate.md
    │   │       │   ├── ipropchangedeventargs.md
    │   │       │   ├── iseparatorcontextitem.md
    │   │       │   ├── iseparatorfilteritem.md
    │   │       │   ├── istatusmessage.md
    │   │       │   ├── itag.md
    │   │       │   ├── itoastargs.md
    │   │       │   ├── itreecontent.md
    │   │       │   ├── itreecontent_getchildren.md
    │   │       │   ├── keychord.md
    │   │       │   ├── messagestate.md
    │   │       │   ├── microsoft-commandpalette-extensions.md
    │   │       │   ├── navigationmode.md
    │   │       │   ├── optionalcolor.md
    │   │       │   └── providertype.md
    │   │       └── microsoft-commandpalette-extensions-toolkit/
    │   │           ├── anonymouscommand.md
    │   │           ├── anonymouscommand_constructor.md
    │   │           ├── anonymouscommand_invoke.md
    │   │           ├── baseobservable.md
    │   │           ├── baseobservable_onpropertychanged.md
    │   │           ├── choice.md
    │   │           ├── choicesetsetting.md
    │   │           ├── choicesetsetting_constructor.md
    │   │           ├── choicesetsetting_loadfromjson.md
    │   │           ├── choicesetsetting_todictionary.md
    │   │           ├── choicesetsetting_tostate.md
    │   │           ├── choicesetsetting_update.md
    │   │           ├── clipboardhelper.md
    │   │           ├── clipboardhelper_gettext.md
    │   │           ├── clipboardhelper_setrtf.md
    │   │           ├── clipboardhelper_settext.md
    │   │           ├── colorhelpers.md
    │   │           ├── colorhelpers_fromargb.md
    │   │           ├── colorhelpers_fromrgb.md
    │   │           ├── colorhelpers_nocolor.md
    │   │           ├── colorhelpers_transparent.md
    │   │           ├── command.md
    │   │           ├── commandcontextitem.md
    │   │           ├── commandcontextitem_constructor.md
    │   │           ├── commanditem.md
    │   │           ├── commanditem_constructor.md
    │   │           ├── commandprovider.md
    │   │           ├── commandprovider_dispose.md
    │   │           ├── commandprovider_fallbackcommands.md
    │   │           ├── commandprovider_getcommand.md
    │   │           ├── commandprovider_initializewithhost.md
    │   │           ├── commandprovider_raiseitemschanged.md
    │   │           ├── commandprovider_toplevelcommands.md
    │   │           ├── commandresult.md
    │   │           ├── commandresult_confirm.md
    │   │           ├── commandresult_dismiss.md
    │   │           ├── commandresult_goback.md
    │   │           ├── commandresult_gohome.md
    │   │           ├── commandresult_gotopage.md
    │   │           ├── commandresult_hide.md
    │   │           ├── commandresult_keepopen.md
    │   │           ├── commandresult_showtoast_string.md
    │   │           ├── commandresult_showtoast_toastargs.md
    │   │           ├── confirmationargs.md
    │   │           ├── contentpage.md
    │   │           ├── contentpage_getcontent.md
    │   │           ├── contentpage_raiseitemschanged.md
    │   │           ├── copytextcommand.md
    │   │           ├── copytextcommand_constructor.md
    │   │           ├── copytextcommand_invoke.md
    │   │           ├── details.md
    │   │           ├── detailscommand.md
    │   │           ├── detailselement.md
    │   │           ├── detailslink.md
    │   │           ├── detailslink_constructor.md
    │   │           ├── detailsseparator.md
    │   │           ├── detailstags.md
    │   │           ├── dynamiclistpage.md
    │   │           ├── dynamiclistpage_updatesearchtext.md
    │   │           ├── extensionhost.md
    │   │           ├── extensionhost_hidestatus.md
    │   │           ├── extensionhost_initialize.md
    │   │           ├── extensionhost_logmessage_ilogmessage.md
    │   │           ├── extensionhost_logmessage_string.md
    │   │           ├── extensionhost_showstatus.md
    │   │           ├── fallbackcommanditem.md
    │   │           ├── fallbackcommanditem_constructor.md
    │   │           ├── fallbackcommanditem_updatequery.md
    │   │           ├── filter.md
    │   │           ├── formcontent.md
    │   │           ├── formcontent_submitform_string.md
    │   │           ├── formcontent_submitform_stringstring.md
    │   │           ├── gotopageargs.md
    │   │           ├── icondata.md
    │   │           ├── icondata_constructor.md
    │   │           ├── iconhelpers.md
    │   │           ├── iconhelpers_fromrelativepath.md
    │   │           ├── iconhelpers_fromrelativepaths.md
    │   │           ├── iconinfo.md
    │   │           ├── iconinfo_constructor.md
    │   │           ├── invokablecommand.md
    │   │           ├── invokablecommand_invoke.md
    │   │           ├── invokablecommand_invoke_object.md
    │   │           ├── isettingsform.md
    │   │           ├── isettingsform_todataidentifier.md
    │   │           ├── isettingsform_todictionary.md
    │   │           ├── isettingsform_toform.md
    │   │           ├── isettingsform_tostate.md
    │   │           ├── isettingsform_update.md
    │   │           ├── itemschangedeventargs.md
    │   │           ├── itemschangedeventargs_constructor.md
    │   │           ├── jsonsettingsmanager.md
    │   │           ├── jsonsettingsmanager_loadsettings.md
    │   │           ├── jsonsettingsmanager_savesettings.md
    │   │           ├── keychordhelpers.md
    │   │           ├── keychordhelpers_frommodifiers.md
    │   │           ├── listhelpers.md
    │   │           ├── listhelpers_filterlist.md
    │   │           ├── listhelpers_filterlist_t.md
    │   │           ├── listhelpers_inplaceupdatelist.md
    │   │           ├── listhelpers_scored.md
    │   │           ├── listhelpers_scoredlistitem.md
    │   │           ├── listhelpers_scorelistitem.md
    │   │           ├── listitem.md
    │   │           ├── listitem_constructor.md
    │   │           ├── listpage.md
    │   │           ├── listpage_getitems.md
    │   │           ├── listpage_loadmore.md
    │   │           ├── listpage_raiseitemschanged.md
    │   │           ├── logmessage.md
    │   │           ├── logmessage_constructor.md
    │   │           ├── markdowncontent.md
    │   │           ├── matchoption.md
    │   │           ├── matchresult.md
    │   │           ├── matchresult_constructor.md
    │   │           ├── matchresult_issearchprecisionscoremet.md
    │   │           ├── microsoft-commandpalette-extensions-toolkit.md
    │   │           ├── noopcommand.md
    │   │           ├── noopcommand_invoke.md
    │   │           ├── openurlcommand.md
    │   │           ├── openurlcommand_constructor.md
    │   │           ├── openurlcommand_invoke.md
    │   │           ├── page.md
    │   │           ├── progressstate.md
    │   │           ├── propchangedeventargs.md
    │   │           ├── propchangedeventargs_constructor.md
    │   │           ├── searchprecisionscore.md
    │   │           ├── setting.md
    │   │           ├── setting_constructor.md
    │   │           ├── setting_todataidentifier.md
    │   │           ├── setting_todictionary.md
    │   │           ├── setting_toform.md
    │   │           ├── setting_tostate.md
    │   │           ├── setting_update.md
    │   │           ├── settings.md
    │   │           ├── settings_add.md
    │   │           ├── settings_getsetting.md
    │   │           ├── settings_tocontent.md
    │   │           ├── settings_tojson.md
    │   │           ├── settings_trygetsetting.md
    │   │           ├── settings_update.md
    │   │           ├── settingsform.md
    │   │           ├── settingsform_submitform.md
    │   │           ├── shellhelpers.md
    │   │           ├── shellhelpers_opencommandinshell.md
    │   │           ├── shellhelpers_openinshell.md
    │   │           ├── shellrunastype.md
    │   │           ├── statusmessage.md
    │   │           ├── stringmatcher.md
    │   │           ├── stringmatcher_constructor.md
    │   │           ├── stringmatcher_fuzzymatch_stringstring.md
    │   │           ├── stringmatcher_fuzzymatch_stringstringmatchoption.md
    │   │           ├── stringmatcher_fuzzysearch.md
    │   │           ├── tag.md
    │   │           ├── tag_constructor.md
    │   │           ├── textsetting.md
    │   │           ├── textsetting_constructor.md
    │   │           ├── textsetting_loadfromjson.md
    │   │           ├── textsetting_todictionary.md
    │   │           ├── textsetting_tostate.md
    │   │           ├── textsetting_update.md
    │   │           ├── thumbnailhelper.md
    │   │           ├── thumbnailhelper_getthumbnail.md
    │   │           ├── toastargs.md
    │   │           ├── toaststatusmessage.md
    │   │           ├── toaststatusmessage_constructor.md
    │   │           ├── toaststatusmessage_show.md
    │   │           ├── togglesetting.md
    │   │           ├── togglesetting_constructor.md
    │   │           ├── togglesetting_loadfromjson.md
    │   │           ├── togglesetting_todictionary.md
    │   │           ├── togglesetting_tostate.md
    │   │           ├── togglesetting_update.md
    │   │           ├── treecontent.md
    │   │           ├── treecontent_getchildren.md
    │   │           ├── treecontent_raiseitemschanged.md
    │   │           ├── utilities.md
    │   │           ├── utilities_basesettingspath.md
    │   │           └── utilities_ispackaged.md
    │   ├── python/
    │   │   ├── beginners.md
    │   │   ├── faqs.yml
    │   │   ├── index.yml
    │   │   ├── scripting.md
    │   │   └── web-frameworks.md
    │   └── web/
    │       ├── apis.md
    │       ├── index.md
    │       └── toc.yml
    ├── landing/
    │   └── arm-docs/
    │       ├── add-arm-support.md
    │       ├── apps-on-arm-program-compat-troubleshooter.md
    │       ├── apps-on-arm-troubleshooting-arm32.md
    │       ├── apps-on-arm-troubleshooting-x86.md
    │       ├── apps-on-arm-x86-emulation.md
    │       ├── arm32-to-arm64.md
    │       ├── arm64ec-abi.md
    │       ├── arm64ec-build.md
    │       ├── arm64ec.md
    │       ├── arm64x-build.md
    │       ├── arm64x-pe.md
    │       ├── create-arm-vm.md
    │       ├── docfx.json
    │       ├── faq.yml
    │       ├── iso.md
    │       ├── overview.md
    │       ├── toc.yml
    │       ├── breadcrumb/
    │       │   └── toc.yml
    │       ├── dev-kit/
    │       │   ├── history.md
    │       │   └── index.md
    │       └── images/
    │           ├── Capture.PNG
    │           ├── Capture2.PNG
    │           ├── Capture3.PNG
    │           ├── Capture4.PNG
    │           ├── Capture5.PNG
    │           └── create-arm-vm/
    │               └── .gitignore
    ├── uwp/
    │   ├── bx3iqq53.3rb.json
    │   ├── docfx.json
    │   ├── index.yml
    │   ├── toc.yml
    │   ├── app-resources/
    │   │   ├── build-resources-into-app-package.md
    │   │   ├── compile-resources-manually-with-makepri.md
    │   │   ├── how-rms-matches-and-chooses-resources.md
    │   │   ├── how-rms-matches-lang-tags.md
    │   │   ├── images-tailored-for-scale-theme-contrast.md
    │   │   ├── index.md
    │   │   ├── localize-strings-ui-manifest.md
    │   │   ├── makepri-exe-command-options.md
    │   │   ├── makepri-exe-configuration.md
    │   │   ├── makepri-exe-format-specific-indexers.md
    │   │   ├── pri-apis-custom-build-systems.md
    │   │   ├── pri-apis-scenario-1.md
    │   │   ├── resource-management-system.md
    │   │   ├── specify-default-resources-installed.md
    │   │   ├── tailor-resources-lang-scale-contrast.md
    │   │   ├── uri-schemes.md
    │   │   ├── using-mrt-for-converted-desktop-apps-and-games.md
    │   │   └── images/
    │   │       ├── language_matching_1.vsdx
    │   │       ├── language_matching_1.xml
    │   │       ├── language_matching_2.vsdx
    │   │       └── language_matching_2.xml
    │   ├── app-to-app/
    │   │   ├── copy-and-paste.md
    │   │   ├── index.md
    │   │   ├── receive-data.md
    │   │   ├── share-data.md
    │   │   └── code/
    │   │       ├── dev_app_to_app.sln
    │   │       ├── copy_paste/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── copy_paste.csproj
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── Properties/
    │   │       │       │   ├── AssemblyInfo.cs
    │   │       │       │   └── Default.rd.xml
    │   │       │       └── Service References/
    │   │       │           └── Application Insights/
    │   │       │               └── ConnectedService.json
    │   │       ├── drag_drop/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── drag_drop.csproj
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── Properties/
    │   │       │       │   ├── AssemblyInfo.cs
    │   │       │       │   └── Default.rd.xml
    │   │       │       └── Service References/
    │   │       │           └── Application Insights/
    │   │       │               └── ConnectedService.json
    │   │       ├── receive_data/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── receive_data.csproj
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       └── share_data/
    │   │           └── cs/
    │   │               ├── App.xaml
    │   │               ├── App.xaml.cs
    │   │               ├── MainPage.xaml
    │   │               ├── MainPage.xaml.cs
    │   │               ├── Package.appxmanifest
    │   │               ├── share_data.csproj
    │   │               ├── ShareData.csproj
    │   │               ├── Properties/
    │   │               │   ├── AssemblyInfo.cs
    │   │               │   └── Default.rd.xml
    │   │               └── Service References/
    │   │                   └── Application Insights/
    │   │                       └── ConnectedService.json
    │   ├── apps-for-education/
    │   │   ├── index.md
    │   │   ├── take-a-test-api.md
    │   │   └── troubleshooting.md
    │   ├── apps-for-xbox/
    │   │   ├── application-architecture.md
    │   │   ├── development-options.md
    │   │   ├── partner-center-xbox.md
    │   │   └── supported-technologies.md
    │   ├── audio-video-camera/
    │   │   ├── adaptive-streaming-with-playready.md
    │   │   ├── adaptive-streaming.md
    │   │   ├── audio-device-information-properties.md
    │   │   ├── audio-graphs.md
    │   │   ├── background-audio.md
    │   │   ├── bitmapencoder-options-reference.md
    │   │   ├── camera-independent-flashlight.md
    │   │   ├── camera-privacy-setting.md
    │   │   ├── camera-ui-features-for-mobile-devices.md
    │   │   ├── camera.md
    │   │   ├── capture-photos-and-video-with-cameracaptureui.md
    │   │   ├── codec-query.md
    │   │   ├── create-schedule-and-manage-media-breaks.md
    │   │   ├── custom-audio-effects.md
    │   │   ├── custom-video-effects.md
    │   │   ├── dash-profile-support.md
    │   │   ├── detect-and-respond-to-audio-state-changes.md
    │   │   ├── detect-and-track-faces-in-an-image.md
    │   │   ├── enable-remote-audio-playback.md
    │   │   ├── get-a-preview-frame.md
    │   │   ├── handle-device-orientation-with-mediacapture.md
    │   │   ├── hardware-drm.md
    │   │   ├── hevc-xbox.md
    │   │   ├── hls-tag-support.md
    │   │   ├── image-metadata.md
    │   │   ├── imaging.md
    │   │   ├── import-media-from-a-device.md
    │   │   ├── index.md
    │   │   ├── integrate-with-systemmediatransportcontrols.md
    │   │   ├── legacy-background-media-playback.md
    │   │   ├── media-casting.md
    │   │   ├── media-compositions-and-editing.md
    │   │   ├── media-playback-with-mediasource.md
    │   │   ├── media-playback.md
    │   │   ├── midi.md
    │   │   ├── play-audio-and-video-with-mediaplayer.md
    │   │   ├── playready-client-sdk.md
    │   │   ├── playready-encrypted-media-extension.md
    │   │   ├── process-bitmaps-low-light-fusion.md
    │   │   ├── process-media-files-in-the-background.md
    │   │   ├── process-software-bitmaps-with-opencv.md
    │   │   ├── screen-capture-video.md
    │   │   ├── screen-capture.md
    │   │   ├── simple-camera-preview-access.md
    │   │   ├── supported-codecs.md
    │   │   ├── supported-play-type-strings.md
    │   │   ├── system-media-transport-controls.md
    │   │   ├── system-supported-metadata-cues.md
    │   │   ├── transcode-media-files.md
    │   │   ├── use-opencv-with-mediaframereader.md
    │   │   └── code/
    │   │       ├── AdaptiveStreaming_RS1/
    │   │       │   └── cs/
    │   │       │       ├── AdaptiveStreaming_RS1.csproj
    │   │       │       ├── AdaptiveStreaming_RS1_TemporaryKey.pfx
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── AdaptiveStreaming_Win10/
    │   │       │   └── cs/
    │   │       │       ├── AdaptiveStreaming_Win10.csproj
    │   │       │       ├── AdaptiveStreaming_Win10_TemporaryKey.pfx
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── AudioGraph/
    │   │       │   ├── AudioEffectComponent/
    │   │       │   │   ├── AudioEffectComponent.csproj
    │   │       │   │   ├── ExampleAudioEffect.cs
    │   │       │   │   └── Properties/
    │   │       │   │       └── AssemblyInfo.cs
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── AudioGraphSnippets.csproj
    │   │       │       ├── AudioGraphSnippets.sln
    │   │       │       ├── AudioGraphSnippets_TemporaryKey.pfx
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── BackgroundAudio_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── BackgroundAudio_RS1.csproj
    │   │       │       ├── BackgroundAudio_RS1_TemporaryKey.pfx
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── BasicMediaCaptureWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── BasicCameraWin10.csproj
    │   │       │       ├── BasicCameraWin10_TemporaryKey.pfx
    │   │       │       ├── CameraRotationHelper.cs
    │   │       │       ├── MainPage.ManualControls.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       ├── StreamPropertiesHelper.cs
    │   │       │       ├── properties/
    │   │       │       │   ├── AssemblyInfo.cs
    │   │       │       │   └── Default.rd.xml
    │   │       │       └── Service References/
    │   │       │           └── Application Insights/
    │   │       │               └── ConnectedService.json
    │   │       ├── FaceDetection_Win10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── FaceDetection_Win10.csproj
    │   │       │       ├── FaceDetection_Win10_TemporaryKey.pfx
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── Frames_Win10/
    │   │       │   ├── Frames_Win10.sln
    │   │       │   └── Frames_Win10/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── FrameRenderer.cs
    │   │       │       ├── Frames_Win10.csproj
    │   │       │       ├── Frames_Win10_TemporaryKey.pfx
    │   │       │       ├── MainPage.OpenCV.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── RemoteCameraPairingHelper.cs
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── ImagingWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── ImagingWin10.csproj
    │   │       │       ├── ImagingWin10.sln
    │   │       │       ├── ImagingWin10_TemporaryKey.pfx
    │   │       │       ├── MainPage.OpenCV.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── OpenCVBridge/
    │   │       │       │   ├── OpenCVBridge.vcxproj
    │   │       │       │   ├── OpenCVBridge.vcxproj.filters
    │   │       │       │   ├── OpenCVHelper.cpp
    │   │       │       │   ├── OpenCVHelper.h
    │   │       │       │   ├── pch.cpp
    │   │       │       │   └── pch.h
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── Lamp/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── LampSnippets.csproj
    │   │       │       ├── LampSnippets_TemporaryKey.pfx
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── LowLightFusionSample/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── LowLightFusionSample.csproj
    │   │       │       ├── LowLightFusionSample_TemporaryKey.pfx
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaBreaks_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaBreaks_RS1.csproj
    │   │       │       ├── MediaBreaks_RS1_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaCasting_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaCasting_RS1.csproj
    │   │       │       ├── MediaCasting_RS1_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaCastingWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaCastingWin10.csproj
    │   │       │       ├── MediaCastingWin10_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaEditing/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaEditingSnippets.csproj
    │   │       │       ├── MediaEditingSnippets.sln
    │   │       │       ├── MediaEditingSnippets_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaPlayer_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaPlayer_Win10.csproj
    │   │       │       ├── MediaPlayer_Win10_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── Assets/
    │   │       │       │   ├── example_video.mkv
    │   │       │       │   └── example_video_2.mkv
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaProcessingTriggerWin10/
    │   │       │   └── cs/
    │   │       │       ├── MediaProcessingTriggerWin10.sln
    │   │       │       ├── MediaProcessingBackgroundTask/
    │   │       │       │   ├── MediaProcessingBackgroundTask.csproj
    │   │       │       │   ├── MediaProcessingTask.cs
    │   │       │       │   ├── project.json
    │   │       │       │   └── Properties/
    │   │       │       │       └── AssemblyInfo.cs
    │   │       │       └── MediaProcessingTriggerWin10/
    │   │       │           ├── App.xaml
    │   │       │           ├── App.xaml.cs
    │   │       │           ├── ApplicationInsights.config
    │   │       │           ├── MainPage.xaml
    │   │       │           ├── MainPage.xaml.cs
    │   │       │           ├── MediaProcessingTriggerWin10.csproj
    │   │       │           ├── MediaProcessingTriggerWin10_TemporaryKey.pfx
    │   │       │           ├── Package.appxmanifest
    │   │       │           ├── project.json
    │   │       │           └── Properties/
    │   │       │               ├── AssemblyInfo.cs
    │   │       │               └── Default.rd.xml
    │   │       ├── MediaSource_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MainPage_Cues.xaml.cs
    │   │       │       ├── MediaSource_RS1.csproj
    │   │       │       ├── MediaSource_RS1_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MediaSource_Win10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MediaSource_Win10.csproj
    │   │       │       ├── MediaSource_Win10_TemporaryKey.pfx
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── MIDIWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── MIDIWin10.csproj
    │   │       │       ├── MIDIWin10_TemporaryKey.pfx
    │   │       │       ├── MyMidiDeviceWatcher.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── PhotoImport_Win10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── GeneratorIncrementalLoadingClass.cs
    │   │       │       ├── ImportableItemWrapper.cs
    │   │       │       ├── IncrementalLoadingBase.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── PhotoImport_Win10.csproj
    │   │       │       ├── PhotoImport_Win10_TemporaryKey.pfx
    │   │       │       ├── project.json
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── ScreenCaptureWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── ApplicationInsights.config
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       ├── ScreenCaptureWin10.csproj
    │   │       │       ├── ScreenCaptureWin10_TemporaryKey.pfx
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── SimpleCameraPreview_Win10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── CameraRotationHelper.cs
    │   │       │       ├── MainPage.Effects.xaml.cs
    │   │       │       ├── MainPage.ManualControls.xaml.cs
    │   │       │       ├── MainPage.MultiRecord.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── SimpleCameraPreview_Win10.csproj
    │   │       │       ├── SimpleCameraPreview_Win10_TemporaryKey.pfx
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── SMTC_RS1/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── project.json
    │   │       │       ├── SMTC_RS1.csproj
    │   │       │       ├── SMTC_RS1_TemporaryKey.pfx
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── SMTCWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── SMTC_Win10.csproj
    │   │       │       ├── SMTC_Win10_TemporaryKey.pfx
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       ├── TranscodeWin10/
    │   │       │   └── cs/
    │   │       │       ├── App.xaml
    │   │       │       ├── App.xaml.cs
    │   │       │       ├── MainPage.xaml
    │   │       │       ├── MainPage.xaml.cs
    │   │       │       ├── Package.appxmanifest
    │   │       │       ├── TranscodeWin10.csproj
    │   │       │       ├── TranscodeWin10_TemporaryKey.pfx
    │   │       │       └── Properties/
    │   │       │           ├── AssemblyInfo.cs
    │   │       │           └── Default.rd.xml
    │   │       └── VideoEffect_Win10/
    │   │           └── cs/
    │   │               ├── VideoEffect_Win10.sln
    │   │               ├── VideoEffect_Win10/
    │   │               │   ├── App.xaml
    │   │               │   ├── App.xaml.cs
    │   │               │   ├── ApplicationInsights.config
    │   │               │   ├── MainPage.xaml
    │   │               │   ├── MainPage.xaml.cs
    │   │               │   ├── Package.appxmanifest
    │   │               │   ├── project.json
    │   │               │   ├── StreamPropertiesHelper.cs
    │   │               │   ├── VideoEffect_Win10.csproj
    │   │               │   ├── VideoEffect_Win10_TemporaryKey.pfx
    │   │               │   └── Properties/
    │   │               │       ├── AssemblyInfo.cs
    │   │               │       └── Default.rd.xml
    │   │               └── VideoEffectComponent/
    │   │                   ├── ExampleVideoEffect.cs
    │   │                   ├── ExampleVideoEffectWin2D.cs
    │   │                   ├── project.json
    │   │                   ├── VideoEffectComponent.csproj
    │   │                   └── Properties/
    │   │                       └── AssemblyInfo.cs
    │   ├── breadcrumbs/
    │   │   └── toc.yml
    │   ├── communication/
    │   │   ├── interprocess-communication.md
    │   │   └── sharing-named-objects.md
    │   ├── composition/
    │   │   ├── composition-animation.md
    │   │   ├── composition-brushes.md
    │   │   ├── composition-effects.md
    │   │   ├── composition-lighting.md
    │   │   ├── composition-native-interop.md
    │   │   ├── composition-shadows.md
    │   │   ├── composition-tailoring.md
    │   │   ├── composition-visual-tree.md
    │   │   ├── inertia-modifiers.md
    │   │   ├── input-driven-animations.md
    │   │   ├── interaction-tracker-manipulations.md
    │   │   ├── natural-animations.md
    │   │   ├── pointer-input-animations.md
    │   │   ├── relation-animations.md
    │   │   ├── scroll-input-animations.md
    │   │   ├── source-modifiers.md
    │   │   ├── spring-animations.md
    │   │   ├── time-animations.md
    │   │   ├── using-the-visual-layer-with-xaml.md
    │   │   ├── visual-layer.md
    │   │   └── xaml-lighting.md
    │   ├── contacts-and-calendar/
    │   │   ├── index.md
    │   │   ├── integrating-with-contacts.md
    │   │   ├── managing-appointments.md
    │   │   ├── my-people-notifications.md
    │   │   ├── my-people-sharing.md
    │   │   ├── my-people-support.md
    │   │   ├── selecting-contacts.md
    │   │   ├── sending-an-sms-message.md
    │   │   ├── sending-email.md
    │   │   └── images/
    │   │       ├── mini-contact-card.PNG
    │   │       └── screen-shots.vsdx
    │   ├── cpp-and-winrt-apis/
    │   │   ├── agile-objects.md
    │   │   ├── author-apis.md
    │   │   ├── author-coclasses.md
    │   │   ├── author-events.md
    │   │   ├── base-type.md
    │   │   ├── binding-collection.md
    │   │   ├── binding-property.md
    │   │   ├── boxing.md
    │   │   ├── clipboard-to-winrt-from-csharp.md
    │   │   ├── collections.md
    │   │   ├── concurrency-2.md
    │   │   ├── concurrency-3.md
    │   │   ├── concurrency.md
    │   │   ├── consume-apis.md
    │   │   ├── consume-com.md
    │   │   ├── cpp-value-categories.md
    │   │   ├── details-about-destructors.md
    │   │   ├── diag-direct-alloc.md
    │   │   ├── error-handling.md
    │   │   ├── faq.yml
    │   │   ├── get-started.md
    │   │   ├── handle-events.md
    │   │   ├── index.md
    │   │   ├── interop-winrt-abi.md
    │   │   ├── interop-winrt-cx-async.md
    │   │   ├── interop-winrt-cx.md
    │   │   ├── intro-to-using-cpp-with-winrt.md
    │   │   ├── macros.md
    │   │   ├── move-to-winrt-from-csharp.md
    │   │   ├── move-to-winrt-from-cx.md
    │   │   ├── move-to-winrt-from-wrl.md
    │   │   ├── naming.md
    │   │   ├── natvis.md
    │   │   ├── news.md
    │   │   ├── pass-parms-to-abi.md
    │   │   ├── photo-editor-sample.md
    │   │   ├── simple-winui-example.md
    │   │   ├── std-cpp-data-types.md
    │   │   ├── strings.md
    │   │   ├── troubleshooting.md
    │   │   ├── use-csharp-component-from-cpp-winrt.md
    │   │   ├── weak-references.md
    │   │   └── xaml-cust-ctrl.md
    │   ├── data-access/
    │   │   ├── index.md
    │   │   ├── sql-server-databases.md
    │   │   └── sqlite-databases.md
    │   ├── data-binding/
    │   │   ├── data-binding-and-mvvm.md
    │   │   ├── data-binding-in-depth.md
    │   │   ├── data-binding-quickstart.md
    │   │   ├── displaying-data-in-the-designer.md
    │   │   ├── function-bindings.md
    │   │   ├── how-to-bind-to-hierarchical-data-and-create-a-master-details-view.md
    │   │   ├── index.md
    │   │   └── xaml-basics-data-binding.md
    │   ├── debug-test-perf/
    │   │   ├── app-analysis.md
    │   │   ├── best-practices-for-your-app-s-startup-performance.md
    │   │   ├── beta-testing.md
    │   │   ├── conditional-xaml.md
    │   │   ├── deploying-and-debugging-uwp-apps.md
    │   │   ├── device-portal-api-core.md
    │   │   ├── device-portal-desktop.md
    │   │   ├── device-portal-mobile.md
    │   │   ├── device-portal-plugin.md
    │   │   ├── device-portal-ssl.md
    │   │   ├── device-portal.md
    │   │   ├── improve-garbage-collection-performance.md
    │   │   ├── index.md
    │   │   ├── keep-the-ui-thread-responsive.md
    │   │   ├── listview-and-gridview-data-optimization.md
    │   │   ├── loose-file-registration.md
    │   │   ├── mvvm-performance-tips.md
    │   │   ├── optimize-animations-and-media.md
    │   │   ├── optimize-background-activity.md
    │   │   ├── optimize-file-access.md
    │   │   ├── optimize-gridview-and-listview.md
    │   │   ├── optimize-suspend-resume.md
    │   │   ├── optimize-xaml-loading.md
    │   │   ├── optimize-your-xaml-layout.md
    │   │   ├── performance-and-xaml-ui.md
    │   │   ├── pgo-for-uwp.md
    │   │   ├── planning-and-measuring-performance.md
    │   │   ├── test-surface-hub-apps-using-visual-studio.md
    │   │   ├── test-with-the-emulator.md
    │   │   ├── testing-debugging-plm.md
    │   │   ├── tools-for-profiling-and-performance.md
    │   │   ├── version-adaptive-apps.md
    │   │   ├── version-adaptive-code.md
    │   │   ├── windows-app-certification-kit-tests.md
    │   │   ├── windows-app-certification-kit.md
    │   │   ├── windows-desktop-bridge-app-tests.md
    │   │   ├── windows-runtime-components-and-optimizing-interop.md
    │   │   └── images/
    │   │       ├── command-line-arguments-cpp.PNG
    │   │       ├── command-line-arguments-debugging.PNG
    │   │       ├── command-line-arguments.PNG
    │   │       ├── em-frameratecounters.PNG
    │   │       └── device-portal/
    │   │           ├── device-portal-desk-settings-developer-mode.PNG
    │   │           ├── device-portal-desk-settings-install.PNG
    │   │           └── device-portal-desk-settings.PNG
    │   ├── develop/
    │   │   ├── index.md
    │   │   └── toc.yml
    │   ├── devices-sensors/
    │   │   ├── 3d-generate-3mf.md
    │   │   ├── 3d-print-from-app.md
    │   │   ├── 3d-printing.md
    │   │   ├── aep-service-class-ids.md
    │   │   ├── ble-beacon.md
    │   │   ├── bluetooth-dev-faq.yml
    │   │   ├── bluetooth-low-energy-overview.md
    │   │   ├── bluetooth.md
    │   │   ├── build-a-device-selector.md
    │   │   ├── calibrate-sensors.md
    │   │   ├── deploy-scanner-profiles-with-mdm.md
    │   │   ├── device-information-properties.md
    │   │   ├── enable-device-capabilities.md
    │   │   ├── enable-usermode-access.md
    │   │   ├── enumerate-devices-over-a-network.md
    │   │   ├── enumerate-devices.md
    │   │   ├── epson-esc-pos-with-formatting.md
    │   │   ├── gatt-client.md
    │   │   ├── gatt-server.md
    │   │   ├── get-battery-info.md
    │   │   ├── host-card-emulation.md
    │   │   ├── index.md
    │   │   ├── lighting-dynamic-lamparray.md
    │   │   ├── pair-devices.md
    │   │   ├── pairing-a-set.md
    │   │   ├── point-of-service.md
    │   │   ├── pos-barcodescanner-configure.md
    │   │   ├── pos-barcodescanner-scan-data.md
    │   │   ├── pos-barcodescanner-software-trigger.md
    │   │   ├── pos-barcodescanner-symbologies.md
    │   │   ├── pos-barcodescanner.md
    │   │   ├── pos-basics-capability.md
    │   │   ├── pos-basics-claim.md
    │   │   ├── pos-basics-deviceobject.md
    │   │   ├── pos-basics-enumerating.md
    │   │   ├── pos-basics-sharing.md
    │   │   ├── pos-basics.md
    │   │   ├── pos-camerabarcode-advancedconfig.md
    │   │   ├── pos-camerabarcode-enable-disable.md
    │   │   ├── pos-camerabarcode-get-started.md
    │   │   ├── pos-camerabarcode-hosting-preview.md
    │   │   ├── pos-camerabarcode-symbologies.md
    │   │   ├── pos-camerabarcode-system-requirements.md
    │   │   ├── pos-camerabarcode.md
    │   │   ├── pos-device-support.md
    │   │   ├── pos-get-started.md
    │   │   ├── pos-magnetic-stripe-reader-data.md
    │   │   ├── pos-magnetic-stripe-reader.md
    │   │   ├── pos-printer.md
    │   │   ├── print-workflow-customize.md
    │   │   ├── send-or-receive-files-with-rfcomm.md
    │   │   ├── sensor-orientation.md
    │   │   ├── sensors.md
    │   │   ├── use-the-accelerometer.md
    │   │   ├── use-the-compass.md
    │   │   ├── use-the-gyrometer.md
    │   │   ├── use-the-inclinometer.md
    │   │   ├── use-the-light-sensor.md
    │   │   ├── use-the-orientation-sensor.md
    │   │   ├── code/
    │   │   │   ├── 3DPrintHowTo.sln
    │   │   │   └── 3dprinthowto/
    │   │   │       └── cs/
    │   │   │           ├── 3DPrintHowTo.csproj
    │   │   │           ├── 3DPrintHowTo.sln
    │   │   │           ├── 3DPrintHowTo_TemporaryKey.pfx
    │   │   │           ├── App.xaml
    │   │   │           ├── App.xaml.cs
    │   │   │           ├── ApplicationInsights.config
    │   │   │           ├── Generate3MFMethods.cs
    │   │   │           ├── MainPage.xaml
    │   │   │           ├── MainPage.xaml.cs
    │   │   │           ├── Package.appxmanifest
    │   │   │           ├── project.json
    │   │   │           └── Properties/
    │   │   │               ├── AssemblyInfo.cs
    │   │   │               └── Default.rd.xml
    │   │   └── includes/
    │   │       └── pos-feedback.md
    │   ├── dotnet-native/
    │   │   ├── apis-that-rely-on-reflection.md
    │   │   ├── application-element-net-native.md
    │   │   ├── assembly-element-net-native.md
    │   │   ├── attributeimplies-element-net-native.md
    │   │   ├── directives-element-net-native.md
    │   │   ├── event-element-net-native.md
    │   │   ├── example-handling-exceptions-when-binding-data.md
    │   │   ├── example-troubleshooting-dynamic-programming.md
    │   │   ├── field-element-net-native.md
    │   │   ├── genericparameter-element-net-native.md
    │   │   ├── getting-started-with-net-native.md
    │   │   ├── impliestype-element-net-native.md
    │   │   ├── index.md
    │   │   ├── library-element-net-native.md
    │   │   ├── measuring-startup-improvement-with-net-native.md
    │   │   ├── method-element-net-native.md
    │   │   ├── methodinstantiation-element-net-native.md
    │   │   ├── migrating-your-windows-store-app-to-net-native.md
    │   │   ├── missinginteropdataexception-class-net-native.md
    │   │   ├── missingmetadataexception-class-net-native.md
    │   │   ├── missingruntimeartifactexception-class-net-native.md
    │   │   ├── namespace-element-net-native.md
    │   │   ├── net-native-and-compilation.md
    │   │   ├── net-native-general-troubleshooting.md
    │   │   ├── net-native-reflection-api-reference.md
    │   │   ├── parameter-element-net-native.md
    │   │   ├── property-element-net-native.md
    │   │   ├── reflection-and-net-native.md
    │   │   ├── runtime-directive-elements.md
    │   │   ├── runtime-directive-policy-settings.md
    │   │   ├── runtime-directives-rd-xml-configuration-file-reference.md
    │   │   ├── runtime-exceptions-in-net-native-apps.md
    │   │   ├── serialization-and-metadata.md
    │   │   ├── subtypes-element-net-native.md
    │   │   ├── type-element-net-native.md
    │   │   ├── typeinstantiation-element-net-native.md
    │   │   ├── typeparameter-element-net-native.md
    │   │   └── code/
    │   │       ├── array1.cs
    │   │       ├── compat1.cs
    │   │       ├── compat2.cs
    │   │       ├── compat3.cs
    │   │       ├── etw1.cs
    │   │       ├── etw2.cs
    │   │       ├── makegenericmethod1.cs
    │   │       ├── missinginteropdataexception_syntax1.cs
    │   │       ├── missingmetadataexception_syntax1.cs
    │   │       ├── missingruntimeartifactexception_syntax1.cs
    │   │       ├── serialize1.cs
    │   │       ├── type_makegenerictype1.cs
    │   │       └── reflection/
    │   │           ├── browsegenerictype1.cs
    │   │           ├── makegenerictype1.cs
    │   │           ├── method1.cs
    │   │           ├── property1.cs
    │   │           ├── propertyinfo1.cs
    │   │           └── subtypes.cs
    │   ├── enterprise/
    │   │   ├── customer-database-app-structure.md
    │   │   ├── customer-database-tutorial.md
    │   │   ├── enterprise-shared-storage.md
    │   │   ├── index.md
    │   │   ├── wip-dev-guide.md
    │   │   ├── wip-hub.md
    │   │   └── images/
    │   │       ├── screen-shots.vsdx
    │   │       ├── wip-lifecycle.PNG
    │   │       └── customer-database-tutorial/
    │   │           ├── add-new-customer.PNG
    │   │           ├── blank-customer-list.PNG
    │   │           ├── customer-list.PNG
    │   │           ├── delete-new-customer.PNG
    │   │           ├── edit-customer-inline.PNG
    │   │           ├── initial-customers.PNG
    │   │           └── solution-explorer.PNG
    │   ├── files/
    │   │   ├── access-the-sd-card.md
    │   │   ├── best-practices-for-writing-to-files.md
    │   │   ├── change-tracking-filesystem.md
    │   │   ├── fast-file-properties.md
    │   │   ├── file-access-permissions.md
    │   │   ├── how-to-track-recently-used-files-and-folders.md
    │   │   ├── index.md
    │   │   ├── quickstart-accessing-homegroup-content.md
    │   │   ├── quickstart-determining-availability-of-microsoft-onedrive-files.md
    │   │   ├── quickstart-getting-file-properties.md
    │   │   ├── quickstart-listing-files-and-folders.md
    │   │   ├── quickstart-managing-folders-in-the-music-pictures-and-videos-libraries.md
    │   │   ├── quickstart-reading-and-writing-files.md
    │   │   ├── quickstart-save-a-file-with-a-picker.md
    │   │   ├── quickstart-using-file-and-folder-pickers.md
    │   │   ├── supplemental-properties.md
    │   │   ├── thumbnails.md
    │   │   └── images/
    │   │       └── file-write-call-sequence.vsdx
    │   ├── gaming/
    │   │   ├── about-the-uwp-user-interface-and-directx.md
    │   │   ├── accessibility-for-games.md
    │   │   ├── adding-audio-to-the-marble-maze-sample.md
    │   │   ├── adding-input-and-interactivity-to-the-marble-maze-sample.md
    │   │   ├── adding-visual-content-to-the-marble-maze-sample.md
    │   │   ├── additional-directx-game-programming-resources.md
    │   │   ├── an-introduction-to-3d-graphics-with-directx.md
    │   │   ├── applying-textures-to-primitives.md
    │   │   ├── arcade-stick.md
    │   │   ├── asynchronous-programming-directx-and-cpp.md
    │   │   ├── capture-game-audio-video-screenshots-and-metadata.md
    │   │   ├── change-your-shader-loading-code.md
    │   │   ├── cloud-for-games.md
    │   │   ├── compare-opengl-es-2-0-api-design-to-directx.md
    │   │   ├── complete-code-for-basicloader.md
    │   │   ├── complete-code-for-basicreaderwriter.md
    │   │   ├── complete-code-for-ddstextureloader.md
    │   │   ├── concept-approval.md
    │   │   ├── create-a-basic-mesh.md
    │   │   ├── create-depth-buffer-resource--view--and-sampler-state.md
    │   │   ├── creating-shaders-and-drawing-primitives.md
    │   │   ├── developing-marble-maze-a-windows-store-game-in-cpp-and-directx.md
    │   │   ├── directx-add-features.md
    │   │   ├── directx-and-xaml-interop.md
    │   │   ├── directx-fundamentals.md
    │   │   ├── directx-game-input.md
    │   │   ├── directx-getting-started.md
    │   │   ├── directx-optimization-and-advanced-topics.md
    │   │   ├── directx-porting-faq.yml
    │   │   ├── directx-programming.md
    │   │   ├── directx-samples.md
    │   │   ├── draw-to-the-screen.md
    │   │   ├── e2e.md
    │   │   ├── feature-mapping.md
    │   │   ├── flight-stick.md
    │   │   ├── game-broadcast-and-capture.md
    │   │   ├── game-development-platform-guide.md
    │   │   ├── game-development-videos.md
    │   │   ├── gamepad-and-vibration.md
    │   │   ├── getting-started.md
    │   │   ├── glsl-to-hlsl-reference.md
    │   │   ├── handling-device-lost-scenarios.md
    │   │   ├── headset.md
    │   │   ├── how-to-activate-an-app-directx-and-cpp.md
    │   │   ├── how-to-resume-an-app-directx-and-cpp.md
    │   │   ├── how-to-suspend-an-app-directx-and-cpp.md
    │   │   ├── implementing-depth-buffers-for-shadow-mapping.md
    │   │   ├── index.md
    │   │   ├── input-for-games.md
    │   │   ├── input-practices-for-games.md
    │   │   ├── launching-and-resuming-apps-directx-and-cpp.md
    │   │   ├── load-a-game-asset.md
    │   │   ├── manage-game-broadcasting.md
    │   │   ├── map-concepts-and-infrastructure.md
    │   │   ├── marble-maze-application-structure.md
    │   │   ├── marble-maze-sample-fundamentals.md
    │   │   ├── missing-dot-net-apis-in-unity-and-uwp.md
    │   │   ├── monetization-for-games.md
    │   │   ├── moving-from-egl-to-dxgi.md
    │   │   ├── multisampling--multi-sample-anti-aliasing--in-windows-store-apps.md
    │   │   ├── multisampling--scaling--and-overlay-swap-chains.md
    │   │   ├── opengl-es-2-0-to-directx-11-1-reference.md
    │   │   ├── optimize-performance-for-windows-store-direct3d-11-apps-with-coredispatcher.md
    │   │   ├── package-your-windows-store-directx-game.md
    │   │   ├── plan-your-directx-port.md
    │   │   ├── planning.md
    │   │   ├── port-a-simple-opengl-es-2-0-renderer-to-directx-11-1.md
    │   │   ├── port-from-opengl-es-2-0-to-directx-11-1.md
    │   │   ├── port-the-glsl.md
    │   │   ├── port-the-shader-config.md
    │   │   ├── port-the-vertex-buffers-and-data-config.md
    │   │   ├── porting-considerations.md
    │   │   ├── porting-guides.md
    │   │   ├── porting-uniforms-and-attributes.md
    │   │   ├── porting-your-directx-9-game-to-windows-store.md
    │   │   ├── prepare-your-dev-environment-for-windows-store-directx-game-development.md
    │   │   ├── racing-wheel-and-force-feedback.md
    │   │   ├── raw-game-controller.md
    │   │   ├── reduce-latency-with-dxgi-1-3-swap-chains.md
    │   │   ├── registry-data-for-game-controllers.md
    │   │   ├── relative-mouse-movement.md
    │   │   ├── render-the-scene-with-depth-testing.md
    │   │   ├── render-the-shadow-map-to-the-depth-buffer.md
    │   │   ├── set-up-visual-studio-for-game-development.md
    │   │   ├── setting-up-directx-resources.md
    │   │   ├── simple-port-from-direct3d-9-to-11-1-part-1--initializing-direct3d.md
    │   │   ├── simple-port-from-direct3d-9-to-11-1-part-2--rendering.md
    │   │   ├── simple-port-from-direct3d-9-to-11-1-part-3--viewport-and-game-loop.md
    │   │   ├── supporting-screen-rotation-directx-and-cpp.md
    │   │   ├── target-a-range-of-hardware.md
    │   │   ├── toc.yml
    │   │   ├── tutorial--adding-a-user-interface.md
    │   │   ├── tutorial--adding-controls.md
    │   │   ├── tutorial--adding-move-look-controls-to-your-directx-game.md
    │   │   ├── tutorial--adding-sound.md
    │   │   ├── tutorial--adding-touch-controls-to-your-directx-game.md
    │   │   ├── tutorial--assembling-the-rendering-pipeline.md
    │   │   ├── tutorial--building-the-games-uwp-app-framework.md
    │   │   ├── tutorial--create-your-first-uwp-directx-game.md
    │   │   ├── tutorial--defining-the-main-game-loop.md
    │   │   ├── tutorial--setting-up-the-games-infrastructure.md
    │   │   ├── tutorial-game-flow-management.md
    │   │   ├── tutorial-game-rendering.md
    │   │   ├── tutorial-resources.md
    │   │   ├── ui-navigation-controller.md
    │   │   ├── understand-direct3d-11-1-concepts.md
    │   │   ├── use-the-directx-runtime-and-visual-studio-graphics-diagnostic-features.md
    │   │   ├── user-interface.md
    │   │   ├── using-depth-and-effects-on-primitives.md
    │   │   ├── uwp-programming.md
    │   │   ├── walkthrough--simple-port-from-direct3d-9-to-11-1.md
    │   │   ├── walkthrough-sample-ports-from-opengl-es-2-0.md
    │   │   ├── work-with-networking-in-your-directx-game.md
    │   │   ├── working-with-2d-graphics-in-your-directx-game.md
    │   │   ├── working-with-audio-in-your-directx-game.md
    │   │   ├── code/
    │   │   │   ├── AppBroadcast/
    │   │   │   │   └── cpp/
    │   │   │   │       └── AppBroadcastExampleApp/
    │   │   │   │           ├── App.cpp
    │   │   │   │           ├── App.h
    │   │   │   │           ├── AppBroadcastExampleApp.vcxproj
    │   │   │   │           ├── AppBroadcastExampleApp.vcxproj.filters
    │   │   │   │           ├── AppBroadcastExampleApp_TemporaryKey.pfx
    │   │   │   │           ├── AppBroadcastExampleAppMain.cpp
    │   │   │   │           ├── AppBroadcastExampleAppMain.h
    │   │   │   │           ├── Package.appxmanifest
    │   │   │   │           ├── pch.cpp
    │   │   │   │           ├── pch.h
    │   │   │   │           ├── Common/
    │   │   │   │           │   ├── DeviceResources.cpp
    │   │   │   │           │   ├── DeviceResources.h
    │   │   │   │           │   ├── DirectXHelper.h
    │   │   │   │           │   └── StepTimer.h
    │   │   │   │           └── Content/
    │   │   │   │               ├── Sample3DSceneRenderer.cpp
    │   │   │   │               ├── Sample3DSceneRenderer.h
    │   │   │   │               ├── SampleFpsTextRenderer.cpp
    │   │   │   │               ├── SampleFpsTextRenderer.h
    │   │   │   │               ├── SamplePixelShader.hlsl
    │   │   │   │               ├── SampleVertexShader.hlsl
    │   │   │   │               └── ShaderStructures.h
    │   │   │   └── AppRecordingExample/
    │   │   │       └── cpp/
    │   │   │           └── AppRecordingExample/
    │   │   │               ├── App.cpp
    │   │   │               ├── App.h
    │   │   │               ├── AppRecordingExample.vcxproj
    │   │   │               ├── AppRecordingExample.vcxproj.filters
    │   │   │               ├── AppRecordingExample_TemporaryKey.pfx
    │   │   │               ├── AppRecordingExampleMain.cpp
    │   │   │               ├── AppRecordingExampleMain.h
    │   │   │               ├── Package.appxmanifest
    │   │   │               ├── pch.cpp
    │   │   │               ├── pch.h
    │   │   │               ├── Common/
    │   │   │               │   ├── DeviceResources.cpp
    │   │   │               │   ├── DeviceResources.h
    │   │   │               │   ├── DirectXHelper.h
    │   │   │               │   └── StepTimer.h
    │   │   │               └── Content/
    │   │   │                   ├── Sample3DSceneRenderer.cpp
    │   │   │                   ├── Sample3DSceneRenderer.h
    │   │   │                   ├── SampleFpsTextRenderer.cpp
    │   │   │                   ├── SampleFpsTextRenderer.h
    │   │   │                   ├── SamplePixelShader.hlsl
    │   │   │                   ├── SampleVertexShader.hlsl
    │   │   │                   └── ShaderStructures.h
    │   │   └── images/
    │   │       ├── simple-dx-game-extend-xaml.PNG
    │   │       ├── simple-dx-game-setup-app-manifest.PNG
    │   │       └── simple-dx-game-setup-capabilities.PNG
    │   ├── get-started/
    │   │   ├── construct-form-learning-track.md
    │   │   ├── create-a-basic-windows-10-app-in-cpp.md
    │   │   ├── create-a-basic-windows-10-app-in-cppwinrt.md
    │   │   ├── create-a-hello-world-app-xaml-universal.md
    │   │   ├── create-uwp-apps.md
    │   │   ├── display-customers-in-list-learning-track.md
    │   │   ├── fileio-learning-track.md
    │   │   ├── index.md
    │   │   ├── plan-your-app.md
    │   │   ├── settings-learning-track.md
    │   │   ├── toc.yml
    │   │   ├── universal-application-platform-guide.md
    │   │   ├── your-first-app.md
    │   │   ├── images/
    │   │   │   └── js-tut-state-diagram.vsd
    │   │   └── winui2/
    │   │       ├── getting-started.md
    │   │       ├── index.md
    │   │       ├── nuget-packages.md
    │   │       └── release-notes/
    │   │           ├── index.md
    │   │           ├── winui-2.0.md
    │   │           ├── winui-2.1.md
    │   │           ├── winui-2.2.md
    │   │           ├── winui-2.3.md
    │   │           ├── winui-2.4.md
    │   │           ├── winui-2.5.md
    │   │           ├── winui-2.6.md
    │   │           ├── winui-2.7.md
    │   │           └── winui-2.8.md
    │   ├── graphics-concepts/
    │   │   ├── address-space-available-for-streaming-resources.md
    │   │   ├── ambient-lighting.md
    │   │   ├── anisotropic-texture-filtering.md
    │   │   ├── appendix.md
    │   │   ├── attenuation-and-spotlight-factor.md
    │   │   ├── basic-texturing-concepts.md
    │   │   ├── bc6h-format.md
    │   │   ├── bc7-format.md
    │   │   ├── bilinear-texture-filtering.md
    │   │   ├── blending-stages.md
    │   │   ├── block-compression.md
    │   │   ├── buffer-tiling.md
    │   │   ├── camera-space-transformations.md
    │   │   ├── choosing-a-resource.md
    │   │   ├── color-light-maps.md
    │   │   ├── compressed-texture-formats.md
    │   │   ├── compressed-texture-resources.md
    │   │   ├── compute-pipeline.md
    │   │   ├── compute-shader-stage--cs-.md
    │   │   ├── configuring-depth-stencil-functionality.md
    │   │   ├── constant-buffer-view--cbv-.md
    │   │   ├── coordinate-systems-and-geometry.md
    │   │   ├── coordinate-systems.md
    │   │   ├── copying-and-accessing-resource-data.md
    │   │   ├── creating-streaming-resources.md
    │   │   ├── data-type-conversion.md
    │   │   ├── depth-and-stencil-buffers.md
    │   │   ├── depth-buffers.md
    │   │   ├── depth-stencil-view--dsv-.md
    │   │   ├── device-types.md
    │   │   ├── devices.md
    │   │   ├── diffuse-light-maps.md
    │   │   ├── diffuse-lighting.md
    │   │   ├── domain-shader-stage--ds-.md
    │   │   ├── emissive-lighting.md
    │   │   ├── face-and-vertex-normal-vectors.md
    │   │   ├── floating-point-rules.md
    │   │   ├── geometry-shader-stage--gs-.md
    │   │   ├── graphics-pipeline.md
    │   │   ├── hazard-tracking-versus-tile-pool-resources.md
    │   │   ├── hlsl-streaming-resources-exposure.md
    │   │   ├── how-a-streaming-resource-s-area-is-tiled.md
    │   │   ├── hull-shader-stage--hs-.md
    │   │   ├── index-buffers.md
    │   │   ├── index.md
    │   │   ├── input-assembler-stage--ia-.md
    │   │   ├── introduction-to-buffers.md
    │   │   ├── introduction-to-rasterization-rules.md
    │   │   ├── introduction-to-textures.md
    │   │   ├── light-mapping-with-textures.md
    │   │   ├── light-properties.md
    │   │   ├── light-types.md
    │   │   ├── lighting-overview.md
    │   │   ├── lights-and-materials.md
    │   │   ├── line-lists.md
    │   │   ├── line-strips.md
    │   │   ├── lost-devices.md
    │   │   ├── mappings-are-into-a-tile-pool.md
    │   │   ├── mathematics-of-lighting.md
    │   │   ├── mipmap-packing.md
    │   │   ├── monochrome-light-maps.md
    │   │   ├── multipass-texture-blending.md
    │   │   ├── nearest-point-sampling.md
    │   │   ├── opaque-and-1-bit-alpha-textures.md
    │   │   ├── operations-available-on-streaming-resources.md
    │   │   ├── operations-available-on-tile-pools.md
    │   │   ├── output-merger-stage--om-.md
    │   │   ├── pipeline-access-to-streaming-resources.md
    │   │   ├── pixel-shader-stage--ps-.md
    │   │   ├── point-lists.md
    │   │   ├── primitive-topologies.md
    │   │   ├── primitives.md
    │   │   ├── projection-transform.md
    │   │   ├── rasterization-rules.md
    │   │   ├── rasterizer-behavior-with-non-mapped-tiles.md
    │   │   ├── rasterizer-ordered-view--rov-.md
    │   │   ├── rasterizer-stage--rs-.md
    │   │   ├── rectangles.md
    │   │   ├── render-target-view--rtv-.md
    │   │   ├── resource-types.md
    │   │   ├── resources.md
    │   │   ├── sampler.md
    │   │   ├── shader-resource-view--srv-.md
    │   │   ├── specular-light-maps.md
    │   │   ├── specular-lighting.md
    │   │   ├── srv-behavior-with-non-mapped-tiles.md
    │   │   ├── state-objects.md
    │   │   ├── stencil-buffers.md
    │   │   ├── stencil-formats-not-supported-with-streaming-resources.md
    │   │   ├── stream-output-stage--so-.md
    │   │   ├── stream-output-view--sov-.md
    │   │   ├── streaming-resource-creation-parameters.md
    │   │   ├── streaming-resource-cross-process-and-device-sharing.md
    │   │   ├── streaming-resources-features-tiers.md
    │   │   ├── streaming-resources-texture-sampling-features.md
    │   │   ├── streaming-resources.md
    │   │   ├── swap-chains.md
    │   │   ├── tessellator-stage--ts-.md
    │   │   ├── texture-addressing-modes.md
    │   │   ├── texture-blending.md
    │   │   ├── texture-block-compression.md
    │   │   ├── texture-filtering-with-mipmaps.md
    │   │   ├── texture-filtering.md
    │   │   ├── texture-resources.md
    │   │   ├── texture-views.md
    │   │   ├── texture-wrapping.md
    │   │   ├── texture2d-and-texture2darray-subresource-tiling.md
    │   │   ├── texture3d-subresource-tiling.md
    │   │   ├── textures-with-alpha-channels.md
    │   │   ├── textures.md
    │   │   ├── the-need-for-streaming-resources.md
    │   │   ├── tier-1.md
    │   │   ├── tier-2.md
    │   │   ├── tier-3.md
    │   │   ├── tile-access-limitations-with-duplicate-mappings.md
    │   │   ├── tile-pool-creation-parameters.md
    │   │   ├── tile-pool-creation.md
    │   │   ├── tile-pool-resizing.md
    │   │   ├── TOC_down1.txt
    │   │   ├── TOC_down2.txt
    │   │   ├── transform-overview.md
    │   │   ├── transforms.md
    │   │   ├── triangle-interpolation.md
    │   │   ├── triangle-lists.md
    │   │   ├── triangle-strips.md
    │   │   ├── uav-behavior-with-non-mapped-tiles.md
    │   │   ├── using-system-generated-values.md
    │   │   ├── vectors--vertices--and-quaternions.md
    │   │   ├── vertex-and-index-buffers.md
    │   │   ├── vertex-buffer-view--vbv-.md
    │   │   ├── vertex-shader-stage--vs-.md
    │   │   ├── view-transform.md
    │   │   ├── viewports-and-clipping.md
    │   │   ├── views.md
    │   │   ├── windowed-vs--full-screen-mode.md
    │   │   └── world-transform.md
    │   ├── launch-resume/
    │   │   ├── access-sensors-and-devices-from-a-background-task.md
    │   │   ├── activate-an-app.md
    │   │   ├── adaptive-tiles-schema.md
    │   │   ├── add-a-splash-screen.md
    │   │   ├── app-lifecycle.md
    │   │   ├── app-services.md
    │   │   ├── auto-launching-with-autoplay.md
    │   │   ├── chaseable-tile-notifications.md
    │   │   ├── communicate-with-a-remote-app-service.md
    │   │   ├── connected-apps-and-devices.md
    │   │   ├── console-uwp.md
    │   │   ├── convert-app-service-in-process.md
    │   │   ├── convert-out-of-process-background-task.md
    │   │   ├── create-a-customized-splash-screen.md
    │   │   ├── create-adaptive-tiles.md
    │   │   ├── create-and-host-a-package-extension.md
    │   │   ├── create-and-register-a-background-task.md
    │   │   ├── create-and-register-a-winmain-background-task.md
    │   │   ├── create-and-register-an-inproc-background-task.md
    │   │   ├── creating-tiles.md
    │   │   ├── debug-a-background-task.md
    │   │   ├── declare-background-tasks-in-the-application-manifest.md
    │   │   ├── discover-remote-devices.md
    │   │   ├── extend-your-app-with-services-extensions-packages.md
    │   │   ├── group-background-tasks.md
    │   │   ├── guidelines-for-background-tasks.md
    │   │   ├── handle-a-cancelled-background-task.md
    │   │   ├── handle-app-prelaunch.md
    │   │   ├── hosted-apps.md
    │   │   ├── how-to-create-an-extension.md
    │   │   ├── how-to-create-and-consume-an-app-service.md
    │   │   ├── how-to-launch-an-app-for-results.md
    │   │   ├── index.md
    │   │   ├── launch-a-remote-app.md
    │   │   ├── launch-ringtone-picker.md
    │   │   ├── monitor-background-task-progress-and-completion.md
    │   │   ├── multi-instance-uwp.md
    │   │   ├── primary-tile-apis.md
    │   │   ├── reduce-memory-usage.md
    │   │   ├── register-a-background-task.md
    │   │   ├── remote-sessions.md
    │   │   ├── respond-to-system-events-with-background-tasks.md
    │   │   ├── resume-an-app.md
    │   │   ├── run-a-background-task-during-updatetask.md
    │   │   ├── run-a-background-task-on-a-timer-.md
    │   │   ├── run-in-the-background-indefinetly.md
    │   │   ├── run-minimized-with-extended-execution.md
    │   │   ├── secondary-tiles-guidance.md
    │   │   ├── secondary-tiles-pin-to-taskbar.md
    │   │   ├── secondary-tiles-pinning.md
    │   │   ├── secondary-tiles.md
    │   │   ├── sending-a-local-tile-notification.md
    │   │   ├── set-conditions-for-running-a-background-task.md
    │   │   ├── special-tile-templates-catalog.md
    │   │   ├── splash-screens.md
    │   │   ├── support-your-app-with-background-tasks.md
    │   │   ├── suspend-an-app.md
    │   │   ├── tile-schema.md
    │   │   ├── tile-toast-language-scale-contrast.md
    │   │   ├── trigger-background-task-from-app.md
    │   │   ├── update-a-live-tile-from-a-background-task.md
    │   │   ├── use-a-maintenance-trigger.md
    │   │   ├── useractivities-best-practices.md
    │   │   ├── useractivities.md
    │   │   ├── code/
    │   │   │   ├── RemoteScenarios.sln
    │   │   │   ├── DiscoverDevices/
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── App.xaml.cs
    │   │   │   │   ├── DiscoverDevices.csproj
    │   │   │   │   ├── DiscoverDevices_TemporaryKey.pfx
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   ├── project.json
    │   │   │   │   └── Properties/
    │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │       └── Default.rd.xml
    │   │   │   ├── ReduceMemory/
    │   │   │   │   └── cs/
    │   │   │   │       └── App.xaml.cs
    │   │   │   ├── RemoteAppService/
    │   │   │   │   ├── App.xaml
    │   │   │   │   ├── App.xaml.cs
    │   │   │   │   ├── MainPage.xaml
    │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   ├── project.json
    │   │   │   │   ├── RemoteAppService.csproj
    │   │   │   │   ├── RemoteAppService_TemporaryKey.pfx
    │   │   │   │   └── Properties/
    │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │       └── Default.rd.xml
    │   │   │   └── RemoteLaunchScenario/
    │   │   │       ├── App.xaml
    │   │   │       ├── App.xaml.cs
    │   │   │       ├── App1_TemporaryKey.pfx
    │   │   │       ├── LaunchRemoteUri.csproj
    │   │   │       ├── MainPage.xaml
    │   │   │       ├── MainPage.xaml.cs
    │   │   │       ├── Package.appxmanifest
    │   │   │       ├── project.json
    │   │   │       └── Properties/
    │   │   │           ├── AssemblyInfo.cs
    │   │   │           └── Default.rd.xml
    │   │   ├── images/
    │   │   │   └── shared-experiences-settings.PNG
    │   │   └── includes/
    │   │       └── live-tiles-note.md
    │   ├── maps-and-location/
    │   │   ├── authentication-key.md
    │   │   ├── display-maps.md
    │   │   ├── display-poi.md
    │   │   ├── elements-of-map-style-sheet.md
    │   │   ├── geocoding.md
    │   │   ├── get-location.md
    │   │   ├── guidelines-and-checklist-for-detecting-location.md
    │   │   ├── guidelines-for-geofencing.md
    │   │   ├── guidelines-for-visits.md
    │   │   ├── index.md
    │   │   ├── overlay-tiled-images.md
    │   │   ├── routes-and-directions.md
    │   │   └── set-up-a-geofence.md
    │   ├── monetize/
    │   │   ├── access-analytics-data-using-windows-store-services.md
    │   │   ├── acquisitions-data.md
    │   │   ├── ad-mediation-service.md
    │   │   ├── adcontrol-in-html-5-and-javascript.md
    │   │   ├── adcontrol-in-xaml-and--net.md
    │   │   ├── add-advertisements-to-video-content.md
    │   │   ├── add-on-acquisitions-data.md
    │   │   ├── banner-ads.md
    │   │   ├── best-practices-for-ads-in-apps.md
    │   │   ├── change-the-billing-state-of-a-subscription-for-a-user.md
    │   │   ├── code-examples-for-the-windows-store-submission-api.md
    │   │   ├── code-your-experiment-in-your-app.md
    │   │   ├── commit-a-flight-submission.md
    │   │   ├── commit-an-add-on-submission.md
    │   │   ├── commit-an-app-submission.md
    │   │   ├── configure-your-app-to-receive-dev-center-notifications.md
    │   │   ├── create-a-flight-submission.md
    │   │   ├── create-a-flight.md
    │   │   ├── create-a-project-and-define-remote-variables-in-the-dev-center-dashboard.md
    │   │   ├── create-an-add-on-submission.md
    │   │   ├── create-an-add-on.md
    │   │   ├── create-an-app-submission.md
    │   │   ├── create-and-manage-submissions-using-windows-store-services.md
    │   │   ├── create-and-run-your-first-experiment-with-a-b-testing.md
    │   │   ├── csharp-code-examples-for-submissions-game-options-and-trailers.md
    │   │   ├── csharp-code-examples-for-the-windows-store-submission-api.md
    │   │   ├── data-schemas-for-store-products.md
    │   │   ├── define-your-experiment-in-the-dev-center-dashboard.md
    │   │   ├── delete-a-flight-submission.md
    │   │   ├── delete-a-flight.md
    │   │   ├── delete-an-add-on-submission.md
    │   │   ├── delete-an-add-on.md
    │   │   ├── delete-an-app-submission.md
    │   │   ├── developer-walkthroughs.md
    │   │   ├── display-ads-in-your-app.md
    │   │   ├── download-the-cab-file-for-an-error-in-your-app.md
    │   │   ├── download-the-cab-file-for-an-error-in-your-desktop-application.md
    │   │   ├── enable-consumable-add-on-purchases.md
    │   │   ├── enable-consumable-in-app-product-purchases.md
    │   │   ├── enable-in-app-product-purchases.md
    │   │   ├── enable-in-app-purchases-of-apps-and-add-ons.md
    │   │   ├── enable-subscription-add-ons-for-your-app.md
    │   │   ├── error-codes-for-store-operations.md
    │   │   ├── error-handling-in-javascript-walkthrough.md
    │   │   ├── error-handling-in-xamlc-walkthrough.md
    │   │   ├── error-handling-with-advertising-libraries.md
    │   │   ├── exclude-or-limit-features-in-a-trial-version-of-your-app.md
    │   │   ├── finalize-the-package-rollout-for-a-flight-submission.md
    │   │   ├── finalize-the-package-rollout-for-an-app-submission.md
    │   │   ├── get-a-flight-submission.md
    │   │   ├── get-a-flight.md
    │   │   ├── get-acquisition-funnel-data.md
    │   │   ├── get-ad-campaign-performance-data.md
    │   │   ├── get-ad-performance-data.md
    │   │   ├── get-add-on-conversions-by-channel.md
    │   │   ├── get-add-ons-for-an-app.md
    │   │   ├── get-all-add-ons.md
    │   │   ├── get-all-apps.md
    │   │   ├── get-an-add-on-submission.md
    │   │   ├── get-an-add-on.md
    │   │   ├── get-an-app-submission.md
    │   │   ├── get-an-app.md
    │   │   ├── get-app-acquisitions.md
    │   │   ├── get-app-conversions-by-channel.md
    │   │   ├── get-app-data.md
    │   │   ├── get-app-installs.md
    │   │   ├── get-app-ratings.md
    │   │   ├── get-app-reviews.md
    │   │   ├── get-app-usage-daily.md
    │   │   ├── get-app-usage-monthly.md
    │   │   ├── get-desktop-app-installs.md
    │   │   ├── get-desktop-application-error-reporting-data.md
    │   │   ├── get-desktop-block-data-details.md
    │   │   ├── get-desktop-block-data.md
    │   │   ├── get-details-for-an-error-in-your-app.md
    │   │   ├── get-details-for-an-error-in-your-desktop-application.md
    │   │   ├── get-error-reporting-data.md
    │   │   ├── get-flights-for-an-app.md
    │   │   ├── get-in-app-acquisitions.md
    │   │   ├── get-insights-data-for-your-app.md
    │   │   ├── get-insights-data-for-your-desktop-app.md
    │   │   ├── get-license-info-for-apps-and-add-ons.md
    │   │   ├── get-package-rollout-info-for-a-flight-submission.md
    │   │   ├── get-package-rollout-info-for-an-app-submission.md
    │   │   ├── get-product-info-for-apps-and-add-ons.md
    │   │   ├── get-response-info-for-app-reviews.md
    │   │   ├── get-status-for-a-flight-submission.md
    │   │   ├── get-status-for-an-add-on-submission.md
    │   │   ├── get-status-for-an-app-submission.md
    │   │   ├── get-subscription-acquisitions.md
    │   │   ├── get-subscriptions-for-a-user.md
    │   │   ├── get-targeted-offers.md
    │   │   ├── get-the-stack-trace-for-an-error-in-your-app.md
    │   │   ├── get-the-stack-trace-for-an-error-in-your-desktop-application.md
    │   │   ├── grant-free-products.md
    │   │   ├── halt-the-package-rollout-for-a-flight-submission.md
    │   │   ├── halt-the-package-rollout-for-an-app-submission.md
    │   │   ├── html-and-javascript-troubleshooting-guide.md
    │   │   ├── implement-a-trial-version-of-your-app.md
    │   │   ├── in-app-purchases-and-trials-using-the-windows-applicationmodel-store-namespace.md
    │   │   ├── in-app-purchases-and-trials.md
    │   │   ├── index.md
    │   │   ├── install-the-microsoft-advertising-libraries.md
    │   │   ├── interstitial-ad-sample-code-in-c.md
    │   │   ├── interstitial-ad-sample-code-in-javascript.md
    │   │   ├── interstitial-ads.md
    │   │   ├── java-code-examples-for-submissions-game-options-and-trailers.md
    │   │   ├── java-code-examples-for-the-windows-store-submission-api.md
    │   │   ├── known-issues-for-the-advertising-libraries.md
    │   │   ├── launch-feedback-hub-from-your-app.md
    │   │   ├── log-custom-events-for-dev-center.md
    │   │   ├── manage-a-large-catalog-of-in-app-products.md
    │   │   ├── manage-ad-campaigns.md
    │   │   ├── manage-add-on-submissions.md
    │   │   ├── manage-add-ons.md
    │   │   ├── manage-app-submissions.md
    │   │   ├── manage-creatives-for-ad-campaigns.md
    │   │   ├── manage-delivery-lines-for-ad-campaigns.md
    │   │   ├── manage-flight-submissions.md
    │   │   ├── manage-flights.md
    │   │   ├── manage-targeted-offers-using-windows-store-services.md
    │   │   ├── manage-targeting-profiles-for-ad-campaigns.md
    │   │   ├── manage-your-experiment.md
    │   │   ├── microsoft-store-services-sdk.md
    │   │   ├── native-ads.md
    │   │   ├── optimize-ad-unit-viewability.md
    │   │   ├── python-code-examples-for-submissions-game-options-and-trailers.md
    │   │   ├── python-code-examples-for-the-windows-store-submission-api.md
    │   │   ├── query-for-products.md
    │   │   ├── release-notes-for-the-advertising-libraries.md
    │   │   ├── renew-a-windows-store-id-key.md
    │   │   ├── report-consumable-products-as-fulfilled.md
    │   │   ├── request-ratings-and-reviews.md
    │   │   ├── respond-to-reviews-using-windows-store-services.md
    │   │   ├── retail-demo-experience.md
    │   │   ├── run-ad-campaigns-using-windows-store-services.md
    │   │   ├── run-app-experiments-with-a-b-testing.md
    │   │   ├── send-requests-to-the-store.md
    │   │   ├── set-up-ad-units-in-your-app.md
    │   │   ├── submit-responses-to-app-reviews.md
    │   │   ├── supported-ad-sizes-for-banner-ads.md
    │   │   ├── ui-and-user-experience-guidelines.md
    │   │   ├── update-a-flight-submission.md
    │   │   ├── update-an-add-on-submission.md
    │   │   ├── update-an-app-submission.md
    │   │   ├── update-the-package-rollout-percentage-for-a-flight-submission.md
    │   │   ├── update-the-package-rollout-percentage-for-an-app-submission.md
    │   │   ├── update-your-app-to-the-latest-advertising-libraries.md
    │   │   ├── use-receipts-to-verify-product-purchases.md
    │   │   ├── using-windows-store-services.md
    │   │   ├── view-and-grant-products-from-a-service.md
    │   │   ├── windows-premium-ads-publishers-program.md
    │   │   ├── xaml-and-c-troubleshooting-guide.md
    │   │   ├── code/
    │   │   │   ├── AdvertisingSamples/
    │   │   │   │   ├── AdControlSamples/
    │   │   │   │   │   ├── cs/
    │   │   │   │   │   │   ├── AdControlSamples.csproj
    │   │   │   │   │   │   ├── AdControlSamples_TemporaryKey.pfx
    │   │   │   │   │   │   ├── App.xaml
    │   │   │   │   │   │   ├── App.xaml.cs
    │   │   │   │   │   │   ├── MainPage.xaml
    │   │   │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   │   │   ├── MiscellaneousSnippets.cs
    │   │   │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   │   │   ├── project.json
    │   │   │   │   │   │   └── Properties/
    │   │   │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │   │   │       └── Default.rd.xml
    │   │   │   │   │   └── js/
    │   │   │   │   │       └── main.js
    │   │   │   │   ├── AdSchedulerSamples/
    │   │   │   │   │   └── js/
    │   │   │   │   │       ├── AdSchedulerSamples.jsproj
    │   │   │   │   │       ├── AdSchedulerSamples.sln
    │   │   │   │   │       ├── AdSchedulerSamples_TemporaryKey.pfx
    │   │   │   │   │       ├── index.html
    │   │   │   │   │       ├── package.appxmanifest
    │   │   │   │   │       ├── css/
    │   │   │   │   │       │   └── default.css
    │   │   │   │   │       └── js/
    │   │   │   │   │           ├── AdScheduler.js
    │   │   │   │   │           └── main.js
    │   │   │   │   ├── InterstitialAdSamples/
    │   │   │   │   │   ├── cpp/
    │   │   │   │   │   │   ├── App.xaml
    │   │   │   │   │   │   ├── App.xaml.cpp
    │   │   │   │   │   │   ├── App.xaml.h
    │   │   │   │   │   │   ├── DirectXPage.xaml
    │   │   │   │   │   │   ├── DirectXPage.xaml.cpp
    │   │   │   │   │   │   ├── DirectXPage.xaml.h
    │   │   │   │   │   │   ├── InterstitialAdSamplesCpp.vcxproj
    │   │   │   │   │   │   ├── InterstitialAdSamplesCpp.vcxproj.filters
    │   │   │   │   │   │   ├── InterstitialAdSamplesCpp_TemporaryKey.pfx
    │   │   │   │   │   │   ├── InterstitialAdSamplesCppMain.cpp
    │   │   │   │   │   │   ├── InterstitialAdSamplesCppMain.h
    │   │   │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   │   │   ├── pch.cpp
    │   │   │   │   │   │   ├── pch.h
    │   │   │   │   │   │   ├── Common/
    │   │   │   │   │   │   │   ├── DeviceResources.cpp
    │   │   │   │   │   │   │   ├── DeviceResources.h
    │   │   │   │   │   │   │   ├── DirectXHelper.h
    │   │   │   │   │   │   │   └── StepTimer.h
    │   │   │   │   │   │   └── Content/
    │   │   │   │   │   │       ├── Sample3DSceneRenderer.cpp
    │   │   │   │   │   │       ├── Sample3DSceneRenderer.h
    │   │   │   │   │   │       ├── SampleFpsTextRenderer.cpp
    │   │   │   │   │   │       ├── SampleFpsTextRenderer.h
    │   │   │   │   │   │       ├── SamplePixelShader.hlsl
    │   │   │   │   │   │       ├── SampleVertexShader.hlsl
    │   │   │   │   │   │       └── ShaderStructures.h
    │   │   │   │   │   ├── cs/
    │   │   │   │   │   │   ├── App.xaml
    │   │   │   │   │   │   ├── App.xaml.cs
    │   │   │   │   │   │   ├── InterstitialAdSamplesCSharp.csproj
    │   │   │   │   │   │   ├── InterstitialAdSamplesCSharp_TemporaryKey.pfx
    │   │   │   │   │   │   ├── MainPage.xaml
    │   │   │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   │   │   ├── project.json
    │   │   │   │   │   │   └── Properties/
    │   │   │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │   │   │       └── Default.rd.xml
    │   │   │   │   │   └── js/
    │   │   │   │   │       ├── index.html
    │   │   │   │   │       ├── main.js
    │   │   │   │   │       ├── samples.js
    │   │   │   │   │       └── script.js
    │   │   │   │   ├── MigrateToAdControl/
    │   │   │   │   │   └── cs/
    │   │   │   │   │       ├── App.xaml
    │   │   │   │   │       ├── App.xaml.cs
    │   │   │   │   │       ├── ExamplePage1.xaml
    │   │   │   │   │       ├── ExamplePage1.xaml.cs
    │   │   │   │   │       ├── MainPage.xaml
    │   │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │   │       ├── MigrateToAdControl.csproj
    │   │   │   │   │       ├── MigrateToAdControl.sln
    │   │   │   │   │       ├── MigrateToAdControl_TemporaryKey.pfx
    │   │   │   │   │       ├── Package.appxmanifest
    │   │   │   │   │       ├── project.json
    │   │   │   │   │       └── Properties/
    │   │   │   │   │           ├── AssemblyInfo.cs
    │   │   │   │   │           └── Default.rd.xml
    │   │   │   │   └── NativeAdSamples/
    │   │   │   │       └── cs/
    │   │   │   │           ├── App.xaml
    │   │   │   │           ├── App.xaml.cs
    │   │   │   │           ├── MainPage.xaml
    │   │   │   │           ├── MainPage.xaml.cs
    │   │   │   │           ├── NativeAdSamples.csproj
    │   │   │   │           ├── NativeAdSamples_TemporaryKey.pfx
    │   │   │   │           ├── Package.appxmanifest
    │   │   │   │           └── Properties/
    │   │   │   │               ├── AssemblyInfo.cs
    │   │   │   │               └── Default.rd.xml
    │   │   │   ├── InAppPurchasesAndLicenses/
    │   │   │   │   └── cs/
    │   │   │   │       ├── App.xaml
    │   │   │   │       ├── App.xaml.cs
    │   │   │   │       ├── EnableConsumablePurchases.cs
    │   │   │   │       ├── EnableInAppPurchases.cs
    │   │   │   │       ├── InAppPurchasesAndLicenses.csproj
    │   │   │   │       ├── InAppPurchasesAndLicenses_TemporaryKey.pfx
    │   │   │   │       ├── MainPage.xaml
    │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │       ├── ManageCatalog.cs
    │   │   │   │       ├── Package.appxmanifest
    │   │   │   │       ├── project.json
    │   │   │   │       ├── TrialVersion.cs
    │   │   │   │       └── Properties/
    │   │   │   │           ├── AssemblyInfo.cs
    │   │   │   │           └── Default.rd.xml
    │   │   │   ├── InAppPurchasesAndLicenses_RS1/
    │   │   │   │   ├── cs/
    │   │   │   │   │   ├── App.xaml
    │   │   │   │   │   ├── App.xaml.cs
    │   │   │   │   │   ├── ConsumeAddOnPage.xaml
    │   │   │   │   │   ├── ConsumeAddOnPage.xaml.cs
    │   │   │   │   │   ├── GetAddOnInfoPage.xaml
    │   │   │   │   │   ├── GetAddOnInfoPage.xaml.cs
    │   │   │   │   │   ├── GetAppInfoPage.xaml
    │   │   │   │   │   ├── GetAppInfoPage.xaml.cs
    │   │   │   │   │   ├── GetLicenseInfoPage.xaml
    │   │   │   │   │   ├── GetLicenseInfoPage.xaml.cs
    │   │   │   │   │   ├── GetProductInfoPage.xaml
    │   │   │   │   │   ├── GetProductInfoPage.xaml.cs
    │   │   │   │   │   ├── GetRemainingAddOnBalancePage.xaml
    │   │   │   │   │   ├── GetRemainingAddOnBalancePage.xaml.cs
    │   │   │   │   │   ├── GetSubscriptionAddOnsPage.xaml
    │   │   │   │   │   ├── GetSubscriptionAddOnsPage.xaml.cs
    │   │   │   │   │   ├── GetUserCollectionPage.xaml
    │   │   │   │   │   ├── GetUserCollectionPage.xaml.cs
    │   │   │   │   │   ├── ImplementTrialPage.xaml
    │   │   │   │   │   ├── ImplementTrialPage.xaml.cs
    │   │   │   │   │   ├── InAppPurchasesAndLicenses_UWP.csproj
    │   │   │   │   │   ├── MainPage.xaml
    │   │   │   │   │   ├── MainPage.xaml.cs
    │   │   │   │   │   ├── Package.appxmanifest
    │   │   │   │   │   ├── project.json
    │   │   │   │   │   ├── PurchaseAddOnPage.xaml
    │   │   │   │   │   ├── PurchaseAddOnPage.xaml.cs
    │   │   │   │   │   ├── PurchaseSubscriptionAddOnPage.xaml
    │   │   │   │   │   ├── PurchaseSubscriptionAddOnPage.xaml.cs
    │   │   │   │   │   ├── PurchaseSubscriptionAddOnTrialPage.xaml
    │   │   │   │   │   ├── PurchaseSubscriptionAddOnTrialPage.xaml.cs
    │   │   │   │   │   └── Properties/
    │   │   │   │   │       ├── AssemblyInfo.cs
    │   │   │   │   │       └── Default.rd.xml
    │   │   │   │   └── json/
    │   │   │   │       ├── StoreAppLicense.ExtendedJsonData.json
    │   │   │   │       ├── StoreAppLicense.ExtendedJsonDataExample.json
    │   │   │   │       ├── StoreProduct.ExtendedJsonData.json
    │   │   │   │       ├── StoreProduct.ExtendedJsonDataExample.json
    │   │   │   │       └── StorePurchaseProperties.ExtendedJsonData.json
    │   │   │   ├── PaymentsApiSample/
    │   │   │   │   ├── PaymentsApiSample.sln
    │   │   │   │   └── PaymentsApiSample/
    │   │   │   │       ├── App.xaml
    │   │   │   │       ├── App.xaml.cs
    │   │   │   │       ├── MainPage.xaml
    │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │       ├── Package.appxmanifest
    │   │   │   │       ├── PaymentsApiSample.csproj
    │   │   │   │       ├── PaymentsApiSample_TemporaryKey.pfx
    │   │   │   │       └── Properties/
    │   │   │   │           ├── AssemblyInfo.cs
    │   │   │   │           └── Default.rd.xml
    │   │   │   ├── ReceiptVerificationSample/
    │   │   │   │   └── cs/
    │   │   │   │       ├── App.config
    │   │   │   │       ├── Program.cs
    │   │   │   │       ├── ReceiptVerificationSample.csproj
    │   │   │   │       └── Properties/
    │   │   │   │           └── AssemblyInfo.cs
    │   │   │   ├── StoreSDKSamples/
    │   │   │   │   └── cs/
    │   │   │   │       ├── App.xaml
    │   │   │   │       ├── App.xaml.cs
    │   │   │   │       ├── DevCenterNotifications.cs
    │   │   │   │       ├── ExperimentExamples.cs
    │   │   │   │       ├── ExperimentPage.xaml
    │   │   │   │       ├── ExperimentPage.xaml.cs
    │   │   │   │       ├── FeedbackPage.xaml
    │   │   │   │       ├── FeedbackPage.xaml.cs
    │   │   │   │       ├── LogEvents.cs
    │   │   │   │       ├── MainPage.xaml
    │   │   │   │       ├── MainPage.xaml.cs
    │   │   │   │       ├── Package.appxmanifest
    │   │   │   │       ├── project.json
    │   │   │   │       ├── StoreSDKSamples.csproj
    │   │   │   │       ├── StoreSDKSamples_TemporaryKey.pfx
    │   │   │   │       └── Properties/
    │   │   │   │           ├── AssemblyInfo.cs
    │   │   │   │           └── Default.rd.xml
    │   │   │   ├── StoreServicesExamples_Analytics/
    │   │   │   │   └── cs/
    │   │   │   │       ├── App.config
    │   │   │   │       ├── Program.cs
    │   │   │   │       ├── StoreServicesExamples.csproj
    │   │   │   │       ├── StoreServicesExamples.sln
    │   │   │   │       └── Properties/
    │   │   │   │           └── AssemblyInfo.cs
    │   │   │   ├── StoreServicesExamples_Promotions/
    │   │   │   │   └── cs/
    │   │   │   │       ├── App.config
    │   │   │   │       ├── Program.cs
    │   │   │   │       ├── StoreServicesExamples.csproj
    │   │   │   │       ├── StoreServicesExamples.sln
    │   │   │   │       └── Properties/
    │   │   │   │           └── AssemblyInfo.cs
    │   │   │   ├── StoreServicesExamples_Submission/
    │   │   │   │   ├── cs/
    │   │   │   │   │   ├── App.config
    │   │   │   │   │   ├── AppSubmissionUpdateSample.cs
    │   │   │   │   │   ├── ClientConfiguration.cs
    │   │   │   │   │   ├── FlightSubmissionUpdateSample.cs
    │   │   │   │   │   ├── InAppProductSubmissionCreateSample.cs
    │   │   │   │   │   ├── InAppProductSubmissionUpdateSample.cs
    │   │   │   │   │   ├── IngestionClient.cs
    │   │   │   │   │   ├── Program.cs
    │   │   │   │   │   ├── StoreServicesExamples_Submission.csproj
    │   │   │   │   │   ├── StoreServicesExamples_Submission.sln
    │   │   │   │   │   └── Properties/
    │   │   │   │   │       └── AssemblyInfo.cs
    │   │   │   │   ├── java/
    │   │   │   │   │   ├── CompleteExample.java
    │   │   │   │   │   └── MainExample.java
    │   │   │   │   └── python/
    │   │   │   │       └── Examples.py
    │   │   │   ├── StoreServicesExamples_SubmissionAdvancedListings/
    │   │   │   │   ├── cs/
    │   │   │   │   │   ├── CreateAndSubmitSubmissionExample.cs
    │   │   │   │   │   ├── DevCenterAccessTokenClient.cs
    │   │   │   │   │   └── DevCenterClient.cs
    │   │   │   │   ├── java/
    │   │   │   │   │   ├── CreateAndSubmitSubmissionExample.java
    │   │   │   │   │   ├── DevCenterAccessTokenClient.java
    │   │   │   │   │   └── DevCenterClient.java
    │   │   │   │   └── python/
    │   │   │   │       ├── CreateAndSubmitAppSubmissionExample.py
    │   │   │   │       ├── devcenterclient.py
    │   │   │   │       └── submissiondatasamples.py
    │   │   │   └── StoreServicesExamples_TargetedOffers/
    │   │   │       └── cs/
    │   │   │           └── TargetedOffers.cs
    │   │   └── images/
    │   │       ├── b2b-1.PNG
    │   │       ├── b2b-1.vsdx
    │   │       ├── b2b-2.vsdx
    │   │       └── feedback_icon.PNG
    │   ├── networking/
    │   │   ├── background-transfers.md
    │   │   ├── httpclient.md
    │   │   ├── index.md
    │   │   ├── network-communications-in-the-background.md
    │   │   ├── networking-basics.md
    │   │   ├── sockets.md
    │   │   ├── web-feeds.md
    │   │   ├── websockets.md
    │   │   ├── which-networking-technology.md
    │   │   └── code/
    │   │       └── backgroundtransfer/
    │   │           ├── download_quickstart/
    │   │           │   └── js/
    │   │           │       └── main.js
    │   │           ├── download_quickstartcs/
    │   │           │   └── cs/
    │   │           │       ├── main.cs
    │   │           │       └── main.xaml.cs
    │   │           └── upload_quickstart/
    │   │               └── js/
    │   │                   └── main.js
    │   ├── packaging/
    │   │   ├── app-capability-declarations.md
    │   │   ├── auto-build-package-uwp-apps.md
    │   │   ├── index.md
    │   │   ├── install-universal-windows-apps-with-the-winappdeploycmd-tool.md
    │   │   └── self-install-package-updates.md
    │   ├── porting/
    │   │   ├── desktop-to-uwp-migrate.md
    │   │   ├── index.md
    │   │   ├── w8x-to-uwp-case-study-bookstore1.md
    │   │   ├── w8x-to-uwp-case-study-bookstore2.md
    │   │   ├── w8x-to-uwp-case-study-quizgame.md
    │   │   ├── w8x-to-uwp-input-and-sensors.md
    │   │   ├── w8x-to-uwp-porting-to-a-uwp-project.md
    │   │   ├── w8x-to-uwp-porting-xaml-and-ui.md
    │   │   ├── w8x-to-uwp-root.md
    │   │   ├── w8x-to-uwp-troubleshooting.md
    │   │   ├── wpsl-to-uwp-business-and-data.md
    │   │   ├── wpsl-to-uwp-case-study-bookstore1.md
    │   │   ├── wpsl-to-uwp-case-study-bookstore2.md
    │   │   ├── wpsl-to-uwp-form-factors-and-ux.md
    │   │   ├── wpsl-to-uwp-input-and-sensors.md
    │   │   ├── wpsl-to-uwp-namespace-and-class-mappings.md
    │   │   ├── wpsl-to-uwp-porting-to-a-uwp-project.md
    │   │   ├── wpsl-to-uwp-porting-xaml-and-ui.md
    │   │   ├── wpsl-to-uwp-root.md
    │   │   └── wpsl-to-uwp-troubleshooting.md
    │   ├── security/
    │   │   ├── authentication-and-user-identity.md
    │   │   ├── certificates.md
    │   │   ├── common-cryptography-tasks.md
    │   │   ├── companion-device-unlock.md
    │   │   ├── compare-buffers.md
    │   │   ├── convert-between-strings-and-binary-data.md
    │   │   ├── copy-to-and-from-byte-arrays.md
    │   │   ├── create-random-numbers.md
    │   │   ├── cryptographic-keys.md
    │   │   ├── cryptography.md
    │   │   ├── data-protection.md
    │   │   ├── encode-and-decode-data.md
    │   │   ├── export-restrictions-on-cryptography.md
    │   │   ├── index.md
    │   │   ├── intro-to-secure-windows-app-development.md
    │   │   ├── macs-hashes-and-signatures.md
    │   │   ├── share-certificates.md
    │   │   ├── web-account-manager.md
    │   │   ├── web-authentication-broker.md
    │   │   └── code/
    │   │       └── token-broker/
    │   │           ├── App.xaml
    │   │           ├── App.xaml.cs
    │   │           ├── MainPage.xaml
    │   │           ├── MainPage.xaml.cs
    │   │           ├── Package.appxmanifest
    │   │           ├── Package.StoreAssociation.xml
    │   │           ├── project.json
    │   │           ├── token-broker.csproj
    │   │           ├── token-broker.sln
    │   │           ├── .gitignore
    │   │           └── Properties/
    │   │               ├── AssemblyInfo.cs
    │   │               └── Default.rd.xml
    │   ├── threading-async/
    │   │   ├── asynchronous-programming-in-cpp-universal-windows-platform-apps.md
    │   │   ├── asynchronous-programming-universal-windows-platform-apps.md
    │   │   ├── best-practices-for-using-the-thread-pool.md
    │   │   ├── call-asynchronous-apis-in-csharp-or-visual-basic.md
    │   │   ├── create-a-periodic-work-item.md
    │   │   ├── index.md
    │   │   ├── submit-a-work-item-to-the-thread-pool.md
    │   │   ├── use-a-timer-to-submit-a-work-item.md
    │   │   ├── using-windows-runtime-objects-in-a-multithreaded-environment.md
    │   │   └── AsyncSnippets/
    │   │       ├── csharp/
    │   │       │   ├── App.xaml
    │   │       │   ├── App.xaml.cs
    │   │       │   ├── AsyncSnippets.csproj
    │   │       │   ├── MainPage.xaml
    │   │       │   ├── MainPage.xaml.cs
    │   │       │   ├── Package.appxmanifest
    │   │       │   └── Properties/
    │   │       │       └── AssemblyInfo.cs
    │   │       ├── metadata/
    │   │       │   └── creator.txt
    │   │       └── vbnet/
    │   │           ├── App.xaml
    │   │           ├── App.xaml.vb
    │   │           ├── MainPage.xaml
    │   │           ├── MainPage.xaml.vb
    │   │           ├── Package.appxmanifest
    │   │           ├── VBAsync.vbproj
    │   │           ├── Common/
    │   │           │   └── StandardStyles.xaml
    │   │           └── My Project/
    │   │               └── AssemblyInfo.vb
    │   ├── ui-input/
    │   │   ├── app-navigation.md
    │   │   ├── app-window.md
    │   │   ├── application-view.md
    │   │   ├── back-navigation.md
    │   │   ├── index.md
    │   │   ├── mica-uwp.md
    │   │   ├── reveal-focus.md
    │   │   ├── show-multiple-views.md
    │   │   └── title-bar.md
    │   ├── updates-and-versions/
    │   │   ├── application-development-for-windows-as-a-service.md
    │   │   └── choose-a-uwp-version.md
    │   ├── whats-new/
    │   │   ├── experimental-apis.md
    │   │   ├── toc.yml
    │   │   ├── windows-10-build-10240.md
    │   │   ├── windows-10-build-10586.md
    │   │   ├── windows-10-build-14393-api-diff.md
    │   │   ├── windows-10-build-14393.md
    │   │   ├── windows-10-build-15063-api-diff.md
    │   │   ├── windows-10-build-15063.md
    │   │   ├── windows-10-build-16299-api-diff.md
    │   │   ├── windows-10-build-16299.md
    │   │   ├── windows-10-build-17134-api-diff.md
    │   │   ├── windows-10-build-17134.md
    │   │   ├── windows-10-build-17763-api-diff.md
    │   │   ├── windows-10-build-17763.md
    │   │   ├── windows-10-build-18362-api-diff.md
    │   │   ├── windows-10-build-18362.md
    │   │   ├── windows-10-build-19041-api-diff.md
    │   │   ├── windows-10-build-19041.md
    │   │   └── images/
    │   │       └── windows-learn.PNG
    │   ├── winrt-components/
    │   │   ├── create-a-windows-runtime-component-in-cppwinrt.md
    │   │   ├── creating-windows-runtime-components-in-cpp.md
    │   │   ├── creating-windows-runtime-components-in-csharp-and-visual-basic.md
    │   │   ├── custom-events-and-event-accessors-in-windows-runtime-components.md
    │   │   ├── diagnosing-windows-runtime-component-error-conditions.md
    │   │   ├── distributing-a-managed-windows-runtime-component.md
    │   │   ├── index.md
    │   │   ├── net-framework-mappings-of-windows-runtime-types.md
    │   │   ├── passing-arrays-to-a-windows-runtime-component.md
    │   │   ├── raising-events-in-windows-runtime-components.md
    │   │   ├── walkthrough-creating-a-basic-windows-runtime-component-in-cpp-and-calling-it-from-javascript-or-csharp.md
    │   │   └── walkthrough-creating-a-simple-windows-runtime-component-and-calling-it-from-javascript.md
    │   ├── xaml-platform/
    │   │   ├── attached-properties-overview.md
    │   │   ├── binding-markup-extension.md
    │   │   ├── custom-attached-properties.md
    │   │   ├── custom-dependency-properties.md
    │   │   ├── customresource-markup-extension.md
    │   │   ├── dependency-properties-overview.md
    │   │   ├── events-and-routed-events-overview.md
    │   │   ├── index.md
    │   │   ├── move-draw-commands-syntax.md
    │   │   ├── property-path-syntax.md
    │   │   ├── relativesource-markup-extension.md
    │   │   ├── staticresource-markup-extension.md
    │   │   ├── template-settings-classes.md
    │   │   ├── templatebinding-markup-extension.md
    │   │   ├── themeresource-markup-extension.md
    │   │   ├── x-bind-markup-extension.md
    │   │   ├── x-class-attribute.md
    │   │   ├── x-defaultbindmode-attribute.md
    │   │   ├── x-deferloadstrategy-attribute.md
    │   │   ├── x-fieldmodifier-attribute.md
    │   │   ├── x-key-attribute.md
    │   │   ├── x-load-attribute.md
    │   │   ├── x-name-attribute.md
    │   │   ├── x-null-markup-extension.md
    │   │   ├── x-phase-attribute.md
    │   │   ├── x-uid-directive.md
    │   │   ├── xaml-and-whitespace.md
    │   │   ├── xaml-intrinsic-data-types.md
    │   │   ├── xaml-namescopes.md
    │   │   ├── xaml-namespaces-and-namespace-mapping.md
    │   │   ├── xaml-overview.md
    │   │   └── xaml-syntax-guide.md
    │   └── xbox-apps/
    │       └── frequently-asked-questions.yml
    ├── windows-apps-src/
    │   ├── develop/
    │   │   └── index.md
    │   └── porting/
    │       └── index.md
    └── .github/
        └── ISSUE_TEMPLATE/
            ├── 0-customer-feedback-repo.yml
            ├── 1-customer-feedback.yml
            └── config.yml


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
## Rename Notification
This repo has recently been renamed from "windows-uwp" to "windows-dev-docs" to better represent the content source files contained.

If you have a copy of the repo on your local machine, you will need to update the associated URL following these steps:

1. `cd` to your local Git directory for the repo and find the remote name with the command: `git remote -v`

You will receive a response like the following example:
`origin  https://github.com/MicrosoftDocs/windows-uwp.git (fetch)`
`origin  https://github.com/MicrosoftDocs/windows-uwp.git (push)`

2. Set the new URL using the command:
`git remote set-url origin https://github.com/MicrosoftDocs/windows-dev-docs.git`

*Alternatively, you can just delete your local copy of the repo and reclone it if you don't have any active work on the repo that you are concerned with losing.

Following the rename of this repo, the content team will also be working on renaming and restructuring the source file directories within the repo to align more closely with the structure of our live documentation. We are aiming to have this work complete by September 16, 2022.

## Legal Notices
Microsoft and any contributors grant you a license to the Microsoft documentation and other content
in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode),
see the [LICENSE](LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT). See the
[LICENSE-CODE](LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure, and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at https://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all others rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel, or otherwise.



================================================
FILE: auto-publish.yml
================================================


trigger:
- main

jobs:
- job: MergeMainToLive
  pool:
    vmImage: 'ubuntu-latest'
  steps:
  - checkout: self
    persistCredentials: true
  - script: |
      git config --global user.name "Quinn Radich"
      git config --global user.email "quinnradich@users.noreply.github.com"
      git checkout main
      git checkout live
      git merge main --no-ff --no-commit
      if [ $? -eq 0 ]; then
        git commit -m "Merged main into live"
        git push origin live
      else
        echo "Error merging main to live"
        exit 1
      fi
    displayName: 'Merge main to live if main has changed'



================================================
FILE: CONTRIBUTING.md
================================================
# Contributing to this documentation

Thank you for your interest in contributing to our documentation! We appreciate your feedback, edits, and additions to our docs. Please see the [Microsoft Learn documentation contributor guide](https://learn.microsoft.com/contribute/) for information on how to do quick edits, get a local contribution environment set up, review open pull requests, and create quality issues, along with some "Microsoft writing essentials", the Learn site authoring pack for VS Code, and info about Hacktoberfest.

## Internal contributions

If you are a Microsoft employee, please contribute through the [private content repository](https://github.com/microsoftdocs/windows-dev-docs-pr).



================================================
FILE: LICENSE
================================================
Attribution 4.0 International

=======================================================================

Creative Commons Corporation ("Creative Commons") is not a law firm and
does not provide legal services or legal advice. Distribution of
Creative Commons public licenses does not create a lawyer-client or
other relationship. Creative Commons makes its licenses and related
information available on an "as-is" basis. Creative Commons gives no
warranties regarding its licenses, any material licensed under their
terms and conditions, or any related information. Creative Commons
disclaims all liability for damages resulting from their use to the
fullest extent possible.

Using Creative Commons Public Licenses

Creative Commons public licenses provide a standard set of terms and
conditions that creators and other rights holders may use to share
original works of authorship and other material subject to copyright
and certain other rights specified in the public license below. The
following considerations are for informational purposes only, are not
exhaustive, and do not form part of our licenses.

     Considerations for licensors: Our public licenses are
     intended for use by those authorized to give the public
     permission to use material in ways otherwise restricted by
     copyright and certain other rights. Our licenses are
     irrevocable. Licensors should read and understand the terms
     and conditions of the license they choose before applying it.
     Licensors should also secure all rights necessary before
     applying our licenses so that the public can reuse the
     material as expected. Licensors should clearly mark any
     material not subject to the license. This includes other CC-
     licensed material, or material used under an exception or
     limitation to copyright. More considerations for licensors:
	wiki.creativecommons.org/Considerations_for_licensors

     Considerations for the public: By using one of our public
     licenses, a licensor grants the public permission to use the
     licensed material under specified terms and conditions. If
     the licensor's permission is not necessary for any reason--for
     example, because of any applicable exception or limitation to
     copyright--then that use is not regulated by the license. Our
     licenses grant only permissions under copyright and certain
     other rights that a licensor has authority to grant. Use of
     the licensed material may still be restricted for other
     reasons, including because others have copyright or other
     rights in the material. A licensor may make special requests,
     such as asking that all changes be marked or described.
     Although not required by our licenses, you are encouraged to
     respect those requests where reasonable. More_considerations
     for the public:
	wiki.creativecommons.org/Considerations_for_licensees

=======================================================================

Creative Commons Attribution 4.0 International Public License

By exercising the Licensed Rights (defined below), You accept and agree
to be bound by the terms and conditions of this Creative Commons
Attribution 4.0 International Public License ("Public License"). To the
extent this Public License may be interpreted as a contract, You are
granted the Licensed Rights in consideration of Your acceptance of
these terms and conditions, and the Licensor grants You such rights in
consideration of benefits the Licensor receives from making the
Licensed Material available under these terms and conditions.


Section 1 -- Definitions.

  a. Adapted Material means material subject to Copyright and Similar
     Rights that is derived from or based upon the Licensed Material
     and in which the Licensed Material is translated, altered,
     arranged, transformed, or otherwise modified in a manner requiring
     permission under the Copyright and Similar Rights held by the
     Licensor. For purposes of this Public License, where the Licensed
     Material is a musical work, performance, or sound recording,
     Adapted Material is always produced where the Licensed Material is
     synched in timed relation with a moving image.

  b. Adapter's License means the license You apply to Your Copyright
     and Similar Rights in Your contributions to Adapted Material in
     accordance with the terms and conditions of this Public License.

  c. Copyright and Similar Rights means copyright and/or similar rights
     closely related to copyright including, without limitation,
     performance, broadcast, sound recording, and Sui Generis Database
     Rights, without regard to how the rights are labeled or
     categorized. For purposes of this Public License, the rights
     specified in Section 2(b)(1)-(2) are not Copyright and Similar
     Rights.

  d. Effective Technological Measures means those measures that, in the
     absence of proper authority, may not be circumvented under laws
     fulfilling obligations under Article 11 of the WIPO Copyright
     Treaty adopted on December 20, 1996, and/or similar international
     agreements.

  e. Exceptions and Limitations means fair use, fair dealing, and/or
     any other exception or limitation to Copyright and Similar Rights
     that applies to Your use of the Licensed Material.

  f. Licensed Material means the artistic or literary work, database,
     or other material to which the Licensor applied this Public
     License.

  g. Licensed Rights means the rights granted to You subject to the
     terms and conditions of this Public License, which are limited to
     all Copyright and Similar Rights that apply to Your use of the
     Licensed Material and that the Licensor has authority to license.

  h. Licensor means the individual(s) or entity(ies) granting rights
     under this Public License.

  i. Share means to provide material to the public by any means or
     process that requires permission under the Licensed Rights, such
     as reproduction, public display, public performance, distribution,
     dissemination, communication, or importation, and to make material
     available to the public including in ways that members of the
     public may access the material from a place and at a time
     individually chosen by them.

  j. Sui Generis Database Rights means rights other than copyright
     resulting from Directive 96/9/EC of the European Parliament and of
     the Council of 11 March 1996 on the legal protection of databases,
     as amended and/or succeeded, as well as other essentially
     equivalent rights anywhere in the world.

  k. You means the individual or entity exercising the Licensed Rights
     under this Public License. Your has a corresponding meaning.


Section 2 -- Scope.

  a. License grant.

       1. Subject to the terms and conditions of this Public License,
          the Licensor hereby grants You a worldwide, royalty-free,
          non-sublicensable, non-exclusive, irrevocable license to
          exercise the Licensed Rights in the Licensed Material to:

            a. reproduce and Share the Licensed Material, in whole or
               in part; and

            b. produce, reproduce, and Share Adapted Material.

       2. Exceptions and Limitations. For the avoidance of doubt, where
          Exceptions and Limitations apply to Your use, this Public
          License does not apply, and You do not need to comply with
          its terms and conditions.

       3. Term. The term of this Public License is specified in Section
          6(a).

       4. Media and formats; technical modifications allowed. The
          Licensor authorizes You to exercise the Licensed Rights in
          all media and formats whether now known or hereafter created,
          and to make technical modifications necessary to do so. The
          Licensor waives and/or agrees not to assert any right or
          authority to forbid You from making technical modifications
          necessary to exercise the Licensed Rights, including
          technical modifications necessary to circumvent Effective
          Technological Measures. For purposes of this Public License,
          simply making modifications authorized by this Section 2(a)
          (4) never produces Adapted Material.

       5. Downstream recipients.

            a. Offer from the Licensor -- Licensed Material. Every
               recipient of the Licensed Material automatically
               receives an offer from the Licensor to exercise the
               Licensed Rights under the terms and conditions of this
               Public License.

            b. No downstream restrictions. You may not offer or impose
               any additional or different terms or conditions on, or
               apply any Effective Technological Measures to, the
               Licensed Material if doing so restricts exercise of the
               Licensed Rights by any recipient of the Licensed
               Material.

       6. No endorsement. Nothing in this Public License constitutes or
          may be construed as permission to assert or imply that You
          are, or that Your use of the Licensed Material is, connected
          with, or sponsored, endorsed, or granted official status by,
          the Licensor or others designated to receive attribution as
          provided in Section 3(a)(1)(A)(i).

  b. Other rights.

       1. Moral rights, such as the right of integrity, are not
          licensed under this Public License, nor are publicity,
          privacy, and/or other similar personality rights; however, to
          the extent possible, the Licensor waives and/or agrees not to
          assert any such rights held by the Licensor to the limited
          extent necessary to allow You to exercise the Licensed
          Rights, but not otherwise.

       2. Patent and trademark rights are not licensed under this
          Public License.

       3. To the extent possible, the Licensor waives any right to
          collect royalties from You for the exercise of the Licensed
          Rights, whether directly or through a collecting society
          under any voluntary or waivable statutory or compulsory
          licensing scheme. In all other cases the Licensor expressly
          reserves any right to collect such royalties.


Section 3 -- License Conditions.

Your exercise of the Licensed Rights is expressly made subject to the
following conditions.

  a. Attribution.

       1. If You Share the Licensed Material (including in modified
          form), You must:

            a. retain the following if it is supplied by the Licensor
               with the Licensed Material:

                 i. identification of the creator(s) of the Licensed
                    Material and any others designated to receive
                    attribution, in any reasonable manner requested by
                    the Licensor (including by pseudonym if
                    designated);

                ii. a copyright notice;

               iii. a notice that refers to this Public License;

                iv. a notice that refers to the disclaimer of
                    warranties;

                 v. a URI or hyperlink to the Licensed Material to the
                    extent reasonably practicable;

            b. indicate if You modified the Licensed Material and
               retain an indication of any previous modifications; and

            c. indicate the Licensed Material is licensed under this
               Public License, and include the text of, or the URI or
               hyperlink to, this Public License.

       2. You may satisfy the conditions in Section 3(a)(1) in any
          reasonable manner based on the medium, means, and context in
          which You Share the Licensed Material. For example, it may be
          reasonable to satisfy the conditions by providing a URI or
          hyperlink to a resource that includes the required
          information.

       3. If requested by the Licensor, You must remove any of the
          information required by Section 3(a)(1)(A) to the extent
          reasonably practicable.

       4. If You Share Adapted Material You produce, the Adapter's
          License You apply must not prevent recipients of the Adapted
          Material from complying with this Public License.


Section 4 -- Sui Generis Database Rights.

Where the Licensed Rights include Sui Generis Database Rights that
apply to Your use of the Licensed Material:

  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
     to extract, reuse, reproduce, and Share all or a substantial
     portion of the contents of the database;

  b. if You include all or a substantial portion of the database
     contents in a database in which You have Sui Generis Database
     Rights, then the database in which You have Sui Generis Database
     Rights (but not its individual contents) is Adapted Material; and

  c. You must comply with the conditions in Section 3(a) if You Share
     all or a substantial portion of the contents of the database.

For the avoidance of doubt, this Section 4 supplements and does not
replace Your obligations under this Public License where the Licensed
Rights include other Copyright and Similar Rights.


Section 5 -- Disclaimer of Warranties and Limitation of Liability.

  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.

  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.

  c. The disclaimer of warranties and limitation of liability provided
     above shall be interpreted in a manner that, to the extent
     possible, most closely approximates an absolute disclaimer and
     waiver of all liability.


Section 6 -- Term and Termination.

  a. This Public License applies for the term of the Copyright and
     Similar Rights licensed here. However, if You fail to comply with
     this Public License, then Your rights under this Public License
     terminate automatically.

  b. Where Your right to use the Licensed Material has terminated under
     Section 6(a), it reinstates:

       1. automatically as of the date the violation is cured, provided
          it is cured within 30 days of Your discovery of the
          violation; or

       2. upon express reinstatement by the Licensor.

     For the avoidance of doubt, this Section 6(b) does not affect any
     right the Licensor may have to seek remedies for Your violations
     of this Public License.

  c. For the avoidance of doubt, the Licensor may also offer the
     Licensed Material under separate terms or conditions or stop
     distributing the Licensed Material at any time; however, doing so
     will not terminate this Public License.

  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
     License.


Section 7 -- Other Terms and Conditions.

  a. The Licensor shall not be bound by any additional or different
     terms or conditions communicated by You unless expressly agreed.

  b. Any arrangements, understandings, or agreements regarding the
     Licensed Material not stated herein are separate from and
     independent of the terms and conditions of this Public License.


Section 8 -- Interpretation.

  a. For the avoidance of doubt, this Public License does not, and
     shall not be interpreted to, reduce, limit, restrict, or impose
     conditions on any use of the Licensed Material that could lawfully
     be made without permission under this Public License.

  b. To the extent possible, if any provision of this Public License is
     deemed unenforceable, it shall be automatically reformed to the
     minimum extent necessary to make it enforceable. If the provision
     cannot be reformed, it shall be severed from this Public License
     without affecting the enforceability of the remaining terms and
     conditions.

  c. No term or condition of this Public License will be waived and no
     failure to comply consented to unless expressly agreed to by the
     Licensor.

  d. Nothing in this Public License constitutes or may be interpreted
     as a limitation upon, or waiver of, any privileges and immunities
     that apply to the Licensor or You, including from the legal
     processes of any jurisdiction or authority.


=======================================================================

Creative Commons is not a party to its public
licenses. Notwithstanding, Creative Commons may elect to apply one of
its public licenses to material it publishes and in those instances
will be considered the “Licensor.” The text of the Creative Commons
public licenses is dedicated to the public domain under the CC0 Public
Domain Dedication. Except for the limited purpose of indicating that
material is shared under a Creative Commons public license or as
otherwise permitted by the Creative Commons policies published at
creativecommons.org/policies, Creative Commons does not authorize the
use of the trademark "Creative Commons" or any other trademark or logo
of Creative Commons without its prior written consent including,
without limitation, in connection with any unauthorized modifications
to any of its public licenses or any other arrangements,
understandings, or agreements concerning use of licensed material. For
the avoidance of doubt, this paragraph does not form part of the
public licenses.

Creative Commons may be contacted at creativecommons.org.


================================================
FILE: LICENSE-CODE
================================================
The MIT License (MIT)
Copyright (c) Microsoft Corporation

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial
portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


================================================
FILE: master-branch-inf.txt
================================================
This file indicates the source of the current branch's content.


================================================
FILE: SECURITY.md
================================================
<!-- BEGIN MICROSOFT SECURITY.MD V0.0.8 BLOCK -->

## Security

Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [our GitHub organizations](https://opensource.microsoft.com/).

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
FILE: ThirdPartyNotices
================================================
##Legal Notices
Microsoft and any contributors grant you a license to the Microsoft documentation and other content
in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode),
see the [LICENSE](LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the
[LICENSE-CODE](LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all others rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel or otherwise.


================================================
FILE: .localization-config
================================================
{
  "locales": [ "ja-jp", "de-de", "fr-fr", "zh-cn", "zh-tw", "ko-kr", "es-es", "it-it", "ru-ru", "pt-br" ],
  "files": ["!/*.md", "**/**/*.md", "**/*.md"],
  "includeDependencies": false,
  "autoPush": true,
  "xliffVersion": "2.0",
  "useJavascriptMarkdownTransformer": true,
  "markdownTransformerOptions": {
  	"lockBackslashEscapeChars": false,
    "linkifyHeaders": true
  }
}



================================================
FILE: .openpublishing.publish.config.json
================================================
{
  "build_entry_point": "op",
  "docsets_to_publish": [
    {
      "docset_name": "windows-uwp",
      "build_source_folder": "uwp",
      "build_output_subfolder": "uwp",
      "locale": "en-us",
      "xref_query_tags": [
        "/uwp/api",
        "/dotnet"
      ],
      "open_to_public_contributors": true,
      "type_mapping": {
        "ZonePivotGroups": "Toc",
        "Conceptual": "Content",
        "ManagedReference": "Content",
        "RestApi": "Content"
      },
      "build_entry_point": "docs",
      "template_folder": "_themes",
      "is_dynamic_rendering": false,
      "version": 0
    },
    {
      "docset_name": "windows-uwp-arm",
      "build_source_folder": "landing/arm-docs",
      "build_output_subfolder": "arm",
      "locale": "en-us",
      "monikers": [],
      "moniker_ranges": [],
      "xref_query_tags": [
        "/uwp/api"
      ],
      "open_to_public_contributors": true,
      "type_mapping": {
        "ZonePivotGroups": "Toc",
        "Conceptual": "Content",
        "ManagedReference": "Content",
        "RestApi": "Content"
      },
      "build_entry_point": "docs",
      "template_folder": "_themes"
    },
    {
      "docset_name": "windows-uwp-hub",
      "build_source_folder": "hub",
      "build_output_subfolder": "hub",
      "locale": "en-us",
      "xref_query_tags": [
        "/uwp/api"
      ],
      "open_to_public_contributors": true,
      "type_mapping": {
        "ZonePivotGroups": "Toc",
        "Conceptual": "Content",
        "ManagedReference": "Content",
        "RestApi": "Content"
      },
      "build_entry_point": "docs",
      "template_folder": "_themes",
      "is_dynamic_rendering": false,
      "version": 0
    }
  ],
  "notification_subscribers": [],
  "sync_notification_subscribers": [
    "jkendir@microsoft.com"
  ],
  "branches_to_filter": [],
  "git_repository_url_open_to_public_contributors": "https://github.com/MicrosoftDocs/windows-dev-docs",
  "git_repository_branch_open_to_public_contributors": "docs",
  "need_preview_pull_request": true,
  "resolve_user_profile_using_github": true,
  "dependent_repositories": [
    {
      "path_to_root": "_themes",
      "url": "https://github.com/Microsoft/templates.docs.msft",
      "branch": "main",
      "branch_mapping": {}
    },
    {
      "path_to_root": "samples-xaml-gallery",
      "url": "https://github.com/microsoft/Xaml-Controls-Gallery",
      "branch": "master",
      "branch_mapping": {}
    },
    {
      "path_to_root": "snippets-windows",
      "url": "https://github.com/MicrosoftDocs/windows-code-snippets-pr",
      "branch": "master",
      "branch_mapping": {}
    },
    {
      "path_to_root": "_themes.pdf",
      "url": "https://github.com/Microsoft/templates.docs.msft.pdf",
      "branch": "main",
      "branch_mapping": {}
    }
  ],
  "branch_target_mapping": {
    "live": [
      "Publish",
      "Pdf"
    ]
  },
  "targets": {
    "pdf": {
      "template_folder": "_themes.pdf"
    }
  },
  "docs_build_engine": {},
  "skip_source_output_uploading": false,
  "contribution_branch_mappings": {},
  "need_generate_pdf_url_template": true,
  "need_generate_pdf": false
}


================================================
FILE: .openpublishing.redirection.json
================================================
{
  "redirections": [
	{
		"source_path": "hub/apps/whats-new/latest-docs-updates.md",
		"redirect_url": "https://learn.microsoft.com/windows/apps/whats-new/windows-11-build-22000",
		"redirect_document_id": false
	  },
	  {
      "source_path": "hub/apps/design/devices/kinect-for-windows.md",
      "redirect_url": "https://azure.microsoft.com/en-us/products/kinect-dk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/automate-launching-uwp-apps.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/automate-launching-uwp-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/cpusets-games.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/cpusets-games",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/dev-home.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/dev-home",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-environment-setup.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-environment-setup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-lanes-custom-cpp.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-lanes-custom-cpp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-lanes-html.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-lanes-html",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-lanes-landing.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-lanes-landing",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-lanes-unity-versioning.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-lanes-unity-versioning",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/development-lanes-unity.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/development-lanes-unity",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-capture.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-capture",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-home.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-home",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-live.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-live",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-networking.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-networking",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-performance.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-performance",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devhome-settings.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devhome-settings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/device-portal-xbox.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/device-portal-xbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devkit-activation.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devkit-activation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/devkit-deactivation.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/devkit-deactivation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/disable-scaling.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/disable-scaling",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/getting-started.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/getting-started",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/how-to-disable-mouse-mode.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/how-to-disable-mouse-mode",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/index.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/introduction-to-xbox-tools.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/introduction-to-xbox-tools",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/known-issues.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/known-issues",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/multi-user-applications.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/multi-user-applications",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/reference.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/reference",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/samples-xaml-dev.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/samples-xaml-dev",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/samples-xaml-media.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/samples-xaml-media",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/samples.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/samples",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/system-resource-allocation.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/system-resource-allocation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/tailoring-for-xbox.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/tailoring-for-xbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/turn-off-overscan.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/turn-off-overscan",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-deployinfo-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-deployinfo-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-fiddler.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-fiddler",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-networkcredentials-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-networkcredentials-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-remoteinput-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-remoteinput-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-remoteinput-controllers-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-remoteinput-controllers-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/uwp-sshpins-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/uwp-sshpins-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/ves-on-xbox.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/ves-on-xbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-fiddler-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-fiddler-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-folder-upload.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-folder-upload",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-httpMonitor-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-httpMonitor-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-loose-folder-register-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-loose-folder-register-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-media-capture-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-media-capture-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-sandbox-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-sandbox-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-smb-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-smb-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-user-management.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-user-management",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-xboxinfo-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-xboxinfo-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/wdp-xboxsettings-api.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/wdp-xboxsettings-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/whats-new.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-apps/xbox-dev-mode-companion.md",
      "redirect_url": "/previous-versions/windows/uwp/xbox-apps/xbox-dev-mode-companion",
      "redirect_document_id": false
    },
  {
      "source_path": "uwp/whats-new/windows-docs-august-2017.md",
      "redirect_url": "/windows/uwp/",
      "redirect_document_id": false
  },
  {
		"source_path": "uwp/whats-new/windows-docs-august-2018.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-december-2017.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-february-2018.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-january-2019.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-july-2017.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-july-2018.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-may-2018.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-september-2017.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
	{
		"source_path": "uwp/whats-new/windows-docs-september-2018.md",
		"redirect_url": "/windows/uwp/",
		"redirect_document_id": false
	},
    {
      "source_path": "uwp/monetize/get-xbox-live-analytics.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-achievements-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-health-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-game-hub-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-club-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-multiplayer-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-live-concurrent-usage-data.md",
      "redirect_url": "/windows/uwp/publish/xbox-analytics-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/debug-test-perf/device-portal-hololens.md",
      "redirect_url": "/windows/mixed-reality/develop/platform-capabilities-and-apis/using-the-windows-device-portal",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/debug-test-perf/device-portal-api-hololens.md",
      "redirect_url": "/windows/mixed-reality/develop/platform-capabilities-and-apis/device-portal-api-reference",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-uwp-app-samples.md",
      "redirect_url": "/windows/apps/get-started/samples",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/home.md",
      "redirect_url": "/windows/uwp/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/app-to-app/use-edp-to-protect-enterprise-data-transferred-between-apps.md",
      "redirect_url": "/windows/uwp/enterprise/wip-dev-guide",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/audio-video-camera/capture-photos-and-video-with-mediacapture.md",
      "redirect_url": "/windows/uwp/audio-video-camera/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/contacts-and-calendar/integrating-social-feeds-into-contact-cards.md",
      "redirect_url": "/windows/uwp/contacts-and-calendar",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/dialogs-popups-menus.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/dialogs-and-flyouts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/nav-pane.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/navigationview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/segoe-ui-symbol-font.md",
      "redirect_url": "/windows/uwp/design/style/segoe-ui-symbol-font",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/spell-checking-and-prediction.md",
      "redirect_url": "/windows/uwp/controls-and-patterns/text-controls",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/styling-controls.md",
      "redirect_url": "/windows/uwp/controls-and-patterns/xaml-styles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/hub.md",
      "redirect_url": "/windows/uwp/design/basics/navigation-basics",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/files/protect-your-enterprise-data-with-edp.md",
      "redirect_url": "/windows/uwp/files/../enterprise/wip-dev-guide",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/files/use-edp-to-protect-streams-and-buffers.md",
      "redirect_url": "/windows/uwp/files/../enterprise/wip-dev-guide",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/application-development-for-windows-as-a-service.md",
      "redirect_url": "/windows/uwp/get-started/../updates-and-versions/application-development-for-windows-as-a-service/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/create-js-apps.md",
      "redirect_url": "/windows/uwp/get-started/your-first-app#javascript-and-html",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/radialcontroller-walkthrough.md",
      "redirect_url": "/windows/uwp/design/input/radialcontroller-walkthrough/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/ink-walkthrough.md",
      "redirect_url": "/windows/uwp/design/input/ink-walkthrough/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/xaml-basics-intro.md",
      "redirect_url": "/windows/uwp/design/basics/xaml-basics-ui",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/xaml-basics-ui.md",
      "redirect_url": "/windows/uwp/design/basics/xaml-basics-ui",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/xaml-basics-style.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/xaml-styles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/xaml-basics-adaptive-layout.md",
      "redirect_url": "/windows/uwp/design/basics/xaml-basics-adaptive-layout",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/xaml-basics-data-binding.md",
      "redirect_url": "/windows/uwp/data-binding/xaml-basics-data-binding",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/choose-a-uwp-version.md",
      "redirect_url": "/windows/uwp/get-started/../updates-and-versions/choose-a-uwp-version/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/enable-your-device-for-development.md",
      "redirect_url": "/windows/apps/get-started/enable-your-device-for-development",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/sign-up.md",
      "redirect_url": "/windows/apps/get-started/sign-up",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/adding-webvr-to-a-babylonjs-game.md",
      "redirect_url": "/windows/apps/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/create-a-hello-world-app-js-uwp.md",
      "redirect_url": "/windows/apps/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-started-tutorial-fullstack-web-app.md",
      "redirect_url": "/windows/uwp/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-started-tutorial-game-js2d.md",
      "redirect_url": "/windows/uwp/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-started-tutorial-game-js3d.md",
      "redirect_url": "/windows/uwp/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-started-tutorial-game-mg2d.md",
      "redirect_url": "/windows/uwp/get-started/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/composition-animation.md",
      "redirect_url": "/windows/uwp/composition/composition-animation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/composition-brushes.md",
      "redirect_url": "/windows/uwp/composition/composition-brushes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/composition-effects.md",
      "redirect_url": "/windows/uwp/composition/composition-effects",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/composition-native-interop.md",
      "redirect_url": "/windows/uwp/composition/composition-native-interop",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/composition-visual-tree.md",
      "redirect_url": "/windows/uwp/composition/composition-visual-tree",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/using-the-visual-layer-with-xaml.md",
      "redirect_url": "/windows/uwp/composition/using-the-visual-layer-with-xaml",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/visual-layer.md",
      "redirect_url": "/windows/uwp/composition/visual-layer",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-user-interaction.md",
      "redirect_url": "/windows/uwp/input-and-devices/touch-interactions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/layout/peer-to-peer-navigation-between-two-pages.md",
      "redirect_url": "/windows/uwp/layout/navigate-between-two-pages",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/maps-and-location/controls-map.md",
      "redirect_url": "/windows/uwp/maps-and-location/display-maps#display-map-in-a-control",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/maps-and-location/display-maps#map-control",
      "redirect_url": "/windows/uwp/maps-and-location/display-maps#display-map-in-a-control",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/adcontrol-error-handling.md",
      "redirect_url": "/windows/uwp/monetize/error-handling-in-xamlc-walkthrough",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/adcontrol-events-in-c.md",
      "redirect_url": "/windows/uwp/monetize/adcontrol-in-xaml-and--net",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/adcontrol-events-in-javascript.md",
      "redirect_url": "/windows/uwp/monetize/adcontrol-in-html-5-and-javascript",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/adcontrol-in-windows-phone-silverlight.md",
      "redirect_url": "/previous-versions/windows/apps/mt842563(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/add-ads-to-apps-with-microsoft-advertising.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/add-and-use-the-ad-mediator-control.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/additional-help.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app#additional-help",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/claim-a-targeted-offer.md",
      "redirect_url": "/windows/uwp/monetize/manage-targeted-offers-using-windows-store-services",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/code-samples.md",
      "redirect_url": "/windows/uwp/monetize/developer-walkthroughs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/create-an-adcontrol-in-javascript.md",
      "redirect_url": "/windows/uwp/monetize/adcontrol-in-html-5-and-javascript",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/developer-information.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/display-ads-using-the-microsoft-advertising-libraries.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-app-failures.md",
      "redirect_url": "/windows/uwp/monetize/get-error-reporting-data",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-started-with-microsoft-advertising-libraries.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/html-properties-example.md",
      "redirect_url": "/windows/uwp/monetize/adcontrol-in-html-5-and-javascript",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/important-notice-eula.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/install-the-microsoft-universal-ad-client-sdk.md",
      "redirect_url": "/windows/uwp/monetize/microsoft-store-services-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/migrate-from-admediatorcontrol-to-adcontrol.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/monetize-your-app-with-the-microsoft-store-engagement-and-monetization-sdk.md",
      "redirect_url": "/windows/uwp/monetize/microsoft-store-services-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/select-and-manage-your-ad-networks.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/submit-an-app-with-ads-to-the-windows-store.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/submit-your-app-and-configure-ad-mediation.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/supported-markets-for-microsoft-advertising.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/test-mode-values.md",
      "redirect_url": "/windows/uwp/monetize/set-up-ad-units-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/test-your-ad-mediation-implementation.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/troubleshoot-ad-mediation.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/troubleshooting-guides.md",
      "redirect_url": "/windows/uwp/monetize/known-issues-for-the-advertising-libraries",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/use-ad-mediation-to-maximize-revenue.md",
      "redirect_url": "/previous-versions/windows/apps/dn792120(v=win.10)",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/what-is-the-difference-admediatorcontrol-or-adcontrol.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/workflows-for-creating-apps-with-ads.md",
      "redirect_url": "/windows/uwp/monetize/display-ads-in-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/xaml-properties-example.md",
      "redirect_url": "/windows/uwp/monetize/adcontrol-in-xaml-and--net",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/networking/tagging_network_connections_with_edp_identity.md",
      "redirect_url": "/windows/uwp/networking/../enterprise/wip-dev-guide",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-deploy-and-debug.md",
      "redirect_url": "/windows/uwp/porting/desktop-to-uwp-debug",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-signing.md",
      "redirect_url": "/windows/uwp/porting/desktop-to-uwp-debug#test-your-app",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/update-your-visual-studio-2015-rc-project-to-rtm.md",
      "redirect_url": "/visualstudio/porting/port-migrate-and-upgrade-visual-studio-projects",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/about-affiliate-ads.md",
      "redirect_url": "/windows/uwp/publish/in-app-ads",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/ad-mediation-report.md",
      "redirect_url": "/windows/uwp/publish/advertising-performance-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/affiliates-performance-report.md",
      "redirect_url": "/windows/uwp/publish/advertising-performance-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/app-install-ads-reports.md",
      "redirect_url": "/windows/uwp/publish/ad-campaign-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/app-promotion-and-customer-engagement.md",
      "redirect_url": "/windows/uwp/publish/attract-customers-and-promote-your-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/channels-and-conversions-report.md",
      "redirect_url": "/windows/uwp/publish/acquisitions-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/create-add-on-descriptions.md",
      "redirect_url": "/windows/uwp/publish/create-app-store-listings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/create-app-descriptions.md",
      "redirect_url": "/windows/uwp/publish/create-app-store-listings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/create-iap-descriptions.md",
      "redirect_url": "/windows/uwp/publish/create-add-on-store-listings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/create-platform-specific-descriptions.md",
      "redirect_url": "/windows/uwp/publish/create-platform-specific-store-listings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/enter-iap-properties.md",
      "redirect_url": "/windows/uwp/publish/enter-add-on-properties",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/how-your-app-appears-in-the-store-for-windows-10-customers.md",
      "redirect_url": "/windows/uwp/publish/using-the-windows-dev-center-dashboard",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/iap-acquisitions-report.md",
      "redirect_url": "/windows/uwp/publish/add-on-acquisitions-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/iap-submissions.md",
      "redirect_url": "/windows/uwp/publish/add-on-submissions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/installs-report.md",
      "redirect_url": "/windows/uwp/publish/acquisitions-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/manage-iaps-in-bulk.md",
      "redirect_url": "/windows/uwp/publish/add-on-submissions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/microsoft-advertising-payment-process.md",
      "redirect_url": "/windows/uwp/publish/payout-summary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/monetize-with-ads.md",
      "redirect_url": "/windows/uwp/publish/in-app-ads",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/pubcenter-dev-center-integration.md",
      "redirect_url": "/windows/uwp/publish/in-app-ads",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/pubcenter-devcenter-payout-account-and-tax-profile-consolidation.md",
      "redirect_url": "/windows/uwp/publish/setting-up-your-payout-account-and-tax-forms",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/put-apps-and-iaps-on-sale.md",
      "redirect_url": "/windows/uwp/publish/put-apps-and-add-ons-on-sale",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/set-iap-pricing-and-availability.md",
      "redirect_url": "/windows/uwp/publish/set-add-on-pricing-and-availability",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/set-your-iap-product-id.md",
      "redirect_url": "/windows/uwp/publish/set-your-add-on-product-id",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/using-the-windows-dev-center-dashboard.md",
      "redirect_url": "/windows/uwp/publish/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/use-map-services.md",
      "redirect_url": "/windows/uwp/publish/app-management-and-services",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-15021-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-16299-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-16190-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-16299-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-16225-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-16299-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-creators-preview.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-15063",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-latest-preview-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-19041-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1710-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-16299-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1507.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-10240",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1511.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-10586",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-sdk-preview.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-14393",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1607.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-14393",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1607-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-14393-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1703.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-15063",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1703-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-15063-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-16190.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-17134",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-latest.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-19041",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-latest-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-19041-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-17110.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-17134",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-build-17110-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-17134-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-docs-latest.md",
      "redirect_url": "/windows/uwp/whats-new/windows-docs-january-2019",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/whats-new/windows-10-version-1709-api-diff.md",
      "redirect_url": "/windows/uwp/whats-new/windows-10-build-16299-api-diff",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/whats-new/windows-11-build-22000-apis.md",
      "redirect_url": "/windows/apps/whats-new/windows-11-build-22000",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/accessibility/accessibility-checklist.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessibility-checklist",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/accessibility-in-the-store.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessibility-in-the-store",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/accessibility-overview.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessibility-overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/accessibility-testing.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessibility-testing",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/accessibility.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessibility",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/accessible-text-requirements.md",
      "redirect_url": "/windows/uwp/design/accessibility/accessible-text-requirements",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/basic-accessibility-information.md",
      "redirect_url": "/windows/uwp/design/accessibility/basic-accessibility-information",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/control-patterns-and-interfaces.md",
      "redirect_url": "/windows/uwp/design/accessibility/control-patterns-and-interfaces",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/custom-automation-peers.md",
      "redirect_url": "/windows/uwp/design/accessibility/custom-automation-peers",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/designing-inclusive-software.md",
      "redirect_url": "/windows/uwp/design/accessibility/designing-inclusive-software",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/developing-inclusive-windows-apps.md",
      "redirect_url": "/windows/uwp/design/accessibility/developing-inclusive-windows-apps",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/high-contrast-themes.md",
      "redirect_url": "/windows/uwp/design/accessibility/high-contrast-themes",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/keyboard-accessibility.md",
      "redirect_url": "/windows/uwp/design/accessibility/keyboard-accessibility",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/accessibility/practices-to-avoid.md",
      "redirect_url": "/windows/uwp/design/accessibility/practices-to-avoid",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/app-settings/app-settings-and-data.md",
      "redirect_url": "/windows/uwp/design/app-settings/app-settings-and-data",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/app-settings/app-settings-and-data.md",
      "redirect_url": "/windows/uwp/design/app-settings/guidelines-for-app-settings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/app-settings/guidelines-for-app-settings.md",
      "redirect_url": "/windows/uwp/design/app-settings/guidelines-for-app-settings",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/app-settings/store-and-retrieve-app-data.md",
      "redirect_url": "/windows/uwp/design/app-settings/store-and-retrieve-app-data",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/app-bars.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/app-bars",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/auto-suggest-box.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/auto-suggest-box",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/buttons.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/buttons",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/calendar-date-picker.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/calendar-date-picker",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/calendar-view.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/calendar-view",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/checkbox.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/checkbox",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/collection-commanding.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/collection-commanding",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/color-picker.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/color-picker",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/control-templates.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/control-templates",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/controls-and-events-intro.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/controls-and-events-intro",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/controls-by-function.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/controls-by-function.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/custom-transport-controls.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/custom-transport-controls",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/date-and-time.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/date-and-time",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/date-picker.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/date-picker",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/dialogs.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/dialogs",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/flipview.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/flipview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/hub.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/hub",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/hyperlinks.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/hyperlinks",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/images-imagebrushes.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/images-imagebrushes",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/index.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/inking-controls.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/inking-controls",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/inverted-lists.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/inverted-lists",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/item-templates-gridview.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/item-templates-gridview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/item-templates-listview.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/item-templates-listview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/labels.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/labels",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/lists.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/lists",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/listview-and-gridview.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/listview-and-gridview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/listview-item-templates.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/item-templates-listview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/master-details.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/master-details",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/media-playback.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/media-playback",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/menus.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/menus",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/navigationview.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/navigationview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/nested-ui.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/nested-ui",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/password-box.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/password-box",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/person-picture.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/person-picture",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/pin-to-taskbar.md",
      "redirect_url": "/windows/uwp/design/shell/pin-to-taskbar",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/progress-controls.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/progress-controls",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/pull-to-refresh.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/pull-to-refresh",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/radio-button.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/radio-button",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/rating.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/rating",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/resourcedictionary-and-xaml-resource-references.md",
      "redirect_url": "/windows/apps/design/style/xaml-resource-dictionary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/rich-edit-box.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/rich-edit-box",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/rich-text-block.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/rich-text-block",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/scroll-controls.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/scroll-controls",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/search.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/search.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/semantic-zoom.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/semantic-zoom",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/slider.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/slider",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/split-view.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/split-view",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/swipe.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/swipe",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tabs-pivot.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/tab-view",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/text-block.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/text-block",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/text-box.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/text-box",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/text-controls.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/text-controls",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-adaptive-interactive-toasts.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/adaptive-interactive-toasts",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-adaptive-tiles-schema.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/adaptive-tiles-schema",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-app-assets.md",
      "redirect_url": "/windows/uwp/app-resources/images-tailored-for-scale-theme-contrast",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-badges.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/badges",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-choosing-a-notification-delivery-method.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/choosing-a-notification-delivery-method",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-create-adaptive-tiles.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/create-adaptive-tiles",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-creating-tiles.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/creating-tiles",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-notifications-visualizer.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/notifications-visualizer",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-periodic-notification-overview.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/periodic-notification-overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-primary-tile-apis.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/primary-tile-apis",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-raw-notification-overview.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-secondary-tiles-desktop-pinning.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles-desktop-pinning",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-secondary-tiles-guidance.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles-guidance",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-secondary-tiles-pinning.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles-pinning",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-secondary-tiles.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-send-local-toast.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/send-local-toast",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-sending-a-local-tile-notification.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/sending-a-local-tile-notification",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-special-tile-templates-catalog.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/special-tile-templates-catalog",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-the-code-generated-by-the-push-notification-wizard.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/the-code-generated-by-the-push-notification-wizard",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-toast-schema.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/toast-schema",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-toast-xml-schema.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/toast-xml-schema",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications-windows-push-notification-services--wns--overview.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/windows-push-notification-services--wns--overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-badges-notifications.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/time-picker.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/time-picker",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/toggles.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/toggles",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tooltips.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/tooltips",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tree-view.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/tree-view",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/web-view.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/web-view",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/xaml-styles.md",
      "redirect_url": "/windows/apps/develop/platform/xaml/xaml-styles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/xaml-theme-resources.md",
      "redirect_url": "/windows/apps/develop/platform/xaml/xaml-theme-resources",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications/channel-types.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/channel-types",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications/chaseable-tile-notifications.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/chaseable-tile-notifications",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications/notification-listener.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/notification-listener",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/controls-and-patterns/tiles-and-notifications/tile-schema.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/tile-schema",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design-downloads/index.md",
      "redirect_url": "/windows/uwp/design/downloads/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/in-app-help/external-help.md",
      "redirect_url": "/windows/uwp/design/in-app-help/external-help",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/in-app-help/guidelines-for-app-help.md",
      "redirect_url": "/windows/uwp/design/in-app-help/guidelines-for-app-help",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/in-app-help/in-app-help.md",
      "redirect_url": "/windows/uwp/design/in-app-help/in-app-help",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/in-app-help/instructional-ui.md",
      "redirect_url": "/windows/uwp/design/in-app-help/instructional-ui",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/in-app-help/voice-and-tone.md",
      "redirect_url": "/windows/uwp/design/style/writing-style",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/style/voice-and-tone.md",
      "redirect_url": "/windows/uwp/design/style/writing-style",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/access-keys.md",
      "redirect_url": "/windows/uwp/design/input/access-keys",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/convert-ink-to-text.md",
      "redirect_url": "/windows/uwp/design/input/convert-ink-to-text",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/custom-keyboard-interactions.md",
      "redirect_url": "/windows/uwp/design/input/custom-keyboard-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/custom-text-input.md",
      "redirect_url": "/windows/uwp/design/input/custom-text-input",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/define-custom-recognition-constraints.md",
      "redirect_url": "/windows/uwp/design/input/define-custom-recognition-constraints",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/designing-for-tv.md",
      "redirect_url": "/windows/uwp/design/devices/designing-for-tv",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/device-primer.md",
      "redirect_url": "/windows/uwp/design/devices/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/enable-continuous-dictation.md",
      "redirect_url": "/windows/uwp/design/input/enable-continuous-dictation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/gamepad-and-remote-interactions.md",
      "redirect_url": "/windows/uwp/design/input/gamepad-and-remote-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-cross-slide.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-cross-slide",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-optical-zoom.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-optical-zoom",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-panning.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-panning",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-rotation.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-rotation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-targeting.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-targeting",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-textselection.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-textselection",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/guidelines-for-visualfeedback.md",
      "redirect_url": "/windows/uwp/design/input/guidelines-for-visualfeedback",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/handle-pointer-input.md",
      "redirect_url": "/windows/uwp/design/input/handle-pointer-input",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/identify-input-devices.md",
      "redirect_url": "/windows/uwp/design/input/identify-input-devices",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/index.md",
      "redirect_url": "/windows/uwp/design/input/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/ink-toolbar.md",
      "redirect_url": "/windows/uwp/design/input/ink-toolbar",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/input-primer.md",
      "redirect_url": "/windows/uwp/design/input/input-primer",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/keyboard-accelerators.md",
      "redirect_url": "/windows/uwp/design/input/keyboard-accelerators",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/keyboard-events.md",
      "redirect_url": "/windows/uwp/design/input/keyboard-events",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/keyboard-interactions.md",
      "redirect_url": "/windows/uwp/design/input/keyboard-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/manage-issues-with-audio-input.md",
      "redirect_url": "/windows/uwp/design/input/manage-issues-with-audio-input",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/managing-focus-navigation.md",
      "redirect_url": "/windows/uwp/design/input/managing-focus-navigation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/mouse-interactions.md",
      "redirect_url": "/windows/uwp/design/input/mouse-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/multiple-input-design-guidelines.md",
      "redirect_url": "/windows/uwp/design/input/multiple-input-design-guidelines",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/pen-and-stylus-interactions.md",
      "redirect_url": "/windows/uwp/design/input/pen-and-stylus-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/respond-to-the-presence-of-the-touch-keyboard.md",
      "redirect_url": "/windows/uwp/design/input/respond-to-the-presence-of-the-touch-keyboard",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/save-and-load-ink.md",
      "redirect_url": "/windows/uwp/design/input/save-and-load-ink",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/set-speech-recognition-timeouts.md",
      "redirect_url": "/windows/uwp/design/input/set-speech-recognition-timeouts",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/specify-the-speech-recognizer-language.md",
      "redirect_url": "/windows/uwp/design/input/specify-the-speech-recognizer-language",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/speech-interactions.md",
      "redirect_url": "/windows/uwp/design/input/speech-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/speech-recognition.md",
      "redirect_url": "/windows/uwp/design/input/speech-recognition",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/touch-interactions.md",
      "redirect_url": "/windows/uwp/design/input/touch-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/touchpad-interactions.md",
      "redirect_url": "/windows/uwp/design/input/touchpad-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/use-input-scope-to-change-the-touch-keyboard.md",
      "redirect_url": "/windows/uwp/design/input/use-input-scope-to-change-the-touch-keyboard",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/input-and-devices/windows-wheel-interactions.md",
      "redirect_url": "/windows/uwp/design/input/windows-wheel-interactions",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/alignment-margin-padding.md",
      "redirect_url": "/windows/uwp/design/layout/alignment-margin-padding",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/boxpanel-example-custom-panel.md",
      "redirect_url": "/windows/uwp/design/layout/boxpanel-example-custom-panel",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/commanding-basics.md",
      "redirect_url": "/windows/uwp/design/basics/commanding-basics",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/content-as-objects.md",
      "redirect_url": "/windows/uwp/design",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/layout/content-basics.md",
      "redirect_url": "/windows/uwp/design/basics/content-basics",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/custom-panels-overview.md",
      "redirect_url": "/windows/uwp/design/layout/custom-panels-overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/design-and-ui-intro.md",
      "redirect_url": "/windows/uwp/design/basics/design-and-ui-intro",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/grid-tutorial.md",
      "redirect_url": "/windows/uwp/design/layout/grid-tutorial",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/index.md",
      "redirect_url": "/windows/uwp/design/layout/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/layout-panels.md",
      "redirect_url": "/windows/uwp/design/layout/layout-panels",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/layouts-with-xaml.md",
      "redirect_url": "/windows/uwp/design/layout/layouts-with-xaml",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/navigate-between-two-pages.md",
      "redirect_url": "/windows/uwp/design/basics/navigate-between-two-pages",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/navigation-basics.md",
      "redirect_url": "/windows/uwp/design/basics/navigation-basics",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/navigation-history-and-backwards-navigation.md",
      "redirect_url": "/windows/uwp/design/basics/navigation-history-and-backwards-navigation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/screen-sizes-and-breakpoints-for-responsive-design.md",
      "redirect_url": "/windows/uwp/design/layout/screen-sizes-and-breakpoints-for-responsive-design",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/layout/show-multiple-views.md",
      "redirect_url": "/windows/uwp/ui-input/show-multiple-views",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/acrylic.md",
      "redirect_url": "/windows/uwp/design/style/acrylic",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/balancing-style-and-consistency.md",
      "redirect_url": "/windows/uwp/design/style/balancing-style-and-consistency",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/color.md",
      "redirect_url": "/windows/uwp/design/style/color",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/connected-animation.md",
      "redirect_url": "/windows/uwp/design/motion/connected-animation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/content-transition-animations.md",
      "redirect_url": "/windows/uwp/design/motion/content-transition-animations",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/icons.md",
      "redirect_url": "/windows/uwp/design/style/icons",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/index.md",
      "redirect_url": "/windows/uwp/design/style/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-dragdrop.md",
      "redirect_url": "/windows/uwp/design/motion/motion-dragdrop",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-edgebased.md",
      "redirect_url": "/windows/uwp/design/motion/motion-edgebased",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-fade.md",
      "redirect_url": "/windows/uwp/design/motion/motion-fade",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-list.md",
      "redirect_url": "/windows/uwp/design/motion/motion-list",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-pointer.md",
      "redirect_url": "/windows/uwp/design/motion/motion-pointer",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-popup-animations.md",
      "redirect_url": "/windows/uwp/design/motion/motion-popup-animations",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion-reposition.md",
      "redirect_url": "/windows/uwp/design/motion/motion-reposition",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/motion.md",
      "redirect_url": "/windows/uwp/design/motion/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/parallax.md",
      "redirect_url": "/windows/uwp/design/motion/parallax",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/reveal.md",
      "redirect_url": "/windows/uwp/design/style/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/style/reveal.md",
      "redirect_url": "/windows/uwp/design/style/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/style/segoe-ui-symbol-font.md",
      "redirect_url": "/windows/uwp/design/style/segoe-ui-symbol-font",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/sound.md",
      "redirect_url": "/windows/uwp/design/style/sound",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/style/title-bar.md",
      "redirect_url": "/windows/uwp/design/shell/title-bar",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/style/fonts.md",
      "redirect_url": "/windows/uwp/design/style/typography",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/usability/index.md",
      "redirect_url": "/windows/uwp/design/usability/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/adjust-layout-and-fonts--and-support-rtl.md",
      "redirect_url": "/windows/uwp/design/globalizing/adjust-layout-and-fonts--and-support-rtl",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/glob-numeralsystem-values.md",
      "redirect_url": "/windows/uwp/design/globalizing/glob-numeralsystem-values",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/globalizing-portal.md",
      "redirect_url": "/windows/uwp/design/globalizing/globalizing-portal",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/guidelines-and-checklist-for-globalizing-your-app.md",
      "redirect_url": "/windows/uwp/design/globalizing/guidelines-and-checklist-for-globalizing-your-app",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/loc-international-fonts.md",
      "redirect_url": "/windows/uwp/design/globalizing/loc-international-fonts",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/manage-language-and-region.md",
      "redirect_url": "/windows/uwp/design/globalizing/manage-language-and-region",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/prepare-your-app-for-localization.md",
      "redirect_url": "/windows/uwp/design/globalizing/prepare-your-app-for-localization",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/use-global-ready-formats.md",
      "redirect_url": "/windows/uwp/design/globalizing/use-global-ready-formats",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/globalizing/use-patterns-to-format-dates-and-times.md",
      "redirect_url": "/windows/uwp/design/globalizing/use-patterns-to-format-dates-and-times",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/data-access/entity-framework-7-with-sqlite-for-csharp-apps.md",
      "redirect_url": "/ef/core/get-started/uwp/getting-started",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/app-resources/tile-toast-language-scale-contrast.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/tile-toast-language-scale-contrast",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/using-brushes.md",
      "redirect_url": "/windows/uwp/design/style/brushes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/animations-overview.md",
      "redirect_url": "/windows/uwp/design/motion/xaml-animation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/storyboarded-animations.md",
      "redirect_url": "/windows/uwp/design/motion/storyboarded-animations",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/key-frame-and-easing-function-animations.md",
      "redirect_url": "/windows/uwp/design/motion/key-frame-and-easing-function-animations",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/drawing-shapes.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/shapes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/transforms-overview.md",
      "redirect_url": "/windows/uwp/design/layout/transforms",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/3-d-perspective-effects.md",
      "redirect_url": "/windows/apps/develop/platform/xaml/3-d-perspective-effects",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/graphics/index.md",
      "redirect_url": "/windows/uwp/design/style",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/debug-test-perf/device-portal-xbox.md",
      "redirect_url": "/windows/uwp/xbox-apps/device-portal-xbox",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/xbox-360-friends-backward-compatibility.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/people-system_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/sign-in-to-xbox-live-in-unity.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/signin/unity-signin_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer-overview.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xbox-integrated-multiplayer",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-clearing.md",
      "redirect_url": "/windows/uwp/xbox-live/storage-platform/connected-storage/connected-storage-xb-storage",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/input/custom-keyboard-interactions.md",
      "redirect_url": "/windows/uwp/design/input/focus-navigation",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/input/managing-focus-navigation.md",
      "redirect_url": "/windows/uwp/design/input/focus-navigation-programmatic",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/privacy-and-people-i-know.md",
      "redirect_url": "/windows/uwp/xbox-live/social-platform/people-system/xbox-live-people-system",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/get-started/whats-a-uwp.md",
      "redirect_url": "/windows/uwp/get-started/universal-application-platform-guide",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/porting/hwa-to-uwp-root.md",
      "redirect_url": "/microsoft-edge/progressive-web-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/hwa-access-features.md",
      "redirect_url": "/microsoft-edge/progressive-web-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/hwa-chrome-conversion.md",
      "redirect_url": "/microsoft-edge/progressive-web-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/hwa-create-mac.md",
      "redirect_url": "/microsoft-edge/progressive-web-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/resolve-package-upload-errors.md",
      "redirect_url": "/windows/uwp/publish/upload-app-packages",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/manage-add-ons-in-bulk.md",
      "redirect_url": "/windows/uwp/publish/add-on-submissions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/associate-azure-ad-with-dev-center.md",
      "redirect_url": "/windows/uwp/publish/associate-azure-ad-with-partner-center",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/managing-your-profile.md",
      "redirect_url": "/partner-center/partner-center-account-setup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/define-pricing-and-market-selection.md",
      "redirect_url": "/windows/uwp/publish/define-market-selection",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/promote-your-app-report.md",
      "redirect_url": "/windows/uwp/publish/ad-campaign-report",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/app-declarations.md",
      "redirect_url": "/windows/uwp/publish/product-declarations",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/hwa-create-windows.md",
      "redirect_url": "/microsoft-edge/progressive-web-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/tabs-pivot.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/pivot",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/dialogs.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/dialogs-and-flyouts/index",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/monetize/download-the-cab-file-for-an-oem-hardware-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/download-the-cab-file-for-an-oem-hardware-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/download-the-cab-file-for-a-windows-10-driver-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/download-the-cab-file-for-a-windows-10-driver-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/download-the-cab-file-for-a-windows-7-or-windows-8.x-driver-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/download-the-cab-file-for-a-windows-7-or-windows-8.x-driver-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-details-for-an-oem-hardware-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-details-for-an-oem-hardware-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-details-for-a-windows-10-driver-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-details-for-a-windows-10-driver-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-details-for-a-windows-7-or-windows-8.x-driver-error.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-details-for-a-windows-7-or-windows-8.x-driver-error",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-error-reporting-data-for-windows-10-drivers.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-error-reporting-data-for-windows-10-drivers",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-error-reporting-data-for-windows-7-and-windows-8.x-drivers.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-error-reporting-data-for-windows-7-and-windows-8.x-drivers",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-oem-hardware-error-reporting-data.md",
      "redirect_url": "/windows-hardware/drivers/dashboard/get-oem-hardware-error-reporting-data",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/index.md",
      "redirect_url": "/windows/ai",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/get-started.md",
      "redirect_url": "/windows/ai",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/overview.md",
      "redirect_url": "/windows/ai",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/conversion-samples.md",
      "redirect_url": "/windows/ai/convert-model-winmltools",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/integrate-model.md",
      "redirect_url": "/windows/ai/integrate-model",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/samples.md",
      "redirect_url": "https://github.com/Microsoft/Windows-Machine-Learning",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/machine-learning/train-ai-model.md",
      "redirect_url": "/windows/ai/get-onnx-model",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/composition/lighting.md",
      "redirect_url": "/windows/uwp/composition/xaml-lighting",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/devices-sensors/nfc.md",
      "redirect_url": "/windows/uwp/devices-sensors/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/devices-sensors/generate-3mf.md",
      "redirect_url": "/windows/uwp/devices-sensors/3d-generate-3mf",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/devices-sensors/pos-advanced-connectivity.md",
      "redirect_url": "/windows/uwp/devices-sensors/point-of-service",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/devices-sensors/pos-barcodescanner-get-started.md",
      "redirect_url": "/windows/uwp/devices-sensors/pos-barcodescanner-configure",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/shell/tiles-and-notifications/app-assets.md",
      "redirect_url": "/windows/apps/design/style/iconography/overview",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/design/style/app-icons-and-logos.md",
      "redirect_url": "/windows/apps/design/style/iconography/overview",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/data-sharing-udc.md",
      "redirect_url": "/windows/uwp/xbox-live/configure-xbl/dev-center/access-policies-udc",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/packaging/appinstaller-root.md",
      "redirect_url": "/windows/msix/app-installer/app-installer-root",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/create-appinstallerfile-vs.md",
      "redirect_url": "/windows/msix/app-installer/create-appinstallerfile-vs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/installing-UWP-apps-web.md",
      "redirect_url": "/windows/msix/app-installer/installing-windows10-apps-web",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/install-related-set.md",
      "redirect_url": "/windows/msix/app-installer/install-related-set",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/troubleshoot-appinstaller-issues.md",
      "redirect_url": "/windows/msix/app-installer/troubleshoot-appinstaller-issues",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/web-install-azure.md",
      "redirect_url": "/windows/msix/app-installer/web-install-azure",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/web-install-IIS.md",
      "redirect_url": "/windows/msix/app-installer/web-install-iis",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/web-install-aws.md",
      "redirect_url": "/windows/msix/app-installer/web-install-aws",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/dev-center-insider-program.md",
      "redirect_url": "/windows/uwp/publish",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/advanced-xbox-live-sandboxes.md",
      "redirect_url": "/gaming/xbox-live/advanced-xbox-live-sandboxes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/developer-program-overview.md",
      "redirect_url": "/gaming/gdk/_content/gc/live/get-started/live-getstarted-nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/flatc-async-patterns.md",
      "redirect_url": "/gaming/xbox-live/flatc-async-patterns",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/index.md",
      "redirect_url": "/gaming/xbox-live/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/introduction-to-xbox-live-apis.md",
      "redirect_url": "/gaming/xbox-live/introduction-to-xbox-live-apis",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/samples.md",
      "redirect_url": "/gaming/xbox-live/samples",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/testing-on-console.md",
      "redirect_url": "/gaming/xbox-live/testing-on-console",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/what-is-xbox-live.md",
      "redirect_url": "/gaming/xbox-live/get-started/what-is-xbox-live",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-resources.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-resources",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-sandboxes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-sandboxes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-service-configuration.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-service-configuration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-test-accounts.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-test-accounts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live.md",
      "redirect_url": "/gaming/xbox-live/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xboxlive-policies.md",
      "redirect_url": "/gaming/xbox-live/xboxlive-policies",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xboxservices-config.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-win10/xboxservices-config",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xsapi-flat-c.md",
      "redirect_url": "/gaming/xbox-live/xsapi-flat-c",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/achievements-2017/achievement-rewards.md",
      "redirect_url": "/gaming/xbox-live/achievements-2017/achievement-rewards",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/achievements-2017/achievements.md",
      "redirect_url": "/gaming/xbox-live/achievements-2017/achievements_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/achievements-2017/simplified-achievements.md",
      "redirect_url": "/gaming/xbox-live/achievements-2017/simplified-achievements",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/windows-dev-center.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/setup-partner-center_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/access-policies-udc.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/access-policies-udc",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/achievements-in-udc.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/achievements-in-udc",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/featured-stats-and-leaderboards.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/featured-stats-and-leaderboards",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/game-dvr.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/game-dvr",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/localized-strings.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/localized-strings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/privileges.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/privileges",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/rich-presence-configuration.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/rich-presence-configuration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/single-sign-on.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/single-sign-on",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/summary.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/summary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/title-storage.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/title-storage",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/web-services.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/web-services",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/configure-xbl/dev-center/xbox-live-setup.md",
      "redirect_url": "/gaming/xbox-live/configure-xbl/dev-center/xbox-live-setup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/contextual-search/configuring-contextual-search.md",
      "redirect_url": "/gaming/xbox-live/contextual-search/configuring-contextual-search",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/contextual-search/introduction-to-contextual-search.md",
      "redirect_url": "/gaming/xbox-live/contextual-search/introduction-to-contextual-search",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/data-platform/data-platform.md",
      "redirect_url": "/gaming/xbox-live/data-platform/player-data_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/data-platform/designing-xbox-live-experiences.md",
      "redirect_url": "/gaming/xbox-live/data-platform/designing-xbox-live-experiences",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/add-controller-support-to-xbox-live-prefabs.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/add-controller-support-to-xbox-live-prefabs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/add-multi-user-support.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/add-multi-user-support",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/add-stats-and-leaderboards-in-unity.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/add-stats-and-leaderboards-in-unity",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/authorize-xbox-live-accounts.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/legacy/authorize-xbox-live-accounts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/check-user-privileges-in-unity.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/check-user-privileges-in-unity",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/configure-xbox-live-in-unity.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/configure-xbox-live-in-unity",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/create-and-test-a-new-creators-title.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/legacy/create-and-test-a-new-creators-title",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/creators-step-by-step-guide.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/creators-step-by-step-guide",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/develop-creators-title-with-unity.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/cr-unity-win10_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/develop-creators-title-with-visual-studio.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/vs-win10/develop-creators-title-with-visual-studio",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/get-started-with-xbox-live-creators.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/setup-partner-center-creators",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/playerauthentication-prefab-sign-in.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/signin/playerauthentication-prefab-sign-in",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/setup-leaderboard-example-scene.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/setup-leaderboard-example-scene",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/sign-in-manager.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/authentication_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/test-visual-studio-build.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/test-visual-studio-build",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/unity-leaderboard-from-scratch-pre1804.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/unity-leaderboard-from-scratch-pre1804",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/unity-leaderboard-from-scratch.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/unity-leaderboard-from-scratch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/unity-prefabs-and-sign-in.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/creators/unity-win10/signin/unity-prefabs-and-sign-in",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/xbox-live-sandboxes-creators.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/xbox-live-sandboxes-creators",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-creators/xbox-live-service-configuration-creators.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-creators/xbox-live-service-configuration-creators",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/add-xbox-live-apis-binary-to-a-uwp-project.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-win10/add-xbox-live-apis-binary-to-a-uwp-project",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/add-xbox-live-apis-source-to-a-uwp-project.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-win10/add-xbox-live-apis-source-to-a-uwp-project",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/add-xbox-live-to-an-xdk-project.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/add-xbox-live-to-an-xdk-project",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/advanced-xbox-live-sandboxes.md",
      "redirect_url": "/gaming/xbox-live/advanced-xbox-live-sandboxes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/compile-the-xdk-xbox-live-api-source.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/compile-the-xdk-xbox-live-api-source",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/configure-your-development-console.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/configure-your-development-console",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/create-a-new-title.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/legacy/create-a-new-title",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/get-started-with-cross-play-games.md",
      "redirect_url": "/gaming/xbox-live/get-started-with-partner/get-started-with-cross-play-games",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/get-started-with-visual-studio-and-uwp.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-win10/get-started-with-visual-studio-and-uwp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/get-started-with-xbox-live-partner.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/legacy/get-started-with-xbox-live-partner",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/partner-add-xbox-live-to-unity-uwp.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/unity-win10/partner-add-xbox-live-to-unity-uwp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/partner-unity-uwp-il2cpp.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/unity-win10/partner-unity-uwp-il2cpp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/partner-unity-xdk-il2cpp.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/unity-xbox/partner-unity-xdk-il2cpp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/partners-step-by-step-guide.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-partner-center/legacy/get-started-with-xbox-live-partner",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/use-xbox-live-nuget-with-xdk.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/use-xbox-live-nuget-with-xdk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/using-xbox-live-apis-built-into-the-xdk.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/using-xbox-live-apis-built-into-the-xdk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/where-to-get-xdk.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/where-to-get-xdk",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/get-started-with-partner/xdk-developers.md",
      "redirect_url": "/gaming/xbox-live/get-started/setup-ide/managed-partners/vs-xbox/mp-vs-xbox_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/leaderboards-and-stats-2017/leaderboards.md",
      "redirect_url": "/gaming/xbox-live/leaderboards-and-stats-2017/leaderboards",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/leaderboards-and-stats-2017/player-stats-configure-2017.md",
      "redirect_url": "/gaming/xbox-live/leaderboards-and-stats-2017/player-stats-configure-2017",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/leaderboards-and-stats-2017/player-stats-updating.md",
      "redirect_url": "/gaming/xbox-live/leaderboards-and-stats-2017/player-stats-updating",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/leaderboards-and-stats-2017/player-stats.md",
      "redirect_url": "/gaming/xbox-live/data-platform/player-data_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/leaderboards-and-stats-2017/stats2017.md",
      "redirect_url": "/gaming/xbox-live/leaderboards-and-stats-2017/stats2017",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-concepts.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-concepts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-intro.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-intro",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-platform",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-roles.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-roles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-scenarios.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-scenarios",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/session-browse.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/session-browse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xbox-integrated-multiplayer",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-apis-metadata.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-apis-metadata",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-notifications.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-notifications",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-title-integration.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-title-integration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-user-scenarios.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-user-scenarios",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-ux-join-tournament.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-ux-join-tournament",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/arena-ux-match-engagement.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/arena-ux-match-engagement",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/discovering-xbox-tournaments.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/discovering-xbox-tournaments",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/operations-portal.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/operations-portal",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/arena/xbox-arena.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/arena/xbox-arena",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/chat/game-chat-2-migration.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/chat/game-chat-2-migration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/chat/game-chat-2-overview.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/chat/game-chat-2-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/chat/real-time-audio-manipulation.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/chat/real-time-audio-manipulation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/chat/using-game-chat-2-winrt.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/chat/using-game-chat-2-winrt",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/chat/using-game-chat-2.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/chat/using-game-chat-2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/common-issues-when-adapting-multiplayer.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/common-issues-when-adapting-multiplayer",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/flows-for-multiplayer-game-invites.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/invite/multiplayer-invite-flows",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/game-session-and-game-party-visibility-and-joinability.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/game-session-and-game-party-visibility-and-joinability",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/introduction-to-the-multiplayer-system.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/introduction-to-the-multiplayer-system",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/migrating-an-arbiter.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/migrating-an-arbiter",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/mpsd-session-details.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-session/mpsd-details",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/multiplayer-2015-faq.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/multiplayer-2015-faq",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/multiplayer-appendix.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/multiplayer-appendix",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/multiplayer-how-tos.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-session/mpsd-how-tos",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/multiplayer-session-directory.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/xbox-one-multiplayer-session-directory",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/multiplayer-session-status-codes.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-session/mpsd-status-codes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/smartmatch-matchmaking.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-play-with-smartmatch-matchmaking",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/using-smartmatch-matchmaking.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/matchmaking/matchmaking",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-appendix/xbox-one-multiplayer-session-directory.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-appendix/xbox-one-multiplayer-session-directory",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/handle-protocol-activation.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/handle-protocol-activation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/multiplayer-manager-api-overview.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/multiplayer-manager-api-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/play-multiplayer-with-friends.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/play-multiplayer-with-friends",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/play-multiplayer-with-matchmaking.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/play-multiplayer-with-matchmaking",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/send-game-invites.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/send-game-invites",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-fill-open-slots.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-fill-open-slots",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-host-migration.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-host-migration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-on-protocol-activation.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-on-protocol-activation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-play-with-friends.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-play-with-friends",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-play-with-smartmatch-matchmaking.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-play-with-smartmatch-matchmaking",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-send-invites.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-send-invites",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-shut-down.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-shut-down",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-use-matchmaking-and-qos.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/multiplayer-manager/mpm-flowcharts/mpm-use-matchmaking-and-qos",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/service-configuration/configure-the-multiplayer-service.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/service-configuration/configure-the-multiplayer-service",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/service-configuration/configure-your-appxmanifest-for-multiplayer.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-manifest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/service-configuration/large-sessions.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/service-configuration/large-sessions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/service-configuration/session-template-constants.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/service-configuration/session-template-constants",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/service-configuration/session-templates.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/service-configuration/session-templates",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/using-xim-cs.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/using-xim-cs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/using-xim.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/using-xim",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-manifest.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-manifest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-release-notes.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-release-notes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-reservations.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-reservations",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-unity-uwp-il2cpp.md",
      "redirect_url": "/gaming/xbox-live/multiplayer/xbox-integrated-multiplayer/xim-unity-uwp-il2cpp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/real-time-activity-service/programming-the-real-time-activity-service.md",
      "redirect_url": "/gaming/xbox-live/real-time-activity-service/programming-the-real-time-activity-service",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/real-time-activity-service/real-time-activity-service.md",
      "redirect_url": "/gaming/xbox-live/real-time-activity-service/real-time-activity-service_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/real-time-activity-service/register-for-stat-notifications.md",
      "redirect_url": "/gaming/xbox-live/real-time-activity-service/register-for-stat-notifications",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/real-time-activity-service/rta-best-practices.md",
      "redirect_url": "/gaming/xbox-live/real-time-activity-service/rta-best-practices",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/intro-to-social-manager.md",
      "redirect_url": "/gaming/xbox-live/social-platform/intro-to-social-manager",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/social-manager-memory-and-performance-overview.md",
      "redirect_url": "/gaming/xbox-live/social-platform/social-manager-memory-and-performance-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/social-platform.md",
      "redirect_url": "/gaming/xbox-live/social-platform/social-platform_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/displaying-people-from-the-people-system.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/displaying-people-from-the-people-system",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/programming-social-services.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/programming-social-services",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/reputation.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/reputation_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/sending-player-feedback-from-your-title.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/sending-player-feedback-from-your-title",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/people-system/xbox-live-people-system.md",
      "redirect_url": "/gaming/xbox-live/social-platform/people-system/xbox-live-people-system",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/programming-rich-presence.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/programming-rich-presence",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-appendix.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-appendix",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-best-practices.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-best-practices",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-configuration.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-configuration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-overview.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-policies-and-limitations.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-policies-and-limitations",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-updating-strings.md",
      "redirect_url": "/gaming/xbox-live/social-platform/rich-presence-strings/rich-presence-strings-updating-strings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/storage-platform.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/cloud-storage_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-best-practices.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-best-practices",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-deleting.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-deleting",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-loading-on-demand.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-loading-on-demand",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-loading.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-loading",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-overview.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-saving.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-saving",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-technical-overview.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-technical-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-using-buffers.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-using-buffers",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/connected-storage/connected-storage-xb-storage.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/connected-storage/connected-storage-xb-storage",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/reading-binary-blobs.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/reading-binary-blobs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/reading-configuration-blobs.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/reading-configuration-blobs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/reading-jsonblobs.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/reading-jsonblobs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/storing-binary-blobs.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/storing-binary-blobs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/storing-jsonblobs.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/storing-jsonblobs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/storage-platform/xbox-live-title-storage/xbox-live-title-storage.md",
      "redirect_url": "/gaming/xbox-live/storage-platform/xbox-live-title-storage/xbox-live-title-storage",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/tools/analyze-service-calls.md",
      "redirect_url": "/gaming/xbox-live/tools/analyze-service-calls",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/tools/tools.md",
      "redirect_url": "/gaming/xbox-live/tools/tools",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/tools/xbox-live-account-tool.md",
      "redirect_url": "/gaming/xbox-live/tools/xbox-live-account-tool",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/porting-xbox-live-code-from-xdk-to-uwp.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/porting-xbox-live-code-from-xdk-to-uwp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/using-xbox-live.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/using-xbox-live",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/auth/authentication-for-UWP-projects.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/authentication-for-UWP-projects",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/auth/authentication-for-XDK-projects.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/authentication-for-XDK-projects",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/auth/authentication.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/authentication_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/auth/retrieving-windows-system-user-on-UWP.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/retrieving-windows-system-user-on-UWP",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/auth/single-point-of-presence.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/auth/single-point-of-presence",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/best-practices/best-practices-for-calling-xbox-live.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/best-practices/best-practices-for-calling-xbox-live",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/best-practices/best-practices-for-offline.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/best-practices/best-practices-for-offline",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/best-practices/fine-grained-rate-limiting.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/best-practices/fine-grained-rate-limiting",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/error-handling/error-handling-cpp.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/error-handling/error-handling-cpp",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/error-handling/error-handling-winrt.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/error-handling/error-handling-winrt",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/error-handling/error-handling.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/error-handling/error-handling_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/troubleshooting/how-to-set-up-fiddler-for-debugging.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/troubleshooting/how-to-set-up-fiddler-for-debugging",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/troubleshooting/troubleshooting-pc-setup.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/troubleshooting/troubleshooting-pc-setup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/troubleshooting/troubleshooting-sign-in.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/troubleshooting/troubleshooting-sign-in",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/troubleshooting/troubleshooting-the-xbox-live-services-api.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/troubleshooting/troubleshooting-the-xbox-live-services-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/using-xbox-live/troubleshooting/troubleshooting.md",
      "redirect_url": "/gaming/xbox-live/using-xbox-live/troubleshooting/troubleshooting_nav",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1506-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1506-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1508-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1508-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1509-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1509-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1510-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1510-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1602-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1602-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1603-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1603-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1604-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1604-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1606-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1606-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1608-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1608-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1611-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1611-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1612-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1612-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1703-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1703-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1704-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1704-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1705-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1705-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1706-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1706-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1707-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1707-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/1708-whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/1708-whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/whats-new/whats-new.md",
      "redirect_url": "/gaming/xbox-live/whats-new/whats-new",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/atoc-xboxlivews-reference.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/atoc-xboxlivews-reference",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/atoc-xboxlivews-reference-additional.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/atoc-xboxlivews-reference-additional",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/authorizationtypes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/authorizationtypes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/datatypeoverview.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/datatypeoverview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/eds-apis.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/eds-apis",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edsauthorization.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edsauthorization",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edscommonheaders.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edscommonheaders",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edsparameters.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edsparameters",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edsqueryrefiners.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edsqueryrefiners",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edsreverselookup.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edsreverselookup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/edstables.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/edstables",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/httpstandardheaders.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/httpstandardheaders",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/httpstatuscodes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/httpstatuscodes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/additional/pagingparameters.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/additional/pagingparameters",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/atoc-xboxlivews-reference-enums.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/atoc-xboxlivews-reference-enums",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipsource.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipsource",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipstate.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipstate",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-gamecliptypes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-gamecliptypes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipuritype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipuritype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipvisibility.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-gameclipvisibility",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-thumbnailsource.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-thumbnailsource",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/gvr-enum-thumbnailtype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/gvr-enum-thumbnailtype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/enums/privacy-enum-permissionid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/enums/privacy-enum-permissionid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/atoc-xboxlivews-reference-json.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/atoc-xboxlivews-reference-json",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-achievementv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-achievementv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-activityrecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-activityrecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-activityrequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-activityrequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-aggregatesessionsresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-aggregatesessionsresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-batchrequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-batchrequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-deviceendpoint.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-deviceendpoint",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-devicerecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-devicerecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-feedback.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-feedback",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gameclip.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gameclip",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gameclipsserviceerrorresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gameclipsserviceerrorresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gameclipthumbnail.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gameclipthumbnail",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gameclipuri.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gameclipuri",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gamemessage.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gamemessage",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gameresult.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gameresult",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gamesession.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gamesession",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-gamesessionsummary.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-gamesessionsummary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-getclipresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-getclipresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-hopperstatsresults.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-hopperstatsresults",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-initialuploadrequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-initialuploadrequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-initialuploadresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-initialuploadresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-inventoryitem.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-inventoryitem",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-lastseenrecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-lastseenrecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-matchticket.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-matchticket",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-mediaasset.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-mediaasset",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-mediarecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-mediarecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-mediarequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-mediarequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-multiplayeractivitydetails.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-multiplayeractivitydetails",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-multiplayersession.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-multiplayersession",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-multiplayersessionreference.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-multiplayersessionreference",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-multiplayersessionrequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-multiplayersessionrequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-paginginfo.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-paginginfo",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-peoplelist.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-peoplelist",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-permissioncheckbatchrequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-permissioncheckbatchrequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-permissioncheckbatchresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-permissioncheckbatchresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-permissioncheckbatchuserresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-permissioncheckbatchuserresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-permissioncheckresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-permissioncheckresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-permissioncheckresult.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-permissioncheckresult",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-person.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-person",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-personsummary.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-personsummary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-player.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-player",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-presencerecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-presencerecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-profile.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-profile",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-progression.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-progression",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-property.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-property",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-queryclipsresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-queryclipsresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-quota.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-quota",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-requirement.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-requirement",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-resetreputation.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-resetreputation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-reward.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-reward",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-richpresencerequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-richpresencerequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-serviceerror.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-serviceerror",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-serviceerrorresponse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-serviceerrorresponse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-sessionentry.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-sessionentry",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-titleassociation.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-titleassociation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-titleblob.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-titleblob",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-titlerecord.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-titlerecord",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-titlerequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-titlerequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-updatemetadatarequest.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-updatemetadatarequest",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-user.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-user",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-userclaims.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-userclaims",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-userlist.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-userlist",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-usersettings.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-usersettings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-usertitlev2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-usertitlev2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-verifystringresult.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-verifystringresult",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/json/json-xuidlist.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/json/json-xuidlist",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/atoc-xboxlivews-reference-uris.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/atoc-xboxlivews-reference-uris",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/achievements/atoc-reference-achievementsv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/achievements/atoc-reference-achievementsv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/achievements/uri-achievementsusersxuidachievementsgetv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/achievements/uri-achievementsusersxuidachievementsgetv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/achievements/uri-achievementsusersxuidachievementsv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/achievements/uri-achievementsusersxuidachievementsv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/achievements/uri-usersxuidachievementsscidachievementid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/achievements/uri-usersxuidachievementsscidachievementid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/achievements/uri-usersxuidachievementsscidachievementidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/achievements/uri-usersxuidachievementsscidachievementidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/atoc-reference-dvr.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/atoc-reference-dvr",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-publicscidclips.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-publicscidclips",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-publicscidclipsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-publicscidclipsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-uri.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-uri",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-uriget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-uriget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-uriput.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-uriput",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclips.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclips",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipiddelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipiddelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipidpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipsgameclipidpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipspost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersmescidclipspost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridclips.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridclips",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridclipsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridclipsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridscidclipsgameclipid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridscidclipsgameclipid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridscidclipsgameclipidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/dvr/uri-usersowneridscidclipsgameclipidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gamerpic/atoc-reference-gamerpic.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gamerpic/atoc-reference-gamerpic",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gamerpic/uri-usersmegamerpic.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gamerpic/uri-usersmegamerpic",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gamerpic/uri-usersmegamerpicput.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gamerpic/uri-usersmegamerpicput",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/atoc-gsdk-uri-reference.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/atoc-gsdk-uri-reference",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-qosservers-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-qosservers-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-qosservers.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-qosservers",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidclusters-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidclusters-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidclusters.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidclusters",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionhosts-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionhosts-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionhosts.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionhosts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionssessionidallocationstatus-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionssessionidallocationstatus-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionssessionidallocationstatus.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidsessionssessionidallocationstatus",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidvariants-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidvariants-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidvariants.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/gsdk/uri-titlestitleidvariants",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/atoc-reference-leaderboard.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/atoc-reference-leaderboard",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardname.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardname",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardnameget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardnameget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardnamegetvaluemetadata.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/uri-scidsscidleaderboardsleaderboardnamegetvaluemetadata",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/uri-usersxuidscidstatnamepeople.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/uri-usersxuidscidstatnamepeople",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/leaderboard/uri-usersxuidscidstatnamepeopleget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/leaderboard/uri-usersxuidscidstatnamepeopleget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/atoc-reference-lists.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/atoc-reference-lists",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistname.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistname",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamecontainsitems.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamecontainsitems",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamecontainsitemspost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamecontainsitemspost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamedelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamedelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameindex.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameindex",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameindexpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameindexpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamepost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnamepost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameput.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameput",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitems.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitems",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitemsdelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitemsdelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitemspost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/lists/uri-usersxuidlistspinslistnameremoveitemspost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/atoc-reference-marketplace.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/atoc-reference-marketplace",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventory.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventory",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryconsumablesitemurl.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryconsumablesitemurl",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryconsumablesitemurlpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryconsumablesitemurlpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryitemurl.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryitemurl",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryitemurlget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-inventoryitemurlget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-localecrossmediagroupsearch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-localecrossmediagroupsearch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-localecrossmediagroupsearchget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-localecrossmediagroupsearchget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalebrowse.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalebrowse",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalebrowseget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalebrowseget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalecontentrating.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalecontentrating",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalecontentratingget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalecontentratingget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocaledetails.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocaledetails",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocaledetailsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocaledetailsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalefields.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalefields",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalefieldsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalefieldsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemediaitemtypequeryrefinersubqueryrefinervalues.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemediaitemtypequeryrefinersubqueryrefinervalues",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemediaitemtypequeryrefinersubqueryrefinervaluesget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemediaitemtypequeryrefinersubqueryrefinervaluesget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroups.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroups",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsmediaitemtypes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsmediaitemtypes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsmediaitemtypesget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediagroupsmediaitemtypesget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypefields.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypefields",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypefieldsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypefieldsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefiners.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefiners",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersqueryrefinername.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersqueryrefinername",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersqueryrefinernameget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypequeryrefinersqueryrefinernameget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypes.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesortorders.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesortorders",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesortordersget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalemetadatamediaitemtypesortordersget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalesinglemediagroupsearch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalesinglemediagroupsearch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalesinglemediagroupsearchget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/marketplace/uri-medialocalesinglemediagroupsearchget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/atoc-reference-matchtickets.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/atoc-reference-matchtickets",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-scidhoppernameticketid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-scidhoppernameticketid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-scidhoppernameticketiddelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-scidhoppernameticketiddelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppername.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppername",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamepost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamepost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamestats.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamestats",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamestatsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/matchtickets/uri-serviceconfigsscidhoppershoppernamestatsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/atoc-reference-people.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/atoc-reference-people",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeople.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeople",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopleget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopleget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopletargetid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopletargetid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopletargetidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeopletargetidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeoplexuids.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeoplexuids",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeoplexuidspost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridpeoplexuidspost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridsummary.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridsummary",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/people/uri-usersowneridsummaryget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/people/uri-usersowneridsummaryget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/atoc-reference-presence.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/atoc-reference-presence",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersbatch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersbatch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersbatchpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersbatchpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersme.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersme",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersmeget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersmeget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersmegroupsmoniker.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersmegroupsmoniker",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersmegroupsmonikerget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersmegroupsmonikerget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrent.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrent",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrentdelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrentdelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrentpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuiddevicescurrenttitlescurrentpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmoniker.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmoniker",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcasting.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcasting",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingcount.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingcount",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingcountget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingcountget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerbroadcastingget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/presence/uri-usersxuidgroupsmonikerget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/atoc-reference-privacyv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/atoc-reference-privacyv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersowneridpeoplemute.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersowneridpeoplemute",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersowneridpeoplemuteget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersowneridpeoplemuteget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidate.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidate",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidateget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidateget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidatepost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersrequestoridpermissionvalidatepost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersxuidpeopleavoid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersxuidpeopleavoid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersxuidpeopleavoidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/privacy/uri-privacyusersxuidpeopleavoidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/profileV2/atoc-reference-profiles.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/profileV2/atoc-reference-profiles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/profileV2/uri-usersbatchprofilesettings.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/profileV2/uri-usersbatchprofilesettings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/profileV2/uri-usersbatchprofilesettingspost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/profileV2/uri-usersbatchprofilesettingspost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/profileV2/uri-usersuseridprofilesettingspeopleuserlist.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/profileV2/uri-usersuseridprofilesettingspeopleuserlist",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/profileV2/uri-usersuseridprofilesettingspeopleuserlistget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/profileV2/uri-usersuseridprofilesettingspeopleuserlistget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/atoc-reference-reputation.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/atoc-reference-reputation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersbatchfeedback.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersbatchfeedback",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersbatchfeedbackpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersbatchfeedbackpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersxuidfeedback.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersxuidfeedback",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersxuidfeedbackpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-reputationusersxuidfeedbackpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersmeresetreputation.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersmeresetreputation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersmeresetreputationpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersmeresetreputationpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuiddeleteuserdata.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuiddeleteuserdata",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuiddeleteuserdatapost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuiddeleteuserdatapost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuidresetreputation.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuidresetreputation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuidresetreputationpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/reputation/uri-usersxuidresetreputationpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/atoc-reference-sessiondirectory.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/atoc-reference-sessiondirectory",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handles.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleiddelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleiddelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsession.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsession",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsessionget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsessionget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsessionput.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handleshandleidsessionput",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlespost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlespost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesquery.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesquery",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesqueryincludepost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesqueryincludepost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesquerypost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-handlesquerypost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigscidsessiontemplatessessiontemplatenamebatch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigscidsessiontemplatessessiontemplatenamebatch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigscidsessiontemplatessessiontemplatenamebatchpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigscidsessiontemplatessessiontemplatenamebatchpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidbatch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidbatch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidbatchpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidbatchpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessions.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessionsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessionsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplates.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplates",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatesget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatesget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatename.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatename",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenameget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenameget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersindex.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersindex",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersindexdelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersindexdelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersservername.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersservername",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersservernamedelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionnamemembersservernamedelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessions.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionname.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionname",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnameget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnameget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnamemembersme.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnamemembersme",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnamemembersmedelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnamemembersmedelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnameput.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/sessiondirectory/uri-serviceconfigsscidsessiontemplatessessiontemplatenamesessionssessionnameput",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/atoc-reference-storagev2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/atoc-reference-storagev2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidsscid-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidsscid-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidsscid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidsscid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapath-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapath-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapath.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapath",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapathandfilenametype-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapathandfilenametype-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-globalscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersbatchscidssciddatapathandfilenametype-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersbatchscidssciddatapathandfilenametype-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersbatchscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersbatchscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidsscid-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidsscid-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidsscid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidsscid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapath-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapath-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapath.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapath",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-delete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-delete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-put.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype-put",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-jsonusersxuidscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidsscid-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidsscid-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidsscid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidsscid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapath-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapath-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapath.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapath",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-delete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-delete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-put.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype-put",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-sessionssessionidscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersbatchscidssciddatapathandfilenametype-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersbatchscidssciddatapathandfilenametype-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersbatchscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersbatchscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidsscid-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidsscid-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidsscid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidsscid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapath-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapath-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapath.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapath",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-delete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-delete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-put.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype-put",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-trustedplatformusersxuidscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersbatchscidssciddatapathandfilenametype-post.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersbatchscidssciddatapathandfilenametype-post",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersbatchscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersbatchscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidsscid-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidsscid-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidsscid.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidsscid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapath-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapath-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapath.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapath",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-delete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-delete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-get.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-get",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-put.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype-put",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/storage/uri-untrustedplatformusersxuidscidssciddatapathandfilenametype",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/stringserver/atoc-reference-systemstringsvalidate.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/stringserver/atoc-reference-systemstringsvalidate",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/stringserver/uri-systemstringsvalidate.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/stringserver/uri-systemstringsvalidate",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/stringserver/uri-systemstringsvalidatepost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/stringserver/uri-systemstringsvalidatepost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/titlehistory/atoc-reference-titlehistoryv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/titlehistory/atoc-reference-titlehistoryv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/titlehistory/uri-titlehistoryusersxuidhistorytitlesgetv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/titlehistory/uri-titlehistoryusersxuidhistorytitlesgetv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/titlehistory/uri-titlehistoryusersxuidhistorytitlesv2.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/titlehistory/uri-titlehistoryusersxuidhistorytitlesv2",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/atoc-reference-users.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/atoc-reference-users",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinbox.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxmessageiddelete.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxmessageiddelete",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxmessageidget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidinboxmessageidget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidoutbox.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidoutbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/users/uri-usersxuidoutboxpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/users/uri-usersxuidoutboxpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/atoc-reference-userstats.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/atoc-reference-userstats",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/uri-batch.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/uri-batch",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/uri-batchpost.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/uri-batchpost",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstats.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstats",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstatsget.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstatsget",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstatsgetvaluemetadata.md",
      "redirect_url": "/gaming/xbox-live/xbox-live-rest/uri/userstats/uri-usersxuidscidsscidstatsgetvaluemetadata",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/composition/visual-layer-in-desktop-apps.md",
      "redirect_url": "/windows/apps/desktop/modernize/visual-layer-in-desktop-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/composition/using-the-visual-layer-with-wpf.md",
      "redirect_url": "/windows/apps/desktop/modernize/using-the-visual-layer-with-wpf",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/composition/using-the-visual-layer-with-windows-forms.md",
      "redirect_url": "/windows/apps/desktop/modernize/using-the-visual-layer-with-windows-forms",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/composition/using-the-visual-layer-with-win32.md",
      "redirect_url": "/windows/apps/desktop/modernize/using-the-visual-layer-with-win32",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xaml-platform/xaml-host-controls.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/xaml-platform/using-the-xaml-hosting-api.md",
      "redirect_url": "/windows/apps/desktop/modernize/using-the-xaml-hosting-api",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/desktop/modernize/advanced-scenarios-xaml-islands-cpp.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/advanced-scenarios-xaml-islands-cpp",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/host-custom-control-with-xaml-islands-cpp.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/host-custom-control-with-xaml-islands-cpp",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/host-custom-control-with-xaml-islands.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/host-custom-control-with-xaml-islands",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/host-standard-control-with-xaml-islands-cpp.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/host-standard-control-with-xaml-islands-cpp",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/host-standard-control-with-xaml-islands.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/host-standard-control-with-xaml-islands",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/using-the-xaml-hosting-api.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/using-the-xaml-hosting-api",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/xaml-islands.md",
      "redirect_url": "/windows/apps/desktop/modernize/xaml-islands/xaml-islands",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/apply-mica-win32.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/apply-mica-win32",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/apply-rounded-corners.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/apply-rounded-corners",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/apply-snap-layout-menu.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/apply-snap-layout-menu",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/apply-windows-themes.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/apply-windows-themes",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/using-the-visual-layer-with-win32.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/using-the-visual-layer-with-win32",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/using-the-visual-layer-with-windows-forms.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/using-the-visual-layer-with-windows-forms",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/using-the-visual-layer-with-wpf.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/using-the-visual-layer-with-wpf",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/desktop/modernize/visual-layer-in-desktop-apps.md",
      "redirect_url": "/windows/apps/desktop/modernize/ui/visual-layer-in-desktop-apps",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-root.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-root",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-prepare.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-prepare",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-packaging-dot-net.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-packaging-dot-net",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-run-desktop-app-converter.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-run-desktop-app-converter",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-manual-conversion.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-manual-conversion",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-r2r.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-r2r",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-behind-the-scenes.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-behind-the-scenes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-known-issues.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-known-issues",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/package-support-framework.md",
      "redirect_url": "/windows/msix/psf/package-support-framework",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-debug.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-debug",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-test-windows-s.md",
      "redirect_url": "/windows/msix/desktop/desktop-to-uwp-test-windows-s",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-distribute.md",
      "redirect_url": "/windows/apps/desktop/modernize/desktop-to-uwp-distribute",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-enhance.md",
      "redirect_url": "/windows/apps/desktop/modernize/desktop-to-uwp-enhance",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-extend.md",
      "redirect_url": "/windows/apps/desktop/modernize/desktop-to-uwp-extend",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-extensions.md",
      "redirect_url": "/windows/apps/desktop/modernize/desktop-to-uwp-extensions",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/desktop-to-uwp-supported-api.md",
      "redirect_url": "/windows/apps/desktop/modernize/desktop-to-uwp-supported-api",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/fluent-design-system/index.md",
      "redirect_url": "/windows/apps/fluent-design-system",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/packaging-uwp-apps.md",
      "redirect_url": "/windows/msix/package/packaging-uwp-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/manual-packaging-root.md",
      "redirect_url": "/windows/msix/package/manual-packaging-root",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/create-app-package-with-makeappx-tool.md",
      "redirect_url": "/windows/msix/package/create-app-package-with-makeappx-tool",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/create-certificate-package-signing.md",
      "redirect_url": "/windows/msix/package/create-certificate-package-signing",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/sign-app-package-using-signtool.md",
      "redirect_url": "/windows/msix/package/sign-app-package-using-signtool",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/package-folding.md",
      "redirect_url": "/windows/msix/package/package-folding",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/flat-bundles.md",
      "redirect_url": "/windows/msix/package/flat-bundles",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/asset-packages.md",
      "redirect_url": "/windows/msix/package/asset-packages",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/packaging-layout.md",
      "redirect_url": "/windows/msix/package/packaging-layout",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/device-architecture.md",
      "redirect_url": "/windows/msix/package/device-architecture",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/streaming-install.md",
      "redirect_url": "/windows/msix/package/streaming-install",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/create-cgm.md",
      "redirect_url": "/windows/msix/package/create-cgm",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/optional-packages.md",
      "redirect_url": "/windows/msix/package/optional-packages",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/packaging/optional-packages-with-executable-code.md",
      "redirect_url": "/windows/msix/package/optional-packages-with-executable-code",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/python/get-started/python-for-education.md",
      "redirect_url": "/windows/python/beginners",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/python/get-started/python-for-web.md",
      "redirect_url": "/windows/python/web-frameworks",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/python/get-started/python-for-scripting.md",
      "redirect_url": "/windows/python/scripting",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/mac-to-windows.md",
      "redirect_url": "/windows/dev-environment/mac-to-windows",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/layout/content-as-objects.md",
      "redirect_url": "/windows/uwp/design",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-one-game-acquisitions.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-xbox-one-add-on-acquisitions.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-error-reporting-data-for-your-xbox-one-game.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-details-for-an-error-in-your-xbox-one-game.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/get-the-stack-trace-for-an-error-in-your-xbox-one-game.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/download-the-cab-file-for-an-error-in-your-xbox-one-game.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/porting/apps-on-arm-limitations.md",
      "redirect_url": "/windows/uwp/porting/apps-on-arm-troubleshooting-x86",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/communication/ipc.md",
      "redirect_url": "/windows/uwp/communication/interprocess-communication",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/android/index.md",
      "redirect_url": "/windows/android/overview",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/python/databases.md",
      "redirect_url": "/windows/wsl/tutorials/wsl-database",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/databases.md",
      "redirect_url": "/windows/wsl/tutorials/wsl-database",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/app-metadata-api-for-advertising-networks.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/dev-environment/overview.md",
      "redirect_url": "/windows/dev-environment/",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/monetize/payment-request.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/shell/tiles-and-notifications/toast-xml-schema.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/toast-schema",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/create-an-ad-campaign-for-your-app.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/managing-your-ad-campaign.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/about-house-ads.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/about-community-ads.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/common-questions.md",
      "redirect_url": "/windows/uwp/monetize",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/tax-details-for-paid-apps.md",
      "redirect_url": "/partner-center/tax-details-marketplace",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/getting-paid-apps.md",
      "redirect_url": "/partner-center/marketplace-get-paid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/setting-up-your-payout-account-and-tax-forms.md",
      "redirect_url": "/partner-center/set-up-your-payout-account ",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/payout-summary.md",
      "redirect_url": "/partner-center/payout-statement",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/understand-irs-tax-forms.md",
      "redirect_url": "/partner-center/understand-irs-tax-forms",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/payment-thresholds-methods-and-timeframes.md",
      "redirect_url": "/partner-center/payment-thresholds-methods-timeframes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/mobile-operator-billing.md",
      "redirect_url": "/partner-center/mobile-operator-billing",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/vat-info.md",
      "redirect_url": "/partner-center/vat-info",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/whats-new/build2020-docs.md",
      "redirect_url": "/windows/apps/whats-new/build2021-docs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/publish/manage-account-settings-and-profile.md",
      "redirect_url": "/partner-center/partner-center-account-setup",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/master-details.md",
      "redirect_url": "/windows/uwp/design/controls-and-patterns/list-details",
      "redirect_document_id": true
    },
    {
      "source_path": "uwp/design/shell/tiles-and-notifications/send-local-toast-desktop.md",
      "redirect_url": "/windows/uwp/design/shell/tiles-and-notifications/send-local-toast",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/index.yml",
      "redirect_url": "/windows/dev-environment/javascript",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/beginners.md",
      "redirect_url": "/windows/dev-environment/javascript/nodejs-beginners-tutorial",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/setup-on-wsl2.md",
      "redirect_url": "/windows/dev-environment/javascript/nodejs-on-wsl",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/setup-on-windows.md",
      "redirect_url": "/windows/dev-environment/javascript/nodejs-on-windows",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/containers.md",
      "redirect_url": "/windows/wsl/tutorials/wsl-containers",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/nodejs/web-frameworks.md",
      "redirect_url": "/windows/dev-environment/javascript",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/android/react-native.md",
      "redirect_url": "/windows/dev-environment/javascript/react-native-for-android",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/features-and-technologies.md",
      "redirect_url": "/windows/apps/develop/index",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/develop/features-and-technologies.md",
      "redirect_url": "/windows/apps/develop/index",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/speech.md",
      "redirect_url": "/windows/apps/develop/speech",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/accessibility.md",
      "redirect_url": "/windows/apps/develop/accessibility",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/windows-app-sdk/older-downloads.md",
      "redirect_url": "/windows/apps/windows-app-sdk/downloads-archive",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/get-started/get-set-up.md",
      "redirect_url": "/windows/apps/windows-app-sdk/set-up-your-development-environment",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/get-started/get-set-up.md",
      "redirect_url": "/windows/apps/windows-app-sdk/set-up-your-development-environment",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/index.md",
      "redirect_url": "/windows/apps/windows-app-sdk/index",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/release-channels.md",
      "redirect_url": "/windows/apps/windows-app-sdk/release-channels",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/stable-channel.md",
      "redirect_url": "/windows/apps/windows-app-sdk/stable-channel",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/preview-channel.md",
      "redirect_url": "/windows/apps/windows-app-sdk/preview-channel",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/set-up-your-development-environment.md",
      "redirect_url": "/windows/apps/windows-app-sdk/set-up-your-development-environment",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/get-started-with-project-reunion.md",
      "redirect_url": "/windows/apps/windows-app-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/get-started.md",
      "redirect_url": "/windows/apps/windows-app-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/windows-app-sdk/get-started.md",
      "redirect_url": "/windows/apps/windows-app-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/update-existing-projects-to-the-latest-release.md",
      "redirect_url": "/windows/apps/windows-app-sdk/update-existing-projects-to-the-latest-release",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/mrtcore/mrtcore-overview.md",
      "redirect_url": "/windows/apps/windows-app-sdk/mrtcore/mrtcore-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/dwritecore.md",
      "redirect_url": "/windows/apps/windows-app-sdk/dwritecore",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/applifecycle/applifecycle-instancing.md",
      "redirect_url": "/windows/apps/windows-app-sdk/applifecycle/applifecycle-instancing",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/applifecycle/applifecycle-rich-activation.md",
      "redirect_url": "/windows/apps/windows-app-sdk/applifecycle/applifecycle-rich-activation",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/deploy-apps-that-use-project-reunion.md",
      "redirect_url": "/windows/apps/windows-app-sdk/deploy-apps-that-use-the-windows-app-sdk",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/deployment-architecture.md",
      "redirect_url": "/windows/apps/windows-app-sdk/deployment-architecture",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/deploy-packaged-apps.md",
      "redirect_url": "/windows/apps/windows-app-sdk/deploy-packaged-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/deploy-unpackaged-apps.md",
      "redirect_url": "/windows/apps/windows-app-sdk/deploy-unpackaged-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/tutorial-unpackaged-deployment.md",
      "redirect_url": "/windows/apps/windows-app-sdk/tutorial-unpackaged-deployment",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/check-project-reunion-versions.md",
      "redirect_url": "/windows/apps/windows-app-sdk/check-windows-app-sdk-versions",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/project-reunion/remove-project-reunion-versions.md",
      "redirect_url": "/windows/apps/windows-app-sdk/remove-windows-app-sdk-versions",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/reference/iwindownative.md",
      "redirect_url": "/windows/windows-app-sdk/api/win32/microsoft.ui.xaml.window/nn-microsoft-ui-xaml-window-iwindownative",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/reference/iwindownative-windowhandle.md",
      "redirect_url": "/windows/windows-app-sdk/api/win32/microsoft.ui.xaml.window/nf-microsoft-ui-xaml-window-iwindownative-get_windowhandle",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/windows-app-sdk/samples.md",
      "redirect_url": "/windows/apps/get-started/samples",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/windows-app-sdk/preview-experimental-install.md",
      "redirect_url": "/windows/apps/windows-app-sdk/set-up-your-development-environment",
      "redirect_document_id": true
    },
    {
      "source_path": "hub/apps/get-started/build-apps-for-windows.md",
      "redirect_url": "/windows/apps/winui/winui3/create-your-first-winui3-app",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3-winui2-comparison.md",
      "redirect_url": "/windows/apps/winui/",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/desktop-build-basic-winui3-app.md",
      "redirect_url": "/windows/apps/winui/winui3/desktop-winui3-app-with-basic-interop",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/release-notes/index.md",
      "redirect_url": "/windows/apps/winui/winui3/release-notes/release-notes-08-preview",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/get-started-winui3-for-desktop.md",
      "redirect_url": "/windows/apps/winui/winui3/create-your-first-winui3-app",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/get-started-winui3-for-uwp.md",
      "redirect_url": "/windows/apps/winui/winui3/create-your-first-winui3-app",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui2/winui-2.6.md",
      "redirect_url": "/windows/apps/winui/winui2/release-notes/winui-2.6",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/index.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getdisplayidfrommonitor.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getdisplayidfrommonitor",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.geticonfromiconid.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.geticonfromiconid",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.geticonidfromicon.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.geticonidfromicon",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getmonitorfromdisplayid.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getmonitorfromdisplayid",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getwindowfromwindowid.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getwindowfromwindowid",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getwindowidfromwindow.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.getwindowidfromwindow",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/winui/winui3/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop.md",
      "redirect_url": "/windows/apps/api-reference/cs-interop-apis/microsoft.ui/microsoft.ui.win32interop",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/desktop/choose-your-platform.md",
      "redirect_url": "/windows/apps/desktop#choose-your-app-type",
      "redirect_document_id": false
    },
    {
      "source_path": "hub/apps/10x/faq.md",
      "redirect_url": "/windows/apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessibility-checklist.md",
      "redirect_url": "/windows/apps/design/accessibility/accessibility-checklist",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessibility-in-the-store.md",
      "redirect_url": "/windows/apps/design/accessibility/accessibility-in-the-store",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessibility-overview.md",
      "redirect_url": "/windows/apps/design/accessibility/accessibility-overview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessibility-testing.md",
      "redirect_url": "/windows/apps/design/accessibility/accessibility-testing",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessibility.md",
      "redirect_url": "/windows/apps/design/accessibility/accessibility",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/accessible-text-requirements.md",
      "redirect_url": "/windows/apps/design/accessibility/accessible-text-requirements",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/basic-accessibility-information.md",
      "redirect_url": "/windows/apps/design/accessibility/basic-accessibility-information",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/control-patterns-and-interfaces.md",
      "redirect_url": "/windows/apps/design/accessibility/control-patterns-and-interfaces",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/custom-automation-peers.md",
      "redirect_url": "/windows/apps/design/accessibility/custom-automation-peers",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/designing-inclusive-software.md",
      "redirect_url": "/windows/apps/design/accessibility/designing-inclusive-software",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/developing-inclusive-windows-apps.md",
      "redirect_url": "/windows/apps/design/accessibility/developing-inclusive-windows-apps",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/high-contrast-themes.md",
      "redirect_url": "/windows/apps/design/accessibility/high-contrast-themes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/keyboard-accessibility.md",
      "redirect_url": "/windows/apps/design/accessibility/keyboard-accessibility",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/landmarks-and-headings.md",
      "redirect_url": "/windows/apps/design/accessibility/landmarks-and-headings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/practices-to-avoid.md",
      "redirect_url": "/windows/apps/design/accessibility/practices-to-avoid",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/accessibility/system-button-narration.md",
      "redirect_url": "/windows/apps/design/accessibility/system-button-narration",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/app-settings/guidelines-for-app-settings.md",
      "redirect_url": "/windows/apps/design/app-settings/guidelines-for-app-settings",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/app-settings/store-and-retrieve-app-data.md",
      "redirect_url": "/windows/apps/design/app-settings/store-and-retrieve-app-data",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/commanding-basics.md",
      "redirect_url": "/windows/apps/design/basics/commanding-basics",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/content-basics.md",
      "redirect_url": "/windows/apps/design/basics/content-basics",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/design-and-ui-intro.md",
      "redirect_url": "/windows/apps/design/basics/design-and-ui-intro",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/index.md",
      "redirect_url": "/windows/apps/design/basics/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/navigate-between-two-pages.md",
      "redirect_url": "/windows/apps/design/basics/navigate-between-two-pages",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/navigation-basics.md",
      "redirect_url": "/windows/apps/design/basics/navigation-basics",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/navigation-history-and-backwards-navigation.md",
      "redirect_url": "/windows/apps/design/basics/navigation-history-and-backwards-navigation",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/xaml-basics-adaptive-layout.md",
      "redirect_url": "/windows/apps/design/basics/xaml-basics-adaptive-layout",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/xaml-basics-style.md",
      "redirect_url": "/windows/apps/design/basics/xaml-basics-style",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/basics/xaml-basics-ui.md",
      "redirect_url": "/windows/apps/design/basics/xaml-basics-ui",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/app-bars.md",
      "redirect_url": "/windows/apps/design/controls/command-bar",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/auto-suggest-box.md",
      "redirect_url": "/windows/apps/design/controls/auto-suggest-box",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/buttons.md",
      "redirect_url": "/windows/apps/design/controls/buttons",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/calendar-date-picker.md",
      "redirect_url": "/windows/apps/design/controls/calendar-date-picker",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/calendar-view.md",
      "redirect_url": "/windows/apps/design/controls/calendar-view",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/checkbox.md",
      "redirect_url": "/windows/apps/design/controls/checkbox",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/collection-commanding.md",
      "redirect_url": "/windows/apps/design/controls/collection-commanding",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/color-picker.md",
      "redirect_url": "/windows/apps/design/controls/color-picker",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/combo-box.md",
      "redirect_url": "/windows/apps/design/controls/combo-box",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/command-bar-flyout.md",
      "redirect_url": "/windows/apps/design/controls/command-bar-flyout",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/commanding.md",
      "redirect_url": "/windows/apps/design/controls/commanding",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/contact-card.md",
      "redirect_url": "/windows/apps/design/controls/contact-card",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/content-links.md",
      "redirect_url": "/windows/apps/design/controls/content-links",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/control-templates.md",
      "redirect_url": "/windows/apps/design/style/xaml-control-templates",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/controls-and-events-intro.md",
      "redirect_url": "/windows/apps/design/controls/controls-and-events-intro",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/custom-transport-controls.md",
      "redirect_url": "/windows/apps/design/controls/custom-transport-controls",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/data-template-selector.md",
      "redirect_url": "/windows/apps/design/controls/data-template-selector",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/date-and-time.md",
      "redirect_url": "/windows/apps/design/controls/date-and-time",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/date-picker.md",
      "redirect_url": "/windows/apps/design/controls/date-picker",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/dialogs-and-flyouts/dialogs.md",
      "redirect_url": "/windows/apps/design/controls/dialogs-and-flyouts/dialogs",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/dialogs-and-flyouts/flyouts.md",
      "redirect_url": "/windows/apps/design/controls/dialogs-and-flyouts/flyouts",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/dialogs-and-flyouts/index.md",
      "redirect_url": "/windows/apps/design/controls/dialogs-and-flyouts/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/dialogs-and-flyouts/teaching-tip.md",
      "redirect_url": "/windows/apps/design/controls/dialogs-and-flyouts/teaching-tip",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/flipview.md",
      "redirect_url": "/windows/apps/design/controls/flipview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/forms.md",
      "redirect_url": "/windows/apps/design/controls/forms",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/hyperlinks.md",
      "redirect_url": "/windows/apps/design/controls/hyperlinks",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/images-imagebrushes.md",
      "redirect_url": "/windows/apps/design/controls/images-imagebrushes",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/index.md",
      "redirect_url": "/windows/apps/design/controls/index",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/infobar.md",
      "redirect_url": "/windows/apps/design/controls/infobar",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/inking-controls.md",
      "redirect_url": "/windows/apps/design/controls/inking-controls",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/inverted-lists.md",
      "redirect_url": "/windows/apps/design/controls/inverted-lists",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/item-containers-templates.md",
      "redirect_url": "/windows/apps/design/controls/item-containers-templates",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/item-templates-gridview.md",
      "redirect_url": "/windows/apps/design/controls/item-templates-gridview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/item-templates-listview.md",
      "redirect_url": "/windows/apps/design/controls/item-templates-listview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/items-repeater.md",
      "redirect_url": "/windows/apps/design/controls/items-repeater",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/labels.md",
      "redirect_url": "/windows/apps/design/controls/labels",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/list-details.md",
      "redirect_url": "/windows/apps/design/controls/list-details",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/lists.md",
      "redirect_url": "/windows/apps/design/controls/lists",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/listview-and-gridview.md",
      "redirect_url": "/windows/apps/design/controls/listview-and-gridview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/listview-filtering.md",
      "redirect_url": "/windows/apps/design/controls/listview-filtering",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/media-playback.md",
      "redirect_url": "/windows/apps/design/controls/media-playback",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/menus.md",
      "redirect_url": "/windows/apps/design/controls/menus",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/navigationview.md",
      "redirect_url": "/windows/apps/design/controls/navigationview",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/nested-ui.md",
      "redirect_url": "/windows/apps/design/controls/nested-ui",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/number-box.md",
      "redirect_url": "/windows/apps/design/controls/number-box",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/password-box.md",
      "redirect_url": "/windows/apps/design/controls/password-box",
      "redirect_document_id": false
    },
    {
      "source_path": "uwp/design/controls-and-patterns/person-picture.md",
      "redirect_url": "/windows/apps/design/controls/person-picture",
      "redirect_document_id":