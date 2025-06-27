Directory structure:
└── microsoftedge-webview2browser/
    ├── README.md
    ├── BrowserWindow.cpp
    ├── BrowserWindow.h
    ├── framework.h
    ├── LICENSE
    ├── packages.config
    ├── Resource.h
    ├── Tab.cpp
    ├── Tab.h
    ├── targetver.h
    ├── WebViewBrowserApp.cpp
    ├── WebViewBrowserApp.h
    ├── WebViewBrowserApp.rc
    ├── WebViewBrowserApp.sln
    ├── WebViewBrowserApp.vcxproj
    ├── WebViewBrowserApp.vcxproj.filters
    ├── .clang-format
    ├── wvbrowser_ui/
    │   ├── commands.js
    │   ├── content_ui/
    │   │   ├── favorites.html
    │   │   ├── favorites.js
    │   │   ├── history.css
    │   │   ├── history.html
    │   │   ├── history.js
    │   │   ├── items.css
    │   │   ├── settings.css
    │   │   ├── settings.html
    │   │   ├── settings.js
    │   │   └── styles.css
    │   └── controls_ui/
    │       ├── address-bar.css
    │       ├── controls.css
    │       ├── default.css
    │       ├── default.html
    │       ├── default.js
    │       ├── favorites.js
    │       ├── history.js
    │       ├── options.css
    │       ├── options.html
    │       ├── options.js
    │       ├── storage.js
    │       ├── strip.css
    │       ├── styles.css
    │       └── tabs.js
    └── .github/
        ├── CODE_OF_CONDUCT.md
        └── ISSUE_TEMPLATE/
            ├── config.yml
            └── issue-with-webview2browser-app.md


Files Content:

================================================
FILE: README.md
================================================
---
description: "A web browser built with the Microsoft Edge WebView2 control."
extendedZipContent:
  -
    path: LICENSE
    target: LICENSE
languages:
  - cpp
  - javascript
page_type: sample
products:
  - microsoft-edge
urlFragment: webview2browser
---
# WebView2Browser

