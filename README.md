# Chrome/Chromium switches.

A quick way to launch Google Chrome or Chromium from the command line with flags / switches.  
"Flags are used to enable particular features or modify otherwise default functionality."

_On OS X:_
```bash
open /Applications/Google\ Chrome.app --fullscreen --kiosk
```
_On Linux:_
```bash
chromium-browser --fullscreen --kiosk
```
_On Windows:_
```bash
start chrome --fullscreen --kiosk
```

A complete list of Flags can be found at: http://peter.sh/examples/?/chromium-switches.html


## Common Flags:


** --action-box **
_Enables or disables the "action box" UI in the toolbar._

** --allow-cross-origin-auth-prompt **  
_Allows third-party content included on a page to prompt for a HTTP basic auth username/password pair._

** --allow-file-access **  
_On ChromeOS, file:access is disabled except for certain whitelisted directories. This switch re-enables file:for testing._

** --allow-http-background-page **  
_Allows non-https URL for background-page for hosted apps._

** --allow-nacl-socket-api **  
_Allows the browser to load extensions that lack a modern manifest when that would otherwise be forbidden._

** --allow-outdated-plugins **  
_Don't block outdated plugins._

** --allow-running-insecure-content **  
_By default, an https page cannot run JavaScript, CSS or plug-ins from http URLs. This provides an override to get the old insecure behavior._

** --allow-scripting-gallery **  
_Allows injecting extensions and user scripts on the extensions gallery site. Normally prevented for security reasons, but can be useful for automation testing of the gallery._

** --always-authorize-plugins **  
_Prevents Chrome from requiring authorization to run certain widely installed but less commonly used plug-ins._

** --app-id **  
_Specifies that the extension-app with the specified id should be launched according to its configuration._

** --app **  
_Specifies that the associated value should be launched in "application" mode._

** --apps-devtool **  
_Flag to enable apps_devtool app._

** --app-window-size **  
_Specifies the initial size for application windows launched with ** --app. --app-window-size=w,h **  
_** --app-notify-channel-server-url **  
_A URL for the server which assigns channel ids for server pushed app notifications._

** --apps-checkout-url **  
_Overrides the apps checkout URL, which is used to determine when to expose some private APIs._

** --apps-gallery-download-url **  
_The URL that the webstore APIs download extensions from. Note: the URL must contain one %s (ie. for a replacable string) for the extension ID._

** --apps-gallery-url **  
_A setting to cause extension/app installs from the webstore skip the normal confirmation dialog. A value of 'accept' means to always act as if the dialog was accepted, and 'cancel' means to always act as if the dialog was cancelled._

** --apps-gallery-update-url **  
_The update url used by gallery/webstore extensions._

** --app-mode-oauth-token **  
_Value of OAuth2 refresh token for ** --force-app-mode. **  
_** --apps-new-install-bubble **  
_Whether to always use the new app install bubble when installing an app._

** --apps-no-throb **  
_Disable throbber for extension apps._

** --auth-schemes **  
_Whitelist of servers that Negotiate will generate delegated Kerberos tickets for._

** --auth-server-whitelist **  
_Whitelist of servers which NTLM and Negotiate can automatically authenticate with using the default credentials of the currently logged in user._

** --auto-launch-at-startup **  
_A flag that is used to tell Chrome that it was launched automatically at computer startup and not by some user action._

** --autofill-service-url **  
_Flag used to tell Chrome the base url of the Autofill service._

** --automation-channel **  
_The value of this switch tells the app to listen for and broadcast automation-related messages on IPC channel with the given ID._

** --check-for-update-interval **  
_Causes the automation provider to reinitialize its IPC channel instead of shutting down when a client disconnects._

** --chrome-frame-shutdown-delay **  
_Checks the cloud print connector policy, informing the service process if the policy is set to disallow the connector, then quits._

** --chrome-version **  
_Tells chrome to load the specified version of chrome.dll on Windows. If this version cannot be loaded, Chrome will exit._

** --cipher-suite-blacklist **  
_Comma-separated list of SSL cipher suites to disable._

** --clear-token-service **  
_Clears the token service before using it. This allows simulating the expiration of credentials during testing._

** --cloud-print-delete-file **  
_Used with kCloudPrintFile. Tells Chrome to delete the file when finished displaying the print dialog._

** --cloud-print-file **  
_Tells chrome to display the cloud print dialog and upload the specified file for printing._

** --cloud-print-file-type **  
_Specifies the mime type to be used when uploading data from the file referenced by cloud-print-file. Defaults to "application/pdf" if unspecified._

** --cloud-print-print-ticket **  
_Used with kCloudPrintFile to specify a JSON print ticket for the resulting print job. Defaults to null if unspecified._

** --cloud-print-job-title **  
_Used with kCloudPrintFile to specify a title for the resulting print job._

** --cloud-print-proxy-id **  
_The unique id to be used for this cloud print proxy instance._

** --cloud-print-service **  
_The URL of the cloud print service to use, overrides any value stored in preferences, and the default. Only used if the cloud print service has been enabled (see enable-cloud-print)._

** --component-updater-debug **  
_Comma-separated options to troubleshoot the component updater. Only valid for the browser process._

** --conflicting-modules-check **  
_Causes the browser process to inspect loaded and registered DLLs for known conflicts and warn the user._

** --new-content-settings **  
_Toggles a new version of the content settings dialog in options._

** --country **  
_The Country we should use. This is normally obtained from the operating system during first run and cached in the preferences afterwards. This is a string value, the 2 letter code from ISO 3166-1._

** --crash-on-hang-threads **  
_Comma-separated list of BrowserThreads that cause browser process to crash if the given browser thread is not responsive. UI,IO,DB,FILE,CACHE are the list of BrowserThreads that are supported._

