# CHANGELOG

## Version 4

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