A web browser built with the [Microsoft Edge WebView2](https://aka.ms/webview2) control.

![WebView2Browser](https://raw.githubusercontent.com/MicrosoftEdge/WebView2Browser/master/screenshots/WebView2Browser.png)

WebView2Browser is a sample Windows desktop application demonstrating the WebView2 control capabilities. It is built as a Win32 [Visual Studio 2019](https://visualstudio.microsoft.com/vs/) project and makes use of both C++ and JavaScript in the WebView2 environment to power its features.

WebView2Browser shows some of the simplest uses of WebView2 -such as creating and navigating a WebView, but also some more complex workflows like using the [PostWebMessageAsJson API](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2#postwebmessageasjson) to communicate WebViews in separate environments. It is intended as a rich code sample to look at how you can use WebView2 APIs to build your own app.

For more information, see the article in the Microsoft Edge Developer documentation: [WebView2Browser](https://learn.microsoft.com/microsoft-edge/webview2/samples/webview2browser).

## Requisites

* [Microsoft Edge (Chromium)](https://www.microsoftedgeinsider.com/download/) installed on a supported OS.
* [Visual Studio](https://visualstudio.microsoft.com/vs/) with C++ support installed.

The [WebView2 Runtime](https://developer.microsoft.com/microsoft-edge/webview2/) is recommended for the installation and the minimum version is 86.0.622.38.

## Build the browser

Clone the repository and open the solution in Visual Studio. WebView2 is already included as a NuGet package* in the project!

* Clone this repository
* Open the solution in Visual Studio 2019**
* Make the changes listed below if you're using a Windows version below Windows 10.
* Set the target you want to build (Debug/Release, x86/x64)
* Build the solution

That's it. Everything should be ready to just launch the app.

*You can get the WebView2 NuGet Package through the Visual Studio NuGet Package Manager.
**You can also use Visual Studio 2017 by changing the project's Platform Toolset in Project Properties/Configuration properties/General/Platform Toolset. You might also need to change the Windows SDK to the latest version available to you.

## Using versions below Windows 10

There's a couple of changes you need to make if you want to build and run the browser in other versions of Windows. This is because of how DPI is handled in Windows 10 vs previous versions of Windows.

In `WebViewBrowserApp.cpp`, you will need to replace the call to `SetProcessDpiAwarenessContext` and call `SetProcessDPIAware` instead.

```cpp
int APIENTRY wWinMain(_In_ HINSTANCE hInstance,
                      _In_opt_ HINSTANCE hPrevInstance,
                      _In_ LPWSTR    lpCmdLine,
                      _In_ int       nCmdShow)
{
    UNREFERENCED_PARAMETER(hPrevInstance);
    UNREFERENCED_PARAMETER(lpCmdLine);

    // Call SetProcessDPIAware() instead when using Windows 7 or any version
    // below 1703 (Windows 10).
    SetProcessDpiAwarenessContext(DPI_AWARENESS_CONTEXT_PER_MONITOR_AWARE_V2);

    BrowserWindow::RegisterClass(hInstance);

    // ...
```

In `BrowserWindow.cpp`, you will need to remove the call to `GetDpiForWindow`.

```cpp
int BrowserWindow::GetDPIAwareBound(int bound)
{
    // Remove the GetDpiForWindow call when using Windows 7 or any version
    // below 1607 (Windows 10). You will also have to make sure the build
    // directory is clean before building again.
    return (bound * GetDpiForWindow(m_hWnd) / DEFAULT_DPI);
}
```

## Browser layout

WebView2Browser has a multi-WebView approach to integrate web content and application UI into a Windows Desktop application. This allows the browser to use standard web technologies (HTML, CSS, JavaScript) to light up the interface but also enables the app to fetch favicons from the web and use IndexedDB for storing favorites and history.

The multi-WebView approach involves using two separate WebView environments (each with its own user data directory): one for the UI WebViews and the other for all content WebViews. UI WebViews (controls and options dropdown) use the UI environment while web content WebViews (one per tab) use the content environment.

![Browser layout](https://raw.githubusercontent.com/MicrosoftEdge/WebView2Browser/master/screenshots/layout.png)

## Features

WebView2Browser provides all the functionalities to make a basic web browser, but there's plenty of room for you to play around.

* Go back/forward
* Reload page
* Cancel navigation
* Multiple tabs
* History
* Favorites
* Search from the address bar
* Page security status
* Clearing cache and cookies

## WebView2 APIs

WebView2Browser makes use of a handful of the APIs available in WebView2. For the APIs not used here, you can find more about them in the [Microsoft Edge WebView2 Reference](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32). The following is a list of the most interesting APIs WebView2Browser uses and the feature(s) they enable.

API | Feature(s)
:--- | :---
CreateCoreWebView2EnvironmentWithOptions | Used to create the environments for UI and content WebViews. Different user data directories are passed to isolate UI from web content. |
ICoreWebView2 | There are several WebViews in WebView2Browser and most features make use of members in this interface, the table below shows how they're used.
ICoreWebView2DevToolsProtocolEventReceivedEventHandler | Used along with add_DevToolsProtocolEventReceived to listen for CDP security events to update the lock icon in the browser UI. |
ICoreWebView2DevToolsProtocolEventReceiver | Used along with add_DevToolsProtocolEventReceived to listen for CDP security events to update the lock icon in the browser UI. |
ICoreWebView2ExecuteScriptCompletedHandler | Used along with ExecuteScript to get the title and favicon from the visited page. |
ICoreWebView2FocusChangedEventHandler | Used along with add_LostFocus to hide the browser options dropdown when it loses focus.
ICoreWebView2HistoryChangedEventHandler | Used along with add_HistoryChanged to update the navigation buttons in the browser UI. |
ICoreWebView2Controller | There are several WebViewControllers in WebView2Browser and we fetch the associated WebViews from them.
ICoreWebView2NavigationCompletedEventHandler | Used along with add_NavigationCompleted to update the reload button in the browser UI.
ICoreWebView2Settings | Used to disable DevTools in the browser UI.
ICoreWebView2SourceChangedEventHandler | Used along with add_SourceChanged to update the address bar in the browser UI. |
ICoreWebView2WebMessageReceivedEventHandler | This is one of the most important APIs to WebView2Browser. Most functionalities involving communication across WebViews use this.

ICoreWebView2 API | Feature(s)
:--- | :---
add_NavigationStarting | Used to display the cancel navigation button in the controls WebView.
add_SourceChanged | Used to update the address bar.
add_HistoryChanged | Used to update go back/forward buttons.
add_NavigationCompleted | Used to display the reload button once a navigation completes.
ExecuteScript | Used to get the title and favicon of a visited page.
PostWebMessageAsJson | Used to communicate WebViews. All messages use JSON to pass parameters needed.
add_WebMessageReceived | Used to handle web messages posted to the WebView.
CallDevToolsProtocolMethod | Used to enable listening for security events, which will notify of security status changes in a document.

ICoreWebView2Controller API | Feature(s)
:--- | :---
get_CoreWebView2 | Used to get the CoreWebView2 associated with this CoreWebView2Controller.
add_LostFocus | Used to hide the options dropdown when the user clicks away of it.

## Implementing the features

The sections below describe how some of the features in WebView2Browser were implemented. You can look at the source code for more details about how everything works here.

* [The basics](#the-basics)
  * [Set up the environment, create a WebView](#set-up-the-environment-create-a-webview)
  * [Navigate to web page](#navigate-to-web-page)
  * [Updating the address bar](#updating-the-address-bar)
  * [Going back, going forward](#going-back-going-forward)
* [Some interesting features](#some-interesting-features)
  * [Communicating the WebViews](#communicating-the-webviews)
  * [Tab handling](#tab-handling)
  * [Updating the security icon](#updating-the-security-icon)
  * [Populating the history](#populating-the-history)
* [Handling JSON and URIs](#handling-json-and-uris)

## The basics

### Set up the environment, create a WebView

WebView2 allows you to host web content in your Windows app. It exposes the globals [CreateCoreWebView2Environment](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/webview2-idl#createcorewebview2environment) and [CreateCoreWebView2EnvironmentWithOptions](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/webview2-idl#createcorewebview2environmentwithoptions) from which we can create the two separate environments for the browser's UI and content.

```cpp
    // Get directory for user data. This will be kept separated from the
    // directory for the browser UI data.
    std::wstring userDataDirectory = GetAppDataDirectory();
    userDataDirectory.append(L"\\User Data");

    // Create WebView environment for web content requested by the user. All
    // tabs will be created from this environment and kept isolated from the
    // browser UI. This environment is created first so the UI can request new
    // tabs when it's ready.
    HRESULT hr = CreateCoreWebView2EnvironmentWithOptions(nullptr, userDataDirectory.c_str(),
        L"", Callback<ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler>(
            [this](HRESULT result, ICoreWebView2Environment* env) -> HRESULT
    {
        RETURN_IF_FAILED(result);

        m_contentEnv = env;
        HRESULT hr = InitUIWebViews();

        if (!SUCCEEDED(hr))
        {
            OutputDebugString(L"UI WebViews environment creation failed\n");
        }

        return hr;
    }).Get());
```

```cpp
HRESULT BrowserWindow::InitUIWebViews()
{
    // Get data directory for browser UI data
    std::wstring browserDataDirectory = GetAppDataDirectory();
    browserDataDirectory.append(L"\\Browser Data");

    // Create WebView environment for browser UI. A separate data directory is
    // used to isolate the browser UI from web content requested by the user.
    return CreateCoreWebView2EnvironmentWithOptions(nullptr, browserDataDirectory.c_str(),
        L"", Callback<ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler>(
            [this](HRESULT result, ICoreWebView2Environment* env) -> HRESULT
    {
        // Environment is ready, create the WebView
        m_uiEnv = env;

        RETURN_IF_FAILED(CreateBrowserControlsWebView());
        RETURN_IF_FAILED(CreateBrowserOptionsWebView());

        return S_OK;
    }).Get());
}
```

We use the [ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2createcorewebview2environmentcompletedhandler) to create the UI WebViews once the environment is ready.

```cpp
HRESULT BrowserWindow::CreateBrowserControlsWebView()
{
    return m_uiEnv->CreateCoreWebView2Controller(m_hWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this](HRESULT result, ICoreWebView2Controller* controller) -> HRESULT
    {
        if (!SUCCEEDED(result))
        {
            OutputDebugString(L"Controls WebView creation failed\n");
            return result;
        }
        // WebView created
        m_controlsController = controller;
        CheckFailure(m_controlsController->get_CoreWebView2(&m_controlsWebView), L"");

        wil::com_ptr<ICoreWebView2Settings> settings;
        RETURN_IF_FAILED(m_controlsWebView->get_Settings(&settings));
        RETURN_IF_FAILED(settings->put_AreDevToolsEnabled(FALSE));

        RETURN_IF_FAILED(m_controlsController->add_ZoomFactorChanged(Callback<ICoreWebView2ZoomFactorChangedEventHandler>(
            [](ICoreWebView2Controller* controller, IUnknown* args) -> HRESULT
        {
            controller->put_ZoomFactor(1.0);
            return S_OK;
        }
        ).Get(), &m_controlsZoomToken));

        RETURN_IF_FAILED(m_controlsWebView->add_WebMessageReceived(m_uiMessageBroker.Get(), &m_controlsUIMessageBrokerToken));
        RETURN_IF_FAILED(ResizeUIWebViews());

        std::wstring controlsPath = GetFullPathFor(L"wvbrowser_ui\\controls_ui\\default.html");
        RETURN_IF_FAILED(m_controlsWebView->Navigate(controlsPath.c_str()));

        return S_OK;
    }).Get());
}
```

We're setting up a few things here. The [ICoreWebView2Settings](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2settings) interface is used to disable DevTools in the WebView powering the browser controls. We're also adding a handler for received web messages. This handler will enable us to do something when the user interacts with the controls in this WebView.

### Navigate to web page

You can navigate to a web page by entering its URI in the address bar. When pressing Enter, the controls WebView will post a web message to the host app so it can navigate the active tab to the specified location. Code below shows how the host Win32 application will handle that message.

```cpp
        case MG_NAVIGATE:
        {
            std::wstring uri(args.at(L"uri").as_string());
            std::wstring browserScheme(L"browser://");

            if (uri.substr(0, browserScheme.size()).compare(browserScheme) == 0)
            {
                // No encoded search URI
                std::wstring path = uri.substr(browserScheme.size());
                if (path.compare(L"favorites") == 0 ||
                    path.compare(L"settings") == 0 ||
                    path.compare(L"history") == 0)
                {
                    std::wstring filePath(L"wvbrowser_ui\\content_ui\\");
                    filePath.append(path);
                    filePath.append(L".html");
                    std::wstring fullPath = GetFullPathFor(filePath.c_str());
                    CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(fullPath.c_str()), L"Can't navigate to browser page.");
                }
                else
                {
                    OutputDebugString(L"Requested unknown browser page\n");
                }
            }
            else if (!SUCCEEDED(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(uri.c_str())))
            {
                CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(args.at(L"encodedSearchURI").as_string().c_str()), L"Can't navigate to requested page.");
            }
        }
        break;
```

WebView2Browser will check the URI against browser pages (i.e. favorites, settings, history) and navigate to the requested location or use the provided URI to search Bing as a fallback.

### Updating the address bar

The address bar is updated every time there is a change in the active tab's document source and along with other controls when switching tabs. Each WebView will fire an event when the state of the document changes, we can use this event to get the new source on updates and forward the change to the controls WebView (we'll also update the go back and go forward buttons).

```cpp
        // Register event handler for doc state change
        RETURN_IF_FAILED(m_contentWebView->add_SourceChanged(Callback<ICoreWebView2SourceChangedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2SourceChangedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabURIUpdate(m_tabId, webview), L"Can't update address bar");

            return S_OK;
        }).Get(), &m_uriUpdateForwarderToken));
```

```cpp
HRESULT BrowserWindow::HandleTabURIUpdate(size_t tabId, ICoreWebView2* webview)
{
    wil::unique_cotaskmem_string source;
    RETURN_IF_FAILED(webview->get_Source(&source));

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_UPDATE_URI);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
    jsonObj[L"args"][L"uri"] = web::json::value(source.get());

    // ...

    RETURN_IF_FAILED(PostJsonToWebView(jsonObj, m_controlsWebView.Get()));

    return S_OK;
}

HRESULT BrowserWindow::HandleTabHistoryUpdate(size_t tabId, ICoreWebView2* webview)
{
    // ...

    BOOL canGoForward = FALSE;
    RETURN_IF_FAILED(webview->get_CanGoForward(&canGoForward));
    jsonObj[L"args"][L"canGoForward"] = web::json::value::boolean(canGoForward);

    BOOL canGoBack = FALSE;
    RETURN_IF_FAILED(webview->get_CanGoBack(&canGoBack));
    jsonObj[L"args"][L"canGoBack"] = web::json::value::boolean(canGoBack);

    RETURN_IF_FAILED(PostJsonToWebView(jsonObj, m_controlsWebView.Get()));

    return S_OK;
}
```

We have sent the `MG_UPDATE_URI` message along with the URI to the controls WebView. Now we want to reflect those changes on the tab state and update the UI if necessary.

```javascript
        case commands.MG_UPDATE_URI:
            if (isValidTabId(args.tabId)) {
                const tab = tabs.get(args.tabId);
                let previousURI = tab.uri;

                // Update the tab state
                tab.uri = args.uri;
                tab.uriToShow = args.uriToShow;
                tab.canGoBack = args.canGoBack;
                tab.canGoForward = args.canGoForward;

                // If the tab is active, update the controls UI
                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }

                // ...
            }
            break;
```

### Going back, going forward

Each WebView will keep a history for the navigations it has performed so we only need to connect the browser UI with the corresponding methods. If the active tab's WebView can be navigated back/forward, the buttons will post a web message to the host application when clicked.

The JavaScript side:

```javascript
    document.querySelector('#btn-forward').addEventListener('click', function(e) {
        if (document.getElementById('btn-forward').className === 'btn') {
            var message = {
                message: commands.MG_GO_FORWARD,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        }
    });

    document.querySelector('#btn-back').addEventListener('click', function(e) {
        if (document.getElementById('btn-back').className === 'btn') {
            var message = {
                message: commands.MG_GO_BACK,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        }
    });
```

The host application side:

```cpp
        case MG_GO_FORWARD:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->GoForward(), L"");
        }
        break;
        case MG_GO_BACK:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->GoBack(), L"");
        }
        break;
```

### Reloading, stop navigation

We use the `NavigationStarting` event fired by a content WebView to update its associated tab loading state in the controls WebView. Similarly, when a WebView fires the `NavigationCompleted` event, we use that event to instruct the controls WebView to update the tab state. The active tab state in the controls WebView will determine whether to show the reload or the cancel button. Each of those will post a message back to the host application when clicked, so that the WebView for that tab can be reloaded or have its navigation canceled, accordingly.

```javascript
function reloadActiveTabContent() {
    var message = {
        message: commands.MG_RELOAD,
        args: {}
    };
    window.chrome.webview.postMessage(message);
}

 // ...

    document.querySelector('#btn-reload').addEventListener('click', function(e) {
        var btnReload = document.getElementById('btn-reload');
        if (btnReload.className === 'btn-cancel') {
            var message = {
                message: commands.MG_CANCEL,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        } else if (btnReload.className === 'btn') {
            reloadActiveTabContent();
        }
    });
```

```cpp
        case MG_RELOAD:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Reload(), L"");
        }
        break;
        case MG_CANCEL:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->CallDevToolsProtocolMethod(L"Page.stopLoading", L"{}", nullptr), L"");
        }
```

## Some interesting features

### Communicating the WebViews

We need to communicate the WebViews powering tabs and UI so that user interactions in one have the desired effect in the other. WebView2Browser makes use of set of very useful WebView2 APIs for this purpose, including [PostWebMessageAsJson](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2#postwebmessageasjson), [add_WebMessageReceived](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2#add_webmessagereceived) and [ICoreWebView2WebMessageReceivedEventHandler](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2webmessagereceivedeventhandler). On the JavaScript side, we're making use of the `window.chrome.webview` object exposed to call the `postMessage` method and add an event lister for received messages.

```cpp
HRESULT BrowserWindow::CreateBrowserControlsWebView()
{
    return m_uiEnv->CreateCoreWebView2Controller(m_hWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this](HRESULT result, ICoreWebView2Controller* controller) -> HRESULT
    {
        // ...

        RETURN_IF_FAILED(m_controlsWebView->add_WebMessageReceived(m_uiMessageBroker.Get(), &m_controlsUIMessageBrokerToken));

        // ...

        return S_OK;
    }).Get());
}
```

```cpp
HRESULT BrowserWindow::PostJsonToWebView(web::json::value jsonObj, ICoreWebView2* webview)
{
    utility::stringstream_t stream;
    jsonObj.serialize(stream);

    return webview->PostWebMessageAsJson(stream.str().c_str());
}

// ...

HRESULT BrowserWindow::HandleTabNavStarting(size_t tabId, ICoreWebView2* webview)
{
    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_NAV_STARTING);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);

    return PostJsonToWebView(jsonObj, m_controlsWebView.Get());
}
```

```javascript
function init() {
    window.chrome.webview.addEventListener('message', messageHandler);
    refreshControls();
    refreshTabs();

    createNewTab(true);
}

// ...

function reloadActiveTabContent() {
    var message = {
        message: commands.MG_RELOAD,
        args: {}
    };
    window.chrome.webview.postMessage(message);
}
```

### Tab handling

A new tab will be created whenever the user clicks on the new tab button to the right of the open tabs. The controls WebView will post a message to the host application to create the WebView for that tab and create an object tracking its state.

```javascript
function createNewTab(shouldBeActive) {
    const tabId = getNewTabId();

    var message = {
        message: commands.MG_CREATE_TAB,
        args: {
            tabId: parseInt(tabId),
            active: shouldBeActive || false
        }
    };

    window.chrome.webview.postMessage(message);

    tabs.set(parseInt(tabId), {
        title: 'New Tab',
        uri: '',
        uriToShow: '',
        favicon: 'img/favicon.png',
        isFavorite: false,
        isLoading: false,
        canGoBack: false,
        canGoForward: false,
        securityState: 'unknown',
        historyItemId: INVALID_HISTORY_ID
    });

    loadTabUI(tabId);

    if (shouldBeActive) {
        switchToTab(tabId, false);
    }
}
```

On the host app side, the registered [ICoreWebView2WebMessageReceivedEventHandler](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2webmessagereceivedeventhandler) will catch the message and create the WebView for that tab.

```cpp
        case MG_CREATE_TAB:
        {
            size_t id = args.at(L"tabId").as_number().to_uint32();
            bool shouldBeActive = args.at(L"active").as_bool();
            std::unique_ptr<Tab> newTab = Tab::CreateNewTab(m_hWnd, m_contentEnv.Get(), id, shouldBeActive);

            std::map<size_t, std::unique_ptr<Tab>>::iterator it = m_tabs.find(id);
            if (it == m_tabs.end())
            {
                m_tabs.insert(std::pair<size_t,std::unique_ptr<Tab>>(id, std::move(newTab)));
            }
            else
            {
                m_tabs.at(id)->m_contentWebView->Close();
                it->second = std::move(newTab);
            }
        }
        break;
```

```cpp
std::unique_ptr<Tab> Tab::CreateNewTab(HWND hWnd, ICoreWebView2Environment* env, size_t id, bool shouldBeActive)
{
    std::unique_ptr<Tab> tab = std::make_unique<Tab>();

    tab->m_parentHWnd = hWnd;
    tab->m_tabId = id;
    tab->SetMessageBroker();
    tab->Init(env, shouldBeActive);

    return tab;
}

HRESULT Tab::Init(ICoreWebView2Environment* env, bool shouldBeActive)
{
    return env->CreateCoreWebView2Controller(m_parentHWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this, shouldBeActive](HRESULT result, ICoreWebView2Controller* controller) -> HRESULT {
        if (!SUCCEEDED(result))
        {
            OutputDebugString(L"Tab WebView creation failed\n");
            return result;
        }
        m_contentController = controller;
        BrowserWindow::CheckFailure(m_contentController->get_CoreWebView2(&m_contentWebView), L"");
        BrowserWindow* browserWindow = reinterpret_cast<BrowserWindow*>(GetWindowLongPtr(m_parentHWnd, GWLP_USERDATA));
        RETURN_IF_FAILED(m_contentWebView->add_WebMessageReceived(m_messageBroker.Get(), &m_messageBrokerToken));

        // Register event handler for history change
        RETURN_IF_FAILED(m_contentWebView->add_HistoryChanged(Callback<ICoreWebView2HistoryChangedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, IUnknown* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabHistoryUpdate(m_tabId, webview), L"Can't update go back/forward buttons.");

            return S_OK;
        }).Get(), &m_historyUpdateForwarderToken));

        // Register event handler for source change
        RETURN_IF_FAILED(m_contentWebView->add_SourceChanged(Callback<ICoreWebView2SourceChangedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2SourceChangedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabURIUpdate(m_tabId, webview), L"Can't update address bar");

            return S_OK;
        }).Get(), &m_uriUpdateForwarderToken));

        RETURN_IF_FAILED(m_contentWebView->add_NavigationStarting(Callback<ICoreWebView2NavigationStartingEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2NavigationStartingEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabNavStarting(m_tabId, webview), L"Can't update reload button");

            return S_OK;
        }).Get(), &m_navStartingToken));

        RETURN_IF_FAILED(m_contentWebView->add_NavigationCompleted(Callback<ICoreWebView2NavigationCompletedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2NavigationCompletedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabNavCompleted(m_tabId, webview, args), L"Can't update reload button");
            return S_OK;
        }).Get(), &m_navCompletedToken));

        // Handle security state updates

        RETURN_IF_FAILED(m_contentWebView->Navigate(L"https://www.bing.com"));
        browserWindow->HandleTabCreated(m_tabId, shouldBeActive);

        return S_OK;
    }).Get());
}
```

The tab registers all handlers so it can forward updates to the controls WebView when events fire. The tab is ready and will be shown on the content area of the browser. Clicking on a tab in the controls WebView will post a message to the host application, which will in turn hide the WebView for the previously active tab and show the one for the clicked tab.

```cpp
HRESULT BrowserWindow::SwitchToTab(size_t tabId)
{
    size_t previousActiveTab = m_activeTabId;

    RETURN_IF_FAILED(m_tabs.at(tabId)->ResizeWebView());
    RETURN_IF_FAILED(m_tabs.at(tabId)->m_contentWebView->put_IsVisible(TRUE));
    m_activeTabId = tabId;

    if (previousActiveTab != INVALID_TAB_ID && previousActiveTab != m_activeTabId)
    {
        RETURN_IF_FAILED(m_tabs.at(previousActiveTab)->m_contentWebView->put_IsVisible(FALSE));
    }

    return S_OK;
}
```

### Updating the security icon

We use the [CallDevToolsProtocolMethod](https://learn.microsoft.com/microsoft-edge/webview2/reference/win32/icorewebview2#calldevtoolsprotocolmethod) to enable listening for security events. Whenever a `securityStateChanged` event is fired, we will use the new state to update the security icon on the controls WebView.

```cpp
        // Enable listening for security events to update secure icon
        RETURN_IF_FAILED(m_contentWebView->CallDevToolsProtocolMethod(L"Security.enable", L"{}", nullptr));

        BrowserWindow::CheckFailure(m_contentWebView->GetDevToolsProtocolEventReceiver(L"Security.securityStateChanged", &m_securityStateChangedReceiver), L"");

        // Forward security status updates to browser
        RETURN_IF_FAILED(m_securityStateChangedReceiver->add_DevToolsProtocolEventReceived(Callback<ICoreWebView2DevToolsProtocolEventReceivedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2DevToolsProtocolEventReceivedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabSecurityUpdate(m_tabId, webview, args), L"Can't update security icon");
            return S_OK;
        }).Get(), &m_securityUpdateToken));
```

```cpp
HRESULT BrowserWindow::HandleTabSecurityUpdate(size_t tabId, ICoreWebView2* webview, ICoreWebView2DevToolsProtocolEventReceivedEventArgs* args)
{
    wil::unique_cotaskmem_string jsonArgs;
    RETURN_IF_FAILED(args->get_ParameterObjectAsJson(&jsonArgs));
    web::json::value securityEvent = web::json::value::parse(jsonArgs.get());

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_SECURITY_UPDATE);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
    jsonObj[L"args"][L"state"] = securityEvent.at(L"securityState");

    return PostJsonToWebView(jsonObj, m_controlsWebView.Get());
}
```

```javascript
        case commands.MG_SECURITY_UPDATE:
            if (isValidTabId(args.tabId)) {
                const tab = tabs.get(args.tabId);
                tab.securityState = args.state;

                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }
            }
            break;
```

### Populating the history

WebView2Browser uses IndexedDB in the controls WebView to store history items, just an example of how WebView2 enables you to access standard web technologies as you would in the browser. The item for a navigation will be created as soon as the URI is updated. These items are then retrieved by the history UI in a tab making use of `window.chrome.postMessage`.

In this case, most functionality is implemented using JavaScript on both ends (controls WebView and content WebView loading the UI) so the host application is only acting as a message broker to communicate those ends.

```javascript
        case commands.MG_UPDATE_URI:
            if (isValidTabId(args.tabId)) {
                // ...

                // Don't add history entry if URI has not changed
                if (tab.uri == previousURI) {
                    break;
                }

                // Filter URIs that should not appear in history
                if (!tab.uri || tab.uri == 'about:blank') {
                    tab.historyItemId = INVALID_HISTORY_ID;
                    break;
                }

                if (tab.uriToShow && tab.uriToShow.substring(0, 10) == 'browser://') {
                    tab.historyItemId = INVALID_HISTORY_ID;
                    break;
                }

                addHistoryItem(historyItemFromTab(args.tabId), (id) => {
                    tab.historyItemId = id;
                });
            }
            break;
```

```javascript
function addHistoryItem(item, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['history'], 'readwrite');
        let historyStore = transaction.objectStore('history');

        // Check if an item for this URI exists on this day
        let currentDate = new Date();
        let year = currentDate.getFullYear();
        let month = currentDate.getMonth();
        let date = currentDate.getDate();
        let todayDate = new Date(year, month, date);

        let existingItemsIndex = historyStore.index('stampedURI');
        let lowerBound = [item.uri, todayDate];
        let upperBound = [item.uri, currentDate];
        let range = IDBKeyRange.bound(lowerBound, upperBound);
        let request = existingItemsIndex.openCursor(range);

        request.onsuccess = function(event) {
            let cursor = event.target.result;
            if (cursor) {
                // There's an entry for this URI, update the item
                cursor.value.timestamp = item.timestamp;
                let updateRequest = cursor.update(cursor.value);

                updateRequest.onsuccess = function(event) {
                    if (callback) {
                        callback(event.target.result.primaryKey);
                    }
                };
            } else {
                // No entry for this URI, add item
                let addItemRequest = historyStore.add(item);

                addItemRequest.onsuccess = function(event) {
                    if (callback) {
                        callback(event.target.result);
                    }
                };
            }
        };

    });
}
```

## Handling JSON and URIs

WebView2Browser uses Microsoft's [cpprestsdk (Casablanca)](https://github.com/Microsoft/cpprestsdk) to handle all JSON in the C++ side of things. IUri and CreateUri are also used to parse file paths into URIs and can be used to for other URIs as well.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.



================================================
FILE: BrowserWindow.cpp
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#include "BrowserWindow.h"
#include "shlobj.h"
#include <Urlmon.h>
#pragma comment (lib, "Urlmon.lib")

using namespace Microsoft::WRL;

WCHAR BrowserWindow::s_windowClass[] = { 0 };
WCHAR BrowserWindow::s_title[] = { 0 };

//
//  FUNCTION: RegisterClass()
//
//  PURPOSE: Registers the window class.
//
ATOM BrowserWindow::RegisterClass(_In_ HINSTANCE hInstance)
{
    // Initialize window class string
    LoadStringW(hInstance, IDC_WEBVIEWBROWSERAPP, s_windowClass, MAX_LOADSTRING);
    WNDCLASSEXW wcex;

    wcex.cbSize = sizeof(WNDCLASSEX);

    wcex.style = CS_HREDRAW | CS_VREDRAW;
    wcex.lpfnWndProc = WndProcStatic;
    wcex.cbClsExtra = 0;
    wcex.cbWndExtra = 0;
    wcex.hInstance = hInstance;
    wcex.hIcon = LoadIcon(hInstance, MAKEINTRESOURCE(IDI_WEBVIEWBROWSERAPP));
    wcex.hCursor = LoadCursor(nullptr, IDC_ARROW);
    wcex.hbrBackground = (HBRUSH)(COLOR_WINDOW + 1);
    wcex.lpszMenuName = MAKEINTRESOURCEW(IDC_WEBVIEWBROWSERAPP);
    wcex.lpszClassName = s_windowClass;
    wcex.hIconSm = LoadIcon(wcex.hInstance, MAKEINTRESOURCE(IDI_SMALL));

    return RegisterClassExW(&wcex);
}

//
//  FUNCTION: WndProcStatic(HWND, UINT, WPARAM, LPARAM)
//
//  PURPOSE: Redirect messages to approriate instance or call default proc
//
//  WM_COMMAND  - process the application menu
//  WM_PAINT    - Paint the main window
//  WM_DESTROY  - post a quit message and return
//
//
LRESULT CALLBACK BrowserWindow::WndProcStatic(HWND hWnd, UINT message, WPARAM wParam, LPARAM lParam)
{
    // Get the ptr to the BrowserWindow instance who created this hWnd.
    // The pointer was set when the hWnd was created during InitInstance.
    BrowserWindow* browser_window = reinterpret_cast<BrowserWindow*>(GetWindowLongPtr(hWnd, GWLP_USERDATA));
    if (browser_window != nullptr)
    {
        return browser_window->WndProc(hWnd, message, wParam, lParam);  // Forward message to instance-aware WndProc
    }
    else
    {
        return DefWindowProc(hWnd, message, wParam, lParam);
    }
}

//
//  FUNCTION: WndProc(HWND, UINT, WPARAM, LPARAM)
//
//  PURPOSE: Processes messages for each browser window instance.
//
//  WM_COMMAND  - process the application menu
//  WM_PAINT    - Paint the main window
//  WM_DESTROY  - post a quit message and return
//
//
LRESULT CALLBACK BrowserWindow::WndProc(HWND hWnd, UINT message, WPARAM wParam, LPARAM lParam)
{

    switch (message)
    {
    case WM_GETMINMAXINFO:
    {
        MINMAXINFO* minmax = reinterpret_cast<MINMAXINFO*>(lParam);
        minmax->ptMinTrackSize.x = m_minWindowWidth;
        minmax->ptMinTrackSize.y = m_minWindowHeight;
    }
    break;
    case WM_DPICHANGED:
    {
        UpdateMinWindowSize();
    }
    case WM_SIZE:
    {
        ResizeUIWebViews();
        if (m_tabs.find(m_activeTabId) != m_tabs.end())
        {
            m_tabs.at(m_activeTabId)->ResizeWebView();
        }
    }
    break;
    case WM_CLOSE:
    {
        web::json::value jsonObj = web::json::value::parse(L"{}");
        jsonObj[L"message"] = web::json::value(MG_CLOSE_WINDOW);
        jsonObj[L"args"] = web::json::value::parse(L"{}");

        CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Try again.");
    }
    break;
    case WM_NCDESTROY:
    {
        SetWindowLongPtr(hWnd, GWLP_USERDATA, NULL);
        delete this;
        PostQuitMessage(0);
    }
    case WM_PAINT:
    {
        PAINTSTRUCT ps;
        HDC hdc = BeginPaint(hWnd, &ps);
        EndPaint(hWnd, &ps);
    }
    break;
    default:
    {
        return DefWindowProc(hWnd, message, wParam, lParam);
    }
    break;
    }
    return 0;
}


BOOL BrowserWindow::LaunchWindow(_In_ HINSTANCE hInstance, _In_ int nCmdShow)
{
    // BrowserWindow keeps a reference to itself in its host window and will
    // delete itself when the window is destroyed.
    BrowserWindow* window = new BrowserWindow();
    if (!window->InitInstance(hInstance, nCmdShow))
    {
        delete window;
        return FALSE;
    }
    return TRUE;
}

//
//   FUNCTION: InitInstance(HINSTANCE, int)
//
//   PURPOSE: Saves instance handle and creates main window
//
//   COMMENTS:
//
//        In this function, we save the instance handle in a global variable and
//        create and display the main program window.
//
BOOL BrowserWindow::InitInstance(HINSTANCE hInstance, int nCmdShow)
{
    m_hInst = hInstance; // Store app instance handle
    LoadStringW(m_hInst, IDS_APP_TITLE, s_title, MAX_LOADSTRING);

    SetUIMessageBroker();

    m_hWnd = CreateWindowW(s_windowClass, s_title, WS_OVERLAPPEDWINDOW,
        CW_USEDEFAULT, 0, CW_USEDEFAULT, 0, nullptr, nullptr, m_hInst, nullptr);

    if (!m_hWnd)
    {
        return FALSE;
    }

    // Make the BrowserWindow instance ptr available through the hWnd
    SetWindowLongPtr(m_hWnd, GWLP_USERDATA, reinterpret_cast<LONG_PTR>(this));

    UpdateMinWindowSize();
    ShowWindow(m_hWnd, nCmdShow);
    UpdateWindow(m_hWnd);

    // Get directory for user data. This will be kept separated from the
    // directory for the browser UI data.
    std::wstring userDataDirectory = GetAppDataDirectory();
    userDataDirectory.append(L"\\User Data");

    // Create WebView environment for web content requested by the user. All
    // tabs will be created from this environment and kept isolated from the
    // browser UI. This enviroment is created first so the UI can request new
    // tabs when it's ready.
    HRESULT hr = CreateCoreWebView2EnvironmentWithOptions(nullptr, userDataDirectory.c_str(),
        nullptr, Callback<ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler>(
            [this](HRESULT result, ICoreWebView2Environment* env) -> HRESULT
    {
        RETURN_IF_FAILED(result);

        m_contentEnv = env;
        HRESULT hr = InitUIWebViews();

        if (!SUCCEEDED(hr))
        {
            OutputDebugString(L"UI WebViews environment creation failed\n");
        }

        return hr;
    }).Get());

    if (!SUCCEEDED(hr))
    {
        OutputDebugString(L"Content WebViews environment creation failed\n");
        return FALSE;
    }

    return TRUE;
}

HRESULT BrowserWindow::InitUIWebViews()
{
    // Get data directory for browser UI data
    std::wstring browserDataDirectory = GetAppDataDirectory();
    browserDataDirectory.append(L"\\Browser Data");

    // Create WebView environment for browser UI. A separate data directory is
    // used to isolate the browser UI from web content requested by the user.
    return CreateCoreWebView2EnvironmentWithOptions(nullptr, browserDataDirectory.c_str(),
        nullptr, Callback<ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler>(
            [this](HRESULT result, ICoreWebView2Environment* env) -> HRESULT
    {
        // Environment is ready, create the WebView
        m_uiEnv = env;

        RETURN_IF_FAILED(CreateBrowserControlsWebView());
        RETURN_IF_FAILED(CreateBrowserOptionsWebView());

        return S_OK;
    }).Get());
}

HRESULT BrowserWindow::CreateBrowserControlsWebView()
{
    return m_uiEnv->CreateCoreWebView2Controller(m_hWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this](HRESULT result, ICoreWebView2Controller* host) -> HRESULT
    {
        if (!SUCCEEDED(result))
        {
            OutputDebugString(L"Controls WebView creation failed\n");
            return result;
        }
        // WebView created
        m_controlsController = host;
        CheckFailure(m_controlsController->get_CoreWebView2(&m_controlsWebView), L"");

        wil::com_ptr<ICoreWebView2Settings> settings;
        RETURN_IF_FAILED(m_controlsWebView->get_Settings(&settings));
        RETURN_IF_FAILED(settings->put_AreDevToolsEnabled(FALSE));

        RETURN_IF_FAILED(m_controlsController->add_ZoomFactorChanged(Callback<ICoreWebView2ZoomFactorChangedEventHandler>(
            [](ICoreWebView2Controller* host, IUnknown* args) -> HRESULT
        {
            host->put_ZoomFactor(1.0);
            return S_OK;
        }
        ).Get(), &m_controlsZoomToken));

        RETURN_IF_FAILED(m_controlsWebView->add_WebMessageReceived(m_uiMessageBroker.Get(), &m_controlsUIMessageBrokerToken));
        RETURN_IF_FAILED(ResizeUIWebViews());

        std::wstring controlsPath = GetFullPathFor(L"wvbrowser_ui\\controls_ui\\default.html");
        RETURN_IF_FAILED(m_controlsWebView->Navigate(controlsPath.c_str()));

        return S_OK;
    }).Get());
}

HRESULT BrowserWindow::CreateBrowserOptionsWebView()
{
    return m_uiEnv->CreateCoreWebView2Controller(m_hWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this](HRESULT result, ICoreWebView2Controller* host) -> HRESULT
    {
        if (!SUCCEEDED(result))
        {
            OutputDebugString(L"Options WebView creation failed\n");
            return result;
        }
        // WebView created
        m_optionsController = host;
        CheckFailure(m_optionsController->get_CoreWebView2(&m_optionsWebView), L"");

        wil::com_ptr<ICoreWebView2Settings> settings;
        RETURN_IF_FAILED(m_optionsWebView->get_Settings(&settings));
        RETURN_IF_FAILED(settings->put_AreDevToolsEnabled(FALSE));

        RETURN_IF_FAILED(m_optionsController->add_ZoomFactorChanged(Callback<ICoreWebView2ZoomFactorChangedEventHandler>(
            [](ICoreWebView2Controller* host, IUnknown* args) -> HRESULT
        {
            host->put_ZoomFactor(1.0);
            return S_OK;
        }
        ).Get(), &m_optionsZoomToken));

        // Hide by default
        RETURN_IF_FAILED(m_optionsController->put_IsVisible(FALSE));
        RETURN_IF_FAILED(m_optionsWebView->add_WebMessageReceived(m_uiMessageBroker.Get(), &m_optionsUIMessageBrokerToken));

        // Hide menu when focus is lost
        RETURN_IF_FAILED(m_optionsController->add_LostFocus(Callback<ICoreWebView2FocusChangedEventHandler>(
            [this](ICoreWebView2Controller* sender, IUnknown* args) -> HRESULT
        {
            web::json::value jsonObj = web::json::value::parse(L"{}");
            jsonObj[L"message"] = web::json::value(MG_OPTIONS_LOST_FOCUS);
            jsonObj[L"args"] = web::json::value::parse(L"{}");

            PostJsonToWebView(jsonObj, m_controlsWebView.Get());

            return S_OK;
        }).Get(), &m_lostOptionsFocus));

        RETURN_IF_FAILED(ResizeUIWebViews());

        std::wstring optionsPath = GetFullPathFor(L"wvbrowser_ui\\controls_ui\\options.html");
        RETURN_IF_FAILED(m_optionsWebView->Navigate(optionsPath.c_str()));

        return S_OK;
    }).Get());
}

// Set the message broker for the UI webview. This will capture messages from ui web content.
// Lambda is used to capture the instance while satisfying Microsoft::WRL::Callback<T>()
void BrowserWindow::SetUIMessageBroker()
{
    m_uiMessageBroker = Callback<ICoreWebView2WebMessageReceivedEventHandler>(
        [this](ICoreWebView2* webview, ICoreWebView2WebMessageReceivedEventArgs* eventArgs) -> HRESULT
    {
        wil::unique_cotaskmem_string jsonString;
        CheckFailure(eventArgs->get_WebMessageAsJson(&jsonString), L"");  // Get the message from the UI WebView as JSON formatted string
        web::json::value jsonObj = web::json::value::parse(jsonString.get());

        if (!jsonObj.has_field(L"message"))
        {
            OutputDebugString(L"No message code provided\n");
            return S_OK;
        }

        if (!jsonObj.has_field(L"args"))
        {
            OutputDebugString(L"The message has no args field\n");
            return S_OK;
        }

        int message = jsonObj.at(L"message").as_integer();
        web::json::value args = jsonObj.at(L"args");

        switch (message)
        {
        case MG_CREATE_TAB:
        {
            size_t id = args.at(L"tabId").as_number().to_uint32();
            bool shouldBeActive = args.at(L"active").as_bool();
            std::unique_ptr<Tab> newTab = Tab::CreateNewTab(m_hWnd, m_contentEnv.Get(), id, shouldBeActive);

            std::map<size_t, std::unique_ptr<Tab>>::iterator it = m_tabs.find(id);
            if (it == m_tabs.end())
            {
                m_tabs.insert(std::pair<size_t,std::unique_ptr<Tab>>(id, std::move(newTab)));
            }
            else
            {
                m_tabs.at(id)->m_contentController->Close();
                it->second = std::move(newTab);
            }
        }
        break;
        case MG_NAVIGATE:
        {
            std::wstring uri(args.at(L"uri").as_string());
            std::wstring browserScheme(L"browser://");

            if (uri.substr(0, browserScheme.size()).compare(browserScheme) == 0)
            {
                // No encoded search URI
                std::wstring path = uri.substr(browserScheme.size());
                if (path.compare(L"favorites") == 0 ||
                    path.compare(L"settings") == 0 ||
                    path.compare(L"history") == 0)
                {
                    std::wstring filePath(L"wvbrowser_ui\\content_ui\\");
                    filePath.append(path);
                    filePath.append(L".html");
                    std::wstring fullPath = GetFullPathFor(filePath.c_str());
                    CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(fullPath.c_str()), L"Can't navigate to browser page.");
                }
                else
                {
                    OutputDebugString(L"Requested unknown browser page\n");
                }
            }
            else if (!SUCCEEDED(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(uri.c_str())))
            {
                CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Navigate(args.at(L"encodedSearchURI").as_string().c_str()), L"Can't navigate to requested page.");
            }
        }
        break;
        case MG_GO_FORWARD:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->GoForward(), L"");
        }
        break;
        case MG_GO_BACK:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->GoBack(), L"");
        }
        break;
        case MG_RELOAD:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->Reload(), L"");
        }
        break;
        case MG_CANCEL:
        {
            CheckFailure(m_tabs.at(m_activeTabId)->m_contentWebView->CallDevToolsProtocolMethod(L"Page.stopLoading", L"{}", nullptr), L"");
        }
        break;
        case MG_SWITCH_TAB:
        {
            size_t tabId = args.at(L"tabId").as_number().to_uint32();

            SwitchToTab(tabId);
        }
        break;
        case MG_CLOSE_TAB:
        {
            size_t id = args.at(L"tabId").as_number().to_uint32();
            m_tabs.at(id)->m_contentController->Close();
            m_tabs.erase(id);
        }
        break;
        case MG_CLOSE_WINDOW:
        {
            DestroyWindow(m_hWnd);
        }
        break;
        case MG_SHOW_OPTIONS:
        {
            CheckFailure(m_optionsController->put_IsVisible(TRUE), L"");
            m_optionsController->MoveFocus(COREWEBVIEW2_MOVE_FOCUS_REASON_PROGRAMMATIC);
        }
        break;
        case MG_HIDE_OPTIONS:
        {
            CheckFailure(m_optionsController->put_IsVisible(FALSE), L"Something went wrong when trying to close the options dropdown.");
        }
        break;
        case MG_OPTION_SELECTED:
        {
            m_tabs.at(m_activeTabId)->m_contentController->MoveFocus(COREWEBVIEW2_MOVE_FOCUS_REASON_PROGRAMMATIC);
        }
        break;
        case MG_GET_FAVORITES:
        case MG_GET_SETTINGS:
        case MG_GET_HISTORY:
        {
            // Forward back to requesting tab
            size_t tabId = args.at(L"tabId").as_number().to_uint32();
            jsonObj[L"args"].erase(L"tabId");

            CheckFailure(PostJsonToWebView(jsonObj, m_tabs.at(tabId)->m_contentWebView.Get()), L"Requesting history failed.");
        }
        break;
        default:
        {
            OutputDebugString(L"Unexpected message\n");
        }
        break;
        }

        return S_OK;
    });
}

HRESULT BrowserWindow::SwitchToTab(size_t tabId)
{
    size_t previousActiveTab = m_activeTabId;

    RETURN_IF_FAILED(m_tabs.at(tabId)->ResizeWebView());
    RETURN_IF_FAILED(m_tabs.at(tabId)->m_contentController->put_IsVisible(TRUE));
    m_activeTabId = tabId;

    if (previousActiveTab != INVALID_TAB_ID && previousActiveTab != m_activeTabId) {
        auto previousTabIterator = m_tabs.find(previousActiveTab);
        if (previousTabIterator != m_tabs.end() && previousTabIterator->second &&
            previousTabIterator->second->m_contentController)
        {
            auto hr = m_tabs.at(previousActiveTab)->m_contentController->put_IsVisible(FALSE);
            if (hr == HRESULT_FROM_WIN32(ERROR_INVALID_STATE)) {
                web::json::value jsonObj = web::json::value::parse(L"{}");
                jsonObj[L"message"] = web::json::value(MG_CLOSE_TAB);
                jsonObj[L"args"] = web::json::value::parse(L"{}");
                jsonObj[L"args"][L"tabId"] = web::json::value::number(previousActiveTab);

                PostJsonToWebView(jsonObj, m_controlsWebView.Get());
            }
            RETURN_IF_FAILED(hr);
        }
    }

    return S_OK;
}

HRESULT BrowserWindow::HandleTabURIUpdate(size_t tabId, ICoreWebView2* webview)
{
    wil::unique_cotaskmem_string source;
    RETURN_IF_FAILED(webview->get_Source(&source));

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_UPDATE_URI);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
    jsonObj[L"args"][L"uri"] = web::json::value(source.get());

    std::wstring uri(source.get());
    std::wstring favoritesURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\favorites.html"));
    std::wstring settingsURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\settings.html"));
    std::wstring historyURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\history.html"));

    if (uri.compare(favoritesURI) == 0)
    {
        jsonObj[L"args"][L"uriToShow"] = web::json::value(L"browser://favorites");
    }
    else if (uri.compare(settingsURI) == 0)
    {
        jsonObj[L"args"][L"uriToShow"] = web::json::value(L"browser://settings");
    }
    else if (uri.compare(historyURI) == 0)
    {
        jsonObj[L"args"][L"uriToShow"] = web::json::value(L"browser://history");
    }

    RETURN_IF_FAILED(PostJsonToWebView(jsonObj, m_controlsWebView.Get()));

    return S_OK;
}

HRESULT BrowserWindow::HandleTabHistoryUpdate(size_t tabId, ICoreWebView2* webview)
{
    wil::unique_cotaskmem_string source;
    RETURN_IF_FAILED(webview->get_Source(&source));

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_UPDATE_URI);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
    jsonObj[L"args"][L"uri"] = web::json::value(source.get());

    BOOL canGoForward = FALSE;
    RETURN_IF_FAILED(webview->get_CanGoForward(&canGoForward));
    jsonObj[L"args"][L"canGoForward"] = web::json::value::boolean(canGoForward);

    BOOL canGoBack = FALSE;
    RETURN_IF_FAILED(webview->get_CanGoBack(&canGoBack));
    jsonObj[L"args"][L"canGoBack"] = web::json::value::boolean(canGoBack);

    RETURN_IF_FAILED(PostJsonToWebView(jsonObj, m_controlsWebView.Get()));

    return S_OK;
}

HRESULT BrowserWindow::HandleTabNavStarting(size_t tabId, ICoreWebView2* webview)
{
    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_NAV_STARTING);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);

    return PostJsonToWebView(jsonObj, m_controlsWebView.Get());
}

HRESULT BrowserWindow::HandleTabNavCompleted(size_t tabId, ICoreWebView2* webview, ICoreWebView2NavigationCompletedEventArgs* args)
{
    std::wstring getTitleScript(
        // Look for a title tag
        L"(() => {"
        L"    const titleTag = document.getElementsByTagName('title')[0];"
        L"    if (titleTag) {"
        L"        return titleTag.innerHTML;"
        L"    }"
        // No title tag, look for the file name
        L"    pathname = window.location.pathname;"
        L"    var filename = pathname.split('/').pop();"
        L"    if (filename) {"
        L"        return filename;"
        L"    }"
        // No file name, look for the hostname
        L"    const hostname =  window.location.hostname;"
        L"    if (hostname) {"
        L"        return hostname;"
        L"    }"
        // Fallback: let the UI use a generic title
        L"    return '';"
        L"})();"
    );

    std::wstring getFaviconURI(
        L"(() => {"
        // Let the UI use a fallback favicon
        L"    let faviconURI = '';"
        L"    let links = document.getElementsByTagName('link');"
        // Test each link for a favicon
        L"    Array.from(links).map(element => {"
        L"        let rel = element.rel;"
        // Favicon is declared, try to get the href
        L"        if (rel && (rel == 'shortcut icon' || rel == 'icon')) {"
        L"            if (!element.href) {"
        L"                return;"
        L"            }"
        // href to icon found, check it's full URI
        L"            try {"
        L"                let urlParser = new URL(element.href);"
        L"                faviconURI = urlParser.href;"
        L"            } catch(e) {"
        // Try prepending origin
        L"                let origin = window.location.origin;"
        L"                let faviconLocation = `${origin}/${element.href}`;"
        L"                try {"
        L"                    urlParser = new URL(faviconLocation);"
        L"                    faviconURI = urlParser.href;"
        L"                } catch (e2) {"
        L"                    return;"
        L"                }"
        L"            }"
        L"        }"
        L"    });"
        L"    return faviconURI;"
        L"})();"
    );

    CheckFailure(webview->ExecuteScript(getTitleScript.c_str(), Callback<ICoreWebView2ExecuteScriptCompletedHandler>(
        [this, tabId](HRESULT error, PCWSTR result) -> HRESULT
    {
        RETURN_IF_FAILED(error);

        web::json::value jsonObj = web::json::value::parse(L"{}");
        jsonObj[L"message"] = web::json::value(MG_UPDATE_TAB);
        jsonObj[L"args"] = web::json::value::parse(L"{}");
        jsonObj[L"args"][L"title"] = web::json::value::parse(result);
        jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);

        CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Can't update title.");
        return S_OK;
    }).Get()), L"Can't update title.");

    CheckFailure(webview->ExecuteScript(getFaviconURI.c_str(), Callback<ICoreWebView2ExecuteScriptCompletedHandler>(
        [this, tabId](HRESULT error, PCWSTR result) -> HRESULT
    {
        RETURN_IF_FAILED(error);

        web::json::value jsonObj = web::json::value::parse(L"{}");
        jsonObj[L"message"] = web::json::value(MG_UPDATE_FAVICON);
        jsonObj[L"args"] = web::json::value::parse(L"{}");
        jsonObj[L"args"][L"uri"] = web::json::value::parse(result);
        jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);

        CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Can't update favicon.");
        return S_OK;
    }).Get()), L"Can't update favicon");

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_NAV_COMPLETED);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);

    BOOL navigationSucceeded = FALSE;
    if (SUCCEEDED(args->get_IsSuccess(&navigationSucceeded)))
    {
        jsonObj[L"args"][L"isError"] = web::json::value::boolean(!navigationSucceeded);
    }

    return PostJsonToWebView(jsonObj, m_controlsWebView.Get());
}

HRESULT BrowserWindow::HandleTabSecurityUpdate(size_t tabId, ICoreWebView2* webview, ICoreWebView2DevToolsProtocolEventReceivedEventArgs* args)
{
    wil::unique_cotaskmem_string jsonArgs;
    RETURN_IF_FAILED(args->get_ParameterObjectAsJson(&jsonArgs));
    web::json::value securityEvent = web::json::value::parse(jsonArgs.get());

    web::json::value jsonObj = web::json::value::parse(L"{}");
    jsonObj[L"message"] = web::json::value(MG_SECURITY_UPDATE);
    jsonObj[L"args"] = web::json::value::parse(L"{}");
    jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
    jsonObj[L"args"][L"state"] = securityEvent.at(L"securityState");

    return PostJsonToWebView(jsonObj, m_controlsWebView.Get());
}

void BrowserWindow::HandleTabCreated(size_t tabId, bool shouldBeActive)
{
    if (shouldBeActive)
    {
        CheckFailure(SwitchToTab(tabId), L"");
    }
}

HRESULT BrowserWindow::HandleTabMessageReceived(size_t tabId, ICoreWebView2* webview, ICoreWebView2WebMessageReceivedEventArgs* eventArgs)
{
    wil::unique_cotaskmem_string jsonString;
    RETURN_IF_FAILED(eventArgs->get_WebMessageAsJson(&jsonString));
    web::json::value jsonObj = web::json::value::parse(jsonString.get());

    wil::unique_cotaskmem_string uri;
    RETURN_IF_FAILED(webview->get_Source(&uri));

    int message = jsonObj.at(L"message").as_integer();
    web::json::value args = jsonObj.at(L"args");

    wil::unique_cotaskmem_string source;
    RETURN_IF_FAILED(webview->get_Source(&source));

    switch (message)
    {
    case MG_GET_FAVORITES:
    case MG_REMOVE_FAVORITE:
    {
        std::wstring fileURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\favorites.html"));
        // Only the favorites UI can request favorites
        if (fileURI.compare(source.get()) == 0)
        {
            jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
            CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Couldn't perform favorites operation.");
        }
    }
    break;
    case MG_GET_SETTINGS:
    {
        std::wstring fileURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\settings.html"));
        // Only the settings UI can request settings
        if (fileURI.compare(source.get()) == 0)
        {
            jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
            CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Couldn't retrieve settings.");
        }
    }
    break;
    case MG_CLEAR_CACHE:
    {
        std::wstring fileURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\settings.html"));
        // Only the settings UI can request cache clearing
        if (fileURI.compare(uri.get()) == 0)
        {
            jsonObj[L"args"][L"content"] = web::json::value::boolean(false);
            jsonObj[L"args"][L"controls"] = web::json::value::boolean(false);

            if (SUCCEEDED(ClearContentCache()))
            {
                jsonObj[L"args"][L"content"] = web::json::value::boolean(true);
            }

            if (SUCCEEDED(ClearControlsCache()))
            {
                jsonObj[L"args"][L"controls"] = web::json::value::boolean(true);
            }

            CheckFailure(PostJsonToWebView(jsonObj, m_tabs.at(tabId)->m_contentWebView.Get()), L"");
        }
    }
    break;
    case MG_CLEAR_COOKIES:
    {
        std::wstring fileURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\settings.html"));
        // Only the settings UI can request cookies clearing
        if (fileURI.compare(uri.get()) == 0)
        {
            jsonObj[L"args"][L"content"] = web::json::value::boolean(false);
            jsonObj[L"args"][L"controls"] = web::json::value::boolean(false);

            if (SUCCEEDED(ClearContentCookies()))
            {
                jsonObj[L"args"][L"content"] = web::json::value::boolean(true);
            }


            if (SUCCEEDED(ClearControlsCookies()))
            {
                jsonObj[L"args"][L"controls"] = web::json::value::boolean(true);
            }

            CheckFailure(PostJsonToWebView(jsonObj, m_tabs.at(tabId)->m_contentWebView.Get()), L"");
        }
    }
    break;
    case MG_GET_HISTORY:
    case MG_REMOVE_HISTORY_ITEM:
    case MG_CLEAR_HISTORY:
    {
        std::wstring fileURI = GetFilePathAsURI(GetFullPathFor(L"wvbrowser_ui\\content_ui\\history.html"));
        // Only the history UI can request history
        if (fileURI.compare(uri.get()) == 0)
        {
            jsonObj[L"args"][L"tabId"] = web::json::value::number(tabId);
            CheckFailure(PostJsonToWebView(jsonObj, m_controlsWebView.Get()), L"Couldn't perform history operation");
        }
    }
    break;
    default:
    {
        OutputDebugString(L"Unexpected message\n");
    }
    break;
    }

    return S_OK;
}

HRESULT BrowserWindow::ClearContentCache()
{
    return m_tabs.at(m_activeTabId)->m_contentWebView->CallDevToolsProtocolMethod(L"Network.clearBrowserCache", L"{}", nullptr);
}

HRESULT BrowserWindow::ClearControlsCache()
{
    return m_controlsWebView->CallDevToolsProtocolMethod(L"Network.clearBrowserCache", L"{}", nullptr);
}

HRESULT BrowserWindow::ClearContentCookies()
{
    return m_tabs.at(m_activeTabId)->m_contentWebView->CallDevToolsProtocolMethod(L"Network.clearBrowserCookies", L"{}", nullptr);
}

HRESULT BrowserWindow::ClearControlsCookies()
{
    return m_controlsWebView->CallDevToolsProtocolMethod(L"Network.clearBrowserCookies", L"{}", nullptr);
}

HRESULT BrowserWindow::ResizeUIWebViews()
{
    if (m_controlsWebView != nullptr)
    {
        RECT bounds;
        GetClientRect(m_hWnd, &bounds);
        bounds.bottom = bounds.top + GetDPIAwareBound(c_uiBarHeight);
        bounds.bottom += 1;

        RETURN_IF_FAILED(m_controlsController->put_Bounds(bounds));
    }

    if (m_optionsWebView != nullptr)
    {
        RECT bounds;
        GetClientRect(m_hWnd, &bounds);
        bounds.top = GetDPIAwareBound(c_uiBarHeight);
        bounds.bottom = bounds.top + GetDPIAwareBound(c_optionsDropdownHeight);
        bounds.left = bounds.right - GetDPIAwareBound(c_optionsDropdownWidth);

        RETURN_IF_FAILED(m_optionsController->put_Bounds(bounds));
    }

    // Workaround for black controls WebView issue in Windows 7
    HWND wvWindow = GetWindow(m_hWnd, GW_CHILD);
    while (wvWindow != nullptr)
    {
        UpdateWindow(wvWindow);
        wvWindow = GetWindow(wvWindow, GW_HWNDNEXT);
    }

    return S_OK;
}

void BrowserWindow::UpdateMinWindowSize()
{
    RECT clientRect;
    RECT windowRect;

    GetClientRect(m_hWnd, &clientRect);
    GetWindowRect(m_hWnd, &windowRect);

    int bordersWidth = (windowRect.right - windowRect.left) - clientRect.right;
    int bordersHeight = (windowRect.bottom - windowRect.top) - clientRect.bottom;

    m_minWindowWidth = GetDPIAwareBound(MIN_WINDOW_WIDTH) + bordersWidth;
    m_minWindowHeight = GetDPIAwareBound(MIN_WINDOW_HEIGHT) + bordersHeight;
}

void BrowserWindow::CheckFailure(HRESULT hr, LPCWSTR errorMessage)
{
    if (FAILED(hr))
    {
        std::wstring message;
        if (!errorMessage || !errorMessage[0])
        {
            message = std::wstring(L"Something went wrong.");
        }
        else
        {
            message = std::wstring(errorMessage);
        }

        MessageBoxW(nullptr, message.c_str(), nullptr, MB_OK);
    }
}

int BrowserWindow::GetDPIAwareBound(int bound)
{
    // Remove the GetDpiForWindow call when using Windows 7 or any version
    // below 1607 (Windows 10). You will also have to make sure the build
    // directory is clean before building again.
    return (bound * GetDpiForWindow(m_hWnd) / DEFAULT_DPI);
}

std::wstring BrowserWindow::GetAppDataDirectory()
{
    TCHAR path[MAX_PATH];
    std::wstring dataDirectory;
    HRESULT hr = SHGetFolderPath(nullptr, CSIDL_APPDATA, NULL, 0, path);
    if (SUCCEEDED(hr))
    {
        dataDirectory = std::wstring(path);
        dataDirectory.append(L"\\Microsoft\\");
    }
    else
    {
        dataDirectory = std::wstring(L".\\");
    }

    dataDirectory.append(s_title);
    return dataDirectory;
}

std::wstring BrowserWindow::GetFullPathFor(LPCWSTR relativePath)
{
    WCHAR path[MAX_PATH];
    GetModuleFileNameW(m_hInst, path, MAX_PATH);
    std::wstring pathName(path);

    std::size_t index = pathName.find_last_of(L"\\") + 1;
    pathName.replace(index, pathName.length(), relativePath);

    return pathName;
}

std::wstring BrowserWindow::GetFilePathAsURI(std::wstring fullPath)
{
    std::wstring fileURI;
    ComPtr<IUri> uri;
    DWORD uriFlags = Uri_CREATE_ALLOW_IMPLICIT_FILE_SCHEME;
    HRESULT hr = CreateUri(fullPath.c_str(), uriFlags, 0, &uri);

    if (SUCCEEDED(hr))
    {
        wil::unique_bstr absoluteUri;
        uri->GetAbsoluteUri(&absoluteUri);
        fileURI = std::wstring(absoluteUri.get());
    }

    return fileURI;
}

HRESULT BrowserWindow::PostJsonToWebView(web::json::value jsonObj, ICoreWebView2* webview)
{
    utility::stringstream_t stream;
    jsonObj.serialize(stream);

    return webview->PostWebMessageAsJson(stream.str().c_str());
}



================================================
FILE: BrowserWindow.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#pragma once

#include "framework.h"
#include "Tab.h"

class BrowserWindow
{
public:
    static const int c_uiBarHeight = 70;
    static const int c_optionsDropdownHeight = 108;
    static const int c_optionsDropdownWidth = 200;

    static ATOM RegisterClass(_In_ HINSTANCE hInstance);
    static LRESULT CALLBACK WndProcStatic(HWND hWnd, UINT message, WPARAM wParam, LPARAM lParam);
    LRESULT CALLBACK WndProc(HWND hWnd, UINT message, WPARAM wParam, LPARAM lParam);

    static BOOL LaunchWindow(_In_ HINSTANCE hInstance, _In_ int nCmdShow);
    static std::wstring GetAppDataDirectory();
    std::wstring GetFullPathFor(LPCWSTR relativePath);
    HRESULT HandleTabURIUpdate(size_t tabId, ICoreWebView2* webview);
    HRESULT HandleTabHistoryUpdate(size_t tabId, ICoreWebView2* webview);
    HRESULT HandleTabNavStarting(size_t tabId, ICoreWebView2* webview);
    HRESULT HandleTabNavCompleted(size_t tabId, ICoreWebView2* webview, ICoreWebView2NavigationCompletedEventArgs* args);
    HRESULT HandleTabSecurityUpdate(size_t tabId, ICoreWebView2* webview, ICoreWebView2DevToolsProtocolEventReceivedEventArgs* args);
    void HandleTabCreated(size_t tabId, bool shouldBeActive);
    HRESULT HandleTabMessageReceived(size_t tabId, ICoreWebView2* webview, ICoreWebView2WebMessageReceivedEventArgs* eventArgs);
    int GetDPIAwareBound(int bound);
    static void CheckFailure(HRESULT hr, LPCWSTR errorMessage);
protected:
    HINSTANCE m_hInst = nullptr;  // Current app instance
    HWND m_hWnd = nullptr;

    static WCHAR s_windowClass[MAX_LOADSTRING];  // The window class name
    static WCHAR s_title[MAX_LOADSTRING];  // The title bar text

    int m_minWindowWidth = 0;
    int m_minWindowHeight = 0;

    Microsoft::WRL::ComPtr<ICoreWebView2Environment> m_uiEnv;
    Microsoft::WRL::ComPtr<ICoreWebView2Environment> m_contentEnv;
    Microsoft::WRL::ComPtr<ICoreWebView2Controller> m_controlsController;
    Microsoft::WRL::ComPtr<ICoreWebView2Controller> m_optionsController;
    Microsoft::WRL::ComPtr<ICoreWebView2> m_controlsWebView;
    Microsoft::WRL::ComPtr<ICoreWebView2> m_optionsWebView;
    std::map<size_t,std::unique_ptr<Tab>> m_tabs;
    size_t m_activeTabId = 0;

    EventRegistrationToken m_controlsUIMessageBrokerToken = {};  // Token for the UI message handler in controls WebView
    EventRegistrationToken m_controlsZoomToken = {};
    EventRegistrationToken m_optionsUIMessageBrokerToken = {};  // Token for the UI message handler in options WebView
    EventRegistrationToken m_optionsZoomToken = {};
    EventRegistrationToken m_lostOptionsFocus = {};  // Token for the lost focus handler in options WebView
    Microsoft::WRL::ComPtr<ICoreWebView2WebMessageReceivedEventHandler> m_uiMessageBroker;

    BOOL InitInstance(HINSTANCE hInstance, int nCmdShow);
    HRESULT InitUIWebViews();
    HRESULT CreateBrowserControlsWebView();
    HRESULT CreateBrowserOptionsWebView();
    HRESULT ClearContentCache();
    HRESULT ClearControlsCache();
    HRESULT ClearContentCookies();
    HRESULT ClearControlsCookies();

    void SetUIMessageBroker();
    HRESULT ResizeUIWebViews();
    void UpdateMinWindowSize();
    HRESULT PostJsonToWebView(web::json::value jsonObj, ICoreWebView2* webview);
    HRESULT SwitchToTab(size_t tabId);
    std::wstring GetFilePathAsURI(std::wstring fullPath);
};



================================================
FILE: framework.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#pragma once

#include "targetver.h"
#define WIN32_LEAN_AND_MEAN  // Exclude rarely-used stuff from Windows headers
// Windows Header Files
#include <atlstr.h>
#include <strsafe.h>
#include <wil/result.h>
#include <wil/com.h>
#include <windows.h>
#include <wrl.h>
// C RunTime Header Files
#include <cpprest/json.h>
#include <malloc.h>
#include <memory.h>
#include <memory>
#include <stdlib.h>
#include <tchar.h>
#include <map>

// App specific includes
#include "resource.h"
#include "webview2.h"

#define DEFAULT_DPI 96
#define MIN_WINDOW_WIDTH 510
#define MIN_WINDOW_HEIGHT 75
#define MAX_LOADSTRING 256

#define INVALID_TAB_ID 0
#define MG_NAVIGATE 1
#define MG_UPDATE_URI 2
#define MG_GO_FORWARD 3
#define MG_GO_BACK 4
#define MG_NAV_STARTING 5
#define MG_NAV_COMPLETED 6
#define MG_RELOAD 7
#define MG_CANCEL 8
#define MG_CREATE_TAB 10
#define MG_UPDATE_TAB 11
#define MG_SWITCH_TAB 12
#define MG_CLOSE_TAB 13
#define MG_CLOSE_WINDOW 14
#define MG_SHOW_OPTIONS 15
#define MG_HIDE_OPTIONS 16
#define MG_OPTIONS_LOST_FOCUS 17
#define MG_OPTION_SELECTED 18
#define MG_SECURITY_UPDATE 19
#define MG_UPDATE_FAVICON 20
#define MG_GET_SETTINGS 21
#define MG_GET_FAVORITES 22
#define MG_REMOVE_FAVORITE 23
#define MG_CLEAR_CACHE 24
#define MG_CLEAR_COOKIES 25
#define MG_GET_HISTORY 26
#define MG_REMOVE_HISTORY_ITEM 27
#define MG_CLEAR_HISTORY 28



================================================
FILE: LICENSE
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * The name of Google Inc, Microsoft Corporation, or the names of its
// contributors may not be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


================================================
FILE: packages.config
================================================
﻿<?xml version="1.0" encoding="utf-8"?>
<packages>
  <package id="cpprestsdk.v141" version="2.10.12.1" targetFramework="native" />
  <package id="Microsoft.Web.WebView2" version="1.0.961.33" targetFramework="native" />
  <package id="Microsoft.Windows.ImplementationLibrary" version="1.0.191107.2" targetFramework="native" />
</packages>


================================================
FILE: Resource.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

//{{NO_DEPENDENCIES}}
// Microsoft Visual C++ generated include file.
// Used by WebViewBrowserApp.rc
//
#define IDC_MYICON                      2
#define IDD_WEBVIEWBROWSERAPP_DIALOG    102
#define IDS_APP_TITLE                   103
#define IDM_ABOUT                       104
#define IDI_WEBVIEWBROWSERAPP           107
#define IDI_SMALL                       108
#define IDC_WEBVIEWBROWSERAPP           109
#define IDR_MAINFRAME                   128
#define IDC_STATIC                      -1

// Next default values for new objects
//
#ifdef APSTUDIO_INVOKED
#ifndef APSTUDIO_READONLY_SYMBOLS
#define _APS_NO_MFC                     1
#define _APS_NEXT_RESOURCE_VALUE        131
#define _APS_NEXT_COMMAND_VALUE         32771
#define _APS_NEXT_CONTROL_VALUE         1000
#define _APS_NEXT_SYMED_VALUE           110
#endif
#endif



================================================
FILE: Tab.cpp
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#include "BrowserWindow.h"
#include "Tab.h"

using namespace Microsoft::WRL;

std::unique_ptr<Tab> Tab::CreateNewTab(HWND hWnd, ICoreWebView2Environment* env, size_t id, bool shouldBeActive)
{
    std::unique_ptr<Tab> tab = std::make_unique<Tab>();

    tab->m_parentHWnd = hWnd;
    tab->m_tabId = id;
    tab->SetMessageBroker();
    tab->Init(env, shouldBeActive);

    return tab;
}

HRESULT Tab::Init(ICoreWebView2Environment* env, bool shouldBeActive)
{
    return env->CreateCoreWebView2Controller(m_parentHWnd, Callback<ICoreWebView2CreateCoreWebView2ControllerCompletedHandler>(
        [this, shouldBeActive](HRESULT result, ICoreWebView2Controller* host) -> HRESULT {
        if (!SUCCEEDED(result))
        {
            OutputDebugString(L"Tab WebView creation failed\n");
            return result;
        }
        m_contentController = host;
        BrowserWindow::CheckFailure(m_contentController->get_CoreWebView2(&m_contentWebView), L"");
        BrowserWindow* browserWindow = reinterpret_cast<BrowserWindow*>(GetWindowLongPtr(m_parentHWnd, GWLP_USERDATA));
        RETURN_IF_FAILED(m_contentWebView->add_WebMessageReceived(m_messageBroker.Get(), &m_messageBrokerToken));

        // Register event handler for history change
        RETURN_IF_FAILED(m_contentWebView->add_HistoryChanged(Callback<ICoreWebView2HistoryChangedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, IUnknown* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabHistoryUpdate(m_tabId, webview), L"Can't update go back/forward buttons.");

            return S_OK;
        }).Get(), &m_historyUpdateForwarderToken));

        // Register event handler for source change
        RETURN_IF_FAILED(m_contentWebView->add_SourceChanged(Callback<ICoreWebView2SourceChangedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2SourceChangedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabURIUpdate(m_tabId, webview), L"Can't update address bar");

            return S_OK;
        }).Get(), &m_uriUpdateForwarderToken));

        RETURN_IF_FAILED(m_contentWebView->add_NavigationStarting(Callback<ICoreWebView2NavigationStartingEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2NavigationStartingEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabNavStarting(m_tabId, webview), L"Can't update reload button");

            return S_OK;
        }).Get(), &m_navStartingToken));

        RETURN_IF_FAILED(m_contentWebView->add_NavigationCompleted(Callback<ICoreWebView2NavigationCompletedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2NavigationCompletedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabNavCompleted(m_tabId, webview, args), L"Can't udpate reload button");
            return S_OK;
        }).Get(), &m_navCompletedToken));

        // Enable listening for security events to update secure icon
        RETURN_IF_FAILED(m_contentWebView->CallDevToolsProtocolMethod(L"Security.enable", L"{}", nullptr));

        BrowserWindow::CheckFailure(m_contentWebView->GetDevToolsProtocolEventReceiver(L"Security.securityStateChanged", &m_securityStateChangedReceiver), L"");

        // Forward security status updates to browser
        RETURN_IF_FAILED(m_securityStateChangedReceiver->add_DevToolsProtocolEventReceived(Callback<ICoreWebView2DevToolsProtocolEventReceivedEventHandler>(
            [this, browserWindow](ICoreWebView2* webview, ICoreWebView2DevToolsProtocolEventReceivedEventArgs* args) -> HRESULT
        {
            BrowserWindow::CheckFailure(browserWindow->HandleTabSecurityUpdate(m_tabId, webview, args), L"Can't udpate security icon");
            return S_OK;
        }).Get(), &m_securityUpdateToken));

        RETURN_IF_FAILED(m_contentWebView->Navigate(L"https://www.bing.com"));
        browserWindow->HandleTabCreated(m_tabId, shouldBeActive);

        return S_OK;
    }).Get());
}

