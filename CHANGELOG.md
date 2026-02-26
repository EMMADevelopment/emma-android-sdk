# CHANGELOG

## Version 4

## 4.16.0 - 22/02/2026

[NEW] Added setEmail method to set the user's email <br/>
[NEW] Added setUserProfile method to manage the user's profile <br/>
[NEW] Added trackUserTags method to track user tags <br/>
[DEPRECATED] trackExtraUserInfo method deprecated in favor of trackUserTags <br/>
[IMPROVE] Refactored setCustomerId <br/>
[FIX] Added STKPrewarmingViewController to the auto-event blacklist <br/>
[NEW] Added trackPurchase as a new unified method for purchase tracking <br/>
[IMPROVE] Internal refactor renaming order to purchase for improved consistency <br/>
[NEW] Added unregisterPushSystem method to unsubscribe from the push notification system

## 4.15.7 - 13/11/2025

[FIX] ANR when downloading images from push notifications <br/>
[FIX] Crash when receiving push notifications when the configuration is not initialized <br/>
[FIX] Adaptation of the Strip to support edge-to-edge on Android 15 <br/>
[IMPROVE] Improvement of the animation of the text in the Strip <br/>
[IMPROVE] Color management for the status bar and icons in Strip and StartView

## 4.15.6 - 03/10/2025

[FIX] Always call onSessionStarted even if the session is already started

## 4.15.5 - 04/04/2025

[NEW] Added new setUserLanguage method. Allows users to manually set the language instead of relying on auto-detection

## 4.15.4 - 10/03/2025

[FIX] Added cummunication params for NativeAd

## 4.15.3 - 10/02/2025

[IMPROVE] Prism and StartView are now displayed in the correct order, StartView is always displayed on top of any format

## 4.15.2 - 29/12/2024

[IMPROVE] Optimize Proguard rules

## 4.15.1 - 11/10/2024

[FIX] Fixed ANR issue with tag sending when the device's connection is poor or nonexistent. In some cases, this could cause an ANR or a crash in the event of total connection loss

## 4.14.2 - 11/10/2024

[FIX] Fixed ANR issue with tag sending when the device's connection is poor or nonexistent. In some cases, this could cause an ANR or a crash in the event of total connection loss

## 4.15.0 - 26/09/2024

[NEW] Added new install attribution info callback in start session <br/>
[IMPROVE] Sessions with times less than 10 seconds are discarded <br/>
[FIX] Android notification miniature only when notification collapses

## 4.14.1 - 20/08/2024

[FIX] Fixed fatal crash with retrofit2 dependency when app has Android Gradle Plugin v8 and minifyEnabled is true

## 4.14.0 - 11/07/2024

[NEW] Added new method sendDismissedClick to send clicks when inapp is dismissed <br/>
[IMPROVE] PII data saved in preferences is encrypted.

## 4.13.0 - 05/02/2024

[NEW] setCurrencyCode method and startOrder currencyCode param are removed. Currency code is selected in EMMA Dashboard. All prices sent in the order will not be converted by EMMA to a specific currency, they will be interpreted as a unit value <br/>
[NEW] Updated minSdkTarget to Android 21 Lollipop <br/>
[FIX] Some RT clicks can fail if SDK is started before than click is processed.

## 4.12.1 - 28/06/2023

[NEW] Support for notifications with title

## 4.12.0 - 22/02/2023

[NEW] New method to request Android 13 notification permission `requestNotificationsPermission` <br/>
[NEW] New method to check if notifications are enabled `areNotificationsEnabled` <br/>
[NEW] Updated minSdkTarget to Android 19 KikKat <br/>
[FIX] Minor fixes and improves <br/>

## 4.11.4 - 15/11/2022

[NEW] Close webview from web with deeplink ://startview/close

## 4.11.3 - 10/10/2022

[FIX] Sometimes attribution causes ConcurrentModificationException when sending events in different threads.

## 4.11.2 - 05/07/2022

[NEW] Compatibility with Families policy

## 4.11.1 - 16/06/2022

[NEW] Support for Facebook install referrer

## 4.11.0 - 05/05/2022

[NEW] Click types for inapp communications Adball and StartView <br/>
[IMPROVE] Improved performance on events attribution, events are cached and disk reads has been decreased

## 4.10.2 - 01/02/2022

[IMPROVE] New Google Advertising ID policy. **IMPORTANT UPDATE to avoid device loss**

## 4.10.0 - 20/01/2022

[NEW] Notifications with action buttons

## 4.9.6 - 01/02/2022

[IMPROVE] New Google Advertising ID policy. **IMPORTANT UPDATE to avoid device loss**

## 4.9.5 - 10/11/2021

[IMPROVE] Update Android SDK target to 31

## 4.9.3 - 07/10/2021

[FIX] Update network dependency version

## 4.9.2 - 19/08/2021

[IMPROVE] Support with library FCM > 22.0.0 to obtain push token

## 4.9.1 - 01/08/2021

[NEW] New method handleLink to manage applink click in other entry point

## 4.9.0 - 15/03/2021

[NEW] New method to add inapp plugins

