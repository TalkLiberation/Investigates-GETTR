## GETTR
We have statically analyzed the Android application GETTR `com.gettr.gettr` available on [Google Play](https://play.google.com/store/apps/details?id=com.gettr.gettr) in its version `1.3.0`.

### Permissions
This application requests the following permissions:

* `android.permission.INTERNET` have full network access
* `com.sec.android.provider.badge.permission.WRITE` Unknown permission from android reference
* `com.anddoes.launcher.permission.UPDATE_COUNT` Unknown permission from android reference
* `android.permission.VIBRATE` control vibration
* `android.permission.RECEIVE_BOOT_COMPLETED` run at startup
* `android.permission.CAMERA` take pictures and videos
* `com.sec.android.provider.badge.permission.READ` Unknown permission from android reference
* `com.htc.launcher.permission.READ_SETTINGS` Unknown permission from android reference
* `android.permission.READ_EXTERNAL_STORAGE` read the contents of SD card
* `android.permission.ACCESS_NETWORK_STATE` view network connections
* `com.google.android.c2dm.permission.RECEIVE` Unknown permission from android reference
* `com.majeur.launcher.permission.UPDATE_BADGE` Unknown permission from android reference
* `com.oppo.launcher.permission.WRITE_SETTINGS` Unknown permission from android reference
* `com.huawei.android.launcher.permission.READ_SETTINGS` Unknown permission from android reference
* `android.permission.WAKE_LOCK` prevent phone from sleeping
* `com.huawei.android.launcher.permission.WRITE_SETTINGS` Unknown permission from android reference
* `com.huawei.android.launcher.permission.CHANGE_BADGE` Unknown permission from android reference
* `android.permission.ACCESS_WIFI_STATE` view Wi-Fi connections
* `com.htc.launcher.permission.UPDATE_SHORTCUT` Unknown permission from android reference
* `android.permission.REORDER_TASKS` reorder running apps
* `com.gettr.gettr.CountlyPush.BROADCAST_PERMISSION` Unknown permission from android reference
* `android.permission.WRITE_EXTERNAL_STORAGE` modify or delete the contents of SD card
* `android.permission.RECORD_AUDIO` record audio
* `me.everything.badger.permission.BADGE_COUNT_READ` Unknown permission from android reference
* `android.permission.REQUEST_INSTALL_PACKAGES` request install packages
* `com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE` Unknown permission from android reference
* `android.permission.USE_FULL_SCREEN_INTENT` Unknown permission from android reference
* `com.sonyericsson.home.permission.BROADCAST_BADGE` Unknown permission from android reference
* `me.everything.badger.permission.BADGE_COUNT_WRITE` Unknown permission from android reference
* `com.sonymobile.home.permission.PROVIDER_INSERT_BADGE` Unknown permission from android reference
* `android.permission.READ_APP_BADGE` Unknown permission from android reference
* `com.oppo.launcher.permission.READ_SETTINGS` Unknown permission from android reference
* `android.permission.ACCESS_MEDIA_LOCATION` Unknown permission from android reference
* `android.permission.FOREGROUND_SERVICE` run foreground service

### Behavior
By static analysis, it appears that:

* The application probably opens socket *via* the following technical means [^openServerSocket]:
    * `okhttp3/mockwebserver/MockWebServer$3` provided by the company XXXX [^5a16dee55f1eaa2b840599e10db86d32]
    * `okhttp3/mockwebserver/MockWebServer` provided by the company XXXX [^1fa766c6ecf0c4910e9afd0df4d5c7e3]
* The application probably loads JS-capable web views *via* the following technical means [^loadWebview]:
    * `io/flutter/plugins/urllauncher/WebViewActivity` provided by the company XXXX [^d1650d956ae924d3d8f1b138e0768264]
    * `com/bitmovin/player/ui/a` provided by the company XXXX [^22e21a46807f97cd7e67f47dd3a4df0f]
    * `ly/count/android/sdk/ModuleFeedback$2` provided by the company XXXX [^c9495d0672a95c4266e212cbd0cf1003]
    * `zendesk/support/guide/ViewArticleActivity` provided by the company XXXX [^65b75779c5027cad10b52f6c9b30fdc6]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^7b463c2ff7a185d2bbd13743b34122b6]
    * `ly/count/android/sdk/ModuleRatings$4$1` provided by the company XXXX [^9389f730895a932948be4f7acf4089a9]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^e8616736b9e27e7c23c6b699574c1b28]
    * `io/flutter/plugins/webviewflutter/FlutterWebView` provided by the company XXXX [^ef2a2263b517e05a9731ea34f5966a0b]
    * `com/facebook/internal/c0` provided by the company XXXX [^3978cf26e4234243715599552c588037]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/FlutterWebView` provided by the company XXXX [^4841dffbbd7091bd5abc347c8455e3c2]
    * `io/flutter/plugins/webviewflutter/FlutterWebView` provided by the company XXXX [^8f6e7790427967dbb50afd9ff1a7f3b2]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^e8616736b9e27e7c23c6b699574c1b28]
    * `com/bitmovin/player/ui/a` provided by the company XXXX [^d44dc44bf91432ec9cadc16655924e6f]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_browser/InAppBrowserActivity` provided by the company XXXX [^4655233a1ac756e441565c8205821f34]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^5081f1ad68ad449369933bf4c1e61d25]
    * `com/pichillilorenzo/flutter_inappwebview/JavaScriptBridgeInterface$2$1` provided by the company XXXX [^d819fb4801b4bfe7bc4801b25e1aaff9]
    * `com/facebook/internal/k` provided by the company XXXX [^c19a4141f328b1af9138e103240de700]
    * `ly/count/android/sdk/ModuleFeedback$2` provided by the company XXXX [^c9495d0672a95c4266e212cbd0cf1003]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^5578f617513e3ef4b2b765bb662a72c1]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView$10` provided by the company XXXX [^c1a2e8b30103b1c14504182dbb6c8887]
    * `io/flutter/plugins/urllauncher/WebViewActivity$2` provided by the company XXXX [^77acc85386220b4dc169ce2d8ea3a202]
    * `io/flutter/plugins/urllauncher/WebViewActivity$FlutterWebChromeClient$1` provided by the company XXXX [^b87422697df0217f278c83bdb71a0d33]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^39250dde74d1cdcf2821424460cdfb77]
    * `com/bitmovin/player/ui/a` provided by the company XXXX [^ff92313ba1e8edffb711840096a17e4a]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^c689ecc624b35a264f341a2bbbecb47b]
    * `io/flutter/plugins/webviewflutter/FlutterWebView` provided by the company XXXX [^d41c5e359f93f52b5d8a0b944644f7fb]
    * `com/bitmovin/player/ui/CustomMessageHandler$a` provided by the company XXXX [^81946c5ef339a562eb2c65ba80c8da41]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_browser/InAppBrowserActivity$1` provided by the company XXXX [^294d47a5e8bed68b1c2c34d2b237bb37]
    * `io/flutter/plugins/webviewflutter/FlutterWebViewClient$OnNavigationRequestResult` provided by the company XXXX [^0e948ef9c11dd3ea87c92bd06260d410]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^a51081d4e60e822d69bb05e136d781d6]
    * `com/bitmovin/player/ui/a` provided by the company XXXX [^2d0cad82079a6bc0f5e56cbfb2bf11bd]
    * `io/flutter/plugins/urllauncher/WebViewActivity$2` provided by the company XXXX [^5dd09300d88a10bda8c4fb22818ef821]
    * `ly/count/android/sdk/ModuleRatings$4$1` provided by the company XXXX [^9389f730895a932948be4f7acf4089a9]
    * `io/flutter/plugins/webviewflutter/FlutterWebView$FlutterWebChromeClient$1` provided by the company XXXX [^4c9a4c20d8ffe03d25ceca0ef737b811]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^d336ac512fdbb037beab29f850a79703]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/FlutterWebView` provided by the company XXXX [^4841dffbbd7091bd5abc347c8455e3c2]
    * `io/flutter/plugins/webviewflutter/FlutterWebView$FlutterWebChromeClient$1` provided by the company XXXX [^fdb2233c7c5e24806519c3d57dbf414c]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^da3d86654c86a7b140771171490b8609]
    * `com/pichillilorenzo/flutter_inappwebview/content_blocker/ContentBlockerHandler$2` provided by the company XXXX [^33a82bb7fc6d9ae9fb89c2bb8a39b8ea]
    * `com/facebook/internal/c0` provided by the company XXXX [^3978cf26e4234243715599552c588037]
    * `io/flutter/plugins/urllauncher/WebViewActivity$FlutterWebChromeClient$1` provided by the company XXXX [^2b9592930fcfab35079857d32bf30967]
    * `io/flutter/plugins/urllauncher/WebViewActivity` provided by the company XXXX [^d1650d956ae924d3d8f1b138e0768264]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebViewClient` provided by the company XXXX [^c689ecc624b35a264f341a2bbbecb47b]
    * `io/flutter/plugins/webviewflutter/FlutterWebView` provided by the company XXXX [^0eb1db73cb0d10032a2071f1fffe2f25]
    * `io/flutter/plugins/webviewflutter/FlutterWebViewClient$OnNavigationRequestResult` provided by the company XXXX [^0e948ef9c11dd3ea87c92bd06260d410]
    * `com/pichillilorenzo/flutter_inappwebview/in_app_webview/InAppWebView` provided by the company XXXX [^5578f617513e3ef4b2b765bb662a72c1]
* The application probably dynamically loads code *via* the following technical means [^loadExternalCode]:
    * `com/gyf/immersionbar/l` provided by the company XXXX [^53c3d24a7fa9249809ff941e8f1329db]
    * `com/google/android/gms/dynamite/DynamiteModule` provided by the company XXXX [^f6c91f3efd0661cab5cec1e6718de11b]
    * `com/facebook/z/s/g` provided by the company XXXX [^334731336fa82ea0bfa52e50ee41945f]
    * `com/google/android/gms/dynamite/DynamiteModule` provided by the company XXXX [^085bdf0595b28728b9b3d47084d8e31a]
    * `kotlin/o0/a0/d/o$a$d` provided by the company XXXX [^0554bbb29027ec7cb0d029da44c3b31b]
    * `kotlin/o0/a0/d/m0/c/m1/b/a` provided by the company XXXX [^3fc2e3134fa7013b3ffe33b9210fcc62]
    * `h/n/a/d/c/c` provided by the company XXXX [^95352b8ff6e5e4e09e4522983f479bc2]
    * `kotlin/g0/j/a/i` provided by the company XXXX [^cbc924f442c0a3d76d82a410c9214e4a]
    * `com/gyf/immersionbar/l` provided by the company XXXX [^08017a14a9ed30e923c2d0c4130a1268]
    * `com/google/android/gms/dynamite/DynamiteModule` provided by the company XXXX [^315dc05986856cc605da8d3a1375d092]
    * `com/google/android/gms/common/l/a` provided by the company XXXX [^afd222b062d81c9c85a767051d9506f1]
    * `kotlin/o0/a0/d/j` provided by the company XXXX [^b7a29ebbd98cb497210e853383e56448]
    * `com/google/android/gms/dynamite/DynamiteModule` provided by the company XXXX [^944e659661ecee36b4ebc727fe7a0d1f]
    * `com/gyf/immersionbar/l` provided by the company XXXX [^d9bc495ccc3d57cef5f4c461de59dd58]
    * `androidx/appcompat/widget/w$d` provided by the company XXXX [^c5582d199b27032c41d2099fef55cddb]
    * `com/google/android/gms/measurement/internal/e3` provided by the company XXXX [^cf1a9258e5bc0c911ee2b46edad9236a]
    * `com/google/android/gms/dynamite/DynamiteModule` provided by the company XXXX [^9cde6feb641cd681932d48e3efea4279]
    * `com/google/android/material/internal/i` provided by the company XXXX [^3fb8a87107d6de87959d43348f7b1d6d]
    * `com/appsflyer/internal/bt` provided by the company XXXX [^7cee4b649e6b988e34612aadc219c4b1]
    * `com/google/android/gms/cloudmessaging/f` provided by the company XXXX [^4c8241105ae51df70c4c216ecfa9e3b0]
* The application probably gets different information regarding the telephony capabilities *via* the following technical means [^readTelephonyInfo]:
    * `ly/count/android/sdk/DeviceInfo` provided by the company XXXX [^5fe0818afed86f9f77515a9fe9efa13b]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `h/d/a/t` provided by the company XXXX [^b3fb250d95991f061f9e198edd717709]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `h/d/a/t` provided by the company XXXX [^b3fb250d95991f061f9e198edd717709]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `com/google/android/datatransport/cct/d` provided by the company XXXX [^280629040473128c660f4071cb0f6934]
    * `com/google/android/exoplayer2/z2/r0` provided by the company XXXX [^c5caf5a5ec725be671e7ceeac46eb912]
    * `h/t/a/a` provided by the company XXXX [^c25337aab1b5a6e6207b7c891112749f]
    * `com/bitmovin/android/exoplayer2/c2/n0` provided by the company XXXX [^0b312a1272f70101981f1a36cb6393f8]
* The application probably gets the location based on GPS and/or Wi-Fi *via* the following technical means [^readLocation]:
    * `androidx/appcompat/app/l` provided by the company XXXX [^e2132945b87cf77c7c3661e2c646345f]
    * `com/appsflyer/internal/ai` provided by the company XXXX [^c1fc8395973a2461ba354729d185741d]
    * `androidx/appcompat/app/l` provided by the company XXXX [^e2132945b87cf77c7c3661e2c646345f]
    * `com/appsflyer/internal/ai` provided by the company XXXX [^c1fc8395973a2461ba354729d185741d]
    * `androidx/appcompat/app/l` provided by the company XXXX [^61a04737acc1b517f82df6cbb097163e]
    * `com/appsflyer/internal/x` provided by the company XXXX [^270291e0748f33557e369c249a31b236]