void Tab::SetMessageBroker()
{
    m_messageBroker = Callback<ICoreWebView2WebMessageReceivedEventHandler>(
        [this](ICoreWebView2* webview, ICoreWebView2WebMessageReceivedEventArgs* eventArgs) -> HRESULT
    {
        BrowserWindow* browserWindow = reinterpret_cast<BrowserWindow*>(GetWindowLongPtr(m_parentHWnd, GWLP_USERDATA));
        BrowserWindow::CheckFailure(browserWindow->HandleTabMessageReceived(m_tabId, webview, eventArgs), L"");

        return S_OK;
    });
}

HRESULT Tab::ResizeWebView()
{
    RECT bounds;
    GetClientRect(m_parentHWnd, &bounds);

    BrowserWindow* browserWindow = reinterpret_cast<BrowserWindow*>(GetWindowLongPtr(m_parentHWnd, GWLP_USERDATA));
    bounds.top += browserWindow->GetDPIAwareBound(BrowserWindow::c_uiBarHeight);

    return m_contentController->put_Bounds(bounds);
}



================================================
FILE: Tab.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#pragma once

#include "framework.h"

class Tab
{
public:
    Microsoft::WRL::ComPtr<ICoreWebView2Controller> m_contentController;
    Microsoft::WRL::ComPtr<ICoreWebView2> m_contentWebView;
    Microsoft::WRL::ComPtr<ICoreWebView2DevToolsProtocolEventReceiver> m_securityStateChangedReceiver;