For example:

** --crash-on-hang-threads=UI:3:18,IO:3:18 --> Crash the browser if UI or IO is not responsive for 18 seconds and the number of browser threads that are responding is less than or equal to 3. **  
_** --debug-enable-frame-toggle **  
_Some platforms like ChromeOS default to empty desktop. Browser tests may need to add this switch so that at least one browser instance is created on startup._

** --debug-packed-apps **  
_Adds debugging entries such as Inspect Element to context menus of packed apps._

** --debug-print **  
_Enables support to debug printing subsystem._

** --device-management-url **  
_Specifies the URL at which to fetch configuration policy from the device management backend. Specifying this switch turns on managed policy from the device management backend._

** --diagnostics **  
_Triggers a plethora of diagnostic modes._

** --disable-async-dns **  
_Disables the experimental asynchronous DNS client._

** --disable-background-mode **  
_Disables CNAME lookup of the host when generating the Kerberos SPN for a Negotiate challenge. See HttpAuthHandlerNegotiate::CreateSPN for more background._

** --disable-background-networking **  
_Disable several subsystems which run network requests in the background. This is for use when doing network performance testing to avoid noise in the measurements._

** --disable-bundled-ppapi-flash **  
_Disables the bundled PPAPI version of Flash._

** --disable-component-update **  
_Disables the bookmark autocomplete provider (BookmarkProvider)._

** --disable-crl-sets **  
_Disables establishing certificate revocation information by downloading a set of CRLs rather than performing on-line checks._

** --disable-custom-jumplist **  
_Disables the custom JumpList on Windows 7._

** --disable-default-apps **  
_Disables installation of default apps on first run. This is used during automated testing._

** --disable-dhcp-wpad **  
_Disables retrieval of PAC URLs from DHCP as per the WPAD standard._

** --disable-extensions **  
_Disable extensions._

** --disable-instant-extended-api **  
_Disable checking for user opt-in for extensions that want to inject script into file URLs (ie, always allow it). This is used during automated testing._

** --disable-ipv6 **  
_Disables improved SafeBrowsing download protection._

** --disable-ip-pooling **  
_Disables IP Pooling within the networks stack (SPDY only). When a connection is needed for a domain which shares an IP with an existing connection, attempt to use the existing connection._

** --disable-ntp-other-sessions-menu **  
_Disables the menu on the NTP for accessing sessions from other devices._

** --disable-popup-blocking **  
_Disable pop-up blocking._

** --disable-preconnect **  
_Disable speculative TCP/IP preconnection._

** --disable-prompt-on-repost **  
_Normally when the user attempts to navigate to a page that was the result of a post we prompt to make sure they want to. This switch may be used to disable that check. This switch is used during automated testing._

** --disable-restore-session-state **  
_Prevents the URLs of BackgroundContents from being remembered and re-launched when the browser restarts._

** --disable-sync **  
_Disables throttling prints initiated by scripts._

** --disable-sync-app-settings **  
_Disables syncing of app settings._

** --disable-sync-apps **  
_Disables syncing of apps._

** --disable-sync-app-notifications **  
_Disable syncing app notifications._

** --disable-sync-autofill **  
_Disables syncing of autofill._

** --disable-sync-autofill-profile **  
_Disables syncing of autofill Profile._

** --disable-sync-bookmarks **  
_Disables syncing of bookmarks._

** --disable-sync-dictionary **  
_Disables syncing of dictionary._

** --disable-sync-extension-settings **  
_Disables syncing extension settings._

** --disable-sync-extensions **  
_Disables syncing of extensions._

** --disable-sync-passwords **  
_Disables syncing of history delete directives._

** --disable-sync-preferences **  
_Disables syncing of preferences._

** --disable-sync-search-engines **  
_Disable syncing custom search engines._

** --disable-sync-tabs **  
_Disables syncing browser sessions. Will override kEnableSyncTabs._

** --disable-sync-themes **  
_Disables syncing of themes._

** --disable-sync-typed-urls **  
_Disables syncing browser typed urls._

** --disable-translate **  
_Allows disabling of translate from the command line to assist with automated browser testing (e.g. Selenium/WebDriver). Normal browser users should disable translate with the preference._

** --disable-tls-channel-id **  
_Disables TLS Channel ID extension._

** --disable-web-resources **  
_Disables the backend service for web resources._

** --disable-web-security **  
_Don't enforce the same-origin policy. (Used by people testing their sites.)

** --disable-web-sockets **  
_Disable Web Sockets support._

** --disable-webaudio **  
_Disable web audio API

** --disable-webgl **  
_Disable WebGL support._

** --disk-cache-dir **  
_Some tests seem to require the application to close when the last browser window is closed. Thus, we need a switch to force this behavior for ChromeOS Aura, disable "zero window mode"._

** --disk-cache-size **  
_Forces the maximum disk space to be used by the disk cache, in bytes._

** --dns-log-details **  
_Undocumented, but self explanatory. Log DNS details._

** --dns-prefetch-disable **  
_Disables prefetching of DNS information._

** --dump-histograms-on-exit **  
_Dump any accumualted histograms to the log when browser terminates (requires logging to be enabled to really do anything). Used by developers and test scripts._

** --enable-async-dns **  
_Enables the experimental asynchronous DNS client._

** --enable-auth-negotiate-port **  
_Enables the inclusion of non-standard ports when generating the Kerberos SPN in response to a Negotiate challenge. See HttpAuthHandlerNegotiate::CreateSPN for more background._

** --enable-autologin **  
_Enables the pre- and auto-login features. When a user signs in to sync, the browser's cookie jar is pre-filled with GAIA cookies. When the user visits a GAIA login page, an info bar can help the user login._

** --enable-benchmarking **  
_Enables the benchmarking extensions._