* The application probably gets the network connections information *via* the following technical means [^readNetworkInfo]:
    * `com/google/firebase/messaging/SyncTask` provided by the company XXXX [^785ad2af9a2852f101a56319031e556d]
    * `ly/count/android/sdk/CrashDetails` provided by the company XXXX [^1d8407e7d363261ceef53e0cf8ccc1d2]
    * `zendesk/core/ZendeskNetworkInfoProvider` provided by the company XXXX [^e01ce3a097d8bf0a79fe6b14ec78ea6b]
    * `com/google/android/gms/measurement/internal/y4` provided by the company XXXX [^102d402f068c107080f1d5660b01aa91]
    * `com/bitmovin/player/offline/service/k` provided by the company XXXX [^ee62f57ac82e79d792f35d17a9df9457]
    * `zendesk/core/ZendeskNetworkInfoProvider` provided by the company XXXX [^66213d0a3ad3019a3783a3f04038234e]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `com/squareup/picasso/i$c` provided by the company XXXX [^b6aff93651566f75ac008bef6e40692d]
    * `io/flutter/plugins/connectivity/Connectivity` provided by the company XXXX [^eb1fc426e0ef91a0c15bfc8f1cfe73fd]
    * `org/getter/bridge/larix/c` provided by the company XXXX [^658824dec0028e0fd135bf40d32eee88]
    * `com/bitmovin/android/exoplayer2/scheduler/Requirements` provided by the company XXXX [^5dac6a9d55e9b9d84fdf6ac0bd5991f0]
    * `io/sentry/android/core/util/ConnectivityChecker` provided by the company XXXX [^32cce924e9ecf099d1b382bd1896d3c4]
    * `com/squareup/picasso/i` provided by the company XXXX [^15dc49803492c3c6fe138db794ab59f2]
    * `com/bumptech/glide/manager/DefaultConnectivityMonitor` provided by the company XXXX [^dbc8db33e6d74316799deb8fdd9c349c]
    * `com/google/android/gms/measurement/internal/t3` provided by the company XXXX [^c920139545877eded9b825f0dade35ef]
    * `zendesk/core/NetworkUtils` provided by the company XXXX [^a25a7647783319f572a8bb84d31768a1]
    * `com/google/android/exoplayer2/z2/b0` provided by the company XXXX [^c3a56222190e3dce1f1cfdf1daa35a7d]
    * `com/banuba/sdk/a/c/e` provided by the company XXXX [^e2177d09c88ef1a0a1cf665f7c1ce705]
    * `com/google/firebase/crashlytics/internal/common/CommonUtils` provided by the company XXXX [^5adb1780ee7fbc6e715ec3e30770a4bb]
    * `com/google/android/datatransport/cct/d` provided by the company XXXX [^280629040473128c660f4071cb0f6934]
    * `com/google/firebase/messaging/TopicsSyncTask` provided by the company XXXX [^1705b1036740617a3bbbca2110b13f93]
    * `com/google/android/datatransport/runtime/scheduling/jobscheduling/t` provided by the company XXXX [^9dfcf164c294dcb00368ce12dbd58968]
    * `io/sentry/android/core/util/ConnectivityChecker` provided by the company XXXX [^bcc1028e4c42f15391a6fb83771c8041]
    * `com/google/android/exoplayer2/scheduler/Requirements` provided by the company XXXX [^f4988c36a3625a70996e38d8cedd41df]
    * `zendesk/support/guide/NetworkUtils` provided by the company XXXX [^e62f8abb9375ed220212dc9ee5064f89]
    * `com/bitmovin/android/exoplayer2/c2/n0` provided by the company XXXX [^0bf1cac28ceb2b981fcf111e173682ff]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `d/i/k/a` provided by the company XXXX [^de0fb94acdbdb4c22791834523b23915]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
    * `com/appsflyer/internal/ai` provided by the company XXXX [^84eb1005faba38c105a6285693caf5b3]
    * `com/appsflyer/internal/u` provided by the company XXXX [^be42a4aa0c9c7ca8741f2f5ec3c4c134]
* The application probably gets network interfaces addresses (IP and/or MAC) *via* the following technical means [^readNetworkAddresses]:
    * `com/appsflyer/internal/ai` provided by the company XXXX [^84eb1005faba38c105a6285693caf5b3]
    * `okhttp3/mockwebserver/MockWebServer$4` provided by the company XXXX [^fc9a185c9a99819ab63c668321d7196c]
    * `okhttp3/mockwebserver/MockWebServer` provided by the company XXXX [^7a1227a5ca0e29de4945dad31832fe52]
    * `okhttp3/mockwebserver/MockWebServer$4` provided by the company XXXX [^13224f2135f1c5949202c60e49601558]
    * `okhttp3/mockwebserver/MockWebServer` provided by the company XXXX [^0575555de499beda9d2cf1f2899b89e4]
    * `okhttp3/internal/Util` provided by the company XXXX [^5e2f41d491cda87074679a245ea29b7e]
* The application probably uses cryptography *via* the following technical means [^useCrypto]:
    * `com/bitmovin/android/exoplayer2/source/hls/d` provided by the company XXXX [^9ff1d152ccff6fa058b44d8ad92133da]
    * `s/b` provided by the company XXXX [^f03f4123f52a9abb5942e20d1d0b997a]
    * `com/google/android/exoplayer2/source/hls/d` provided by the company XXXX [^5009bd63d15c95375372c1e492986b31]
    * `s/b` provided by the company XXXX [^f03f4123f52a9abb5942e20d1d0b997a]
    * `com/bitmovin/android/exoplayer2/source/hls/d` provided by the company XXXX [^0e1265d3ecd05705142bb42620c9bc90]
    * `com/bitmovin/android/exoplayer2/upstream/o0/o$b` provided by the company XXXX [^119bfe22ed14cc3ef94609804ef1a304]
    * `com/google/android/exoplayer2/source/hls/d` provided by the company XXXX [^7126d50e35c6c38f4f344dc92156f3f0]
    * `com/bitmovin/android/exoplayer2/upstream/o0/o$b` provided by the company XXXX [^d606701b5dabba7ae512f454002ee725]
    * `s/b` provided by the company XXXX [^026a98f4db36f8ce8747a59d8c089c79]
* The application probably uses reflection *via* the following technical means [^useReflection]:
    * `com/google/firebase/database/core/utilities/encoding/CustomClassMapper$BeanMapper` provided by the company XXXX [^ee8079deb5f2a58485efc001e38007d1]
    * `com/google/firebase/database/core/utilities/encoding/CustomClassMapper$BeanMapper` provided by the company XXXX [^ee8079deb5f2a58485efc001e38007d1]
    * `com/google/gson/internal/reflect/PreJava9ReflectionAccessor` provided by the company XXXX [^79869d92c67ae12b9e5c190c1ab9e894]
    * `com/google/gson/internal/reflect/UnsafeReflectionAccessor` provided by the company XXXX [^b61d13ff5e5b1610d1eb9dba62a39cd3]
* The application probably uses the phone sensors *via* the following technical means [^useSensors]:
    * `com/appsflyer/internal/ab$3` provided by the company XXXX [^29697fdbbddcd21fce93baf85ab9d8c6]
    * `com/appsflyer/internal/c$d` provided by the company XXXX [^295331c815f28aeb873ea631510269c0]
    * `com/google/android/exoplayer2/video/spherical/SphericalGLSurfaceView` provided by the company XXXX [^6a8096b24473cafd21b24a016a682165]
    * `com/google/firebase/crashlytics/internal/common/CommonUtils` provided by the company XXXX [^e3c0746ed3dd8a43edd300483f467c31]
    * `com/bitmovin/android/exoplayer2/ui/spherical/SphericalGLSurfaceView` provided by the company XXXX [^c2373c56abd241b5368ab30e5a8e8fe4]
    * `com/facebook/z/r/b` provided by the company XXXX [^5f76814231dea690138f04a114bd5842]
    * `com/bitmovin/player/v/k/a` provided by the company XXXX [^cf77b122427726b313ee7fa4825b6823]
    * `io/sentry/android/core/TempSensorBreadcrumbsIntegration` provided by the company XXXX [^4b60dfe9f7e25a1f4123d98fa48929d8]
    * `com/appsflyer/internal/ab$3` provided by the company XXXX [^29697fdbbddcd21fce93baf85ab9d8c6]
    * `com/bitmovin/player/v/k/a` provided by the company XXXX [^5b9ae3bb83c39cd0dbda81574c2c1dd4]
    * `com/facebook/z/r/b` provided by the company XXXX [^5f76814231dea690138f04a114bd5842]
    * `com/google/android/exoplayer2/video/spherical/SphericalGLSurfaceView` provided by the company XXXX [^65b93894d57fa9ef7998938018a3769e]
    * `com/bitmovin/android/exoplayer2/ui/spherical/SphericalGLSurfaceView` provided by the company XXXX [^5b13b1c894787df5f1241db57b79212b]
    * `io/sentry/android/core/TempSensorBreadcrumbsIntegration` provided by the company XXXX [^4b60dfe9f7e25a1f4123d98fa48929d8]
* The application probably plays sound *via* the following technical means [^playSound]:
    * `androidx/appcompat/app/e` provided by the company XXXX [^b7d2f2b371168c9c46dc79e23f3aed04]
* The application probably makes OS calls *via* the following technical means [^doOsCalls]:
    * `d/i/h/h` provided by the company XXXX [^30a8ea666bb56766bedaef480fc2578f]
    * `com/facebook/soloader/SysUtil$LollipopSysdeps` provided by the company XXXX [^2ba3a87efdaf192814dc91770e68ebfa]
    * `d/i/h/h` provided by the company XXXX [^30a8ea666bb56766bedaef480fc2578f]
    * `d/i/h/h` provided by the company XXXX [^30a8ea666bb56766bedaef480fc2578f]
    * `com/facebook/soloader/SysUtil$LollipopSysdeps` provided by the company XXXX [^b0c397868b5b3b069d219d85c58088a8]
* The application probably sends data over UDP protocol *via* the following technical means [^sendDataUdp]:
    * `com/google/android/exoplayer2/z2/j0` provided by the company XXXX [^19cddcb03be5af18afef4010e9774a83]
    * `com/bitmovin/player/m/k0/k/c` provided by the company XXXX [^ed4b2fc1a2aa0783603c55ccb89f545f]
    * `com/bitmovin/android/exoplayer2/c2/f0` provided by the company XXXX [^3adc3403e348fd85296b4fcfe97f5101]
* The application probably receives data over UDP protocol *via* the following technical means [^receiveDataUdp]:
    * `com/google/android/exoplayer2/z2/j0` provided by the company XXXX [^19cddcb03be5af18afef4010e9774a83]
    * `com/bitmovin/player/m/k0/k/c` provided by the company XXXX [^ed4b2fc1a2aa0783603c55ccb89f545f]
    * `com/bitmovin/android/exoplayer2/c2/f0` provided by the company XXXX [^3adc3403e348fd85296b4fcfe97f5101]
    * `com/bitmovin/android/exoplayer2/upstream/n0` provided by the company XXXX [^c3762f4e1d129e95a1988f571f1babaf]
    * `com/google/android/exoplayer2/y2/j0` provided by the company XXXX [^fc69c3bc5f372d96b426c78c4befce57]
* The application probably opens the camera *via* the following technical means [^useCamera]:
    * `io/flutter/plugins/camera/Camera` provided by the company XXXX [^6e5586a8b5556227db309f735fdf31bd]
    * `com/banuba/android/sdk/camera/Camera2` provided by the company XXXX [^a9d2c2e0be30a4d2e25b999a6be81d53]
    * `h/b0/a/e0` provided by the company XXXX [^e1969beaaa04813769783d6ad78c6b1a]
* The application probably sends data over HTTP/S *via* the following technical means [^sendDataHttp]:
    * `io/sentry/transport/HttpConnection` provided by the company XXXX [^f0d85fbea563e6c3d136d280f5e63ded]
    * `com/google/firebase/installations/remote/FirebaseInstallationServiceClient` provided by the company XXXX [^29053cfeb33ea5482a03c8548afa173f]
    * `com/appsflyer/internal/am` provided by the company XXXX [^c6983615f2e39165be69df951fd0ba0e]
    * `h/l/a/b/d/b/b$b` provided by the company XXXX [^6ce1692b7553b30c537241e7ddb2b880]
    * `com/airbnb/lottie/w/b` provided by the company XXXX [^56f84080e47c035c959ed23e715ec11b]
    * `com/bitmovin/android/exoplayer2/upstream/w` provided by the company XXXX [^3fc3c278e6097a569204566ce9ae7808]
    * `com/google/firebase/installations/remote/FirebaseInstallationServiceClient` provided by the company XXXX [^8f9c23292bf505cf3d91b41ed3f0753f]
    * `com/google/firebase/installations/remote/FirebaseInstallationServiceClient` provided by the company XXXX [^403550b393109062146184af0edb0b20]
    * `com/appsflyer/internal/bv` provided by the company XXXX [^f0da5a507a64edb99f33c8ef28ab79f3]
    * `com/appsflyer/internal/ah` provided by the company XXXX [^4bd7effe9045918e47a34fe058b62a72]
    * `com/google/android/datatransport/cct/d` provided by the company XXXX [^7c8d968bc325f7350b3cb8566a4ab734]
    * `com/bitmovin/player/m/f$a` provided by the company XXXX [^5c2baedb67a6ab33028a653ee6fc3e44]
    * `com/facebook/GraphRequest` provided by the company XXXX [^c699f438302e67a08866c993e0e36465]
    * `com/appsflyer/internal/ai` provided by the company XXXX [^ef4f5eda488177361d343a6818f8560b]
    * `ly/count/android/sdk/ConnectionProcessor` provided by the company XXXX [^f625e4d5196fbc0df2f890fdf611837e]
    * `com/google/android/exoplayer2/y2/v` provided by the company XXXX [^7d9364d87ec144f072fdbca078bad9b4]
    * `com/appsflyer/internal/bj` provided by the company XXXX [^362db744ced4a12ddd220def8ae9dace]
    * `com/example/r_upgrade/common/UpgradeService$b` provided by the company XXXX [^ace27a987c7b28287c727731ae17158b]
    * `io/sentry/transport/HttpConnection` provided by the company XXXX [^f0d85fbea563e6c3d136d280f5e63ded]
    * `h/l/a/b/d/b/b$b` provided by the company XXXX [^6ce1692b7553b30c537241e7ddb2b880]
    * `com/facebook/imagepipeline/producers/x` provided by the company XXXX [^803d4286458f27cc3d30f3e3d1df698b]
    * `com/bitmovin/android/exoplayer2/upstream/w` provided by the company XXXX [^3fc3c278e6097a569204566ce9ae7808]
    * `com/bitmovin/player/m/g` provided by the company XXXX [^cc26f11dac8699988d9886376d84c885]
    * `com/google/android/datatransport/cct/d` provided by the company XXXX [^7c8d968bc325f7350b3cb8566a4ab734]
    * `com/facebook/GraphRequest` provided by the company XXXX [^39759de375ce11f441971abed075b742]
    * `com/facebook/GraphRequest` provided by the company XXXX [^7dce79ec99cec534ec4cde81378fd4ef]
    * `ly/count/android/sdk/ConnectionProcessor` provided by the company XXXX [^f625e4d5196fbc0df2f890fdf611837e]
    * `com/google/android/exoplayer2/y2/v` provided by the company XXXX [^7d9364d87ec144f072fdbca078bad9b4]
    * `com/example/r_upgrade/common/UpgradeService$b` provided by the company XXXX [^ace27a987c7b28287c727731ae17158b]