    static std::unique_ptr<Tab> CreateNewTab(HWND hWnd, ICoreWebView2Environment* env, size_t id, bool shouldBeActive);
    HRESULT ResizeWebView();
protected:
    HWND m_parentHWnd = nullptr;
    size_t m_tabId = INVALID_TAB_ID;
    EventRegistrationToken m_historyUpdateForwarderToken = {};
    EventRegistrationToken m_uriUpdateForwarderToken = {};
    EventRegistrationToken m_navStartingToken = {};
    EventRegistrationToken m_navCompletedToken = {};
    EventRegistrationToken m_securityUpdateToken = {};
    EventRegistrationToken m_messageBrokerToken = {};  // Message broker for browser pages loaded in a tab
    Microsoft::WRL::ComPtr<ICoreWebView2WebMessageReceivedEventHandler> m_messageBroker;

    HRESULT Init(ICoreWebView2Environment* env, bool shouldBeActive);
    void SetMessageBroker();
};



================================================
FILE: targetver.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#pragma once

// Including SDKDDKVer.h defines the highest available Windows platform.
// If you wish to build your application for a previous Windows platform, include WinSDKVer.h and
// set the _WIN32_WINNT macro to the platform you wish to support before including SDKDDKVer.h.
#include <SDKDDKVer.h>