** --enable-cloud-print-proxy **  
_This applies only when the process type is "service". Enables the Cloud Print Proxy component within the service process._

** --enable-contacts **  
_Enables fetching the user's contacts from Google and showing them in the Chrome OS apps list._

** --enable-crxless-web-apps **  
_Enables web developers to create apps for Chrome without using crx packages._

** --enable-desktop-guest-mode **  
_Enables desktop guest mode._

** --enable-devtools-experiments **  
_If true devtools experimental settings are enabled._

** --enable-interactive-autocomplete **  
_Enables an interactive autocomplete UI and a way to invoke this UI from WebKit by enabling HTMLFormElement#requestAutocomplete (and associated autocomplete events and logic)._

** --easy-off-store-extension-install **  
_Enables extensions to be easily installed from sites other than the web store. Without this flag, they can still be installed, but must be manually dragged onto chrome://extensions/._

** --enable-extension-activity-ui **  
_Enables extension APIs that are in development._

** --extensions-in-action-box **  
_Enables or disables showing extensions in the action box._

** --enable-file-cookies **  
_By default, cookies are not allowed on file://. They are needed for testing, for example page cycler and layout tests._

** --enable-google-now-integration **  
_Enables Google Now integration._

** --enable-instant-extended-api **  
_Enable Instant extended API._

** --enable-ipv6 **  
_Enables IPv6 support, even if probes suggest that it may not be fully supported. Some probes may require internet connections, and this flag will allow support independent of application testing. This flag overrides ** --disable-ipv6 which appears elswhere in this file. **  
_** --enable-ipc-fuzzing **  
_Enables the IPC fuzzer for reliability testing

** --enable-ip-pooling **  
_Enables IP Pooling within the networks stack (SPDY only). When a connection is needed for a domain which shares an IP with an existing connection, attempt to use the existing connection._

** --enable-managed-users **  
_Enables support for user profiles that are managed by another user and can have restrictions applied._

** --enable-memory-info **  
_Allows reporting memory info (JS heap size) to page._

** --enable-memory-internals-ui **  
_Enables metrics recording and reporting in the browser startup sequence, as if this was an official Chrome build where the user allowed metrics reporting. This is used for testing only._

** --enable-nacl **  
_Runs the Native Client inside the renderer process and enables GPU plugin (internally adds lEnableGpuPlugin to the command line)._

** --enable-nacl-debug **  
_Enables debugging via RSP over a socket._

** --nacl-debug-mask **  
_Uses NaCl manifest URL to choose whether NaCl program will be debugged by debug stub. // Switch value format: [!]pattern1,pattern2,...,patternN. Each pattern uses the same syntax as patterns in Chrome extension manifest. The only difference is that * scheme matches all schemes instead of matching only http and https. If the value doesn't start with !, a program will be debugged if manifest URL matches any pattern. If the value starts with !, a program will be debugged if manifest URL does not match any pattern._

** --enable-nacl-exception-handling **  
_Enables hardware exception handling via debugger process._

** --enable-native-messaging **  
_Enables the native messaging extensions API._

** --enable-net-benchmarking **  
_Enables the network-related benchmarking extensions._

** --enable-new-autofill-ui **  
_Enables the new Autofill UI, which is part of the browser process rather than part of the renderer process._

** --enable-npn **  
_Enables NPN and SPDY. In case server supports SPDY, browser will use SPDY._

** --enable-npn-http **  
_Enables NPN with HTTP. It means NPN is enabled but SPDY won't be used. HTTP is still used for all requests._

** --enable-panels **  
_Enables panels (always on-top docked pop-up windows)._

** --enable-panel-stacking **  
_Enables panel stacking support._

** --enable-password-generation **  
_Enables password generation when we detect that the user is going through account creation._

** --enable-pnacl **  
_Enables the installation and usage of Portable Native Client._

** --enable-profiling **  
_Enables tracking of tasks in profiler for viewing via about:profiler. To predominantly disable tracking (profiling), use the command line switch: ** --enable-profiling=0 Some tracking will still take place at startup, but it will be turned off during chrome_browser_main. **  
_** --enable-query-extraction **  
_Enables query extraction in the omnibox._

** --enable-quic **  
_Enables support for the QUIC protocol. This is a temporary testing flag._

** --enable-sdch **  
_Enables content settings based on host and plug-in in the user preferences._

** --enable-spdy3 **  
_Enable SPDY/3. This is a temporary testing flag._

** --enable-spdy-credential-frames **  
_Enable SPDY CREDENTIAL frame support. This is a temporary testing flag._

** --enable-spelling-auto-correct **  
_Enables auto correction for misspelled words._

** --enable-stacked-tab-strip **  
_Enables the stacked tabstrip._

** --enable-suggestions-ntp **  
_Enables experimental suggestions pane in New Tab page._

** --enable-tab-groups-context-menu **  
_Enables synced notifications._

** --enable-watchdog **  
_Enables Alternate-Protocol when the port is user controlled (> 1024)._

** --enable-websocket-over-spdy **  
_Uses WebSocket over SPDY._

** --explicitly-allowed-ports **  
_Explicitly allows additional ports using a comma-separated list of port numbers._

** --event-page-idle-time **  
_The time in seconds that an extension event page can be idle before it is shut down._

** --event-page-unloading-time **  
_The time in seconds that an extension event page has between being notified of its impending unload and that unload happening._

** --extension-process **  
_Marks a renderer as extension process._

** --extensions-update-frequency **  
_Frequency in seconds for Extensions auto-update._

** --fake-variations-channel **  
_Fakes the channel of the browser for purposes of Variations filtering. This is to be used for testing only. Possible values are "stable", "beta", "dev" and "canary". Note that this only applies if the browser's reported channel is UNKNOWN._