## 4.8.1 - 18/02/2021

[FIX] Sometimes restart requests could cause a crash

## 4.8.0 - 12/11/2020

[IMPROVE] Android X migration <br/>
[NEW] New method to update customer id whitout login or register user event <br/>
[FIX] Fixed autogenate udid marked as huawei oaid<br/>
[FIX] Minor fixes and improves

## 4.7.5 - 17/09/2020

[FIX] Fixed crash when startview shows and activity is dying

## 4.7.4 - 07/09/2020

[IMPROVE] Performance improvements at start-up

## 4.7.3 - 14/08/2020

[FIX] Incompatibility with Glide library 4.9

## 4.7.2 - 12/08/2020

[NEW] Huawei attribution

## 4.7.1 - 01/06/2020

[NEW] New method to obtain deviceId

## 4.7.0 - 23/06/2020

[NEW] Integration with Huawei hms push

## 4.6.2 - 02/06/2020

[FIX] Fixed, in new dashboard the adball image looks square. Now is circular

## 4.6.1 - 07/04/2020

[NEW] Click params for install attribution campaigns <br/>
[FIX] Minor bugs.

## 4.6.0 - 27/02/2020

[NEW] Params for campaigns in EMMAInAppMessageInterface <br/>
[FIX] Fixed crash in strip . <br/>
[FIX] Minor bugs.

### 4.5.3 - 27/09/2019

[FIX] Fixed params eatsubx in getUserInfo

### 4.5.2 - 31/05/2019

[NEW] New method to start session in background <br/>
[FIX] Minor bugs fixed

### 4.5.1 - 30/04/2019

[IMPROVE] Public methods in EMMAPushNotificationManager, handleNotification and refreshToken for use an existent FCM service <br/>
[IMPROVE] Internal changes in login/register <br/>
[FIX] Minor bugs fixed

### 4.5.0 - 25/03/2019

[IMPROVE] Replace GCM to FCM for push notification <br/>
[FIX] Fixed problem in Short Url Attribution <br/>
[FIX] Fixed redimension problem in animated gifs for banner <br/>
[FIX] Minor bugs

### 4.4.3 - 21/02/2019

[FIX] Fix crash ConcurrentModification on inapp listeners

### 4.4.2 - 07/02/2019

[FIX] Fix inapp callback onClose() executed with the physical button back <br/>
[FIX] Fixed a crash that occurs, on some occasions, when the SDK is booted and the app goes to the background quickly

### 4.4.1 - 11/12/2018

[FIX] Native Ad request callback

### 4.4.0 - 04/12/2018

[NEW] New listener for check request status (inapp and event) <br/>
[IMPROVE] Changes on inapp and event requests <br/>
[FIX] Fixed bug that caused the method getUserInfo doesn't return data <br/>
[FIX] Fixed minor bugs

### 4.3.2 - 21/11/2018

[FIX] Performance improvement of attribution

### 4.3.1 - 16/11/2018

[FIX] Fixed banner param offset when is added in parent view ID <br/>
[FIX] Fixed minor bugs

### 4.3.0 - 07/11/2018

[NEW] Support for short powlink urls <br/>
[NEW] Support to get install attribution info <br/>
[NEW] Added possibility to add channel name in notifications and new EMMAPushOptions <br/>
[NEW] Support for attribution through Google Play installation referrer API <br/>
[FIX] Location changes <br/>
[FIX] Fixed minor bugs

### 4.2.19 - 07/08/2018

[FIX] Banner show time <br/>
[FIX] Minor bugs fixed

### 4.2.18 - 26/07/2018

[FIX] Fixed crash in offline mode <br/>
[FIX] Minor bugs fixed

### 4.2.17 - 05/07/2018

[FIX] Minor bugs fixed

### 4.2.16 - 27/06/2018

[FIX] Bugs fixed

### 4.2.15 - 13/06/2018

[FIX] Startview with no close action <br/>
[FIX] Minor bugs fixed.

### 4.2.14 - 31/05/2018

[NEW] Unique click retargeting (retargeting 2).

### 4.2.13 - 24/05/2018

[NEW] Disable/enable automatic screen events <br/>
[FIX] Fix bug in versions < 4.4 with play services not installed on device

### 4.2.12 - 23/05/2018

[IMPROVE] GDPR adaptation

### 4.2.11 - 10/05/2018

[NEW] Uninstalls pings

### 4.2.10 - 10/04/2018

[FIX] In some cases version 4.2.9 did not properly download the dependencies by Gradle.

### 4.2.9 - 10/04/2018

[IMPROVE] Open deep links outside applications

### 4.2.8 - 16/03/2018

[NEW] Re-Targeting deep links with inapp CTA

### 4.2.7 - 09/03/2018

[FIX] Fixed problem that causes banner is displayed above the menu

### 4.2.6 - 27/02/2018

[NEW] Multiple Native Ad for a unique template id <br/>
[FIX] Multiples bugs fixed

### 4.2.5 - 12/02/2018

[FIX] Fix location to request permission when the startTrackingLocation method is invoked.

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