================================================
FILE: WebViewBrowserApp.cpp
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

// WebViewBrowserApp.cpp : Defines the entry point for the application.
//

#include "BrowserWindow.h"
#include "WebViewBrowserApp.h"

using namespace Microsoft::WRL;

void tryLaunchWindow(HINSTANCE hInstance, int nCmdShow);

int APIENTRY wWinMain(_In_ HINSTANCE hInstance,
                      _In_opt_ HINSTANCE hPrevInstance,
                      _In_ LPWSTR    lpCmdLine,
                      _In_ int       nCmdShow)
{
    UNREFERENCED_PARAMETER(hPrevInstance);
    UNREFERENCED_PARAMETER(lpCmdLine);

    // Call SetProcessDPIAware() instead when using Windows 7 or any version
    // below 1703 (Windows 10).
    SetProcessDpiAwarenessContext(DPI_AWARENESS_CONTEXT_PER_MONITOR_AWARE_V2);

    BrowserWindow::RegisterClass(hInstance);

    tryLaunchWindow(hInstance, nCmdShow);

    HACCEL hAccelTable = LoadAccelerators(hInstance, MAKEINTRESOURCE(IDC_WEBVIEWBROWSERAPP));

    MSG msg;

    // Main message loop:
    while (GetMessage(&msg, nullptr, 0, 0))
    {
        if (!TranslateAccelerator(msg.hwnd, hAccelTable, &msg))
        {
            TranslateMessage(&msg);
            DispatchMessage(&msg);
        }
    }

    return (int) msg.wParam;
}

void tryLaunchWindow(HINSTANCE hInstance, int nCmdShow)
{
    BOOL launched = BrowserWindow::LaunchWindow(hInstance, nCmdShow);
    if (!launched)
    {
        int msgboxID = MessageBox(NULL, L"Could not launch the browser", L"Error", MB_RETRYCANCEL);

        switch (msgboxID)
        {
        case IDRETRY:
            tryLaunchWindow(hInstance, nCmdShow);
            break;
        case IDCANCEL:
        default:
            PostQuitMessage(0);
        }
    }
}



================================================
FILE: WebViewBrowserApp.h
================================================
// Copyright (C) Microsoft Corporation. All rights reserved.
// Use of this source code is governed by a BSD-style license that can be
// found in the LICENSE file.

#pragma once

#include "framework.h"



================================================
FILE: WebViewBrowserApp.rc
================================================
[Non-text file]


================================================
FILE: WebViewBrowserApp.sln
================================================
﻿
Microsoft Visual Studio Solution File, Format Version 12.00
# Visual Studio Version 16
VisualStudioVersion = 16.0.29001.49
MinimumVisualStudioVersion = 10.0.40219.1
Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "WebView2Browser", "WebViewBrowserApp.vcxproj", "{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}"
EndProject
Global
	GlobalSection(SolutionConfigurationPlatforms) = preSolution
		Debug|x64 = Debug|x64
		Debug|x86 = Debug|x86
		Release|x64 = Release|x64
		Release|x86 = Release|x86
	EndGlobalSection
	GlobalSection(ProjectConfigurationPlatforms) = postSolution
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Debug|x64.ActiveCfg = Debug|x64
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Debug|x64.Build.0 = Debug|x64
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Debug|x86.ActiveCfg = Debug|Win32
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Debug|x86.Build.0 = Debug|Win32
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Release|x64.ActiveCfg = Release|x64
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Release|x64.Build.0 = Release|x64
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Release|x86.ActiveCfg = Release|Win32
		{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}.Release|x86.Build.0 = Release|Win32
	EndGlobalSection
	GlobalSection(SolutionProperties) = preSolution
		HideSolutionNode = FALSE
	EndGlobalSection
	GlobalSection(ExtensibilityGlobals) = postSolution
		SolutionGuid = {0C9921DB-4634-415A-9AB1-087EA9B2EB24}
	EndGlobalSection
EndGlobal



================================================
FILE: WebViewBrowserApp.vcxproj
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
    <ProjectGuid>{D65018E5-6B31-4DC7-AFAC-7999384BA4BD}</ProjectGuid>
    <Keyword>Win32Proj</Keyword>
    <RootNamespace>WebViewBrowserApp</RootNamespace>
    <WindowsTargetPlatformVersion>10.0</WindowsTargetPlatformVersion>
    <ProjectName>WebView2Browser</ProjectName>
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
    <OutDir>$(Configuration)_x86</OutDir>
    <IntDir>$(Configuration)\</IntDir>
    <TargetName>$(ProjectName)</TargetName>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <LinkIncremental>true</LinkIncremental>
    <OutDir>$(Configuration)_$(Platform)</OutDir>
    <IncludePath>$(IncludePath)</IncludePath>
    <TargetName>$(ProjectName)</TargetName>
    <IntDir>$(Configuration)\</IntDir>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <LinkIncremental>false</LinkIncremental>
    <OutDir>$(Configuration)_x86</OutDir>
    <IntDir>$(Configuration)\</IntDir>
    <TargetName>$(ProjectName)</TargetName>
  </PropertyGroup>
  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <LinkIncremental>false</LinkIncremental>
    <OutDir>$(Configuration)_$(Platform)</OutDir>
    <TargetName>$(ProjectName)</TargetName>
    <IntDir>$(Configuration)\</IntDir>
  </PropertyGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
    <ClCompile>
      <PrecompiledHeader>
      </PrecompiledHeader>
      <WarningLevel>Level3</WarningLevel>
      <Optimization>Disabled</Optimization>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>WIN32;_DEBUG;_WINDOWS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Windows</SubSystem>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
    <PostBuildEvent>
      <Command>xcopy "$(ProjectDir)wvbrowser_ui" "$(OutDir)wvbrowser_ui" /S /I /Y</Command>
    </PostBuildEvent>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
    <ClCompile>
      <PrecompiledHeader>
      </PrecompiledHeader>
      <WarningLevel>Level3</WarningLevel>
      <Optimization>Disabled</Optimization>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>_DEBUG;_WINDOWS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Windows</SubSystem>
      <GenerateDebugInformation>true</GenerateDebugInformation>
      <AdditionalDependencies>
      </AdditionalDependencies>
    </Link>
    <PostBuildEvent>
      <Command>xcopy "$(ProjectDir)wvbrowser_ui" "$(OutDir)wvbrowser_ui" /S /I /Y</Command>
    </PostBuildEvent>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
    <ClCompile>
      <PrecompiledHeader>
      </PrecompiledHeader>
      <WarningLevel>Level3</WarningLevel>
      <Optimization>MaxSpeed</Optimization>
      <FunctionLevelLinking>true</FunctionLevelLinking>
      <IntrinsicFunctions>true</IntrinsicFunctions>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>WIN32;NDEBUG;_WINDOWS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Windows</SubSystem>
      <EnableCOMDATFolding>true</EnableCOMDATFolding>
      <OptimizeReferences>true</OptimizeReferences>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
    <PostBuildEvent>
      <Command>xcopy "$(ProjectDir)wvbrowser_ui" "$(OutDir)wvbrowser_ui" /S /I /Y</Command>
    </PostBuildEvent>
  </ItemDefinitionGroup>
  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
    <ClCompile>
      <PrecompiledHeader>
      </PrecompiledHeader>
      <WarningLevel>Level3</WarningLevel>
      <Optimization>MaxSpeed</Optimization>
      <FunctionLevelLinking>true</FunctionLevelLinking>
      <IntrinsicFunctions>true</IntrinsicFunctions>
      <SDLCheck>true</SDLCheck>
      <PreprocessorDefinitions>NDEBUG;_WINDOWS;%(PreprocessorDefinitions)</PreprocessorDefinitions>
      <ConformanceMode>true</ConformanceMode>
    </ClCompile>
    <Link>
      <SubSystem>Windows</SubSystem>
      <EnableCOMDATFolding>true</EnableCOMDATFolding>
      <OptimizeReferences>true</OptimizeReferences>
      <GenerateDebugInformation>true</GenerateDebugInformation>
    </Link>
    <PostBuildEvent>
      <Command>xcopy "$(ProjectDir)wvbrowser_ui" "$(OutDir)wvbrowser_ui" /S /I /Y</Command>
    </PostBuildEvent>
  </ItemDefinitionGroup>
  <ItemGroup>
    <ClInclude Include="BrowserWindow.h" />
    <ClInclude Include="framework.h" />
    <ClInclude Include="Resource.h" />
    <ClInclude Include="Tab.h" />
    <ClInclude Include="targetver.h" />
    <ClInclude Include="WebViewBrowserApp.h" />
  </ItemGroup>
  <ItemGroup>
    <ClCompile Include="BrowserWindow.cpp" />
    <ClCompile Include="Tab.cpp" />
    <ClCompile Include="WebViewBrowserApp.cpp" />
  </ItemGroup>
  <ItemGroup>
    <ResourceCompile Include="WebViewBrowserApp.rc" />
  </ItemGroup>
  <ItemGroup>
    <Image Include="small.ico" />
    <Image Include="WebViewBrowserApp.ico" />
  </ItemGroup>
  <ItemGroup>
    <None Include="packages.config" />
    <None Include="ui_bar.html" />
  </ItemGroup>
  <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets" />
  <ImportGroup Label="ExtensionTargets">
    <Import Project="packages\cpprestsdk.v141.2.10.12.1\build\native\cpprestsdk.v141.targets" Condition="Exists('packages\cpprestsdk.v141.2.10.12.1\build\native\cpprestsdk.v141.targets')" />
    <Import Project="packages\Microsoft.Windows.ImplementationLibrary.1.0.191107.2\build\native\Microsoft.Windows.ImplementationLibrary.targets" Condition="Exists('packages\Microsoft.Windows.ImplementationLibrary.1.0.191107.2\build\native\Microsoft.Windows.ImplementationLibrary.targets')" />
    <Import Project="packages\Microsoft.Web.WebView2.1.0.961.33\build\native\Microsoft.Web.WebView2.targets" Condition="Exists('packages\Microsoft.Web.WebView2.1.0.961.33\build\native\Microsoft.Web.WebView2.targets')" />
  </ImportGroup>
  <Target Name="EnsureNuGetPackageBuildImports" BeforeTargets="PrepareForBuild">
    <PropertyGroup>
      <ErrorText>This project references NuGet package(s) that are missing on this computer. Use NuGet Package Restore to download them.  For more information, see http://go.microsoft.com/fwlink/?LinkID=322105. The missing file is {0}.</ErrorText>
    </PropertyGroup>
    <Error Condition="!Exists('packages\cpprestsdk.v141.2.10.12.1\build\native\cpprestsdk.v141.targets')" Text="$([System.String]::Format('$(ErrorText)', 'packages\cpprestsdk.v141.2.10.12.1\build\native\cpprestsdk.v141.targets'))" />
    <Error Condition="!Exists('packages\Microsoft.Windows.ImplementationLibrary.1.0.191107.2\build\native\Microsoft.Windows.ImplementationLibrary.targets')" Text="$([System.String]::Format('$(ErrorText)', 'packages\Microsoft.Windows.ImplementationLibrary.1.0.191107.2\build\native\Microsoft.Windows.ImplementationLibrary.targets'))" />
    <Error Condition="!Exists('packages\Microsoft.Web.WebView2.1.0.961.33\build\native\Microsoft.Web.WebView2.targets')" Text="$([System.String]::Format('$(ErrorText)', 'packages\Microsoft.Web.WebView2.1.0.961.33\build\native\Microsoft.Web.WebView2.targets'))" />
  </Target>
</Project>


================================================
FILE: WebViewBrowserApp.vcxproj.filters
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
      <Extensions>h;hh;hpp;hxx;hm;inl;inc;ipp;xsd</Extensions>
    </Filter>
    <Filter Include="Resource Files">
      <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
    </Filter>
  </ItemGroup>
  <ItemGroup>
    <ClInclude Include="framework.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="targetver.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="Resource.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="WebViewBrowserApp.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="BrowserWindow.h">
      <Filter>Header Files</Filter>
    </ClInclude>
    <ClInclude Include="Tab.h">
      <Filter>Header Files</Filter>
    </ClInclude>
  </ItemGroup>
  <ItemGroup>
    <ClCompile Include="WebViewBrowserApp.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="BrowserWindow.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
    <ClCompile Include="Tab.cpp">
      <Filter>Source Files</Filter>
    </ClCompile>
  </ItemGroup>
  <ItemGroup>
    <ResourceCompile Include="WebViewBrowserApp.rc">
      <Filter>Resource Files</Filter>
    </ResourceCompile>
  </ItemGroup>
  <ItemGroup>
    <Image Include="small.ico">
      <Filter>Resource Files</Filter>
    </Image>
    <Image Include="WebViewBrowserApp.ico">
      <Filter>Resource Files</Filter>
    </Image>
  </ItemGroup>
  <ItemGroup>
    <None Include="ui_bar.html" />
    <None Include="packages.config" />
  </ItemGroup>
</Project>


================================================
FILE: .clang-format
================================================
# Defines the coding style to apply. See:
# <http://clang.llvm.org/docs/ClangFormatStyleOptions.html>
DisableFormat: true



================================================
FILE: wvbrowser_ui/commands.js
================================================
const commands = {
    MG_NAVIGATE: 1,
    MG_UPDATE_URI: 2,
    MG_GO_FORWARD: 3,
    MG_GO_BACK: 4,
    MG_NAV_STARTING: 5,
    MG_NAV_COMPLETED: 6,
    MG_RELOAD: 7,
    MG_CANCEL: 8,
    MG_CREATE_TAB: 10,
    MG_UPDATE_TAB: 11,
    MG_SWITCH_TAB: 12,
    MG_CLOSE_TAB: 13,
    MG_CLOSE_WINDOW: 14,
    MG_SHOW_OPTIONS: 15,
    MG_HIDE_OPTIONS: 16,
    MG_OPTIONS_LOST_FOCUS: 17,
    MG_OPTION_SELECTED: 18,
    MG_SECURITY_UPDATE: 19,
    MG_UPDATE_FAVICON: 20,
    MG_GET_SETTINGS: 21,
    MG_GET_FAVORITES: 22,
    MG_REMOVE_FAVORITE: 23,
    MG_CLEAR_CACHE: 24,
    MG_CLEAR_COOKIES: 25,
    MG_GET_HISTORY: 26,
    MG_REMOVE_HISTORY_ITEM: 27,
    MG_CLEAR_HISTORY: 28
};



================================================
FILE: wvbrowser_ui/content_ui/favorites.html
================================================
<html>
    <head>
        <title>Favorites</title>
        <link rel="shortcut icon" href="img/favorites.png">
        <link rel="stylesheet" type="text/css" href="styles.css">
        <link rel="stylesheet" type="text/css" href="items.css">
    </head>
    <body>
        <h1 class="main-title">Favorites</h1>
        <div id="entries-container">
            You don't have any favorites.
        </div>
        <script src="../commands.js"></script>
        <script src="favorites.js"></script>
    <body>
</html>



================================================
FILE: wvbrowser_ui/content_ui/favorites.js
================================================
const messageHandler = event => {
    var message = event.data.message;
    var args = event.data.args;

    switch (message) {
        case commands.MG_GET_FAVORITES:
            loadFavorites(args.favorites);
            break;
        default:
            console.log(`Unexpected message: ${JSON.stringify(event.data)}`);
            break;
    }
};

function requestFavorites() {
    let message = {
        message: commands.MG_GET_FAVORITES,
        args: {}
    };

    window.chrome.webview.postMessage(message);
}

function removeFavorite(uri) {
    let message = {
        message: commands.MG_REMOVE_FAVORITE,
        args: {
            uri: uri
        }
    };

    window.chrome.webview.postMessage(message);
}

function loadFavorites(payload) {
    let fragment = document.createDocumentFragment();

    if (payload.length > 0) {
        let container = document.getElementById('entries-container');
        container.textContent = '';
    }

    payload.map(favorite => {
        let favoriteContainer = document.createElement('div');
        favoriteContainer.className = 'item-container';
        let favoriteElement = document.createElement('div');
        favoriteElement.className = 'item';

        let faviconElement = document.createElement('div');
        faviconElement.className = 'favicon';
        let faviconImage = document.createElement('img');
        faviconImage.src = favorite.favicon;
        faviconElement.appendChild(faviconImage);

        let labelElement = document.createElement('div');
        labelElement.className = 'label-title';
        let linkElement = document.createElement('a');
        linkElement.textContent = favorite.title;
        linkElement.href = favorite.uri;
        linkElement.title = favorite.title;
        labelElement.appendChild(linkElement);

        let uriElement = document.createElement('div');
        uriElement.className = 'label-uri';
        let textElement = document.createElement('p');
        textElement.textContent = favorite.uriToShow || favorite.uri;
        textElement.title = favorite.uriToShow || favorite.uri;
        uriElement.appendChild(textElement);

        let buttonElement = document.createElement('div');
        buttonElement.className = 'btn-close';
        buttonElement.addEventListener('click', function(e) {
            favoriteContainer.parentNode.removeChild(favoriteContainer);
            removeFavorite(favorite.uri);
        });

        favoriteElement.appendChild(faviconElement);
        favoriteElement.appendChild(labelElement);
        favoriteElement.appendChild(uriElement);
        favoriteElement.appendChild(buttonElement);

        favoriteContainer.appendChild(favoriteElement);
        fragment.appendChild(favoriteContainer);
    });

    let container = document.getElementById('entries-container');
    container.appendChild(fragment);
}