** --flag-switches-begin / --flag-switches-end **  
_These two flags are added around the switches chrome:flags adds to the command line. This is useful to see which switches were added by chrome:flags on chrome:version. They don't have any effect._

** --feedback-server **  
_Alternative feedback server to use when submitting user feedback

** --file-descriptor-limit **  
_The file descriptor limit is set to the value of this switch, subject to the OS hard limits. Useful for testing that file descriptor exhaustion is handled gracefully._

** --force-app-mode **  
_Forces application mode. This hides certain system UI elements and forces the app to be installed if it hasn't been already._

** --force-first-run **  
_Displays the First Run experience when the browser is started, regardless of whether or not it's actually the First Run (this overrides kNoFirstRun)._

** --force-load-cloud-policy **  
_Tries to load cloud policy for every signed in user, regardless of whether they are a dasher user or not. Used to allow any GAIA account to be used for testing the cloud policy framework._

** --gaia-profile-info **  
_Enables using GAIA information to populate profile name and icon._

** --google-search-domain-check-url **  
_Specifies an alternate URL to use for retrieving the search domain for Google. Useful for testing._

** --gssapi-library-name **  
_Specifies a custom name for the GSSAPI library to load._

** --help / --h **  
_These flags show the man page on Linux. They are equivalent to each other._

** --hide-icons **  
_Makes Windows happy by allowing it to show "Enable access to this program" checkbox in Add/Remove Programs->Set Program Access and Defaults. This only shows an error box because the only way to hide Chrome is by uninstalling it._

** --disable-full-history-sync **  
_Disables full history sync._

** --enable-full-history-sync **  
_Enables full history sync (not just typed URLs) for signed-in users._

** --enable-grouped-history **  
_Enables grouping websites by domain and filtering them by period._

** --homepage **  
_Specifies which page will be displayed in newly-opened tabs. We need this for testing purposes so that the UI tests don't depend on what comes up for http://google.com._

** --host-rules **  
_Comma-separated list of rules that control how hostnames are mapped._

For example:

MAP * 127.0.0.1 → Forces all hostnames to be mapped to 127.0.0.1
MAP *.google.com proxy → Forces all google.com subdomains to be resolved to proxy._
MAP test.com [::1]:77 → Forces test.com to resolve to IPv6 loopback. Will also force the port of the resulting socket address to be 77._
MAP * baz, EXCLUDE www.google.com → Remaps everything to baz, except for www.google.com._
These mappings apply to the endpoint host in a net::URLRequest (the TCP connect and host resolver in a direct connection, and the CONNECT in an http proxy connection, and the endpoint host in a SOCKS proxy connection)._

** --host-resolver-parallelism **  
_The maximum number of concurrent host resolve requests (i.e. DNS) to allow (not counting backup attempts which would also consume threads). ** --host-resolver-retry-attempts must be set to zero for this to be exact. **  
_** --host-resolver-retry-attempts **  
_The maximum number of retry attempts to resolve the host. Set this to zero to disable host resolver retry attempts._

** --hsts-hosts **  
_Takes the JSON-formatted HSTS specification and loads it as if it were a preloaded HSTS entry. Takes precedence over both website-specified rules and built-in rules. The JSON format is the same as that persisted in <profile_dir>/Default/TransportSecurity

** --import **  
_Causes net::URLFetchers to ignore requests for SSL client certificates, causing them to attempt an unauthenticated SSL/TLS session. This is intended for use when testing various service URLs (eg: kPromoServerURL, kInstantURL, kSbURLPrefix,kSyncServiceURL, kWalletServiceUrl, etc.)

** --import-from-file **  
_Performs bookmark importing from an HTML file. The value associated with this setting encodes the file path. It may be used jointly with kImport._

** --incognito **  
_Causes the browser to launch directly in incognito mode._

** --install-from-webstore **  
_Causes Chrome to attempt to get metadata from the webstore for the app/extension ID given, and then prompt the user to download and install it._

** --instant-process **  
_Marks a renderer as an Instant process._

** --instant-url **  
_URL to use for instant. If specified this overrides the url from the TemplateURL._

** --keep-alive-for-test **  
_Used for testing - keeps browser alive after last browser window closes._

** --kiosk **  
_Enable Kiosk mode._

** --kiosk-printing **  
_Print automatically in kiosk mode. 'kKioskMode' must be set as well._

** --limited-install-from-webstore **  
_Causes Chrome to attempt to get metadata from the webstore for the given item, and then prompt the user to download and install it._

** --load-and-launch-app **  
_Loads an app from the specified directory and launches it._

** --load-component-extension **  
_Comma-separated list of directories with component extensions to load._

** --disable-cloud-policy-on-signin **  
_If present, disables the loading and application of cloud policy for signed-in users._

** --load-extension **  
_Loads an extension from the specified directory._

** --load-opencryptoki **  
_Loads the opencryptoki library into NSS at startup. This is only needed temporarily for developers who need to work on WiFi/VPN certificate code._

** --log-net-log **  
_Enables displaying net log events on the command line, or writing the events to a separate file if a file name is given._

** --uninstall-extension **  
_Uninstalls an extension with the specified extension id._

** --managed **  
_Starts the browser in managed mode._

** --make-default-browser **  
_Makes Chrome default browser

** --media-cache-size **  
_Forces the maximum disk space to be used by the media cache, in bytes._

** --memory-profile **  
_Enables dynamic loading of the Memory Profiler DLL, which will trace all memory allocations during the run._

** --message-loop-histogrammer **  
_Enables histograming of tasks served by MessageLoop. See about:histograms/Loop for results, which show frequency of messages on each thread, including APC count, object signalling count, etc._