* The application probably starts another application *via* the following technical means [^startAnotherApp]:
    * `com/google/firebase/messaging/CommonNotificationBuilder` provided by the company XXXX [^64f67d74ad8f27b289f238d4cb841adb]
    * `ly/count/android/sdk/Countly` provided by the company XXXX [^f6f320efffec6fac183e53f1b98672ed]
    * `x/a/a/c` provided by the company XXXX [^f26ed3a7105d7a45e88a7aae730a9017]
    * `ly/count/android/sdk/messaging/CountlyPush` provided by the company XXXX [^48393b7542c097df36876f1095fcd0e6]
    * `com/dexterous/flutterlocalnotifications/FlutterLocalNotificationsPlugin` provided by the company XXXX [^cb9b8d97babd4ed62783b5cc41500b4f]
* The application probably executes OS commands *via* the following technical means [^execCommand]:
    * `com/banuba/sdk/ve/domain/a` provided by the company XXXX [^d0a469b6c4155a9a133b3ab99dce0a6c]
    * `io/sentry/android/core/util/RootChecker` provided by the company XXXX [^4c5f023c2850add8f8aa39cc95c728e8]
* The application probably records sound *via* the following technical means [^recordAudio]:
    * `com/banuba/sdk/veui/ui/d0/a` provided by the company XXXX [^89113233ddc35a1303a604ad41909881]
    * `h/b0/a/j` provided by the company XXXX [^8626fd38b81777c6a4e315cf3a74816f]
    * `com/banuba/sdk/core/encoding/d$d` provided by the company XXXX [^ba28a442e48384418196b89a9e75ab66]
    * `com/banuba/sdk/core/encoding/d$d$a` provided by the company XXXX [^d3b2e43e31a82b5ebf01d96c5f3ef6fd]
    * `h/b0/a/j` provided by the company XXXX [^03d561289427a4dcaa0983211644ec1e]
    * `com/banuba/sdk/core/encoding/d$d` provided by the company XXXX [^ba28a442e48384418196b89a9e75ab66]
    * `com/banuba/sdk/veui/ui/d0/a$c` provided by the company XXXX [^e1238642ad1d6ec4e98c4b59d712f370]
* The application probably records media (audio and/or video *via* the following technical means [^recordVideo]:
    * `io/flutter/plugins/camera/Camera` provided by the company XXXX [^6abe00924930a74fd42528b2a3899b07]
    * `io/flutter/plugins/camera/media/MediaRecorderBuilder` provided by the company XXXX [^b01f084b2b9109ed18f209b4426125fc]
* The application probably gets memory and CPU information *via* the following technical means [^readRuntimeInfo]:
    * `com/getter/video/edit/l/a` provided by the company XXXX [^f8678a0fb8b2fe03618940e22270fcb5]
    * `org/gsuite/flutter_gtv_image/image/e` provided by the company XXXX [^1989887538cbeb3d9d8a0023c306f3fa]
    * `com/banuba/sdk/core/HardwareCapabilitiesDetector` provided by the company XXXX [^79200aa88df9284998a5a6fd52f6fb54]
    * `org/getter/g/b` provided by the company XXXX [^f1839f1ab2649805e56772c96d3b514d]
    * `y/z` provided by the company XXXX [^b53c0be478020a950b37c1c42b176047]
    * `com/google/firebase/crashlytics/internal/common/CrashlyticsController` provided by the company XXXX [^fdd0e0c8524dafca71574a5bcee5f34a]
    * `h/x/b/a` provided by the company XXXX [^026eb81f3608194b38f86e67062d7824]
    * `kotlinx/coroutines/internal/d0` provided by the company XXXX [^e81a312cc28277d05d1d6a620f88af50]
    * `h/n/d/a/c/j` provided by the company XXXX [^0ba9e1df551cac4e3cfd986376f1ef13]
    * `com/bumptech/glide/load/engine/executor/RuntimeCompat` provided by the company XXXX [^eb9cde63fd406d4f331ad041b2b58054]
    * `h/l/a/b/e/a` provided by the company XXXX [^2e473afff55aaf8c9b2afd2f5f62be7a]
    * `com/banuba/sdk/gallery/ui/l$g` provided by the company XXXX [^d3de275e309287a3b38483ab2136642f]
    * `com/facebook/imagepipeline/memory/m` provided by the company XXXX [^42ac93bb2c78643287a0675ca7d9be48]
    * `com/google/firebase/crashlytics/internal/common/CrashlyticsReportDataCapture` provided by the company XXXX [^aee247f930b05abdc214e962acf04faf]
    * `com/facebook/internal/a0` provided by the company XXXX [^90dc9bc61be4dbd5e73df9ca3b647d98]
    * `f/a` provided by the company XXXX [^d97b57b26c925b46e39a594beb13271f]
    * `kotlinx/coroutines/a0` provided by the company XXXX [^3094b886c15f3e2868565a2fc63d8b51]
    * `ly/img/android/pesdk/ui/utils/a` provided by the company XXXX [^493e5a1317633f9ed82aca23d2662976]
    * `com/facebook/j0/d/l` provided by the company XXXX [^8473724cb222f118cc756b6cdd1bfa3e]
    * `ly/img/android/pesdk/utils/k0` provided by the company XXXX [^22b37f2b78813156fc69f06a0d54da27]
    * `com/facebook/imagepipeline/memory/d` provided by the company XXXX [^8935fd1f895c97044cfda28af5ee316c]
    * `com/facebook/imagepipeline/memory/n` provided by the company XXXX [^95d755d39af20583d5b1a07397e2c198]
    * `com/facebook/imagepipeline/memory/n` provided by the company XXXX [^e064f212d46fae345854fd16c2745a34]
    * `ly/img/android/pesdk/ui/utils/a` provided by the company XXXX [^493e5a1317633f9ed82aca23d2662976]
    * `com/facebook/imagepipeline/memory/k` provided by the company XXXX [^4ec931cedc1d62726022584a1a90f0bd]
    * `io/sentry/android/core/DefaultAndroidEventProcessor` provided by the company XXXX [^a5c3455f559199a75c459698b8a7c31c]
    * `ly/img/android/pesdk/ui/utils/a` provided by the company XXXX [^493e5a1317633f9ed82aca23d2662976]
* The application probably creates an accessibility service *via* the following technical means [^createAccessibilityService]:
    * `io/flutter/view/AccessibilityBridge$4` provided by the company XXXX [^10b0ce7f2adf1ba37bbaf970d5acd300]
    * `com/google/android/material/slider/BaseSlider` provided by the company XXXX [^bb93bf4c26fc46126ab7b12f83741593]
    * `androidx/recyclerview/widget/RecyclerView` provided by the company XXXX [^9c23f2ba203bb60d4221f6fb09a901ab]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^f9b9b83d4558f441f56c303e10cdbf14]
    * `d/k/a/a` provided by the company XXXX [^3bcebfcf93073ef663c23657d0167245]
    * `androidx/appcompat/widget/i0` provided by the company XXXX [^3707b4a81714c452dd82600c89e5306f]
    * `d/k/a/a` provided by the company XXXX [^75197c9a4596d55b74020173eb7c09da]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0fb2c8ba44ce41429bb983762ac920aa]
    * `d/k/a/a` provided by the company XXXX [^f1b8e9eb2f659442be5aba5b80f9c0ba]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
    * `d/k/a/a` provided by the company XXXX [^aee49a929061486f87dcc7de9c2df330]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0d0c774a17418d04884391cd41468a39]
    * `com/google/android/material/textfield/d$a` provided by the company XXXX [^b4b22d1f74a7ad7c15a9aa7bf9646339]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^49835ca6ac924b9ed75fb89449ffa863]
    * `io/flutter/view/AccessibilityBridge$2` provided by the company XXXX [^6a29e4f19be7c76870a55bbc71c9c8f5]
    * `com/google/android/material/textfield/MaterialAutoCompleteTextView` provided by the company XXXX [^4e00e0fc297ef9c7e0b7ae929ef7cba5]
    * `d/k/a/a` provided by the company XXXX [^aee49a929061486f87dcc7de9c2df330]
    * `d/k/a/a` provided by the company XXXX [^75197c9a4596d55b74020173eb7c09da]
    * `com/google/android/material/timepicker/c` provided by the company XXXX [^e5d1341df5f1d2788fb3fd299cd110b3]
    * `androidx/appcompat/widget/i0` provided by the company XXXX [^3707b4a81714c452dd82600c89e5306f]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^5a3c3e2d546447067ed1058b89da02a0]
    * `com/google/android/material/snackbar/Snackbar` provided by the company XXXX [^4c2d7b3644e6190975478b202d9b1249]
    * `com/google/android/material/textfield/d$d` provided by the company XXXX [^4ce3587911f63d5c5250787cbda9a936]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `zendesk/belvedere/l` provided by the company XXXX [^59e55794c58143d9bd60a189d9216fe8]
    * `com/google/android/material/snackbar/BaseTransientBottomBar` provided by the company XXXX [^fc9c5f7bfbdc0718718ddf5679d4f0da]
    * `com/google/android/material/snackbar/Snackbar` provided by the company XXXX [^4c2d7b3644e6190975478b202d9b1249]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0086b7438d906caaa04aa43e182ddd55]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0086b7438d906caaa04aa43e182ddd55]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6536115025cf28aa5eedbbf1320f490a]