function init() {
    window.chrome.webview.addEventListener('message', messageHandler);
    requestFavorites();
}

init();



================================================
FILE: wvbrowser_ui/content_ui/history.css
================================================
.header-date {
    font-weight: 400;
    font-size: 14px;
    color: rgb(16, 16, 16);
    line-height: 20px;
    padding-top: 10px;
    padding-bottom: 4px;
    margin: 0;
}

#btn-clear {
    font-size: 14px;
    color: rgb(0, 97, 171);
    cursor: pointer;
    line-height: 20px;
}

#btn-clear.hidden {
    display: none;
}

#overlay {
    position: fixed;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.2);
}

#overlay.hidden {
    display: none;
}

#prompt-box {
    display: flex;
    box-sizing: border-box;
    flex-direction: column;
    position: fixed;
    left: calc(50% - 130px);
    top: calc(50% - 70px);
    width: 260px;
    height: 140px;
    padding: 20px;
    border-radius: 5px;
    background-color: white;

    box-shadow: rgba(0, 0, 0, 0.13) 0px 1.6px 20px, rgba(0, 0, 0, 0.11) 0px 0.3px 10px;
}

#prompt-options {
    flex: 1;
    display: flex;
    justify-content: flex-end;

    user-select: none;
}

.prompt-btn {
    flex: 1;
    flex-grow: 0;
    align-self: flex-end;
    cursor: pointer;
    font-family: 'system-ui', sans-serif;
    display: inline-block;
    padding: 2px 7px;
    font-size: 14px;
    line-height: 20px;
    border-radius: 3px;
    font-weight: 400;
}

#prompt-true {
    background-color: rgb(0, 112, 198);
    color: white;
}

#prompt-false {
    background-color: rgb(210, 210, 210);
    margin-right: 5px;
}



================================================
FILE: wvbrowser_ui/content_ui/history.html
================================================
<html>
    <head>
        <title>History</title>
        <link rel="shortcut icon" href="img/history.png">
        <link rel="stylesheet" type="text/css" href="styles.css">
        <link rel="stylesheet" type="text/css" href="items.css">
        <link rel="stylesheet" type="text/css" href="history.css">
    </head>
    <body>
        <div id="overlay" class="hidden">
            <div id="prompt-box">
                <span class="prompt-text">Clear history?</span>
                <div id="prompt-options">
                    <div class="prompt-btn" id="prompt-false">Cancel</div>
                    <div class="prompt-btn" id="prompt-true">Clear</div>
                </div>
            </div>
        </div>
        <h1 class="main-title">History</h1>
        <div>
            <span id="btn-clear" class="hidden">Clear history</span>
        </div>
        <div id="entries-container">
            Loading...
        </div>

        <script src="../commands.js"></script>
        <script src="history.js"></script>
    </body>
</html>



================================================
FILE: wvbrowser_ui/content_ui/history.js
================================================
const DEFAULT_HISTORY_ITEM_COUNT = 20;
const EMPTY_HISTORY_MESSAGE = `You haven't visited any sites yet.`;
let requestedTop = 0;
let lastRequestSize = 0;
let itemHeight = 48;

const dateStringFormat = new Intl.DateTimeFormat('default', {
    weekday: 'long',
    year: 'numeric',
    month: 'long',
    day: 'numeric'
});

const timeStringFormat = new Intl.DateTimeFormat('default', {
    hour: '2-digit',
    minute: '2-digit'
});

const messageHandler = event => {
    var message = event.data.message;
    var args = event.data.args;

    switch (message) {
        case commands.MG_GET_HISTORY:
            let entriesContainer = document.getElementById('entries-container');
            if (args.from == 0 && args.items.length) {
                entriesContainer.textContent = '';

                let clearButton = document.getElementById('btn-clear');
                clearButton.classList.remove('hidden');
            }

            loadItems(args.items);
            if (args.items.length == lastRequestSize) {
                document.addEventListener('scroll', requestTrigger);
            } else if (entriesContainer.childElementCount == 0) {
                loadUIForEmptyHistory();
            }
            break;
        default:
            console.log(`Unexpected message: ${JSON.stringify(event.data)}`);
            break;
    }
};

const requestTrigger = function(event) {
    let triggerRange = 50;
    let element = document.body;

    if (element.scrollTop + element.clientHeight >= element.scrollHeight - triggerRange) {
        getMoreHistoryItems();
        event.target.removeEventListener('scroll', requestTrigger);
    }
};

function requestHistoryItems(from, count) {
    let message = {
        message: commands.MG_GET_HISTORY,
        args: {
            from: from,
            count: count || DEFAULT_HISTORY_ITEM_COUNT
        }
    };

    window.chrome.webview.postMessage(message);
}

function removeItem(id) {
    let message = {
        message: commands.MG_REMOVE_HISTORY_ITEM,
        args: {
            id: id
        }
    };

    window.chrome.webview.postMessage(message);
}

function createItemElement(item, id, date) {
    let itemContainer = document.createElement('div');
    itemContainer.id = id;
    itemContainer.className = 'item-container';

    let itemElement = document.createElement('div');
    itemElement.className = 'item';

    // Favicon
    let faviconElement = document.createElement('div');
    faviconElement.className = 'favicon';
    let faviconImage = document.createElement('img');
    faviconImage.src = item.favicon;
    faviconElement.append(faviconImage);
    itemElement.append(faviconElement);

    // Title
    let titleLabel = document.createElement('div');
    titleLabel.className = 'label-title';
    let linkElement = document.createElement('a');
    linkElement.href = item.uri;
    linkElement.title = item.title;
    linkElement.textContent = item.title;
    titleLabel.append(linkElement);
    itemElement.append(titleLabel);

    // URI
    let uriLabel = document.createElement('div');
    uriLabel.className = 'label-uri';
    let textElement = document.createElement('p');
    textElement.title = item.uri;
    textElement.textContent = item.uri;
    uriLabel.append(textElement);
    itemElement.append(uriLabel);

    // Time
    let timeLabel = document.createElement('div');
    timeLabel.className = 'label-time';
    let timeText = document.createElement('p');
    timeText.textContent = timeStringFormat.format(date);
    timeLabel.append(timeText);
    itemElement.append(timeLabel);

    // Close button
    let closeButton = document.createElement('div');
    closeButton.className = 'btn-close';
    closeButton.addEventListener('click', function(e) {
        if (itemContainer.parentNode.children.length <= 2) {
            itemContainer.parentNode.remove();
        } else {
            itemContainer.remove();
        }

        let entriesContainer = document.getElementById('entries-container');
        if (entriesContainer.childElementCount == 0) {
            loadUIForEmptyHistory();
        }
        removeItem(parseInt(id.split('-')[1]));
    });
    itemElement.append(closeButton);
    itemContainer.append(itemElement);

    return itemContainer;
}

function createDateContainer(id, date) {
    let dateContainer = document.createElement('div');
    dateContainer.id = id;

    let dateLabel = document.createElement('h3');
    dateLabel.className = 'header-date';
    dateLabel.textContent = dateStringFormat.format(date);
    dateContainer.append(dateLabel);

    return dateContainer;
}

function loadItems(items) {
    let dateContainer;
    let fragment;

    items.map((entry) => {
        let id = entry.id;
        let item = entry.item;
        let itemContainerId = `item-${id}`;

        // Skip the item if already loaded. This could happen if the user
        // visits an item for the current date again before requesting more
        // history items.
        let itemContainer = document.getElementById(itemContainerId);
        if (itemContainer) {
            return;
        }

        let date = new Date(item.timestamp);
        let day = date.getDate();
        let month = date.getMonth();
        let year = date.getFullYear();
        let dateContainerId = `entries-${month}-${day}-${year}`;

        // If entry belongs to a new date, append buffered items for previous
        // date.
        if (dateContainer && dateContainer.id != dateContainerId) {
            dateContainer.append(fragment);
        }

        dateContainer = document.getElementById(dateContainerId);
        if (!dateContainer) {
            dateContainer = createDateContainer(dateContainerId, date);
            fragment = document.createDocumentFragment();

            let entriesContainer = document.getElementById('entries-container');
            entriesContainer.append(dateContainer);
        } else if (!fragment) {
            fragment = document.createDocumentFragment();
        }

        itemContainer = createItemElement(item, itemContainerId, date);
        fragment.append(itemContainer);
    });

    // Append remaining items in buffer
    if (fragment) {
        dateContainer.append(fragment);
    }
}

function getMoreHistoryItems(n) {
    n = n ? n : DEFAULT_HISTORY_ITEM_COUNT;

    requestHistoryItems(requestedTop, n);
    requestedTop += n;
    lastRequestSize = n;
    document.removeEventListener('scroll', requestTrigger);
}

function addUIListeners() {
    let confirmButton = document.getElementById('prompt-true');
    confirmButton.addEventListener('click', function(event) {
        clearHistory();
        event.stopPropagation();
    });

    let cancelButton = document.getElementById('prompt-false');
    cancelButton.addEventListener('click', function(event) {
        toggleClearPrompt();
        event.stopPropagation();
    });

    let promptBox = document.getElementById('prompt-box');
    promptBox.addEventListener('click', function(event) {
        event.stopPropagation();
    });

    let promptOverlay = document.getElementById('overlay');
    promptOverlay.addEventListener('click', toggleClearPrompt);

    let clearButton = document.getElementById('btn-clear');
    clearButton.addEventListener('click', toggleClearPrompt);
}

function toggleClearPrompt() {
    let promptOverlay = document.getElementById('overlay');
    promptOverlay.classList.toggle('hidden');
}

function loadUIForEmptyHistory() {
    let entriesContainer = document.getElementById('entries-container');
    entriesContainer.textContent = EMPTY_HISTORY_MESSAGE;

    let clearButton = document.getElementById('btn-clear');
    clearButton.classList.add('hidden');
}

function clearHistory() {
    toggleClearPrompt();
    loadUIForEmptyHistory();

    let message = {
        message: commands.MG_CLEAR_HISTORY,
        args: {}
    };

    window.chrome.webview.postMessage(message);
}

function init() {
    window.chrome.webview.addEventListener('message', messageHandler);

    let viewportItemsCapacity = Math.round(window.innerHeight / itemHeight);
    addUIListeners();
    getMoreHistoryItems(viewportItemsCapacity);
}

init();



================================================
FILE: wvbrowser_ui/content_ui/items.css
================================================
.item-container {
    box-sizing: border-box;
    padding: 4px 0;
    height: 48px;
}

.item {
    display: flex;
    width: 100%;
    max-width: 820px;
    height: 40px;
    width: 100%;
    border-radius: 4px;
    box-sizing: border-box;
    box-shadow: rgba(0, 0, 0, 0.13) 0px 1.6px 3.6px, rgba(0, 0, 0, 0.11) 0px 0.3px 0.9px;
    align-items: center;
    background: rgb(255, 255, 255);
}

.item:hover {
    box-shadow: 0px 4.8px 10.8px rgba(0,0,0,0.13), 0px 0.9px 2.7px rgba(0,0,0,0.11);
}

.favicon {
    display: flex;
    height: 40px;
    width: 40px;
    justify-content: center;
    align-items: center;
}

.favicon img {
    width: 16px;
    height: 16px;
}

.label-title, .label-uri {
    display: flex;
    flex: 1;
    min-width: 0;
    height: 40px;
    align-items: center;
}

.label-title a {
    cursor: pointer;
    display: inline-block;
    white-space: nowrap;
    text-overflow: ellipsis;
    font-weight: 600;
    font-size: 12px;
    line-height: 16px;
    color: rgb(16, 16, 16);
    border-width: initial;
    border-style: none;
    border-color: initial;
    border-image: initial;
    overflow: hidden;
    background: none;
    text-decoration: none;
}

.label-title a:hover {
    text-decoration: underline;
}

.label-uri, .label-time {
    margin: 0 6px;
    line-height: 16px;
    font-size: 12px;
    color: rgb(115, 115, 115);
}

.label-uri p, .label-time p {
    display: block;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
}

.btn-close {
    height: 28px;
    width: 28px;
    margin: 6px;
    border-radius: 2px;
    background-image: url('img/close.png');
    background-size: 100%;
}

.btn-close:hover {
    background-color: rgb(243, 243, 243);
}



================================================
FILE: wvbrowser_ui/content_ui/settings.css
================================================
.settings-entry {
    display: block;
    height: 48px;
    width: 100%;
    max-width: 500px;

    background: none;
    border: none;
    padding: 4px 0;
	font: inherit;
	cursor: pointer;
}

#entry-script, #entry-popups {
    display: none;
}

.entry {
    display: block;
    height: 100%;
    text-align: left;
    border-radius: 5px;
}

.entry:hover {
    background-color: rgb(220, 220, 220);
}

.entry:focus {
    outline: none;
}

.entry-name, .entry-value {
    display: inline-flex;
    height: 100%;
    vertical-align: middle;
}

.entry-name span, .entry-value span {
    flex: 1;
    align-self: center;
}

.entry-name {
    padding-left: 10px;
}

.entry-value {
    float: right;
    vertical-align: middle;
    margin: 0 15px;
    font-size: 0.8em;
    color: gray;
}



================================================
FILE: wvbrowser_ui/content_ui/settings.html
================================================
<html>
    <head>
        <title>Settings</title>
        <link rel="shortcut icon" href="img/settings.png">
        <link rel="stylesheet" type="text/css" href="styles.css">
        <link rel="stylesheet" type="text/css" href="settings.css">
    </head>
    <body>
        <h1 class="main-title">Settings</h1>
        <div class="page-content">
            <button class="settings-entry" id="entry-cache">
                <div class="entry">
                    <div class="entry-name">
                        <span>Clear cache</span>
                    </div>
                    <div class="entry-value">
                        <span></span>
                    </div>
                </div>
            </button>
            <button class="settings-entry" id="entry-cookies">
                <div class="entry">
                    <div class="entry-name">
                        <span>Clear cookies</span>
                    </div>
                    <div class="entry-value">
                        <span></span>
                    </div>
                </div>
            </button>
            <button class="settings-entry" id="entry-script">
                <div class="entry">
                    <div class="entry-name">
                        <span>Toggle JavaScript</span>
                    </div>
                    <div class="entry-value">
                        <span></span>
                    </div>
                </div>
            </button>
            <button class="settings-entry" id="entry-popups">
                <div class="entry">
                    <div class="entry-name">
                        <span>Block pop-ups</span>
                    </div>
                    <div class="entry-value">
                        <span></span>
                    </div>
                </div>
            </button>
        </div>

        <script src="../commands.js"></script>
        <script src="settings.js"></script>
    </body>
</html>



================================================
FILE: wvbrowser_ui/content_ui/settings.js
================================================
const messageHandler = event => {
    var message = event.data.message;
    var args = event.data.args;

    switch (message) {
        case commands.MG_GET_SETTINGS:
            loadSettings(args.settings);
            break;
        case commands.MG_CLEAR_CACHE:
            if (args.content && args.controls) {
                updateLabelForEntry('entry-cache', 'Cleared');
            } else {
                updateLabelForEntry('entry-cache', 'Try again');
            }
            break;
        case commands.MG_CLEAR_COOKIES:
            if (args.content && args.controls) {
                updateLabelForEntry('entry-cookies', 'Cleared');
            } else {
                updateLabelForEntry('entry-cookies', 'Try again');
            }
            break;
        default:
            console.log(`Unexpected message: ${JSON.stringify(event.data)}`);
            break;
    }
};

function addEntriesListeners() {
    let cacheEntry = document.getElementById('entry-cache');
    cacheEntry.addEventListener('click', function(e) {
        let message = {
            message: commands.MG_CLEAR_CACHE,
            args: {}
        };

        window.chrome.webview.postMessage(message);
    });

    let cookiesEntry = document.getElementById('entry-cookies');
    cookiesEntry.addEventListener('click', function(e) {
        let message = {
            message: commands.MG_CLEAR_COOKIES,
            args: {}
        };

        window.chrome.webview.postMessage(message);
    });

    let scriptEntry = document.getElementById('entry-script');
    scriptEntry.addEventListener('click', function(e) {
        // Toggle script support
    });

    let popupsEntry = document.getElementById('entry-popups');
    popupsEntry.addEventListener('click', function(e) {
        // Toggle popups
    });
}

function requestBrowserSettings() {
    let message = {
        message: commands.MG_GET_SETTINGS,
        args: {}
    };

    window.chrome.webview.postMessage(message);
}

function loadSettings(settings) {
    if (settings.scriptsEnabled) {
        updateLabelForEntry('entry-script', 'Enabled');
    } else {
        updateLabelForEntry('entry-script', 'Disabled');
    }

    if (settings.blockPopups) {
        updateLabelForEntry('entry-popups', 'Blocked');
    } else {
        updateLabelForEntry('entry-popups', 'Allowed');
    }
}

function updateLabelForEntry(elementId, label) {
    let entryElement = document.getElementById(elementId);
    if (!entryElement) {
        console.log(`Element with id ${elementId} does not exist`);
        return;
    }

    let labelSpan = entryElement.querySelector(`.entry-value span`);

    if (!labelSpan) {
        console.log(`${elementId} does not have a label`);
        return;
    }

    labelSpan.textContent = label;
}

function init() {
    window.chrome.webview.addEventListener('message', messageHandler);
    requestBrowserSettings();
    addEntriesListeners();
}

init();



================================================
FILE: wvbrowser_ui/content_ui/styles.css
================================================
html, body {
    margin: 0;
    border: none;
    padding: 0;

    font-family: Arial, Helvetica, sans-serif;
    background-color: rgb(240, 240, 242);
}

p {
    margin: 0;
}

body {
    padding: 32px 50px;
    font-family: 'system-ui', sans-serif;
}

.main-title {
    display: block;
    margin-bottom: 18px;
    font-size: 24px;
    font-weight: 600;
    color: rgb(16, 16, 16);
}



================================================
FILE: wvbrowser_ui/controls_ui/address-bar.css
================================================
#address-bar-container {
    display: flex;
    height: calc(100% - 10px);
    width: 80%;
    max-width: calc(100% - 160px);

    background-color: white;
    border: 1px solid gray;
    border-radius: 5px;

    position: relative;
    align-self: center;
}

#address-bar-container:focus-within {
    outline: none;
    box-shadow: 0 0 3px dodgerblue;
}

#address-bar-container:focus-within #btn-clear {
    display: block;
}

#security-label {
    display: inline-flex;
    height: 100%;
    margin-left: 2px;

    vertical-align: top;
}

#security-label span {
    font-family: Arial;
    font-size: 0.9em;
    color: gray;
    vertical-align: middle;
    flex: 1;
    align-self: center;
    text-align: left;
    padding-left: 5px;
    white-space: nowrap;
}