** --metrics-recording-only **  
_Enables the recording of metrics reports but disables reporting. In contrast to kDisableMetrics, this executes all the code that a normal client would use for reporting, except the report is dropped rather than sent to the server. This is useful for finding issues in the metrics code during UI and performance tests._

** --multi-profiles **  
_Enables multiprofile Chrome._

** --nacl-gdb **  
_Native Client GDB debugger for loader. It needs switches calculated at run time in order to work correctly. That's why NaClLoadCmdPrefix flag can't be used._

** --nacl-gdb-script **  
_GDB script to pass to the nacl-gdb debugger at startup._

** --nacl-loader-cmd-prefix **  
_On POSIX only: the contents of this flag are prepended to the nacl-loader command line. Useful values might be valgrind or xterm -e gdb ** --args. **  
_** --native-messaging-hosts **  
_List of native messaging hosts outside of the default location. Used for tests. The value must be comma-separate lists of key-value pairs separated equal sign. E.g. host1=/path/to/host1/manifest.json,host2=/path/host2.json._

** --net-log-level **  
_Sets the base logging level for the net log. Log 0 logs the most data. Intended primarily for use with ** --log-net-log. **  
_** --no-default-browser-check **  
_Disables the default browser check. Useful for UI/browser tests where we want to avoid having the default browser info-bar displayed._

** --no-displaying-insecure-content **  
_By default, an https page can load images, fonts or frames from an http page. This switch overrides this to block this lesser mixed-content problem._

** --no-events **  
_Don't record/playback events when using record & playback._

** --no-experiments **  
_Disables all experiments set on chrome:flags. Does not disable chrome:flags itself. Useful if an experiment makes chrome crash at startup: One can start chrome with ** --no-experiments, disable the problematic lab at chrome:flags and then restart chrome without this switch again. **  
_** --no-first-run **  
_Skip First Run tasks, whether or not it's actually the First Run. Overridden by kForceFirstRun._

Also drops the First Run beacon so that First Run will not occur in subsequent runs as well._

** --no-js-randomness **  
_Support a separate switch that enables the v8 playback extension. The extension causes javascript calls to Date.now() and Math.random() to return consistent values, such that subsequent loads of the same page will result in consistent js-generated data and XHR requests. Pages may still be able to generate inconsistent data from plugins._

** --no-managed **  
_Starts the browser outside of managed mode._

** --no-network-profile-warning **  
_Whether or not the browser should warn if the profile is on a network share. This flag is only relevant for Windows currently._

** --no-pings **  
_Don't send hyperlink auditing pings

** --no-proxy-server **  
_Don't use a proxy server, always make direct connections. Overrides any other proxy server flags that are passed._

** --no-service-autorun **  
_Disables the service process from adding itself as an autorun process. This does not delete existing autorun registrations, it just prevents the service from registering a new one._

** --no-startup-window **  
_Does not automatically open a browser window on startup (used when launching Chrome for the purpose of hosting background apps)._

** --num-pac-threads **  
_Specifies the maximum number of threads to use for running the Proxy Autoconfig (PAC) script._

** --new-window **  
_When the option to block third-party cookies is enabled, only block third-party cookies from being set._

** --organic **  
_Simulates an organic Chrome install._

** --origin-port-to-force-quic-on **  
_Force use of QUIC for requests over the specified port._

** --pack-extension **  
_Packages an extension to a .crx installable file from a given directory._

** --pack-extension-key **  
_Optional PEM private key to use in signing packaged .crx._

** --parent-profile **  
_Specifies the path to the user data folder for the parent profile._

** --performance-monitor-gathering **  
_Launches PerformanceMonitor at startup, which will gather statistics about Chrome's CPU and memory usage, page load times, startup times, and network usage, and will also store information about events which may be of interest, such as extension-related occurrences and crashes. Optionally, this may be run with an integer value representing the interval between the timed metric gatherings, measured in seconds (if invalid or not provided, the default interval is used)._

** --perform-crash-analysis **  
_Enable the post crash analyzer which uploads detailed crash information in situations where a crash is determined to be particularly interesting._

** --playback-mode **  
_Read previously recorded data from the cache. Only cached data is read. See kRecordMode._

** --pnacl-dir **  
_Overrides the path to the location that PNaCl is installed._

