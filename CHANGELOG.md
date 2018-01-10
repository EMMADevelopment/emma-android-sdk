# CHANGELOG

## Version 4

### 4.2.4 - 10/01/2018
[NEW] New feature Re-Targeting<br>
[IMPROVE] In-app communications improves<br>
[FIX] Fixed bug that was causing the session time calculation was wrong<br>
[FIX] Fixed bug that sometimes produced a wrong behavior on the strip<br>
[FIX] Minor bugs fixes

### 4.2.3 - 20/12/2017
[FIX] Minor bugs fixes

### 4.2.2 - 18/12/2017
[FIX] Fixed bug that added notification title with the app name in Android 7/N notifications<br>
[FIX] Minor bugs fixes

### 4.2.1 - 13/12/2017
[FIX] Multiples bugs fixed

### 4.2.0 - 29/10/2017

[NEW] Added support for Android Oreo (Android 8)<br>
[NEW] Select color for push notification <br>
[IMPROVE] Changes in the style of push notifications<br>
[FIX] Bugs fixed

### 4.1.3 - 08/10/2017

[FIX] Multiples bugs fixed

### 4.1.2 - 20/09/2017
[IMPROVE] Webview flow <br/>
[IMPROVE] Avoid SSL Error on Android version lower than 5.0

### 4.1.1 - 13/09/2017
[NEW] Cancel InAppMessage

### 4.1.0 - 12/09/2017
[NEW] Native Ads <br/>
[NEW] Automated tracking events <br/>
[NEW] Modern method structure <br/>
[IMPROVE] AdBall positioning & performance <br/>
[IMPROVE] Rules: Automatic push now with Deeplinks <br/>
[IMPROVE] Behavior & metrics in Messages <br/>
[FIX] Bugs fixing

### 4.0.9 - 07/07/2017
[IMPROVE] Removed READ_PHONE_STATE permission.

### 4.0.8 - 06/05/2017

[FIX] Fixed strip show problem.

### 4.0.7 - 01/05/2017

[FIX] Multiples bugs fixed

### 4.0.6 - 31/05/2017

[FIX] Banner now opens deeplink correctly in app communication. <br/>
[FIX] Deeplink inside startview don't try to open itself anymore.

### 4.0.5 - 19/05/2017

[FIX] Now deeplinks opens correctly on AdBall. <br/>
[FIX] Fixed crash on adball without startsession.

### 4.0.4 - 16/05/2017

[FIX] Start session when UDID was saved

### 4.0.3 - 11/05/2017

Bug fixed with crash on misconfigured SDK.

### 4.0.2 - 09/05/2017

Bug fixed update user at init with google AID saved.

### 4.0.1 - 28/04/2017

[NEW] - Rules support. <br/>
[NEW] - Event attribute support. <br/>
[IMPROVE] - Banner now uses full screen width. <br/>

## Version 2

### 2.5.9.2 - 09/05/2017

Bug fixed update user at init with google AID saved.

### 2.5.9.1 - 28/03/2017

Bug fixed with UUID.

### 2.5.9 - 23/02/2017
Added capability of open deeplinks in Banner comunications. <br/>
Added capability of open deeplinks in webviews launched by in-app comunications.

### 2.5.8 - 14/02/2017

Bug fixed with close button in webviews when app do more than one call to checkWebView. <br/>
[NEW] Added possibility of configure EMMA SessionKey in Android Manifest.

### 2.5.7 - 03/02/2017

Bug fixed with scroll in webviews.


### 2.5.6 - 25/01/2017

[NEW] Added method `eMMa.setWhitelist(List<String> urls);` to limit urls that will be opened by Webviews.


### 2.5.5 - 17/01/2017

Bug fixed with getUserInfo.


### 2.5.4 - 16/01/2017

[NEW] Added support for custom sounds in push notifications.


### 2.5.3 - 07/11/2016

Minor bugs fixed.


### 2.5.2 - 12/07/2016

[NEW] Added banner callback: <br/>
  `eMMa.checkForBanner(Activity c, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Button button, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, String label, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Map<String,String> params, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Button button, String label, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Button button, String label, int topMarginY, int topMarginX, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Button button, Map<String,String> params, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, String label, Map<String,String> params, eMMaBannerInterface bannerInterface);` <br/>
  `eMMa.checkForBanner(Activity c, Button button, String label, Map<String,String> params, eMMaBannerInterface bannerInterface);` <br/>


### 2.5.0.1 - 10/05/2016

Bug fixed with GCM.


### 2.5.0 - 04/05/2016

Refactor SDK.