.icn {
    display: inline-block;
    margin: 2px 0;
    border-radius: 5px;
    top: 0;
    width: 26px;
    height: 26px;
}

#icn-lock {
    background-size: 100%;
}

#security-label.label-unknown .icn {
    background-image: url('img/unknown.png');
}

#security-label.label-insecure .icn {
    background-image: url('img/insecure.png');
}

#security-label.label-insecure span {
    color: rgb(192, 0, 0);
}

#security-label.label-neutral .icn {
    background-image: url('img/neutral.png');
}

#security-label.label-secure .icn {
    background-image: url('img/secure.png');
}

#security-label.label-secure span, #security-label.label-neutral span {
    display: none;
}

#icn-favicon {
    background-size: 100%;
}

#img-favicon {
    width: 18px;
    height: 18px;
    padding: 4px;
}

#address-form {
    margin: 0;
}

#address-field {
    flex: 1;
    padding: 0;
    border: none;
    border-radius: 5px;
    margin: 0;

    line-height: 30px;
    width: 100%;
}

#address-field:focus {
    outline: none;
}

#btn-fav {
    margin: 2px 5px;
    background-size: 100%;
    background-image: url('img/favorite.png');
}

#btn-fav:hover, #btn-clear:hover {
    background-color: rgb(230, 230, 230);
}

#btn-fav.favorited {
    background-image: url('img/favorited.png');
}

#btn-clear {
    display: none;
    width: 16px;
    height: 16px;
    border: none;
    align-self: center;
    background-color: transparent;
    background-image: url(img/cancel.png);
    background-size: 100%;
    border: none;
    border-radius: 8px;
}



================================================
FILE: wvbrowser_ui/controls_ui/controls.css
================================================
#controls-bar {
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    height: 40px;
    background-color: rgb(230, 230, 230);
}

.btn, .btn-disabled, .btn-cancel, .btn-active {
    display: inline-block;
    border: none;
    margin: 5px 0;
    border-radius: 5px;
    outline: none;
    height: 30px;
    width: 30px;

    background-size: 100%;
}

#btn-forward {
    background-image: url('img/goForward.png');
}

.btn-disabled#btn-forward {
    background-image: url('img/goForward_disabled.png');
}

#btn-back {
    background-image: url('img/goBack.png');
}

.btn-disabled#btn-back {
    background-image: url('img/goBack_disabled.png');
}

#btn-reload {
    background-image: url('img/reload.png');
}

.btn-cancel#btn-reload {
    background-image: url('img/cancel.png');
}

#btn-options {
    background-image: url('img/options.png');
}

.controls-group {
    display: inline-block;
    height: 40px;
}

#nav-controls-container {
    align-self: flex-start;
    padding-left: 10px;
}

#manage-controls-container {
    align-self: flex-end;
    padding-right: 10px;
}

.btn:hover, .btn-cancel:hover, .btn-active {
    background-color: rgb(200, 200, 200);
}



================================================
FILE: wvbrowser_ui/controls_ui/default.css
================================================
html, body {
    height: 70px;
}



================================================
FILE: wvbrowser_ui/controls_ui/default.html
================================================
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="styles.css">
        <link rel="stylesheet" type="text/css" href="default.css">
        <link rel="stylesheet" type="text/css" href="controls.css">
        <link rel="stylesheet" type="text/css" href="address-bar.css">
        <link rel="stylesheet" type="text/css" href="strip.css">
    </head>
    <body>
        <script src="../commands.js"></script>
        <script src="tabs.js"></script>
        <script src="storage.js"></script>
        <script src="favorites.js"></script>
        <script src="history.js"></script>
        <script src="default.js"></script>
    </body>
</html>



================================================
FILE: wvbrowser_ui/controls_ui/default.js
================================================
const WORD_REGEX = /^[^//][^.]*$/;
const VALID_URI_REGEX = /^[-:.&#+()[\]$'*;@~!,?%=\/\w]+$/; // Will check that only RFC3986 allowed characters are included
const SCHEMED_URI_REGEX = /^\w+:.+$/;

let settings = {
    scriptsEnabled: true,
    blockPopups: true
};

const messageHandler = event => {
    var message = event.data.message;
    var args = event.data.args;

    switch (message) {
        case commands.MG_UPDATE_URI:
            if (isValidTabId(args.tabId)) {
                const tab = tabs.get(args.tabId);
                let previousURI = tab.uri;

                // Update the tab state
                tab.uri = args.uri;
                tab.uriToShow = args.uriToShow;
                tab.canGoBack = args.canGoBack;
                tab.canGoForward = args.canGoForward;

                // If the tab is active, update the controls UI
                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }

                isFavorite(tab.uri, (isFavorite) => {
                    tab.isFavorite = isFavorite;
                    updateFavoriteIcon();
                });

                // Don't add history entry if URI has not changed
                if (tab.uri == previousURI) {
                    break;
                }

                // Filter URIs that should not appear in history
                if (!tab.uri || tab.uri == 'about:blank') {
                    tab.historyItemId = INVALID_HISTORY_ID;
                    break;
                }

                if (tab.uriToShow && tab.uriToShow.substring(0, 10) == 'browser://') {
                    tab.historyItemId = INVALID_HISTORY_ID;
                    break;
                }

                addHistoryItem(historyItemFromTab(args.tabId), (id) => {
                    tab.historyItemId = id;
                });
            }
            break;
        case commands.MG_NAV_STARTING:
            if (isValidTabId(args.tabId)) {
                // Update the tab state
                tabs.get(args.tabId).isLoading = true;

                // If the tab is active, update the controls UI
                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }
            }
            break;
        case commands.MG_NAV_COMPLETED:
            if (isValidTabId(args.tabId)) {
                // Update tab state
                tabs.get(args.tabId).isLoading = false;

                // If the tab is active, update the controls UI
                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }
            }
            break;
        case commands.MG_UPDATE_TAB:
            if (isValidTabId(args.tabId)) {
                const tab = tabs.get(args.tabId);
                const tabElement = document.getElementById(`tab-${args.tabId}`);

                if (!tabElement) {
                    refreshTabs();
                    return;
                }

                // Update tab label
                // Use given title or fall back to a generic tab title
                tab.title = args.title || 'Tab';
                const tabLabel = tabElement.firstChild;
                const tabLabelSpan = tabLabel.firstChild;
                tabLabelSpan.textContent = tab.title;

                // Update title in history item
                // Browser pages will keep an invalid history ID
                if (tab.historyItemId != INVALID_HISTORY_ID) {
                    updateHistoryItem(tab.historyItemId, historyItemFromTab(args.tabId));
                }
            }
            break;
        case commands.MG_OPTIONS_LOST_FOCUS:
            let optionsButton = document.getElementById('btn-options');
            if (optionsButton) {
                if (optionsButton.className = 'btn-active') {
                    toggleOptionsDropdown();
                }
            }
            break;
        case commands.MG_SECURITY_UPDATE:
            if (isValidTabId(args.tabId)) {
                const tab = tabs.get(args.tabId);
                tab.securityState = args.state;

                if (args.tabId == activeTabId) {
                    updateNavigationUI(message);
                }
            }
            break;
        case commands.MG_UPDATE_FAVICON:
            if (isValidTabId(args.tabId)) {
                updateFaviconURI(args.tabId, args.uri);
            }
            break;
        case commands.MG_CLOSE_WINDOW:
            closeWindow();
            break;
        case commands.MG_CLOSE_TAB:
            if (isValidTabId(args.tabId)) {
                closeTab(args.tabId);
            }
            break;
        case commands.MG_GET_FAVORITES:
            if (isValidTabId(args.tabId)) {
                getFavoritesAsJson((payload) => {
                    args.favorites = payload;
                    window.chrome.webview.postMessage(event.data);
                });
            }
            break;
        case commands.MG_REMOVE_FAVORITE:
            removeFavorite(args.uri);
            break;
        case commands.MG_GET_SETTINGS:
            if (isValidTabId(args.tabId)) {
                args.settings = settings;
                window.chrome.webview.postMessage(event.data);
            }
            break;
        case commands.MG_GET_HISTORY:
            if (isValidTabId(args.tabId)) {
                getHistoryItems(args.from, args.count, (payload) => {
                    args.items = payload;
                    window.chrome.webview.postMessage(event.data);
                });
            }
            break;
        case commands.MG_REMOVE_HISTORY_ITEM:
            removeHistoryItem(args.id);
            break;
        case commands.MG_CLEAR_HISTORY:
            clearHistory();
            break;
        default:
            console.log(`Received unexpected message: ${JSON.stringify(event.data)}`);
    }
};

function processAddressBarInput() {
    var text = document.querySelector('#address-field').value;
    tryNavigate(text);
}

function tryNavigate(text) {
    try {
        var uriParser = new URL(text);

        // URL creation succeeded, verify protocol is allowed
        switch (uriParser.protocol) {
            case 'http:':
            case 'https:':
            case 'file:':
            case 'ftp:':
                // Allowed protocol, navigate
                navigateActiveTab(uriParser.href, false);
                break;
            default:
                // Protocol not allowed, search Bing
                navigateActiveTab(getSearchURI(text), true);
                break;
        }
    } catch (e) {
        // URL creation failed, check for invalid characters
        if (containsIlegalCharacters(text) || isSingleWord(text)) {
            // Search Bing
            navigateActiveTab(getSearchURI(text), true);
        } else {
            // Try with HTTP
            if (!hasScheme(text)) {
                tryNavigate(`http:${text}`);
            } else {
                navigateActiveTab(getSearchURI(text), true);
            }
        }
    }
}

function navigateActiveTab(uri, isSearch) {
    var message = {
        message: commands.MG_NAVIGATE,
        args: {
            uri: uri,
            encodedSearchURI: isSearch ? uri : getSearchURI(uri)
        }
    };

    window.chrome.webview.postMessage(message);
}

function reloadActiveTabContent() {
    var message = {
        message: commands.MG_RELOAD,
        args: {}
    };
    window.chrome.webview.postMessage(message);
}

function containsIlegalCharacters(query) {
    return !VALID_URI_REGEX.test(query);
}

function isSingleWord(query) {
    return WORD_REGEX.test(query);
}

function hasScheme(query) {
    return SCHEMED_URI_REGEX.test(query);
}

function getSearchURI(query) {
    return `https://www.bing.com/search?q=${encodeURIComponent(query)}`;
}

function closeWindow() {
    var message = {
        message: commands.MG_CLOSE_WINDOW,
        args: {}
    };

    window.chrome.webview.postMessage(message);
}

// Show active tab's URI in the address bar
function updateURI() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);
    document.getElementById('address-field').value = activeTab.uriToShow || activeTab.uri;
}

// Show active tab's favicon in the address bar
function updateFavicon() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);

    let faviconElement = document.getElementById('img-favicon');
    if (!faviconElement) {
        refreshControls();
        return;
    }

    faviconElement.src = activeTab.favicon;

}

// Update back and forward buttons for the active tab
function updateBackForwardButtons() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);
    let btnForward = document.getElementById('btn-forward');
    let btnBack = document.getElementById('btn-back');

    if (!btnBack || !btnForward) {
        refreshControls();
        return;
    }

    if (activeTab.canGoForward)
        btnForward.className = 'btn';
    else
        btnForward.className = 'btn-disabled';

    if (activeTab.canGoBack)
        btnBack.className = 'btn';
    else
        btnBack.className = 'btn-disabled';
}

// Update reload button for the active tab
function updateReloadButton() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);

    let btnReload = document.getElementById('btn-reload');
    if (!btnReload) {
        refreshControls();
        return;
    }

    btnReload.className = activeTab.isLoading ? 'btn-cancel' : 'btn';
}

// Update lock icon for the active tab
function updateLockIcon() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);

    let labelElement = document.getElementById('security-label');
    if (!labelElement) {
        refreshControls();
        return;
    }

    switch (activeTab.securityState) {
        case 'insecure':
            labelElement.className = 'label-insecure';
            break;
        case 'neutral':
            labelElement.className = 'label-neutral';
            break;
        case 'secure':
            labelElement.className = 'label-secure';
            break;
        default:
            labelElement.className = 'label-unknown';
            break;
    }
}

// Update favorite status for the active tab
function updateFavoriteIcon() {
    if (activeTabId == INVALID_TAB_ID) {
        return;
    }

    let activeTab = tabs.get(activeTabId);
    isFavorite(activeTab.uri, (isFavorite) => {
        let favoriteElement = document.getElementById('btn-fav');
        if (!favoriteElement) {
            refreshControls();
            return;
        }

        if (isFavorite) {
            favoriteElement.classList.add('favorited');
            activeTab.isFavorite = true;
        } else {
            favoriteElement.classList.remove('favorited');
            activeTab.isFavorite = false;
        }
    });

}

function updateNavigationUI(reason) {
    switch (reason) {
        case commands.MG_UPDATE_URI:
            updateURI();
            updateFavoriteIcon();
            updateBackForwardButtons();
            break;
        case commands.MG_NAV_COMPLETED:
        case commands.MG_NAV_STARTING:
            updateReloadButton();
            break;
        case commands.MG_SECURITY_UPDATE:
            updateLockIcon();
            break;
        case commands.MG_UPDATE_FAVICON:
            updateFavicon();
            break;
        // If a reason is not provided (for requests not originating from a
        // message), default to switch tab behavior.
        default:
        case commands.MG_SWITCH_TAB:
            updateURI();
            updateLockIcon();
            updateFavicon();
            updateFavoriteIcon();
            updateReloadButton();
            updateBackForwardButtons();
            break;
    }
}

function loadTabUI(tabId) {
    if (isValidTabId(tabId)) {
        let tab = tabs.get(tabId);

        let tabElement = document.createElement('div');
        tabElement.className = tabId == activeTabId ? 'tab-active' : 'tab';
        tabElement.id = `tab-${tabId}`;

        let tabLabel = document.createElement('div');
        tabLabel.className = 'tab-label';

        let labelText = document.createElement('span');
        labelText.textContent = tab.title;
        tabLabel.appendChild(labelText);

        let closeButton = document.createElement('div');
        closeButton.className = 'btn-tab-close';
        closeButton.addEventListener('click', function(e) {
            closeTab(tabId);
        });

        tabElement.appendChild(tabLabel);
        tabElement.appendChild(closeButton);

        var createTabButton = document.getElementById('btn-new-tab');
        document.getElementById('tabs-strip').insertBefore(tabElement, createTabButton);

        tabElement.addEventListener('click', function(e) {
            if (e.srcElement.className != 'btn-tab-close') {
                switchToTab(tabId, true);
            }
        });
    }
}

function toggleOptionsDropdown() {
    const optionsButtonElement = document.getElementById('btn-options');
    const elementClass = optionsButtonElement.className;

    var message;
    if (elementClass === 'btn') {
        // Update UI
        optionsButtonElement.className = 'btn-active';

        message = {
            message: commands.MG_SHOW_OPTIONS,
            args: {}
        };
    } else {
        // Update UI
        optionsButtonElement.className = 'btn';

        message = {
            message:commands.MG_HIDE_OPTIONS,
            args: {}
        };
    }

    window.chrome.webview.postMessage(message);
}

function refreshControls() {
    let controlsElement = document.getElementById('controls-bar');
    if (controlsElement) {
        controlsElement.remove();
    }

    controlsElement = document.createElement('div');
    controlsElement.id = 'controls-bar';

    // Navigation controls
    let navControls = document.createElement('div');
    navControls.className = 'controls-group';
    navControls.id = 'nav-controls-container';

    let backButton = document.createElement('div');
    backButton.className = 'btn-disabled';
    backButton.id = 'btn-back';
    navControls.append(backButton);

    let forwardButton = document.createElement('div');
    forwardButton.className = 'btn-disabled';
    forwardButton.id = 'btn-forward';
    navControls.append(forwardButton);

    let reloadButton = document.createElement('div');
    reloadButton.className = 'btn';
    reloadButton.id = 'btn-reload';
    navControls.append(reloadButton);

    controlsElement.append(navControls);

    // Address bar
    let addressBar = document.createElement('div');
    addressBar.id = 'address-bar-container';

    let securityLabel = document.createElement('div');
    securityLabel.className = 'label-unknown';
    securityLabel.id = 'security-label';

    let labelSpan = document.createElement('span');
    labelSpan.textContent = 'Not secure';
    securityLabel.append(labelSpan);

    let lockIcon = document.createElement('div');
    lockIcon.className = 'icn';
    lockIcon.id = 'icn-lock';
    securityLabel.append(lockIcon);
    addressBar.append(securityLabel);

    let faviconElement = document.createElement('div');
    faviconElement.className = 'icn';
    faviconElement.id = 'icn-favicon';

    let faviconImage = document.createElement('img');
    faviconImage.id = 'img-favicon';
    faviconImage.src = 'img/favicon.png';
    faviconElement.append(faviconImage);
    addressBar.append(faviconElement);

    let addressInput = document.createElement('input');
    addressInput.id = 'address-field';
    addressInput.placeholder = 'Search or enter web address';
    addressInput.type = 'text';
    addressInput.spellcheck = false;
    addressBar.append(addressInput);

    let clearButton = document.createElement('button');
    clearButton.id = 'btn-clear';
    addressBar.append(clearButton);

    let favoriteButton = document.createElement('div');
    favoriteButton.className = 'icn';
    favoriteButton.id = 'btn-fav';
    addressBar.append(favoriteButton);
    controlsElement.append(addressBar);

    // Manage controls
    let manageControls = document.createElement('div');
    manageControls.className = 'controls-group';
    manageControls.id = 'manage-controls-container';

    let optionsButton = document.createElement('div');
    optionsButton.className = 'btn';
    optionsButton.id = 'btn-options';
    manageControls.append(optionsButton);
    controlsElement.append(manageControls);

    // Insert controls bar into document
    let tabsElement = document.getElementById('tabs-strip');
    if (tabsElement) {
        tabsElement.parentElement.insertBefore(controlsElement, tabsElement);
    } else {
        let bodyElement = document.getElementsByTagName('body')[0];
        bodyElement.append(controlsElement);
    }

    addControlsListeners();
    updateNavigationUI();
}

function refreshTabs() {
    let tabsStrip = document.getElementById('tabs-strip');
    if (tabsStrip) {
        tabsStrip.remove();
    }

    tabsStrip = document.createElement('div');
    tabsStrip.id = 'tabs-strip';

    let newTabButton = document.createElement('div');
    newTabButton.id = 'btn-new-tab';

    let buttonSpan = document.createElement('span');
    buttonSpan.textContent = '+';
    buttonSpan.id = 'plus-label';
    newTabButton.append(buttonSpan);
    tabsStrip.append(newTabButton);

    let bodyElement = document.getElementsByTagName('body')[0];
    bodyElement.append(tabsStrip);

    addTabsListeners();

    Array.from(tabs).map((tabEntry) => {
        loadTabUI(tabEntry[0]);
    });
}

function toggleFavorite() {
    activeTab = tabs.get(activeTabId);
    if (activeTab.isFavorite) {
        removeFavorite(activeTab.uri, () => {
            activeTab.isFavorite = false;
            updateFavoriteIcon();
        });
    } else {
        addFavorite(favoriteFromTab(activeTabId), () => {
            activeTab.isFavorite = true;
            updateFavoriteIcon();
        });
    }
}