** --ppapi-flash-in-process **  
_Forces the PPAPI version of Flash (if it's being used) to run in the renderer process rather than in a separate plugin process._

** --ppapi-flash-path **  
_Use the PPAPI (Pepper) Flash found at the given path._

** --ppapi-flash-version **  
_Report the given version for the PPAPI (Pepper) Flash. The version should be numbers separated by .s (e.g., 12.3.456.78). If not specified, it defaults to 10.2.999.999._

** --prerender-from-omnibox **  
_Triggers prerendering of pages from suggestions in the omnibox. Only has an effect when Instant is either disabled or restricted to search, and when prerender is enabled._

** --prerender **  
_These are the values the kPrerenderFromOmnibox switch may have, as in ** --prerender-from-omnibox=auto. **  
_auto Allow field trial selection._
disabled No prerendering._
enabled Guaranteed prerendering._
Controls speculative prerendering of pages, and content prefetching. Both are dispatched from elements._

** --print-raster **  
_These are the values the kPrerenderMode switch may have, as in ** --prerender=auto. **  
_auto Allow field trial selection in both prerender and prefetch._
disabled No prerendering or prefetching._
enabled Both prerendering and prefetching._
prefetch_only No prerendering, but enables prefetching._
Enable conversion from vector to raster for any page._

** --product-version **  
_Outputs the product version information and quit. Used as an internal api to detect the installed version of Chrome on Linux._

** --profile-directory **  
_Selects directory of profile to associate with the first browser launched._

** --profiling-at-start **  
_Starts the sampling based profiler for the browser process at startup. This will only work if chrome has been built with the gyp variable profiling=1. The output will go to the value of kProfilingFile._

** --profiling-file **  
_Specifies a location for profiling output. This will only work if chrome has been built with the gyp variable profiling=1. {pid} if present will be replaced by the pid of the process. {count} if present will be incremented each time a profile is generated for this process. The default is chrome-profile-{pid}._

** --profiling-output-file **  
_Specifies a path for the output of task-level profiling which can be loaded and viewed in about:profiler._

** --profiling-flush **  
_Controls whether profile data is periodically flushed to a file. Normally the data gets written on exit but cases exist where chrome doesn't exit cleanly (especially when using single-process). A time in seconds can be specified._

** --promo-server-url **  
_Specifies a custom URL for fetching NTP promo data._

** --prompt-for-external-extensions **  
_Should we prompt the user before allowing external extensions to install? Default is yes._

** --proxy-auto-detect **  
_Forces proxy auto-detection._

** --proxy-bypass-list **  
_Specifies a list of hosts for whom we bypass proxy settings and use direct connections. Ignored if ** --proxy-auto-detect or --no-proxy-server are also specified. This is a comma-separated list of bypass rules. See: net/proxy/proxy_bypass_rules.h for the format of these rules. **  
_** --proxy-pac-url **  
_Uses the pac script at the given URL

** --proxy-server **  
_Uses a specified proxy server, overrides system settings. This switch only affects HTTP and HTTPS requests._

** --purge-memory-button **  
_Adds a Purge memory"button to the Task Manager, which tries to dump as much memory as possible. This is mostly useful for testing how well the MemoryPurger functionality works._

NOTE: This is only implemented for Views._

** --record-stats **  
_Capture resource consumption information through page cycling and output the data to the specified file._

** --record-mode **  
_Chrome supports a playback and record mode. Record mode saves everything to the cache. Playback mode reads data exclusively from the cache. This allows us to record a session into the cache and then replay it at will. See also kPlaybackMode._

** --remote-debugging-frontend **  
_Uses custom front-end URL for the remote debugging._

** --silent-debugger-extension-api **  
_Does not show an infobar when an extension attaches to a page using chrome.debugger page. Required to attach to extension background pages._

** --renderer-print-preview **  
_Enables print preview in the renderer. This flag is generated internally by Chrome and does nothing when directly passed to the browser._

** --reset-local-passphrase **  
_Forces a reset of the local passphrase of the managed user account, and the managed user settings dialog is shown where a new passphrase can be set._

** --reset-variation-state **  
_Forces a reset of the one-time-randomized FieldTrials on this client, also known as the Chrome Variations state._

** --restore-last-session **  
_Indicates the last session should be restored on startup. This overrides the preferences value and is primarily intended for testing. The value of this switch is the number of tabs to wait until loaded before 'load completed' is sent to the ui_test._

** --save-page-as-mhtml **  
_Disable saving pages as HTML-only, disable saving pages as HTML Complete (with a directory of sub-resources). Enable only saving pages as MHTML._

** --safebrowsing-url-prefix **  
_URL prefix used by safebrowsing to fetch hash, download data and report malware._

** --safebrowsing-disable-auto-update **  
_If present, safebrowsing only performs update when SafeBrowsingProtocolManager::ForceScheduleNextUpdate() is explicitly called. This is used for testing only._

** --script-badges **  
_Disables safebrowsing feature that checks download url and downloads content's hash to make sure the content are not malicious._

** --script-bubble **  
_Enable or diable the script bubble icon in the URL bar that tells you how many extensions are running scripts on a page._

** --search-in-omnibox-hint **  
_Enables the showing of an info-bar instructing user they can search directly from the omnibox._

** --set-token **  
_Sets a token in the token service, for testing._

** --show-app-list **  
_If true the app list will be shown._

** --show-autofill-type-predictions **  
_Annotates forms with Autofill field type predictions._

** --show-icons **  
_Makes component extensions appear in chrome://settings/extensions._

** --show-launcher-alignment-menu **  
_If true the alignment of the launcher can be changed._

** --sideload-wipeout **  
_Enables or disables sideload wipeout extension effort._

** --silent-dump-on-dcheck **  
_Changes the DCHECKS to dump memory and continue instead of displaying error dialog. This is valid only in Release mode when ** --enable-dcheck is specified. **  
_** --silent-launch **  
_Causes Chrome to launch without opening any windows by default. Useful if one wishes to use Chrome as an ash server._

** --simulate-upgrade **  
_Simulates an update being available._

** --simulate-critical-update **  
_Simulates a critical update being available._

** --simulate-outdated **  
_Simulates that current version is outdated._

** --socket-reuse-policy **  
_Socket reuse policy. The value should be of type enum ClientSocketReusePolicy._

** --spdy-proxy-auth-origin **  
_Origin for which SpdyProxy authentication is supported._

** --disabled **  
_Speculative resource prefetching._

** --learning **  
_Speculative resource prefetching will only learn about resources that need to be prefetched but will not prefetch them._

** --enabled **  
_Speculative resource prefetching is enabled._

** --ssl-version-max **  
_Specifies the maximum SSL/TLS version (ssl3, tls1, tls1.1, or tls1.2)._

** --ssl-version-min **  
_Specifies the minimum SSL/TLS version (ssl3, tls1, tls1.1, or tls1.2)._

** --start-maximized **  
_Starts the browser maximized, regardless of any previous settings._

** --suggestion-ntp-filter-width **  
_Controls the width of time-of-day filters on the 'suggested' ntp page, in minutes._

** --suggestion-ntp-gaussian-filter **  
_Enables a normal distribution dropoff to the relevancy of visits with respect to the time of day._

** --suggestion-ntp-linear-filter **  
_Enables a linear dropoff to the relevancy of visits with respect to the time of day._

** --sync-invalidate-xmpp-login **  
_Allows insecure XMPP connections for sync (for testing)._

** --sync-keystore-encryption **  
_Enable support for keystore key based encryption._

** --sync-notification-method **  
_Defines the sync notification method, not documented, but I assume either ntp or xmpp - you'll have to look this one up though._

** --sync-notification-host-port **  
_Overrides the default host:port used for sync notifications._

** --sync-url **  
_Overrides the default server used for profile sync._

** --sync-tab-favicons **  
_Enables syncing of favicons as part of tab sync._

** --sync-throw-unrecoverable-error **  
_Makes the sync code to throw an unrecoverable error after initialization. Useful for testing unrecoverable error scenarios._

** --sync-try-ssltcp-first-for-xmpp **  
_Tries to connect to XMPP using SSLTCP first (for testing)._

** --enable-tab-browser-dragging **  
_Enables tab dragging to create a real browser._

** --enable-tab-capture **  
_Enables tab capture._

** --test-name **  
_Passes the name of the current running automated test to Chrome._

** --test-nacl-sandbox **  
_Runs the security test for the NaCl loader sandbox._

** --test-type **  
_Type of the current test harness ("browser" or "ui")._

** --testing-channel **  
_Tells the app to listen for and broadcast testing-related messages on IPC channel with the given ID._

** --track-active-visit-time **  
_Enables tracking the amount of non-idle time spent viewing pages._

** --trusted-spdy-proxy **  
_Disables same-origin check on HTTP resources pushed via a SPDY proxy. The value is the host:port of the trusted proxy._

** --try-chrome-again **  
_Experimental. Shows a dialog asking the user to try chrome. This flag is to be used only by the upgrade process._

** --uninstall **  
_Runs un-installation steps that were done by chrome first-run._

** --use-spdy **  
_Uses Spdy for the transport protocol instead of HTTP. This is a temporary testing flag._

** --use-spelling-suggestions **  
_Disables use of the spelling web service and only provides suggestions. This will only work if asynchronous spell checking is not disabled._

** --max-spdy-sessions-per-domain **  
_Sets the maximum SPDY sessions per domain._

** --max-spdy-concurrent-streams **  
_Sets the maximum concurrent streams over a SPDY session._

** --user-data-dir **  
_Specifies the user data directory, which is where the browser will look for all of its state._

** --use-client-login-signin-flow **  
_Uses the ClientLogin signin flow instead of the web-based signin flow._

** --variations-server-url **  
_Specifies a custom URL for the server which reports variation data to the client. Specifying this switch enables the Variations service on unofficial builds. See variations_service.cc._

** --version **  
_Prints version information and quits._

** --viewer-connection **  
_Requests that Chrome connect to a remote viewer process using an IPC channel of the given name._

** --visit-urls **  
_Cycle through a series of URLs listed in the specified file._

** --wallet-secure-service-url **  
_Secure service URL for Online Wallet service. Used as the base url to escrow credit card numbers._

** --wallet-service-url **  
_Service URL for Online Wallet service. Used as the base url for Online Wallet API calls._

** --whitelisted-extension-id **  
_Enable the "native services" feature of web-intents._

** --window-position **  
_Specify the initial window position: ** --window-position=x,y **  
_** --window-size **  
_Specify the initial window size: ** --window-size=w,h **  
_** --winhttp-proxy-resolver **  
_Uses WinHTTP to fetch and evaluate PAC scripts. Otherwise the default is to use Chromium's network stack to fetch, and V8 to evaluate._

When plugin installation is enabled

** --plugins-metadata-server-url **  
_Specifies a custom URL for fetching plug-ins metadata. Used for testing._

Android specific switches

** --enable-spdy-proxy-auth **  
_Enable SPDY proxy._

** --enable-translate **  
_Pops the translate infobar if possible._

** --tablet-ui **  
_Uses the tablet specific UI components when available._

Chrome OS switches

For use when running Chrome/Chromium on ChromeOS._

** --ash-webui-init **  
_When wallpaper boot animation is not disabled this switch is used to override OOBE/sign in WebUI init type. Possible values: parallel|postpone. Default: parallel._

** --enable-carrier-switching **  
_Enables switching between different cellular carriers from the UI._

** --disable-boot-animation **  
_Disables wallpaper boot animation (except of OOBE case)._

** --disable-drive **  
_Disables Chrome Captive Portal detector, which initiates Captive Portal detection for new active networks._

** --enable-drive-prefetch **  
_Enables file prefetching in Google Drive Client for Chrome OS._

** --disable-login-animations **  
_Avoid doing expensive animations upon login._

** --disable-oobe-animation **  
_Avoid doing animations upon oobe._

** --enable-app-mode **  
_Enable Kiosk app mode for ChromeOS._

** --enable-background-loader **  
_Enables component extension that initializes background pages of certain hosted applications._

** --enable-drive-metadata-prefetch **  
_Enables Chrome Captive Portal detector, which initiates Captive Portal detection for new active networks._

** --enable-touchpad-three-finger-click **  
_Enables touchpad three-finger-click as middle button._

** --enable-touchpad-three-finger-swipe **  
_Enables touchpad three-finger swipe._

** --enable-kiosk-mode **  
_Enable Kiosk mode for ChromeOS._

** --disable-local-accounts **  
_Disable policy-configured local accounts._

** --enable-request-tablet-site **  
_Enables request of tablet site (via user agent override)._

** --enable-static-ip-config **  
_Enables static ip configuration. This flag should be removed when it's on by default._

** --first-boot **  
_Passed to Chrome on first boot. Not passed on restart after sign out._

** --force-login-manager-in-tests **  
_Usually in browser tests the usual login manager bringup is skipped so that tests can change how it's brought up. This flag disables that._

** --has-chromeos-keyboard **  
_If true, the Chromebook has a Chrome OS keyboard. Don't use the flag for Chromeboxes._

** --has-chromeos-diamond-key **  
_If true, the Chromebook has a keyboard with a diamond key._

** --kiosk-mode-screensaver-path **  
_Path for the screensaver used in Kiosk mode

** --login-manager **  
_Enables Chrome-as-a-login-manager behavior._

** --login-screen **  
_Allows to override the first login screen. The value should be the name of the first login screen to show

** --login-screen-size **  
_Controls the initial login screen size. Pass width,height._

** --login-profile **  
_Specifies the profile to use once a chromeos user is logged in._

** --login-user **  
_Specifies the user which is already logged in._

** --login-password **  
_Specifies a password to be used to login (along with login-user)._

** --enable-natural-scroll-default **  
_Enables natural scroll by default._

** --no-discard-tabs **  
_Disables tab discard in low memory conditions, a feature which silently closes inactive tabs to free memory and to attempt to avoid the kernel's out-of-memory process killer._

** --bwsi **  
_Indicates that the browser is in "browse without sign-in" (Guest session) mode. Should completely disable extensions, sync and bookmarks._

** --echo-ext-path **  
_Enables overriding the path for the default echo component extension. Useful for testing._

** --stub-cros-settings **  
_Indicates that a stub implementation of CrosSettings that stores settings in memory without signing should be used, treating current user as the owner. This option is for testing the chromeos build of chrome on the desktop only._

** --auth-ext-path **  
_Enables overriding the path for the default authentication extension._

** --file-manager-packaged **  
_Power of the power-of-2 initial modulus that will be used by the auto-enrollment client. E.g. "4" means the modulus will be 2^4 = 16._

** --oobe-skip-postlogin **  
_Skips all other OOBE pages after user login. In NDebug mode

Posix specific switches

For running on any *nix, ie. Linux, Solaris, OS X, etc._

** --enable-crash-reporter **  
_A flag, generated internally by Chrome for renderer and other helper process command lines on Linux and Mac. It tells the helper process to enable crash dumping and reporting, because helpers cannot access the profile or other files needed to make this decision._

** --password-store **  
_Used for turning on Breakpad crash reporting in a debug environment where crash reporting is typically compiled but disabled._

OS X specific switches

Mac only stuff..._

** --enable-expose-for-tabs **  
_Enables the tabs expose feature

** --keychain-reauthorize **  
_Performs Keychain reauthorization from the command line on behalf of a special Keychain reauthorization stub executable. Used during auto-update._

** --relauncher **  
_A process type (switches::kProcessType) that relaunches the browser. See chrome/browser/mac/relauncher.h._

** --use-mock-keychain **  
_Uses mock keychain for testing purposes, which prevents blocking dialogs from causing timeouts._

Windows specific switches

** --force-immersive **  
_Enables media transfer protocol device media support for mediaGalleries extension API._

** --force-desktop **  
_For the DelegateExecute verb handler to launch Chrome in desktop mode on Windows 8 and higher. Used when relaunching metro Chrome._

** --overlapped-reads **  
_Allows for disabling the overlapped I/O for TCP reads. Possible values are "on" or "off". The default is "on" which matches the existing behavior. "off" switches to use non-blocking reads and WSAEventSelect._

** --relaunch-shortcut **  
_Relaunches metro Chrome on Windows 8 and higher using a given shortcut._

** --wait-for-mutex **  
_Waits for the given handle to be signaled before relaunching metro Chrome on Windows 8 and higher._

NDebug switches

I don't know what NDebug is, so you'll have to look that up._

** --filemgr-ext-path **  
_Enables overriding the path of file manager extension._

** --image-loader-ext-path **  
_Enables overriding the path of image loader extension._

** --dump-profile-graph **  
_Dumps dependency information about our profile services into a dot file in the profile directory._

Print preview in the browser process._

Google Chrome builds only._

** --disable-print-preview **  
_Disables print preview (For testing, and for users who don't like us. :[ )

** --enable-print-preview **  
_Enables print preview (Force enable on Chromium, which normally does not have the PDF viewer required for print preview.)

Base switches
Although it's likely you'll never need these, I've added them for completeness, and Emacs just made short work of extracting them from the source code, so there you go..._

** --debug-on-start **  
_If the program includes base/debug/debug_on_start_win.h, the process will (on Windows only) start the JIT system-registered debugger on itself and will wait for 60 seconds for the debugger to attach to itself. Then a break point will be hit._

** --disable-breakpad **  
_Disables the crash reporting._

** --enable-dcheck **  
_Enable DCHECKs in release mode._

** --full-memory-crash-report **  
_Generates full memory crash dump._

** --noerrdialogs **  
_Suppresses all error dialogs when present._

** --test-child-process **  
_When running certain tests that spawn child processes, this switch indicates to the test framework that the current process is a child process._

** --v **  
_Gives the default maximal active V-logging level; 0 is the default. Normally positive values are used for V-logging levels._

** --vmodule **  
_Gives the per-module maximal V-logging levels to override the value given by ** --v. E.g. my-module=2,foo*=3 would change the logging level for all code in source files my-module.* and foo*.* (-inl suffixes are also disregarded for this matching). **  
_Any pattern containing a forward or backward slash will be tested against the whole pathname and not just the module. E.g., */foo/bar/*=2 would change the logging level for all code in source files under a foo/bar directory._

** --wait-for-debugger **  
_Will wait for 60 seconds for a debugger to come to attach to the process._

** Compilation of Flags / Switches by: **  
Jason Milkins -  https://github.com/jasonm23  
Peter Beverloo - https://github.com/beverloo