* The application probably listens accessibility events *via* the following technical means [^listenAccessibilityEvents]:
    * `androidx/appcompat/widget/SwitchCompat` provided by the company XXXX [^f4f4d47ec8718d4542790b8cc6868218]
    * `androidx/viewpager2/widget/ViewPager2$j` provided by the company XXXX [^b3ab42bb1d646309428a6e0f65044d6a]
    * `androidx/drawerlayout/widget/DrawerLayout$b` provided by the company XXXX [^ae06e08a969706e5ace5e2d71fd778c0]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `com/google/android/material/button/MaterialButton` provided by the company XXXX [^cd32530947a61228cdef7e37db9469bd]
    * `androidx/appcompat/widget/ActionBarContextView` provided by the company XXXX [^387ee15faf974132074e96aac4696140]
    * `androidx/slidingpanelayout/widget/SlidingPaneLayout$a` provided by the company XXXX [^b582d39a2131ff17544d4c5699bc3ce1]
    * `com/google/android/material/card/MaterialCardView` provided by the company XXXX [^1896537b6182835a96104e1e59340717]
    * `androidx/core/widget/NestedScrollView$a` provided by the company XXXX [^0330e38896710bdc44950b4df747777f]
    * `androidx/appcompat/widget/AppCompatButton` provided by the company XXXX [^b902f7d7ba3dd130264748294a133360]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `com/bitmovin/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^5a76c1b498380c61f8b7877d882fe8ae]
    * `androidx/appcompat/widget/LinearLayoutCompat` provided by the company XXXX [^84ea0d1bd0d5c77e6db723f95140025e]
    * `androidx/appcompat/widget/ScrollingTabContainerView$d` provided by the company XXXX [^3fa4a9882fa5acffeef3f9bab2ebe183]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `com/google/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^e41b523b7fd6fd78afbb593513bb15e5]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `com/bitmovin/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^5a76c1b498380c61f8b7877d882fe8ae]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/drawerlayout/widget/DrawerLayout$b` provided by the company XXXX [^18a034a45a443489ddd843b3b3d8fd82]
    * `io/flutter/view/AccessibilityBridge$1` provided by the company XXXX [^262330ed42d16970529b0f77fb62a62a]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^be10b35f4e03c4452eafcb4c238584c2]
    * `com/google/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^e41b523b7fd6fd78afbb593513bb15e5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^40eb0cd93b972c44100e7f3c0f2a9b6d]
    * `androidx/appcompat/widget/SwitchCompat` provided by the company XXXX [^15fa855ac02a9c7b256d4606f262096a]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `androidx/core/widget/NestedScrollView$a` provided by the company XXXX [^0330e38896710bdc44950b4df747777f]
    * `androidx/recyclerview/widget/RecyclerView$p` provided by the company XXXX [^7281fcadcabab1482540022b58d000a6]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `androidx/recyclerview/widget/RecyclerView$p` provided by the company XXXX [^7281fcadcabab1482540022b58d000a6]
    * `com/bitmovin/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^5a76c1b498380c61f8b7877d882fe8ae]
    * `androidx/appcompat/widget/ActionBarContextView` provided by the company XXXX [^387ee15faf974132074e96aac4696140]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `androidx/viewpager/widget/ViewPager` provided by the company XXXX [^3ce57373e05ffb147498469ece6b2366]
    * `androidx/drawerlayout/widget/DrawerLayout$b` provided by the company XXXX [^18a034a45a443489ddd843b3b3d8fd82]
    * `com/google/android/exoplayer2/ui/DefaultTimeBar` provided by the company XXXX [^e41b523b7fd6fd78afbb593513bb15e5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^6fba231545a8f9b50c613228989581d3]
    * `com/google/android/material/textfield/d$d` provided by the company XXXX [^4ce3587911f63d5c5250787cbda9a936]
    * `d/i/p/j0/b` provided by the company XXXX [^fe6233327ee3ff01fd8f02ed088a726f]
    * `d/i/p/j0/b` provided by the company XXXX [^4b55d10440ac38072d36d30e4b36b687]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^c90fa2c440dad01756758a2c22556d29]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `androidx/recyclerview/widget/RecyclerView` provided by the company XXXX [^d8f1579bb01ce2e2fc1f1bdf3b8c9f7b]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `androidx/recyclerview/widget/RecyclerView` provided by the company XXXX [^d8f1579bb01ce2e2fc1f1bdf3b8c9f7b]
    * `androidx/viewpager2/widget/ViewPager2$j` provided by the company XXXX [^b3ab42bb1d646309428a6e0f65044d6a]
    * `androidx/appcompat/widget/ActionBarContextView` provided by the company XXXX [^387ee15faf974132074e96aac4696140]
    * `d/i/p/x` provided by the company XXXX [^9c813711310d8deab03dd910375024b7]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0c321f093037d88b429e4049e0dfacbc]
    * `androidx/appcompat/widget/ActionBarContextView` provided by the company XXXX [^387ee15faf974132074e96aac4696140]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `androidx/appcompat/widget/ActionBarContextView` provided by the company XXXX [^387ee15faf974132074e96aac4696140]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `androidx/core/widget/NestedScrollView$a` provided by the company XXXX [^0330e38896710bdc44950b4df747777f]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/core/widget/NestedScrollView$a` provided by the company XXXX [^0330e38896710bdc44950b4df747777f]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/recyclerview/widget/StaggeredGridLayoutManager` provided by the company XXXX [^d9e945237f819092afda4efba1adca67]
    * `androidx/viewpager2/widget/ViewPager2$m` provided by the company XXXX [^941a1eefffb8cd96ef5f3331842a8359]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/recyclerview/widget/LinearLayoutManager` provided by the company XXXX [^cf7911b64376b24cdd3ee758e57bf1f5]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^40eb0cd93b972c44100e7f3c0f2a9b6d]
    * `androidx/recyclerview/widget/StaggeredGridLayoutManager` provided by the company XXXX [^d9e945237f819092afda4efba1adca67]
    * `androidx/viewpager2/widget/ViewPager2$m` provided by the company XXXX [^941a1eefffb8cd96ef5f3331842a8359]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `androidx/recyclerview/widget/LinearLayoutManager` provided by the company XXXX [^cf7911b64376b24cdd3ee758e57bf1f5]
    * `androidx/viewpager/widget/ViewPager$g` provided by the company XXXX [^7bca740cd7419a3545d3253912d661a5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0c321f093037d88b429e4049e0dfacbc]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `d/k/a/a` provided by the company XXXX [^d094112098db1c197de38a3a484e1e3e]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `com/google/android/material/button/MaterialButton` provided by the company XXXX [^cd32530947a61228cdef7e37db9469bd]
    * `com/google/android/material/card/MaterialCardView` provided by the company XXXX [^1896537b6182835a96104e1e59340717]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `com/google/android/material/internal/CheckableImageButton$a` provided by the company XXXX [^07eceabdea340d2ea27d81304bfb4932]
    * `d/k/a/a` provided by the company XXXX [^b576f0e03168c52e9d39ebf25768a5e5]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^40eb0cd93b972c44100e7f3c0f2a9b6d]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^40eb0cd93b972c44100e7f3c0f2a9b6d]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^40eb0cd93b972c44100e7f3c0f2a9b6d]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^0c321f093037d88b429e4049e0dfacbc]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `io/flutter/view/AccessibilityBridge` provided by the company XXXX [^24a4559cb166b15cb1fe0de6901a61b9]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]
    * `io/flutter/view/AccessibilityViewEmbedder` provided by the company XXXX [^c7fef7264062be63f3a1fee40bb6df32]


### Evidence files
[^openServerSocket]: `cfg/openServerSocket`
[^5a16dee55f1eaa2b840599e10db86d32]: `code/code_openServerSocket_Lokhttp3-mockwebserver-MockWebServer$3-_5a16dee55f1eaa2b840599e10db86d32.bmp`
[^1fa766c6ecf0c4910e9afd0df4d5c7e3]: `code/code_openServerSocket_Lokhttp3-mockwebserver-MockWebServer-_1fa766c6ecf0c4910e9afd0df4d5c7e3.bmp`
[^loadWebview]: `cfg/loadWebview`
[^d1650d956ae924d3d8f1b138e0768264]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity-_d1650d956ae924d3d8f1b138e0768264.bmp`
[^22e21a46807f97cd7e67f47dd3a4df0f]: `code/code_loadWebview_Lcom-bitmovin-player-ui-a-_22e21a46807f97cd7e67f47dd3a4df0f.bmp`
[^c9495d0672a95c4266e212cbd0cf1003]: `code/code_loadWebview_Lly-count-android-sdk-ModuleFeedback$2-_c9495d0672a95c4266e212cbd0cf1003.bmp`
[^65b75779c5027cad10b52f6c9b30fdc6]: `code/code_loadWebview_Lzendesk-support-guide-ViewArticleActivity-_65b75779c5027cad10b52f6c9b30fdc6.bmp`
[^7b463c2ff7a185d2bbd13743b34122b6]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_7b463c2ff7a185d2bbd13743b34122b6.bmp`
[^9389f730895a932948be4f7acf4089a9]: `code/code_loadWebview_Lly-count-android-sdk-ModuleRatings$4$1-_9389f730895a932948be4f7acf4089a9.bmp`
[^e8616736b9e27e7c23c6b699574c1b28]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_e8616736b9e27e7c23c6b699574c1b28.bmp`
[^ef2a2263b517e05a9731ea34f5966a0b]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView-_ef2a2263b517e05a9731ea34f5966a0b.bmp`
[^3978cf26e4234243715599552c588037]: `code/code_loadWebview_Lcom-facebook-internal-c0-_3978cf26e4234243715599552c588037.bmp`
[^4841dffbbd7091bd5abc347c8455e3c2]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-FlutterWebView-_4841dffbbd7091bd5abc347c8455e3c2.bmp`
[^8f6e7790427967dbb50afd9ff1a7f3b2]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView-_8f6e7790427967dbb50afd9ff1a7f3b2.bmp`
[^e8616736b9e27e7c23c6b699574c1b28]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_e8616736b9e27e7c23c6b699574c1b28.bmp`
[^d44dc44bf91432ec9cadc16655924e6f]: `code/code_loadWebview_Lcom-bitmovin-player-ui-a-_d44dc44bf91432ec9cadc16655924e6f.bmp`
[^4655233a1ac756e441565c8205821f34]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_browser-InAppBrowserActivity-_4655233a1ac756e441565c8205821f34.bmp`
[^5081f1ad68ad449369933bf4c1e61d25]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_5081f1ad68ad449369933bf4c1e61d25.bmp`
[^d819fb4801b4bfe7bc4801b25e1aaff9]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-JavaScriptBridgeInterface$2$1-_d819fb4801b4bfe7bc4801b25e1aaff9.bmp`
[^c19a4141f328b1af9138e103240de700]: `code/code_loadWebview_Lcom-facebook-internal-k-_c19a4141f328b1af9138e103240de700.bmp`
[^c9495d0672a95c4266e212cbd0cf1003]: `code/code_loadWebview_Lly-count-android-sdk-ModuleFeedback$2-_c9495d0672a95c4266e212cbd0cf1003.bmp`
[^5578f617513e3ef4b2b765bb662a72c1]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_5578f617513e3ef4b2b765bb662a72c1.bmp`
[^c1a2e8b30103b1c14504182dbb6c8887]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView$10-_c1a2e8b30103b1c14504182dbb6c8887.bmp`
[^77acc85386220b4dc169ce2d8ea3a202]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity$2-_77acc85386220b4dc169ce2d8ea3a202.bmp`
[^b87422697df0217f278c83bdb71a0d33]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity$FlutterWebChromeClient$1-_b87422697df0217f278c83bdb71a0d33.bmp`
[^39250dde74d1cdcf2821424460cdfb77]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_39250dde74d1cdcf2821424460cdfb77.bmp`
[^ff92313ba1e8edffb711840096a17e4a]: `code/code_loadWebview_Lcom-bitmovin-player-ui-a-_ff92313ba1e8edffb711840096a17e4a.bmp`
[^c689ecc624b35a264f341a2bbbecb47b]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_c689ecc624b35a264f341a2bbbecb47b.bmp`
[^d41c5e359f93f52b5d8a0b944644f7fb]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView-_d41c5e359f93f52b5d8a0b944644f7fb.bmp`
[^81946c5ef339a562eb2c65ba80c8da41]: `code/code_loadWebview_Lcom-bitmovin-player-ui-CustomMessageHandler$a-_81946c5ef339a562eb2c65ba80c8da41.bmp`
[^294d47a5e8bed68b1c2c34d2b237bb37]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_browser-InAppBrowserActivity$1-_294d47a5e8bed68b1c2c34d2b237bb37.bmp`
[^0e948ef9c11dd3ea87c92bd06260d410]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebViewClient$OnNavigationRequestResult-_0e948ef9c11dd3ea87c92bd06260d410.bmp`
[^a51081d4e60e822d69bb05e136d781d6]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_a51081d4e60e822d69bb05e136d781d6.bmp`
[^2d0cad82079a6bc0f5e56cbfb2bf11bd]: `code/code_loadWebview_Lcom-bitmovin-player-ui-a-_2d0cad82079a6bc0f5e56cbfb2bf11bd.bmp`
[^5dd09300d88a10bda8c4fb22818ef821]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity$2-_5dd09300d88a10bda8c4fb22818ef821.bmp`
[^9389f730895a932948be4f7acf4089a9]: `code/code_loadWebview_Lly-count-android-sdk-ModuleRatings$4$1-_9389f730895a932948be4f7acf4089a9.bmp`
[^4c9a4c20d8ffe03d25ceca0ef737b811]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView$FlutterWebChromeClient$1-_4c9a4c20d8ffe03d25ceca0ef737b811.bmp`
[^d336ac512fdbb037beab29f850a79703]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_d336ac512fdbb037beab29f850a79703.bmp`
[^4841dffbbd7091bd5abc347c8455e3c2]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-FlutterWebView-_4841dffbbd7091bd5abc347c8455e3c2.bmp`
[^fdb2233c7c5e24806519c3d57dbf414c]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView$FlutterWebChromeClient$1-_fdb2233c7c5e24806519c3d57dbf414c.bmp`
[^da3d86654c86a7b140771171490b8609]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_da3d86654c86a7b140771171490b8609.bmp`
[^33a82bb7fc6d9ae9fb89c2bb8a39b8ea]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-content_blocker-ContentBlockerHandler$2-_33a82bb7fc6d9ae9fb89c2bb8a39b8ea.bmp`
[^3978cf26e4234243715599552c588037]: `code/code_loadWebview_Lcom-facebook-internal-c0-_3978cf26e4234243715599552c588037.bmp`
[^2b9592930fcfab35079857d32bf30967]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity$FlutterWebChromeClient$1-_2b9592930fcfab35079857d32bf30967.bmp`
[^d1650d956ae924d3d8f1b138e0768264]: `code/code_loadWebview_Lio-flutter-plugins-urllauncher-WebViewActivity-_d1650d956ae924d3d8f1b138e0768264.bmp`
[^c689ecc624b35a264f341a2bbbecb47b]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebViewClient-_c689ecc624b35a264f341a2bbbecb47b.bmp`
[^0eb1db73cb0d10032a2071f1fffe2f25]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebView-_0eb1db73cb0d10032a2071f1fffe2f25.bmp`
[^0e948ef9c11dd3ea87c92bd06260d410]: `code/code_loadWebview_Lio-flutter-plugins-webviewflutter-FlutterWebViewClient$OnNavigationRequestResult-_0e948ef9c11dd3ea87c92bd06260d410.bmp`
[^5578f617513e3ef4b2b765bb662a72c1]: `code/code_loadWebview_Lcom-pichillilorenzo-flutter_inappwebview-in_app_webview-InAppWebView-_5578f617513e3ef4b2b765bb662a72c1.bmp`
[^loadExternalCode]: `cfg/loadExternalCode`
[^53c3d24a7fa9249809ff941e8f1329db]: `code/code_loadExternalCode_Lcom-gyf-immersionbar-l-_53c3d24a7fa9249809ff941e8f1329db.bmp`
[^f6c91f3efd0661cab5cec1e6718de11b]: `code/code_loadExternalCode_Lcom-google-android-gms-dynamite-DynamiteModule-_f6c91f3efd0661cab5cec1e6718de11b.bmp`
[^334731336fa82ea0bfa52e50ee41945f]: `code/code_loadExternalCode_Lcom-facebook-z-s-g-_334731336fa82ea0bfa52e50ee41945f.bmp`
[^085bdf0595b28728b9b3d47084d8e31a]: `code/code_loadExternalCode_Lcom-google-android-gms-dynamite-DynamiteModule-_085bdf0595b28728b9b3d47084d8e31a.bmp`
[^0554bbb29027ec7cb0d029da44c3b31b]: `code/code_loadExternalCode_Lkotlin-o0-a0-d-o$a$d-_0554bbb29027ec7cb0d029da44c3b31b.bmp`
[^3fc2e3134fa7013b3ffe33b9210fcc62]: `code/code_loadExternalCode_Lkotlin-o0-a0-d-m0-c-m1-b-a-_3fc2e3134fa7013b3ffe33b9210fcc62.bmp`
[^95352b8ff6e5e4e09e4522983f479bc2]: `code/code_loadExternalCode_Lh-n-a-d-c-c-_95352b8ff6e5e4e09e4522983f479bc2.bmp`
[^cbc924f442c0a3d76d82a410c9214e4a]: `code/code_loadExternalCode_Lkotlin-g0-j-a-i-_cbc924f442c0a3d76d82a410c9214e4a.bmp`
[^08017a14a9ed30e923c2d0c4130a1268]: `code/code_loadExternalCode_Lcom-gyf-immersionbar-l-_08017a14a9ed30e923c2d0c4130a1268.bmp`
[^315dc05986856cc605da8d3a1375d092]: `code/code_loadExternalCode_Lcom-google-android-gms-dynamite-DynamiteModule-_315dc05986856cc605da8d3a1375d092.bmp`
[^afd222b062d81c9c85a767051d9506f1]: `code/code_loadExternalCode_Lcom-google-android-gms-common-l-a-_afd222b062d81c9c85a767051d9506f1.bmp`
[^b7a29ebbd98cb497210e853383e56448]: `code/code_loadExternalCode_Lkotlin-o0-a0-d-j-_b7a29ebbd98cb497210e853383e56448.bmp`
[^944e659661ecee36b4ebc727fe7a0d1f]: `code/code_loadExternalCode_Lcom-google-android-gms-dynamite-DynamiteModule-_944e659661ecee36b4ebc727fe7a0d1f.bmp`
[^d9bc495ccc3d57cef5f4c461de59dd58]: `code/code_loadExternalCode_Lcom-gyf-immersionbar-l-_d9bc495ccc3d57cef5f4c461de59dd58.bmp`
[^c5582d199b27032c41d2099fef55cddb]: `code/code_loadExternalCode_Landroidx-appcompat-widget-w$d-_c5582d199b27032c41d2099fef55cddb.bmp`
[^cf1a9258e5bc0c911ee2b46edad9236a]: `code/code_loadExternalCode_Lcom-google-android-gms-measurement-internal-e3-_cf1a9258e5bc0c911ee2b46edad9236a.bmp`
[^9cde6feb641cd681932d48e3efea4279]: `code/code_loadExternalCode_Lcom-google-android-gms-dynamite-DynamiteModule-_9cde6feb641cd681932d48e3efea4279.bmp`
[^3fb8a87107d6de87959d43348f7b1d6d]: `code/code_loadExternalCode_Lcom-google-android-material-internal-i-_3fb8a87107d6de87959d43348f7b1d6d.bmp`
[^7cee4b649e6b988e34612aadc219c4b1]: `code/code_loadExternalCode_Lcom-appsflyer-internal-bt-_7cee4b649e6b988e34612aadc219c4b1.bmp`
[^4c8241105ae51df70c4c216ecfa9e3b0]: `code/code_loadExternalCode_Lcom-google-android-gms-cloudmessaging-f-_4c8241105ae51df70c4c216ecfa9e3b0.bmp`
[^readTelephonyInfo]: `cfg/readTelephonyInfo`
[^5fe0818afed86f9f77515a9fe9efa13b]: `code/code_readTelephonyInfo_Lly-count-android-sdk-DeviceInfo-_5fe0818afed86f9f77515a9fe9efa13b.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readTelephonyInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^b3fb250d95991f061f9e198edd717709]: `code/code_readTelephonyInfo_Lh-d-a-t-_b3fb250d95991f061f9e198edd717709.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readTelephonyInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^b3fb250d95991f061f9e198edd717709]: `code/code_readTelephonyInfo_Lh-d-a-t-_b3fb250d95991f061f9e198edd717709.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readTelephonyInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^280629040473128c660f4071cb0f6934]: `code/code_readTelephonyInfo_Lcom-google-android-datatransport-cct-d-_280629040473128c660f4071cb0f6934.bmp`
[^c5caf5a5ec725be671e7ceeac46eb912]: `code/code_readTelephonyInfo_Lcom-google-android-exoplayer2-z2-r0-_c5caf5a5ec725be671e7ceeac46eb912.bmp`
[^c25337aab1b5a6e6207b7c891112749f]: `code/code_readTelephonyInfo_Lh-t-a-a-_c25337aab1b5a6e6207b7c891112749f.bmp`
[^0b312a1272f70101981f1a36cb6393f8]: `code/code_readTelephonyInfo_Lcom-bitmovin-android-exoplayer2-c2-n0-_0b312a1272f70101981f1a36cb6393f8.bmp`
[^readLocation]: `cfg/readLocation`
[^e2132945b87cf77c7c3661e2c646345f]: `code/code_readLocation_Landroidx-appcompat-app-l-_e2132945b87cf77c7c3661e2c646345f.bmp`
[^c1fc8395973a2461ba354729d185741d]: `code/code_readLocation_Lcom-appsflyer-internal-ai-_c1fc8395973a2461ba354729d185741d.bmp`
[^e2132945b87cf77c7c3661e2c646345f]: `code/code_readLocation_Landroidx-appcompat-app-l-_e2132945b87cf77c7c3661e2c646345f.bmp`
[^c1fc8395973a2461ba354729d185741d]: `code/code_readLocation_Lcom-appsflyer-internal-ai-_c1fc8395973a2461ba354729d185741d.bmp`
[^61a04737acc1b517f82df6cbb097163e]: `code/code_readLocation_Landroidx-appcompat-app-l-_61a04737acc1b517f82df6cbb097163e.bmp`
[^270291e0748f33557e369c249a31b236]: `code/code_readLocation_Lcom-appsflyer-internal-x-_270291e0748f33557e369c249a31b236.bmp`
[^readNetworkInfo]: `cfg/readNetworkInfo`
[^785ad2af9a2852f101a56319031e556d]: `code/code_readNetworkInfo_Lcom-google-firebase-messaging-SyncTask-_785ad2af9a2852f101a56319031e556d.bmp`
[^1d8407e7d363261ceef53e0cf8ccc1d2]: `code/code_readNetworkInfo_Lly-count-android-sdk-CrashDetails-_1d8407e7d363261ceef53e0cf8ccc1d2.bmp`
[^e01ce3a097d8bf0a79fe6b14ec78ea6b]: `code/code_readNetworkInfo_Lzendesk-core-ZendeskNetworkInfoProvider-_e01ce3a097d8bf0a79fe6b14ec78ea6b.bmp`
[^102d402f068c107080f1d5660b01aa91]: `code/code_readNetworkInfo_Lcom-google-android-gms-measurement-internal-y4-_102d402f068c107080f1d5660b01aa91.bmp`
[^ee62f57ac82e79d792f35d17a9df9457]: `code/code_readNetworkInfo_Lcom-bitmovin-player-offline-service-k-_ee62f57ac82e79d792f35d17a9df9457.bmp`
[^66213d0a3ad3019a3783a3f04038234e]: `code/code_readNetworkInfo_Lzendesk-core-ZendeskNetworkInfoProvider-_66213d0a3ad3019a3783a3f04038234e.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readNetworkInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^b6aff93651566f75ac008bef6e40692d]: `code/code_readNetworkInfo_Lcom-squareup-picasso-i$c-_b6aff93651566f75ac008bef6e40692d.bmp`
[^eb1fc426e0ef91a0c15bfc8f1cfe73fd]: `code/code_readNetworkInfo_Lio-flutter-plugins-connectivity-Connectivity-_eb1fc426e0ef91a0c15bfc8f1cfe73fd.bmp`
[^658824dec0028e0fd135bf40d32eee88]: `code/code_readNetworkInfo_Lorg-getter-bridge-larix-c-_658824dec0028e0fd135bf40d32eee88.bmp`
[^5dac6a9d55e9b9d84fdf6ac0bd5991f0]: `code/code_readNetworkInfo_Lcom-bitmovin-android-exoplayer2-scheduler-Requirements-_5dac6a9d55e9b9d84fdf6ac0bd5991f0.bmp`
[^32cce924e9ecf099d1b382bd1896d3c4]: `code/code_readNetworkInfo_Lio-sentry-android-core-util-ConnectivityChecker-_32cce924e9ecf099d1b382bd1896d3c4.bmp`
[^15dc49803492c3c6fe138db794ab59f2]: `code/code_readNetworkInfo_Lcom-squareup-picasso-i-_15dc49803492c3c6fe138db794ab59f2.bmp`
[^dbc8db33e6d74316799deb8fdd9c349c]: `code/code_readNetworkInfo_Lcom-bumptech-glide-manager-DefaultConnectivityMonitor-_dbc8db33e6d74316799deb8fdd9c349c.bmp`
[^c920139545877eded9b825f0dade35ef]: `code/code_readNetworkInfo_Lcom-google-android-gms-measurement-internal-t3-_c920139545877eded9b825f0dade35ef.bmp`
[^a25a7647783319f572a8bb84d31768a1]: `code/code_readNetworkInfo_Lzendesk-core-NetworkUtils-_a25a7647783319f572a8bb84d31768a1.bmp`
[^c3a56222190e3dce1f1cfdf1daa35a7d]: `code/code_readNetworkInfo_Lcom-google-android-exoplayer2-z2-b0-_c3a56222190e3dce1f1cfdf1daa35a7d.bmp`
[^e2177d09c88ef1a0a1cf665f7c1ce705]: `code/code_readNetworkInfo_Lcom-banuba-sdk-a-c-e-_e2177d09c88ef1a0a1cf665f7c1ce705.bmp`
[^5adb1780ee7fbc6e715ec3e30770a4bb]: `code/code_readNetworkInfo_Lcom-google-firebase-crashlytics-internal-common-CommonUtils-_5adb1780ee7fbc6e715ec3e30770a4bb.bmp`
[^280629040473128c660f4071cb0f6934]: `code/code_readNetworkInfo_Lcom-google-android-datatransport-cct-d-_280629040473128c660f4071cb0f6934.bmp`
[^1705b1036740617a3bbbca2110b13f93]: `code/code_readNetworkInfo_Lcom-google-firebase-messaging-TopicsSyncTask-_1705b1036740617a3bbbca2110b13f93.bmp`
[^9dfcf164c294dcb00368ce12dbd58968]: `code/code_readNetworkInfo_Lcom-google-android-datatransport-runtime-scheduling-jobscheduling-t-_9dfcf164c294dcb00368ce12dbd58968.bmp`
[^bcc1028e4c42f15391a6fb83771c8041]: `code/code_readNetworkInfo_Lio-sentry-android-core-util-ConnectivityChecker-_bcc1028e4c42f15391a6fb83771c8041.bmp`
[^f4988c36a3625a70996e38d8cedd41df]: `code/code_readNetworkInfo_Lcom-google-android-exoplayer2-scheduler-Requirements-_f4988c36a3625a70996e38d8cedd41df.bmp`
[^e62f8abb9375ed220212dc9ee5064f89]: `code/code_readNetworkInfo_Lzendesk-support-guide-NetworkUtils-_e62f8abb9375ed220212dc9ee5064f89.bmp`
[^0bf1cac28ceb2b981fcf111e173682ff]: `code/code_readNetworkInfo_Lcom-bitmovin-android-exoplayer2-c2-n0-_0bf1cac28ceb2b981fcf111e173682ff.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readNetworkInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^de0fb94acdbdb4c22791834523b23915]: `code/code_readNetworkInfo_Ld-i-k-a-_de0fb94acdbdb4c22791834523b23915.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readNetworkInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^84eb1005faba38c105a6285693caf5b3]: `code/code_readNetworkInfo_Lcom-appsflyer-internal-ai-_84eb1005faba38c105a6285693caf5b3.bmp`
[^be42a4aa0c9c7ca8741f2f5ec3c4c134]: `code/code_readNetworkInfo_Lcom-appsflyer-internal-u-_be42a4aa0c9c7ca8741f2f5ec3c4c134.bmp`
[^readNetworkAddresses]: `cfg/readNetworkAddresses`
[^84eb1005faba38c105a6285693caf5b3]: `code/code_readNetworkAddresses_Lcom-appsflyer-internal-ai-_84eb1005faba38c105a6285693caf5b3.bmp`
[^fc9a185c9a99819ab63c668321d7196c]: `code/code_readNetworkAddresses_Lokhttp3-mockwebserver-MockWebServer$4-_fc9a185c9a99819ab63c668321d7196c.bmp`
[^7a1227a5ca0e29de4945dad31832fe52]: `code/code_readNetworkAddresses_Lokhttp3-mockwebserver-MockWebServer-_7a1227a5ca0e29de4945dad31832fe52.bmp`
[^13224f2135f1c5949202c60e49601558]: `code/code_readNetworkAddresses_Lokhttp3-mockwebserver-MockWebServer$4-_13224f2135f1c5949202c60e49601558.bmp`
[^0575555de499beda9d2cf1f2899b89e4]: `code/code_readNetworkAddresses_Lokhttp3-mockwebserver-MockWebServer-_0575555de499beda9d2cf1f2899b89e4.bmp`
[^5e2f41d491cda87074679a245ea29b7e]: `code/code_readNetworkAddresses_Lokhttp3-internal-Util-_5e2f41d491cda87074679a245ea29b7e.bmp`
[^useCrypto]: `cfg/useCrypto`
[^9ff1d152ccff6fa058b44d8ad92133da]: `code/code_useCrypto_Lcom-bitmovin-android-exoplayer2-source-hls-d-_9ff1d152ccff6fa058b44d8ad92133da.bmp`
[^f03f4123f52a9abb5942e20d1d0b997a]: `code/code_useCrypto_Ls-b-_f03f4123f52a9abb5942e20d1d0b997a.bmp`
[^5009bd63d15c95375372c1e492986b31]: `code/code_useCrypto_Lcom-google-android-exoplayer2-source-hls-d-_5009bd63d15c95375372c1e492986b31.bmp`
[^f03f4123f52a9abb5942e20d1d0b997a]: `code/code_useCrypto_Ls-b-_f03f4123f52a9abb5942e20d1d0b997a.bmp`
[^0e1265d3ecd05705142bb42620c9bc90]: `code/code_useCrypto_Lcom-bitmovin-android-exoplayer2-source-hls-d-_0e1265d3ecd05705142bb42620c9bc90.bmp`
[^119bfe22ed14cc3ef94609804ef1a304]: `code/code_useCrypto_Lcom-bitmovin-android-exoplayer2-upstream-o0-o$b-_119bfe22ed14cc3ef94609804ef1a304.bmp`
[^7126d50e35c6c38f4f344dc92156f3f0]: `code/code_useCrypto_Lcom-google-android-exoplayer2-source-hls-d-_7126d50e35c6c38f4f344dc92156f3f0.bmp`
[^d606701b5dabba7ae512f454002ee725]: `code/code_useCrypto_Lcom-bitmovin-android-exoplayer2-upstream-o0-o$b-_d606701b5dabba7ae512f454002ee725.bmp`
[^026a98f4db36f8ce8747a59d8c089c79]: `code/code_useCrypto_Ls-b-_026a98f4db36f8ce8747a59d8c089c79.bmp`
[^useReflection]: `cfg/useReflection`
[^ee8079deb5f2a58485efc001e38007d1]: `code/code_useReflection_Lcom-google-firebase-database-core-utilities-encoding-CustomClassMapper$BeanMapper-_ee8079deb5f2a58485efc001e38007d1.bmp`
[^ee8079deb5f2a58485efc001e38007d1]: `code/code_useReflection_Lcom-google-firebase-database-core-utilities-encoding-CustomClassMapper$BeanMapper-_ee8079deb5f2a58485efc001e38007d1.bmp`
[^79869d92c67ae12b9e5c190c1ab9e894]: `code/code_useReflection_Lcom-google-gson-internal-reflect-PreJava9ReflectionAccessor-_79869d92c67ae12b9e5c190c1ab9e894.bmp`
[^b61d13ff5e5b1610d1eb9dba62a39cd3]: `code/code_useReflection_Lcom-google-gson-internal-reflect-UnsafeReflectionAccessor-_b61d13ff5e5b1610d1eb9dba62a39cd3.bmp`
[^useSensors]: `cfg/useSensors`
[^29697fdbbddcd21fce93baf85ab9d8c6]: `code/code_useSensors_Lcom-appsflyer-internal-ab$3-_29697fdbbddcd21fce93baf85ab9d8c6.bmp`
[^295331c815f28aeb873ea631510269c0]: `code/code_useSensors_Lcom-appsflyer-internal-c$d-_295331c815f28aeb873ea631510269c0.bmp`
[^6a8096b24473cafd21b24a016a682165]: `code/code_useSensors_Lcom-google-android-exoplayer2-video-spherical-SphericalGLSurfaceView-_6a8096b24473cafd21b24a016a682165.bmp`
[^e3c0746ed3dd8a43edd300483f467c31]: `code/code_useSensors_Lcom-google-firebase-crashlytics-internal-common-CommonUtils-_e3c0746ed3dd8a43edd300483f467c31.bmp`
[^c2373c56abd241b5368ab30e5a8e8fe4]: `code/code_useSensors_Lcom-bitmovin-android-exoplayer2-ui-spherical-SphericalGLSurfaceView-_c2373c56abd241b5368ab30e5a8e8fe4.bmp`
[^5f76814231dea690138f04a114bd5842]: `code/code_useSensors_Lcom-facebook-z-r-b-_5f76814231dea690138f04a114bd5842.bmp`
[^cf77b122427726b313ee7fa4825b6823]: `code/code_useSensors_Lcom-bitmovin-player-v-k-a-_cf77b122427726b313ee7fa4825b6823.bmp`
[^4b60dfe9f7e25a1f4123d98fa48929d8]: `code/code_useSensors_Lio-sentry-android-core-TempSensorBreadcrumbsIntegration-_4b60dfe9f7e25a1f4123d98fa48929d8.bmp`
[^29697fdbbddcd21fce93baf85ab9d8c6]: `code/code_useSensors_Lcom-appsflyer-internal-ab$3-_29697fdbbddcd21fce93baf85ab9d8c6.bmp`
[^5b9ae3bb83c39cd0dbda81574c2c1dd4]: `code/code_useSensors_Lcom-bitmovin-player-v-k-a-_5b9ae3bb83c39cd0dbda81574c2c1dd4.bmp`
[^5f76814231dea690138f04a114bd5842]: `code/code_useSensors_Lcom-facebook-z-r-b-_5f76814231dea690138f04a114bd5842.bmp`
[^65b93894d57fa9ef7998938018a3769e]: `code/code_useSensors_Lcom-google-android-exoplayer2-video-spherical-SphericalGLSurfaceView-_65b93894d57fa9ef7998938018a3769e.bmp`
[^5b13b1c894787df5f1241db57b79212b]: `code/code_useSensors_Lcom-bitmovin-android-exoplayer2-ui-spherical-SphericalGLSurfaceView-_5b13b1c894787df5f1241db57b79212b.bmp`
[^4b60dfe9f7e25a1f4123d98fa48929d8]: `code/code_useSensors_Lio-sentry-android-core-TempSensorBreadcrumbsIntegration-_4b60dfe9f7e25a1f4123d98fa48929d8.bmp`
[^playSound]: `cfg/playSound`
[^b7d2f2b371168c9c46dc79e23f3aed04]: `code/code_playSound_Landroidx-appcompat-app-e-_b7d2f2b371168c9c46dc79e23f3aed04.bmp`
[^doOsCalls]: `cfg/doOsCalls`
[^30a8ea666bb56766bedaef480fc2578f]: `code/code_doOsCalls_Ld-i-h-h-_30a8ea666bb56766bedaef480fc2578f.bmp`
[^2ba3a87efdaf192814dc91770e68ebfa]: `code/code_doOsCalls_Lcom-facebook-soloader-SysUtil$LollipopSysdeps-_2ba3a87efdaf192814dc91770e68ebfa.bmp`
[^30a8ea666bb56766bedaef480fc2578f]: `code/code_doOsCalls_Ld-i-h-h-_30a8ea666bb56766bedaef480fc2578f.bmp`
[^30a8ea666bb56766bedaef480fc2578f]: `code/code_doOsCalls_Ld-i-h-h-_30a8ea666bb56766bedaef480fc2578f.bmp`
[^b0c397868b5b3b069d219d85c58088a8]: `code/code_doOsCalls_Lcom-facebook-soloader-SysUtil$LollipopSysdeps-_b0c397868b5b3b069d219d85c58088a8.bmp`
[^sendDataUdp]: `cfg/sendDataUdp`
[^19cddcb03be5af18afef4010e9774a83]: `code/code_sendDataUdp_Lcom-google-android-exoplayer2-z2-j0-_19cddcb03be5af18afef4010e9774a83.bmp`
[^ed4b2fc1a2aa0783603c55ccb89f545f]: `code/code_sendDataUdp_Lcom-bitmovin-player-m-k0-k-c-_ed4b2fc1a2aa0783603c55ccb89f545f.bmp`
[^3adc3403e348fd85296b4fcfe97f5101]: `code/code_sendDataUdp_Lcom-bitmovin-android-exoplayer2-c2-f0-_3adc3403e348fd85296b4fcfe97f5101.bmp`
[^receiveDataUdp]: `cfg/receiveDataUdp`
[^19cddcb03be5af18afef4010e9774a83]: `code/code_receiveDataUdp_Lcom-google-android-exoplayer2-z2-j0-_19cddcb03be5af18afef4010e9774a83.bmp`
[^ed4b2fc1a2aa0783603c55ccb89f545f]: `code/code_receiveDataUdp_Lcom-bitmovin-player-m-k0-k-c-_ed4b2fc1a2aa0783603c55ccb89f545f.bmp`
[^3adc3403e348fd85296b4fcfe97f5101]: `code/code_receiveDataUdp_Lcom-bitmovin-android-exoplayer2-c2-f0-_3adc3403e348fd85296b4fcfe97f5101.bmp`
[^c3762f4e1d129e95a1988f571f1babaf]: `code/code_receiveDataUdp_Lcom-bitmovin-android-exoplayer2-upstream-n0-_c3762f4e1d129e95a1988f571f1babaf.bmp`
[^fc69c3bc5f372d96b426c78c4befce57]: `code/code_receiveDataUdp_Lcom-google-android-exoplayer2-y2-j0-_fc69c3bc5f372d96b426c78c4befce57.bmp`
[^useCamera]: `cfg/useCamera`
[^6e5586a8b5556227db309f735fdf31bd]: `code/code_useCamera_Lio-flutter-plugins-camera-Camera-_6e5586a8b5556227db309f735fdf31bd.bmp`
[^a9d2c2e0be30a4d2e25b999a6be81d53]: `code/code_useCamera_Lcom-banuba-android-sdk-camera-Camera2-_a9d2c2e0be30a4d2e25b999a6be81d53.bmp`
[^e1969beaaa04813769783d6ad78c6b1a]: `code/code_useCamera_Lh-b0-a-e0-_e1969beaaa04813769783d6ad78c6b1a.bmp`
[^sendDataHttp]: `cfg/sendDataHttp`
[^f0d85fbea563e6c3d136d280f5e63ded]: `code/code_sendDataHttp_Lio-sentry-transport-HttpConnection-_f0d85fbea563e6c3d136d280f5e63ded.bmp`
[^29053cfeb33ea5482a03c8548afa173f]: `code/code_sendDataHttp_Lcom-google-firebase-installations-remote-FirebaseInstallationServiceClient-_29053cfeb33ea5482a03c8548afa173f.bmp`
[^c6983615f2e39165be69df951fd0ba0e]: `code/code_sendDataHttp_Lcom-appsflyer-internal-am-_c6983615f2e39165be69df951fd0ba0e.bmp`
[^6ce1692b7553b30c537241e7ddb2b880]: `code/code_sendDataHttp_Lh-l-a-b-d-b-b$b-_6ce1692b7553b30c537241e7ddb2b880.bmp`
[^56f84080e47c035c959ed23e715ec11b]: `code/code_sendDataHttp_Lcom-airbnb-lottie-w-b-_56f84080e47c035c959ed23e715ec11b.bmp`
[^3fc3c278e6097a569204566ce9ae7808]: `code/code_sendDataHttp_Lcom-bitmovin-android-exoplayer2-upstream-w-_3fc3c278e6097a569204566ce9ae7808.bmp`
[^8f9c23292bf505cf3d91b41ed3f0753f]: `code/code_sendDataHttp_Lcom-google-firebase-installations-remote-FirebaseInstallationServiceClient-_8f9c23292bf505cf3d91b41ed3f0753f.bmp`
[^403550b393109062146184af0edb0b20]: `code/code_sendDataHttp_Lcom-google-firebase-installations-remote-FirebaseInstallationServiceClient-_403550b393109062146184af0edb0b20.bmp`
[^f0da5a507a64edb99f33c8ef28ab79f3]: `code/code_sendDataHttp_Lcom-appsflyer-internal-bv-_f0da5a507a64edb99f33c8ef28ab79f3.bmp`
[^4bd7effe9045918e47a34fe058b62a72]: `code/code_sendDataHttp_Lcom-appsflyer-internal-ah-_4bd7effe9045918e47a34fe058b62a72.bmp`
[^7c8d968bc325f7350b3cb8566a4ab734]: `code/code_sendDataHttp_Lcom-google-android-datatransport-cct-d-_7c8d968bc325f7350b3cb8566a4ab734.bmp`
[^5c2baedb67a6ab33028a653ee6fc3e44]: `code/code_sendDataHttp_Lcom-bitmovin-player-m-f$a-_5c2baedb67a6ab33028a653ee6fc3e44.bmp`
[^c699f438302e67a08866c993e0e36465]: `code/code_sendDataHttp_Lcom-facebook-GraphRequest-_c699f438302e67a08866c993e0e36465.bmp`
[^ef4f5eda488177361d343a6818f8560b]: `code/code_sendDataHttp_Lcom-appsflyer-internal-ai-_ef4f5eda488177361d343a6818f8560b.bmp`
[^f625e4d5196fbc0df2f890fdf611837e]: `code/code_sendDataHttp_Lly-count-android-sdk-ConnectionProcessor-_f625e4d5196fbc0df2f890fdf611837e.bmp`
[^7d9364d87ec144f072fdbca078bad9b4]: `code/code_sendDataHttp_Lcom-google-android-exoplayer2-y2-v-_7d9364d87ec144f072fdbca078bad9b4.bmp`
[^362db744ced4a12ddd220def8ae9dace]: `code/code_sendDataHttp_Lcom-appsflyer-internal-bj-_362db744ced4a12ddd220def8ae9dace.bmp`
[^ace27a987c7b28287c727731ae17158b]: `code/code_sendDataHttp_Lcom-example-r_upgrade-common-UpgradeService$b-_ace27a987c7b28287c727731ae17158b.bmp`
[^f0d85fbea563e6c3d136d280f5e63ded]: `code/code_sendDataHttp_Lio-sentry-transport-HttpConnection-_f0d85fbea563e6c3d136d280f5e63ded.bmp`
[^6ce1692b7553b30c537241e7ddb2b880]: `code/code_sendDataHttp_Lh-l-a-b-d-b-b$b-_6ce1692b7553b30c537241e7ddb2b880.bmp`
[^803d4286458f27cc3d30f3e3d1df698b]: `code/code_sendDataHttp_Lcom-facebook-imagepipeline-producers-x-_803d4286458f27cc3d30f3e3d1df698b.bmp`
[^3fc3c278e6097a569204566ce9ae7808]: `code/code_sendDataHttp_Lcom-bitmovin-android-exoplayer2-upstream-w-_3fc3c278e6097a569204566ce9ae7808.bmp`
[^cc26f11dac8699988d9886376d84c885]: `code/code_sendDataHttp_Lcom-bitmovin-player-m-g-_cc26f11dac8699988d9886376d84c885.bmp`
[^7c8d968bc325f7350b3cb8566a4ab734]: `code/code_sendDataHttp_Lcom-google-android-datatransport-cct-d-_7c8d968bc325f7350b3cb8566a4ab734.bmp`
[^39759de375ce11f441971abed075b742]: `code/code_sendDataHttp_Lcom-facebook-GraphRequest-_39759de375ce11f441971abed075b742.bmp`
[^7dce79ec99cec534ec4cde81378fd4ef]: `code/code_sendDataHttp_Lcom-facebook-GraphRequest-_7dce79ec99cec534ec4cde81378fd4ef.bmp`
[^f625e4d5196fbc0df2f890fdf611837e]: `code/code_sendDataHttp_Lly-count-android-sdk-ConnectionProcessor-_f625e4d5196fbc0df2f890fdf611837e.bmp`
[^7d9364d87ec144f072fdbca078bad9b4]: `code/code_sendDataHttp_Lcom-google-android-exoplayer2-y2-v-_7d9364d87ec144f072fdbca078bad9b4.bmp`
[^ace27a987c7b28287c727731ae17158b]: `code/code_sendDataHttp_Lcom-example-r_upgrade-common-UpgradeService$b-_ace27a987c7b28287c727731ae17158b.bmp`
[^startAnotherApp]: `cfg/startAnotherApp`
[^64f67d74ad8f27b289f238d4cb841adb]: `code/code_startAnotherApp_Lcom-google-firebase-messaging-CommonNotificationBuilder-_64f67d74ad8f27b289f238d4cb841adb.bmp`
[^f6f320efffec6fac183e53f1b98672ed]: `code/code_startAnotherApp_Lly-count-android-sdk-Countly-_f6f320efffec6fac183e53f1b98672ed.bmp`
[^f26ed3a7105d7a45e88a7aae730a9017]: `code/code_startAnotherApp_Lx-a-a-c-_f26ed3a7105d7a45e88a7aae730a9017.bmp`
[^48393b7542c097df36876f1095fcd0e6]: `code/code_startAnotherApp_Lly-count-android-sdk-messaging-CountlyPush-_48393b7542c097df36876f1095fcd0e6.bmp`
[^cb9b8d97babd4ed62783b5cc41500b4f]: `code/code_startAnotherApp_Lcom-dexterous-flutterlocalnotifications-FlutterLocalNotificationsPlugin-_cb9b8d97babd4ed62783b5cc41500b4f.bmp`
[^execCommand]: `cfg/execCommand`
[^d0a469b6c4155a9a133b3ab99dce0a6c]: `code/code_execCommand_Lcom-banuba-sdk-ve-domain-a-_d0a469b6c4155a9a133b3ab99dce0a6c.bmp`
[^4c5f023c2850add8f8aa39cc95c728e8]: `code/code_execCommand_Lio-sentry-android-core-util-RootChecker-_4c5f023c2850add8f8aa39cc95c728e8.bmp`
[^recordAudio]: `cfg/recordAudio`
[^89113233ddc35a1303a604ad41909881]: `code/code_recordAudio_Lcom-banuba-sdk-veui-ui-d0-a-_89113233ddc35a1303a604ad41909881.bmp`
[^8626fd38b81777c6a4e315cf3a74816f]: `code/code_recordAudio_Lh-b0-a-j-_8626fd38b81777c6a4e315cf3a74816f.bmp`
[^ba28a442e48384418196b89a9e75ab66]: `code/code_recordAudio_Lcom-banuba-sdk-core-encoding-d$d-_ba28a442e48384418196b89a9e75ab66.bmp`
[^d3b2e43e31a82b5ebf01d96c5f3ef6fd]: `code/code_recordAudio_Lcom-banuba-sdk-core-encoding-d$d$a-_d3b2e43e31a82b5ebf01d96c5f3ef6fd.bmp`
[^03d561289427a4dcaa0983211644ec1e]: `code/code_recordAudio_Lh-b0-a-j-_03d561289427a4dcaa0983211644ec1e.bmp`
[^ba28a442e48384418196b89a9e75ab66]: `code/code_recordAudio_Lcom-banuba-sdk-core-encoding-d$d-_ba28a442e48384418196b89a9e75ab66.bmp`
[^e1238642ad1d6ec4e98c4b59d712f370]: `code/code_recordAudio_Lcom-banuba-sdk-veui-ui-d0-a$c-_e1238642ad1d6ec4e98c4b59d712f370.bmp`
[^recordVideo]: `cfg/recordVideo`
[^6abe00924930a74fd42528b2a3899b07]: `code/code_recordVideo_Lio-flutter-plugins-camera-Camera-_6abe00924930a74fd42528b2a3899b07.bmp`
[^b01f084b2b9109ed18f209b4426125fc]: `code/code_recordVideo_Lio-flutter-plugins-camera-media-MediaRecorderBuilder-_b01f084b2b9109ed18f209b4426125fc.bmp`
[^readRuntimeInfo]: `cfg/readRuntimeInfo`
[^f8678a0fb8b2fe03618940e22270fcb5]: `code/code_readRuntimeInfo_Lcom-getter-video-edit-l-a-_f8678a0fb8b2fe03618940e22270fcb5.bmp`
[^1989887538cbeb3d9d8a0023c306f3fa]: `code/code_readRuntimeInfo_Lorg-gsuite-flutter_gtv_image-image-e-_1989887538cbeb3d9d8a0023c306f3fa.bmp`
[^79200aa88df9284998a5a6fd52f6fb54]: `code/code_readRuntimeInfo_Lcom-banuba-sdk-core-HardwareCapabilitiesDetector-_79200aa88df9284998a5a6fd52f6fb54.bmp`
[^f1839f1ab2649805e56772c96d3b514d]: `code/code_readRuntimeInfo_Lorg-getter-g-b-_f1839f1ab2649805e56772c96d3b514d.bmp`
[^b53c0be478020a950b37c1c42b176047]: `code/code_readRuntimeInfo_Ly-z-_b53c0be478020a950b37c1c42b176047.bmp`
[^fdd0e0c8524dafca71574a5bcee5f34a]: `code/code_readRuntimeInfo_Lcom-google-firebase-crashlytics-internal-common-CrashlyticsController-_fdd0e0c8524dafca71574a5bcee5f34a.bmp`
[^026eb81f3608194b38f86e67062d7824]: `code/code_readRuntimeInfo_Lh-x-b-a-_026eb81f3608194b38f86e67062d7824.bmp`
[^e81a312cc28277d05d1d6a620f88af50]: `code/code_readRuntimeInfo_Lkotlinx-coroutines-internal-d0-_e81a312cc28277d05d1d6a620f88af50.bmp`
[^0ba9e1df551cac4e3cfd986376f1ef13]: `code/code_readRuntimeInfo_Lh-n-d-a-c-j-_0ba9e1df551cac4e3cfd986376f1ef13.bmp`
[^eb9cde63fd406d4f331ad041b2b58054]: `code/code_readRuntimeInfo_Lcom-bumptech-glide-load-engine-executor-RuntimeCompat-_eb9cde63fd406d4f331ad041b2b58054.bmp`
[^2e473afff55aaf8c9b2afd2f5f62be7a]: `code/code_readRuntimeInfo_Lh-l-a-b-e-a-_2e473afff55aaf8c9b2afd2f5f62be7a.bmp`
[^d3de275e309287a3b38483ab2136642f]: `code/code_readRuntimeInfo_Lcom-banuba-sdk-gallery-ui-l$g-_d3de275e309287a3b38483ab2136642f.bmp`
[^42ac93bb2c78643287a0675ca7d9be48]: `code/code_readRuntimeInfo_Lcom-facebook-imagepipeline-memory-m-_42ac93bb2c78643287a0675ca7d9be48.bmp`
[^aee247f930b05abdc214e962acf04faf]: `code/code_readRuntimeInfo_Lcom-google-firebase-crashlytics-internal-common-CrashlyticsReportDataCapture-_aee247f930b05abdc214e962acf04faf.bmp`
[^90dc9bc61be4dbd5e73df9ca3b647d98]: `code/code_readRuntimeInfo_Lcom-facebook-internal-a0-_90dc9bc61be4dbd5e73df9ca3b647d98.bmp`
[^d97b57b26c925b46e39a594beb13271f]: `code/code_readRuntimeInfo_Lf-a-_d97b57b26c925b46e39a594beb13271f.bmp`
[^3094b886c15f3e2868565a2fc63d8b51]: `code/code_readRuntimeInfo_Lkotlinx-coroutines-a0-_3094b886c15f3e2868565a2fc63d8b51.bmp`
[^493e5a1317633f9ed82aca23d2662976]: `code/code_readRuntimeInfo_Lly-img-android-pesdk-ui-utils-a-_493e5a1317633f9ed82aca23d2662976.bmp`
[^8473724cb222f118cc756b6cdd1bfa3e]: `code/code_readRuntimeInfo_Lcom-facebook-j0-d-l-_8473724cb222f118cc756b6cdd1bfa3e.bmp`
[^22b37f2b78813156fc69f06a0d54da27]: `code/code_readRuntimeInfo_Lly-img-android-pesdk-utils-k0-_22b37f2b78813156fc69f06a0d54da27.bmp`
[^8935fd1f895c97044cfda28af5ee316c]: `code/code_readRuntimeInfo_Lcom-facebook-imagepipeline-memory-d-_8935fd1f895c97044cfda28af5ee316c.bmp`
[^95d755d39af20583d5b1a07397e2c198]: `code/code_readRuntimeInfo_Lcom-facebook-imagepipeline-memory-n-_95d755d39af20583d5b1a07397e2c198.bmp`
[^e064f212d46fae345854fd16c2745a34]: `code/code_readRuntimeInfo_Lcom-facebook-imagepipeline-memory-n-_e064f212d46fae345854fd16c2745a34.bmp`
[^493e5a1317633f9ed82aca23d2662976]: `code/code_readRuntimeInfo_Lly-img-android-pesdk-ui-utils-a-_493e5a1317633f9ed82aca23d2662976.bmp`
[^4ec931cedc1d62726022584a1a90f0bd]: `code/code_readRuntimeInfo_Lcom-facebook-imagepipeline-memory-k-_4ec931cedc1d62726022584a1a90f0bd.bmp`
[^a5c3455f559199a75c459698b8a7c31c]: `code/code_readRuntimeInfo_Lio-sentry-android-core-DefaultAndroidEventProcessor-_a5c3455f559199a75c459698b8a7c31c.bmp`
[^493e5a1317633f9ed82aca23d2662976]: `code/code_readRuntimeInfo_Lly-img-android-pesdk-ui-utils-a-_493e5a1317633f9ed82aca23d2662976.bmp`
[^createAccessibilityService]: `cfg/createAccessibilityService`
[^10b0ce7f2adf1ba37bbaf970d5acd300]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge$4-_10b0ce7f2adf1ba37bbaf970d5acd300.bmp`
[^bb93bf4c26fc46126ab7b12f83741593]: `code/code_createAccessibilityService_Lcom-google-android-material-slider-BaseSlider-_bb93bf4c26fc46126ab7b12f83741593.bmp`
[^9c23f2ba203bb60d4221f6fb09a901ab]: `code/code_createAccessibilityService_Landroidx-recyclerview-widget-RecyclerView-_9c23f2ba203bb60d4221f6fb09a901ab.bmp`
[^f9b9b83d4558f441f56c303e10cdbf14]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_f9b9b83d4558f441f56c303e10cdbf14.bmp`
[^3bcebfcf93073ef663c23657d0167245]: `code/code_createAccessibilityService_Ld-k-a-a-_3bcebfcf93073ef663c23657d0167245.bmp`
[^3707b4a81714c452dd82600c89e5306f]: `code/code_createAccessibilityService_Landroidx-appcompat-widget-i0-_3707b4a81714c452dd82600c89e5306f.bmp`
[^75197c9a4596d55b74020173eb7c09da]: `code/code_createAccessibilityService_Ld-k-a-a-_75197c9a4596d55b74020173eb7c09da.bmp`
[^0fb2c8ba44ce41429bb983762ac920aa]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_0fb2c8ba44ce41429bb983762ac920aa.bmp`
[^f1b8e9eb2f659442be5aba5b80f9c0ba]: `code/code_createAccessibilityService_Ld-k-a-a-_f1b8e9eb2f659442be5aba5b80f9c0ba.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_createAccessibilityService_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^aee49a929061486f87dcc7de9c2df330]: `code/code_createAccessibilityService_Ld-k-a-a-_aee49a929061486f87dcc7de9c2df330.bmp`
[^0d0c774a17418d04884391cd41468a39]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_0d0c774a17418d04884391cd41468a39.bmp`
[^b4b22d1f74a7ad7c15a9aa7bf9646339]: `code/code_createAccessibilityService_Lcom-google-android-material-textfield-d$a-_b4b22d1f74a7ad7c15a9aa7bf9646339.bmp`
[^49835ca6ac924b9ed75fb89449ffa863]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_49835ca6ac924b9ed75fb89449ffa863.bmp`
[^6a29e4f19be7c76870a55bbc71c9c8f5]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge$2-_6a29e4f19be7c76870a55bbc71c9c8f5.bmp`
[^4e00e0fc297ef9c7e0b7ae929ef7cba5]: `code/code_createAccessibilityService_Lcom-google-android-material-textfield-MaterialAutoCompleteTextView-_4e00e0fc297ef9c7e0b7ae929ef7cba5.bmp`
[^aee49a929061486f87dcc7de9c2df330]: `code/code_createAccessibilityService_Ld-k-a-a-_aee49a929061486f87dcc7de9c2df330.bmp`
[^75197c9a4596d55b74020173eb7c09da]: `code/code_createAccessibilityService_Ld-k-a-a-_75197c9a4596d55b74020173eb7c09da.bmp`
[^e5d1341df5f1d2788fb3fd299cd110b3]: `code/code_createAccessibilityService_Lcom-google-android-material-timepicker-c-_e5d1341df5f1d2788fb3fd299cd110b3.bmp`
[^3707b4a81714c452dd82600c89e5306f]: `code/code_createAccessibilityService_Landroidx-appcompat-widget-i0-_3707b4a81714c452dd82600c89e5306f.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^5a3c3e2d546447067ed1058b89da02a0]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_5a3c3e2d546447067ed1058b89da02a0.bmp`
[^4c2d7b3644e6190975478b202d9b1249]: `code/code_createAccessibilityService_Lcom-google-android-material-snackbar-Snackbar-_4c2d7b3644e6190975478b202d9b1249.bmp`
[^4ce3587911f63d5c5250787cbda9a936]: `code/code_createAccessibilityService_Lcom-google-android-material-textfield-d$d-_4ce3587911f63d5c5250787cbda9a936.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_createAccessibilityService_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^59e55794c58143d9bd60a189d9216fe8]: `code/code_createAccessibilityService_Lzendesk-belvedere-l-_59e55794c58143d9bd60a189d9216fe8.bmp`
[^fc9c5f7bfbdc0718718ddf5679d4f0da]: `code/code_createAccessibilityService_Lcom-google-android-material-snackbar-BaseTransientBottomBar-_fc9c5f7bfbdc0718718ddf5679d4f0da.bmp`
[^4c2d7b3644e6190975478b202d9b1249]: `code/code_createAccessibilityService_Lcom-google-android-material-snackbar-Snackbar-_4c2d7b3644e6190975478b202d9b1249.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^0086b7438d906caaa04aa43e182ddd55]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_0086b7438d906caaa04aa43e182ddd55.bmp`
[^0086b7438d906caaa04aa43e182ddd55]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_0086b7438d906caaa04aa43e182ddd55.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^6536115025cf28aa5eedbbf1320f490a]: `code/code_createAccessibilityService_Lio-flutter-view-AccessibilityBridge-_6536115025cf28aa5eedbbf1320f490a.bmp`
[^listenAccessibilityEvents]: `cfg/listenAccessibilityEvents`
[^f4f4d47ec8718d4542790b8cc6868218]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-SwitchCompat-_f4f4d47ec8718d4542790b8cc6868218.bmp`
[^b3ab42bb1d646309428a6e0f65044d6a]: `code/code_listenAccessibilityEvents_Landroidx-viewpager2-widget-ViewPager2$j-_b3ab42bb1d646309428a6e0f65044d6a.bmp`
[^ae06e08a969706e5ace5e2d71fd778c0]: `code/code_listenAccessibilityEvents_Landroidx-drawerlayout-widget-DrawerLayout$b-_ae06e08a969706e5ace5e2d71fd778c0.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^cd32530947a61228cdef7e37db9469bd]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-button-MaterialButton-_cd32530947a61228cdef7e37db9469bd.bmp`
[^387ee15faf974132074e96aac4696140]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ActionBarContextView-_387ee15faf974132074e96aac4696140.bmp`
[^b582d39a2131ff17544d4c5699bc3ce1]: `code/code_listenAccessibilityEvents_Landroidx-slidingpanelayout-widget-SlidingPaneLayout$a-_b582d39a2131ff17544d4c5699bc3ce1.bmp`
[^1896537b6182835a96104e1e59340717]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-card-MaterialCardView-_1896537b6182835a96104e1e59340717.bmp`
[^0330e38896710bdc44950b4df747777f]: `code/code_listenAccessibilityEvents_Landroidx-core-widget-NestedScrollView$a-_0330e38896710bdc44950b4df747777f.bmp`
[^b902f7d7ba3dd130264748294a133360]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-AppCompatButton-_b902f7d7ba3dd130264748294a133360.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^5a76c1b498380c61f8b7877d882fe8ae]: `code/code_listenAccessibilityEvents_Lcom-bitmovin-android-exoplayer2-ui-DefaultTimeBar-_5a76c1b498380c61f8b7877d882fe8ae.bmp`
[^84ea0d1bd0d5c77e6db723f95140025e]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-LinearLayoutCompat-_84ea0d1bd0d5c77e6db723f95140025e.bmp`
[^3fa4a9882fa5acffeef3f9bab2ebe183]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ScrollingTabContainerView$d-_3fa4a9882fa5acffeef3f9bab2ebe183.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^e41b523b7fd6fd78afbb593513bb15e5]: `code/code_listenAccessibilityEvents_Lcom-google-android-exoplayer2-ui-DefaultTimeBar-_e41b523b7fd6fd78afbb593513bb15e5.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^5a76c1b498380c61f8b7877d882fe8ae]: `code/code_listenAccessibilityEvents_Lcom-bitmovin-android-exoplayer2-ui-DefaultTimeBar-_5a76c1b498380c61f8b7877d882fe8ae.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^18a034a45a443489ddd843b3b3d8fd82]: `code/code_listenAccessibilityEvents_Landroidx-drawerlayout-widget-DrawerLayout$b-_18a034a45a443489ddd843b3b3d8fd82.bmp`
[^262330ed42d16970529b0f77fb62a62a]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge$1-_262330ed42d16970529b0f77fb62a62a.bmp`
[^be10b35f4e03c4452eafcb4c238584c2]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_be10b35f4e03c4452eafcb4c238584c2.bmp`
[^e41b523b7fd6fd78afbb593513bb15e5]: `code/code_listenAccessibilityEvents_Lcom-google-android-exoplayer2-ui-DefaultTimeBar-_e41b523b7fd6fd78afbb593513bb15e5.bmp`
[^40eb0cd93b972c44100e7f3c0f2a9b6d]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_40eb0cd93b972c44100e7f3c0f2a9b6d.bmp`
[^15fa855ac02a9c7b256d4606f262096a]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-SwitchCompat-_15fa855ac02a9c7b256d4606f262096a.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_listenAccessibilityEvents_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^0330e38896710bdc44950b4df747777f]: `code/code_listenAccessibilityEvents_Landroidx-core-widget-NestedScrollView$a-_0330e38896710bdc44950b4df747777f.bmp`
[^7281fcadcabab1482540022b58d000a6]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-RecyclerView$p-_7281fcadcabab1482540022b58d000a6.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^7281fcadcabab1482540022b58d000a6]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-RecyclerView$p-_7281fcadcabab1482540022b58d000a6.bmp`
[^5a76c1b498380c61f8b7877d882fe8ae]: `code/code_listenAccessibilityEvents_Lcom-bitmovin-android-exoplayer2-ui-DefaultTimeBar-_5a76c1b498380c61f8b7877d882fe8ae.bmp`
[^387ee15faf974132074e96aac4696140]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ActionBarContextView-_387ee15faf974132074e96aac4696140.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^3ce57373e05ffb147498469ece6b2366]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager-_3ce57373e05ffb147498469ece6b2366.bmp`
[^18a034a45a443489ddd843b3b3d8fd82]: `code/code_listenAccessibilityEvents_Landroidx-drawerlayout-widget-DrawerLayout$b-_18a034a45a443489ddd843b3b3d8fd82.bmp`
[^e41b523b7fd6fd78afbb593513bb15e5]: `code/code_listenAccessibilityEvents_Lcom-google-android-exoplayer2-ui-DefaultTimeBar-_e41b523b7fd6fd78afbb593513bb15e5.bmp`
[^6fba231545a8f9b50c613228989581d3]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_6fba231545a8f9b50c613228989581d3.bmp`
[^4ce3587911f63d5c5250787cbda9a936]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-textfield-d$d-_4ce3587911f63d5c5250787cbda9a936.bmp`
[^fe6233327ee3ff01fd8f02ed088a726f]: `code/code_listenAccessibilityEvents_Ld-i-p-j0-b-_fe6233327ee3ff01fd8f02ed088a726f.bmp`
[^4b55d10440ac38072d36d30e4b36b687]: `code/code_listenAccessibilityEvents_Ld-i-p-j0-b-_4b55d10440ac38072d36d30e4b36b687.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_listenAccessibilityEvents_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^c90fa2c440dad01756758a2c22556d29]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_c90fa2c440dad01756758a2c22556d29.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_listenAccessibilityEvents_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^d8f1579bb01ce2e2fc1f1bdf3b8c9f7b]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-RecyclerView-_d8f1579bb01ce2e2fc1f1bdf3b8c9f7b.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_listenAccessibilityEvents_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^d8f1579bb01ce2e2fc1f1bdf3b8c9f7b]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-RecyclerView-_d8f1579bb01ce2e2fc1f1bdf3b8c9f7b.bmp`
[^b3ab42bb1d646309428a6e0f65044d6a]: `code/code_listenAccessibilityEvents_Landroidx-viewpager2-widget-ViewPager2$j-_b3ab42bb1d646309428a6e0f65044d6a.bmp`
[^387ee15faf974132074e96aac4696140]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ActionBarContextView-_387ee15faf974132074e96aac4696140.bmp`
[^9c813711310d8deab03dd910375024b7]: `code/code_listenAccessibilityEvents_Ld-i-p-x-_9c813711310d8deab03dd910375024b7.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^0c321f093037d88b429e4049e0dfacbc]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_0c321f093037d88b429e4049e0dfacbc.bmp`
[^387ee15faf974132074e96aac4696140]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ActionBarContextView-_387ee15faf974132074e96aac4696140.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^387ee15faf974132074e96aac4696140]: `code/code_listenAccessibilityEvents_Landroidx-appcompat-widget-ActionBarContextView-_387ee15faf974132074e96aac4696140.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^0330e38896710bdc44950b4df747777f]: `code/code_listenAccessibilityEvents_Landroidx-core-widget-NestedScrollView$a-_0330e38896710bdc44950b4df747777f.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^0330e38896710bdc44950b4df747777f]: `code/code_listenAccessibilityEvents_Landroidx-core-widget-NestedScrollView$a-_0330e38896710bdc44950b4df747777f.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^d9e945237f819092afda4efba1adca67]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-StaggeredGridLayoutManager-_d9e945237f819092afda4efba1adca67.bmp`
[^941a1eefffb8cd96ef5f3331842a8359]: `code/code_listenAccessibilityEvents_Landroidx-viewpager2-widget-ViewPager2$m-_941a1eefffb8cd96ef5f3331842a8359.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^cf7911b64376b24cdd3ee758e57bf1f5]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-LinearLayoutManager-_cf7911b64376b24cdd3ee758e57bf1f5.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^40eb0cd93b972c44100e7f3c0f2a9b6d]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_40eb0cd93b972c44100e7f3c0f2a9b6d.bmp`
[^d9e945237f819092afda4efba1adca67]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-StaggeredGridLayoutManager-_d9e945237f819092afda4efba1adca67.bmp`
[^941a1eefffb8cd96ef5f3331842a8359]: `code/code_listenAccessibilityEvents_Landroidx-viewpager2-widget-ViewPager2$m-_941a1eefffb8cd96ef5f3331842a8359.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^cf7911b64376b24cdd3ee758e57bf1f5]: `code/code_listenAccessibilityEvents_Landroidx-recyclerview-widget-LinearLayoutManager-_cf7911b64376b24cdd3ee758e57bf1f5.bmp`
[^7bca740cd7419a3545d3253912d661a5]: `code/code_listenAccessibilityEvents_Landroidx-viewpager-widget-ViewPager$g-_7bca740cd7419a3545d3253912d661a5.bmp`
[^0c321f093037d88b429e4049e0dfacbc]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_0c321f093037d88b429e4049e0dfacbc.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^d094112098db1c197de38a3a484e1e3e]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_d094112098db1c197de38a3a484e1e3e.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^cd32530947a61228cdef7e37db9469bd]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-button-MaterialButton-_cd32530947a61228cdef7e37db9469bd.bmp`
[^1896537b6182835a96104e1e59340717]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-card-MaterialCardView-_1896537b6182835a96104e1e59340717.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^07eceabdea340d2ea27d81304bfb4932]: `code/code_listenAccessibilityEvents_Lcom-google-android-material-internal-CheckableImageButton$a-_07eceabdea340d2ea27d81304bfb4932.bmp`
[^b576f0e03168c52e9d39ebf25768a5e5]: `code/code_listenAccessibilityEvents_Ld-k-a-a-_b576f0e03168c52e9d39ebf25768a5e5.bmp`
[^40eb0cd93b972c44100e7f3c0f2a9b6d]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_40eb0cd93b972c44100e7f3c0f2a9b6d.bmp`
[^40eb0cd93b972c44100e7f3c0f2a9b6d]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_40eb0cd93b972c44100e7f3c0f2a9b6d.bmp`
[^40eb0cd93b972c44100e7f3c0f2a9b6d]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_40eb0cd93b972c44100e7f3c0f2a9b6d.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^0c321f093037d88b429e4049e0dfacbc]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_0c321f093037d88b429e4049e0dfacbc.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^24a4559cb166b15cb1fe0de6901a61b9]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityBridge-_24a4559cb166b15cb1fe0de6901a61b9.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
[^c7fef7264062be63f3a1fee40bb6df32]: `code/code_listenAccessibilityEvents_Lio-flutter-view-AccessibilityViewEmbedder-_c7fef7264062be63f3a1fee40bb6df32.bmp`