function addControlsListeners() {
    let inputField = document.querySelector('#address-field');
    let clearButton = document.querySelector('#btn-clear');

    inputField.addEventListener('keypress', function(e) {
        var key = e.which || e.keyCode;
        if (key === 13) { // 13 is enter
            e.preventDefault();
            processAddressBarInput();
        }
    });

    inputField.addEventListener('focus', function(e) {
        e.target.select();
    });

    inputField.addEventListener('blur', function(e) {
        inputField.setSelectionRange(0, 0);
        if (!inputField.value) {
            updateURI();
        }
    });

    clearButton.addEventListener('click', function(e) {
        inputField.value = '';
        inputField.focus();
        e.preventDefault();
    });

    document.querySelector('#btn-forward').addEventListener('click', function(e) {
        if (document.getElementById('btn-forward').className === 'btn') {
            var message = {
                message: commands.MG_GO_FORWARD,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        }
    });

    document.querySelector('#btn-back').addEventListener('click', function(e) {
        if (document.getElementById('btn-back').className === 'btn') {
            var message = {
                message: commands.MG_GO_BACK,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        }
    });

    document.querySelector('#btn-reload').addEventListener('click', function(e) {
        var btnReload = document.getElementById('btn-reload');
        if (btnReload.className === 'btn-cancel') {
            var message = {
                message: commands.MG_CANCEL,
                args: {}
            };
            window.chrome.webview.postMessage(message);
        } else if (btnReload.className === 'btn') {
            reloadActiveTabContent();
        }
    });

    document.querySelector('#btn-options').addEventListener('click', function(e) {
        toggleOptionsDropdown();
    });

    window.onkeydown = function(event) {
        if (event.ctrlKey) {
            switch (event.key) {
                case 'r':
                case 'R':
                    reloadActiveTabContent();
                    break;
                case 'd':
                case 'D':
                    toggleFavorite();
                    break;
                case 't':
                case 'T':
                    createNewTab(true);
                    break;
                case 'p':
                case 'P':
                case '+':
                case '-':
                case '_':
                case '=':
                    break;
                default:
                    return;
            }

            event.preventDefault();
        }
    };

    // Prevent zooming the UI
    window.addEventListener('wheel', function(event) {
        if (event.ctrlKey) {
            event.preventDefault();
        }}, { passive: false });
}

function addTabsListeners() {
    document.querySelector('#btn-new-tab').addEventListener('click', function(e) {
        createNewTab(true);
    });

    document.querySelector('#btn-fav').addEventListener('click', function(e) {
        toggleFavorite();
    });
}

function init() {
    window.chrome.webview.addEventListener('message', messageHandler);
    refreshControls();
    refreshTabs();

    createNewTab(true);
}

init();



================================================
FILE: wvbrowser_ui/controls_ui/favorites.js
================================================
function isFavorite(uri, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['favorites']);
        let favoritesStore = transaction.objectStore('favorites');
        let favoriteStatusRequest = favoritesStore.get(uri);

        favoriteStatusRequest.onerror = function(event) {
            console.log(`Could not query for ${uri}: ${event.target.error.message}`);
        };

        favoriteStatusRequest.onsuccess = function() {
            callback(favoriteStatusRequest.result);
        };
    });
}

function addFavorite(favorite, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['favorites'], 'readwrite');
        let favoritesStore = transaction.objectStore('favorites');
        let addFavoriteRequest = favoritesStore.add(favorite);

        addFavoriteRequest.onerror = function(event) {
            console.log(`Could not add favorite with key: ${favorite.uri}`);
            console.log(event.target.error.message);
        };

        addFavoriteRequest.onsuccess = function(event) {
            if (callback) {
                callback();
            }
        };
    });
}

function removeFavorite(key, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['favorites'], 'readwrite');
        let favoritesStore = transaction.objectStore('favorites');
        let removeFavoriteRequest = favoritesStore.delete(key);

        removeFavoriteRequest.onerror = function(event) {
            console.log(`Could not remove favorite with key: ${key}`);
            console.log(event.target.error.message);
        };

        removeFavoriteRequest.onsuccess = function(event) {
            if (callback) {
                callback();
            }
        };
    });
}

function getFavoritesAsJson(callback) {
    queryDB((db) => {
        let transaction = db.transaction(['favorites']);
        let favoritesStore = transaction.objectStore('favorites');
        let getFavoritesRequest = favoritesStore.getAll();

        getFavoritesRequest.onerror = function(event) {
            console.log(`Could retrieve favorites`);
            console.log(event.target.error.message);
        };

        getFavoritesRequest.onsuccess = function(event) {
            if (callback) {
                callback(getFavoritesRequest.result);
            }
        };
    });
}



================================================
FILE: wvbrowser_ui/controls_ui/history.js
================================================
const INVALID_HISTORY_ID = -1;

function addHistoryItem(item, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['history'], 'readwrite');
        let historyStore = transaction.objectStore('history');

        // Check if an item for this URI exists on this day
        let currentDate = new Date();
        let year = currentDate.getFullYear();
        let month = currentDate.getMonth();
        let date = currentDate.getDate();
        let todayDate = new Date(year, month, date);

        let existingItemsIndex = historyStore.index('stampedURI');
        let lowerBound = [item.uri, todayDate];
        let upperBound = [item.uri, currentDate];
        let range = IDBKeyRange.bound(lowerBound, upperBound);
        let request = existingItemsIndex.openCursor(range);

        request.onsuccess = function(event) {
            let cursor = event.target.result;
            if (cursor) {
                // There's an entry for this URI, update the item
                cursor.value.timestamp = item.timestamp;
                let updateRequest = cursor.update(cursor.value);

                updateRequest.onsuccess = function(event) {
                    if (callback) {
                        callback(event.target.result.primaryKey);
                    }
                };
            } else {
                // No entry for this URI, add item
                let addItemRequest = historyStore.add(item);

                addItemRequest.onsuccess = function(event) {
                    if (callback) {
                        callback(event.target.result);
                    }
                };
            }
        };

    });
}

function updateHistoryItem(id, item, callback) {
    if (!id) {
        return;
    }

    queryDB((db) => {
        let transaction = db.transaction(['history'], 'readwrite');
        let historyStore = transaction.objectStore('history');
        let storedItemRequest = historyStore.get(id);
        storedItemRequest.onsuccess = function(event) {
            let storedItem = event.target.result;
            item.timestamp = storedItem.timestamp;

            let updateRequest = historyStore.put(item, id);

            updateRequest.onsuccess = function(event) {
                if (callback) {
                    callback();
                }
            };
        };

    });
}

function getHistoryItems(from, n, callback) {
    if (n <= 0 || from < 0) {
        if (callback) {
            callback([]);
        }
    }

    queryDB((db) => {
        let transaction = db.transaction(['history']);
        let historyStore = transaction.objectStore('history');
        let timestampIndex = historyStore.index('timestamp');
        let cursorRequest = timestampIndex.openCursor(null, 'prev');

        let current = 0;
        let items = [];
        cursorRequest.onsuccess = function(event) {
            let cursor = event.target.result;

            if (!cursor || current >= from + n) {
                if (callback) {
                    callback(items);
                }

                return;
            }

            if (current >= from) {
                items.push({
                    id: cursor.primaryKey,
                    item: cursor.value
                });
            }

            ++current;
            cursor.continue();
        };
    });
}

function removeHistoryItem(id, callback) {
    queryDB((db) => {
        let transaction = db.transaction(['history'], 'readwrite');
        let historyStore = transaction.objectStore('history');
        let removeItemRequest = historyStore.delete(id);

        removeItemRequest.onerror = function(event) {
            console.log(`Could not remove history item with ID: ${id}`);
            console.log(event.target.error.message);
        };

        removeItemRequest.onsuccess = function(event) {
            if (callback) {
                callback();
            }
        };
    });
}

function clearHistory(callback) {
    queryDB((db) => {
        let transaction = db.transaction(['history'], 'readwrite');
        let historyStore = transaction.objectStore('history');
        let clearRequest = historyStore.clear();

        clearRequest.onsuccess = function(event) {
            if (callback) {
                callback();
            }
        };
    });
}



================================================
FILE: wvbrowser_ui/controls_ui/options.css
================================================
html, body {
    width: 200px;
    height: 107px;
}

#dropdown-wrapper {
    width: calc(100% - 2px);
    height: calc(100% - 2px);
    border: 1px solid gray;
}

.dropdown-item {
    background-color: rgb(240, 240, 240);
}

.dropdown-item:hover {
    background-color: rgb(220, 220, 220);
}

.item-label {
    display: flex;
    height: 35px;
    text-align: center;
    vertical-align: middle;

    white-space: nowrap;
    overflow: hidden;
}

.item-label span {
    font-family: Arial;
    font-size: 0.8em;
    vertical-align: middle;
    flex: 1;
    align-self: center;
    text-align: left;
    padding-left: 10px;
}



================================================
FILE: wvbrowser_ui/controls_ui/options.html
================================================
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="styles.css">
        <link rel="stylesheet" type="text/css" href="options.css">
    </head>
    <body>
        <div id="dropdown-wrapper">
            <div id="item-settings" class="dropdown-item">
                <div class="item-label">
                    <span>Settings</span>
                </div>
            </div>
            <div id="item-history" class="dropdown-item">
                <div class="item-label">
                    <span>History</span>
                </div>
            </div>
            <div id="item-favorites" class="dropdown-item">
                <div class="item-label">
                    <span>Favorites</span>
                </div>
            </div>
        </div>

        <script src="../commands.js"></script>
        <script src="options.js"></script>
    </body>
</html>



================================================
FILE: wvbrowser_ui/controls_ui/options.js
================================================
function navigateToBrowserPage(path) {
    const navMessage = {
        message: commands.MG_NAVIGATE,
        args: {
            uri: `browser://${path}`
        }
    };

    window.chrome.webview.postMessage(navMessage);
}

// Add listener for the options menu entries
function addItemsListeners() {

    // Close dropdown when item is selected
    (() => {
        const dropdownItems = Array.from(document.getElementsByClassName('dropdown-item'));
        dropdownItems.map(item => {
            item.addEventListener('click', function(e) {
                const closeMessage = {
                    message: commands.MG_OPTION_SELECTED,
                    args: {}
                };
                window.chrome.webview.postMessage(closeMessage);
            });

            // Navigate to browser page
            let entry = item.id.split('-')[1];
            switch (entry) {
                case 'settings':
                case 'history':
                case 'favorites':
                    item.addEventListener('click', function(e) {
                        navigateToBrowserPage(entry);
                    });
                    break;
            }
        });
    })();
}

function init() {
    addItemsListeners();
}

init();



================================================
FILE: wvbrowser_ui/controls_ui/storage.js
================================================
function handleUpgradeEvent(event) {
    console.log('Creating DB');
    let newDB = event.target.result;

    newDB.onerror = function(event) {
        console.log('Something went wrong');
        console.log(event);
    };

    let newFavoritesStore = newDB.createObjectStore('favorites', {
        keyPath: 'uri'
    });

    newFavoritesStore.transaction.oncomplete = function(event) {
        console.log('Object stores created');
    };

    let newHistoryStore = newDB.createObjectStore('history', {
        autoIncrement: true
    });

    newHistoryStore.createIndex('timestamp', 'timestamp', {
        unique: false
    });

    newHistoryStore.createIndex('stampedURI', ['uri', 'timestamp'], {
        unique: false
    });
}

function queryDB(query) {
    let request = window.indexedDB.open('WVBrowser');

    request.onerror = function(event) {
        console.log('Failed to open database');
    };

    request.onsuccess = function(event) {
        let db = event.target.result;
        query(db);
    };

    request.onupgradeneeded = handleUpgradeEvent;
}



================================================
FILE: wvbrowser_ui/controls_ui/strip.css
================================================
#tabs-strip {
    display: flex;
    height: 28px;

    border-top: 1px solid rgb(200, 200, 200);
    border-bottom: 1px solid rgb(200, 200, 200);
    background-color: rgb(230, 230, 230);
}

.tab, .tab-active {
    display: flex;
    flex: 1;
    height: 100%;
    border-right: 1px solid rgb(200, 200, 200);
    overflow: hidden;
    max-width: 250px;
}

.tab-active {
    background-color: rgb(240, 240, 240);
}

#btn-new-tab {
    display: flex;
    height: 100%;
    width: 30px;
}

#btn-new-tab:hover, .btn-tab-close:hover {
    background-color: rgb(200, 200, 200);
}

#plus-label {
    display: block;
    flex: 1;
    align-self: center;
    line-height: 30px;
    width: 30px;
    text-align: center;
}

.btn-tab-close {
    display: inline-block;
    align-self: center;
    min-width: 16px;
    width: 16px;
    height: 16px;
    margin: 0 5px;
    border-radius: 4px;

    background-size: 100%;
    background-image: url('img/cancel.png');
}

.tab-label {
    display: flex;
    flex: 1;
    padding: 5px;
    padding-left: 10px;
    height: calc(100% - 10px);
    vertical-align: middle;

    white-space:nowrap;
    overflow:hidden;
}

.tab-label span {
    font-family: Arial;
    font-size: 0.8em;
    flex: 1;
    align-self: center;
}



================================================
FILE: wvbrowser_ui/controls_ui/styles.css
================================================
html, body {
    margin: 0;
    border: none;
    padding: 0;
}

p {
    margin: 0;
}

* {
    user-select: none;
}



================================================
FILE: wvbrowser_ui/controls_ui/tabs.js
================================================
var tabs = new Map();
var tabIdCounter = 0;
var activeTabId = 0;
const INVALID_TAB_ID = 0;

function getNewTabId() {
    return ++tabIdCounter;
}

function isValidTabId(tabId) {
    return tabId != INVALID_TAB_ID && tabs.has(tabId);
}

function createNewTab(shouldBeActive) {
    const tabId = getNewTabId();

    var message = {
        message: commands.MG_CREATE_TAB,
        args: {
            tabId: parseInt(tabId),
            active: shouldBeActive || false
        }
    };

    window.chrome.webview.postMessage(message);

    tabs.set(parseInt(tabId), {
        title: 'New Tab',
        uri: '',
        uriToShow: '',
        favicon: 'img/favicon.png',
        isFavorite: false,
        isLoading: false,
        canGoBack: false,
        canGoForward: false,
        securityState: 'unknown',
        historyItemId: INVALID_HISTORY_ID
    });

    loadTabUI(tabId);

    if (shouldBeActive) {
        switchToTab(tabId, false);
    }
}

function switchToTab(id, updateOnHost) {
    if (!id) {
        console.log('ID not provided');
        return;
    }

    // Check the tab to switch to is valid
    if (!isValidTabId(id)) {
        return;
    }

    // No need to switch if the tab is already active
    if (id == activeTabId) {
        return;
    }

    // Get the tab element to switch to
    var tab = document.getElementById(`tab-${id}`);
    if (!tab) {
        console.log(`Can't switch to tab ${id}: element does not exist`);
        return;
    }

    // Change the style for the previously active tab
    if (isValidTabId(activeTabId)) {
        const activeTabElement = document.getElementById(`tab-${activeTabId}`);

        // Check the previously active tab element does actually exist
        if (activeTabElement) {
            activeTabElement.className = 'tab';
        }
    }

    // Set tab as active
    tab.className = 'tab-active';
    activeTabId = id;

    // Instruct host app to switch tab
    if (updateOnHost) {
        var message = {
            message: commands.MG_SWITCH_TAB,
            args: {
                tabId: parseInt(activeTabId)
            }
        };

        window.chrome.webview.postMessage(message);
    }

    updateNavigationUI(commands.MG_SWITCH_TAB);
}

function closeTab(id) {
    // If closing tab was active, switch tab or close window
    if (id == activeTabId) {
        if (tabs.size == 1) {
            // Last tab is closing, shut window down
            tabs.delete(id);
            closeWindow();
            return;
        }

        // Other tabs are open, switch to rightmost tab
        var tabsEntries = Array.from(tabs.entries());
        var lastEntry = tabsEntries.pop();
        if (lastEntry[0] == id) {
            lastEntry = tabsEntries.pop();
        }
        switchToTab(lastEntry[0], true);
    }

    // Remove tab element
    var tabElement = document.getElementById(`tab-${id}`);
    if (tabElement) {
        tabElement.parentNode.removeChild(tabElement);
    }
    // Remove tab from map
    tabs.delete(id);

    var message = {
        message: commands.MG_CLOSE_TAB,
        args: {
            tabId: id
        }
    };

    window.chrome.webview.postMessage(message);
}

function updateFaviconURI(tabId, src) {
    let tab = tabs.get(tabId);
    if (tab.favicon != src) {
        let img = new Image();

        // Update favicon element on successful load
        img.onload = () => {
            console.log('Favicon loaded');
            tab.favicon = src;

            if (tabId == activeTabId) {
                updatedFaviconURIHandler(tabId, tab);
            }
        };

        if (src) {
            // Try load from root on failed load
            img.onerror = () => {
                console.log('Cannot load favicon from link, trying with root');
                updateFaviconURI(tabId, '');
            };
        } else {
            // No link for favicon, try loading from root
            try {
                let tabURI = new URL(tab.uri);
                src = `${tabURI.origin}/favicon.ico`;
            } catch(e) {
                console.log(`Could not parse tab ${tabId} URI`);
            }

            img.onerror = () => {
                console.log('No favicon in site root. Using default favicon.');
                tab.favicon = 'img/favicon.png';
                updatedFaviconURIHandler(tabId, tab);
            };
        }

        img.src = src;
    }
}

function updatedFaviconURIHandler(tabId, tab) {
    updateNavigationUI(commands.MG_UPDATE_FAVICON);

    // Update favicon in history item
    if (tab.historyItemId != INVALID_HISTORY_ID) {
        updateHistoryItem(tab.historyItemId, historyItemFromTab(tabId));
    }
}

function favoriteFromTab(tabId) {
    if (!isValidTabId(tabId)) {
        console.log('Invalid tab ID');
        return;
    }

    let tab = tabs.get(tabId);
    let favicon = tab.favicon == 'img/favicon.png' ? '../controls_ui/' + tab.favicon : tab.favicon;
    return {
        uri: tab.uri,
        uriToShow: tab.uriToShow,
        title: tab.title,
        favicon: favicon
    };
}

function historyItemFromTab(tabId) {
    if (!isValidTabId(tabId)) {
        console.log('Invalid tab ID');
        return;
    }

    let tab = tabs.get(tabId);
    let favicon = tab.favicon == 'img/favicon.png' ? '../controls_ui/' + tab.favicon : tab.favicon;
    return {
        uri: tab.uri,
        title: tab.title,
        favicon: favicon,
        timestamp: new Date()
    }
}



================================================
FILE: .github/CODE_OF_CONDUCT.md
================================================
# Microsoft Open Source Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).

Resources:

- [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/)
- [Microsoft Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/)
- Contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with questions or concerns



================================================
FILE: .github/ISSUE_TEMPLATE/config.yml
================================================
blank_issues_enabled: true
contact_links:
  - name: Issue with WebView2
    url:  https://github.com/MicrosoftEdge/WebViewFeedback/issues/new/choose
    about: Please open issues with the WebView2 control in the Feedback repo



================================================
FILE: .github/ISSUE_TEMPLATE/issue-with-webview2browser-app.md
================================================
---
name: Issue with WebView2Browser app
about: Open an issue specifically about the WebView2Browser application (not the WebView2
  control)
title: ''
labels: ''
assignees: ''

---




