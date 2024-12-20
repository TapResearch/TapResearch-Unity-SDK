# Changelog

> <span style="background-color: #FFFF00"> **_NOTE:_** A 3.2.4 and later SDKs are available as a code-signed iOS SDK build with a PrivacyInfo.xcprivacy file.</span>

> <span style="background-color: #FFFF00"> **_NOTE:_** 2.5.18 and later Legacy 2.5.x SDKs are available as a code-signed iOS SDK build with a PrivacyInfo.xcprivacy file.</span>

## v3.5.2
* Update Android SDK to 3.5.1.
  - Fixed UI insets issue in Survey Wall on devices running Android 15 (api 35)
  - Handle onBackPressed issue when enableOnBackInvokedCallback is true on api 33+

## v3.5.1
* Update iOS SDK to 3.5.2.
  - Surveys callback issue fixed.

## v3.5.0
* Update iOS SDK to 3.5.1.
  - Added new callback setters for rewards and Quick Questions.
  - Updated handling of some malformed survey URLs.
  - Improved internal logging.
* Update Android SDK to 3.5.0 with bridge 3.5.0.
  - Added new callback setters for rewards and Quick Questions.
  - Fixed parse bug when errors are reported.
  - Improved internal logging.
* Update included example to show reward and Quick Questions data callbacks setters.

## v3.4.1
* Add Survey Wall Preview.
* Update iOS SDK to 3.4.1.
* Update Android SDK to 3.4.0 wiht bridge 3.4.0.
* Update included example to show Survey Wall Preview.

## v3.2.8
* Update iOS SDK to 3.2.10.

## v3.2.7
* Update Android SDK to 3.3.4.
* Update iOS SDK to 3.2.8.
* Adding isReady() call.

## v3.2.6
* Update Android SDK to 3.3.0.
  - Ability for SDK to self-heal
  - Handle rare error conditions gracefully, such as the unforeseen inability to create new WebView object
  - More logging to be able to diagnose and troubleshoot mentioned conditions
  - Add stack trace and memory snapshot to remote logger
  - Use 'default' WebView caching to improve loadUrl performance

## v3.2.5
* Update iOS SDK to 3.2.6.
* Update Android SDK to 3.3.0-alpha01.
* Update included example scene and scripts.

## v3.2.4
* Send correct error packet from iOS bridge to C#.

## v3.2.3
* Update native iOS SDK to 3.2.5
  - Code-signed iOS framework
  - Added privacy XML to iOS framework
  - iOS banner display fix
  - Additional anti-fraud measures
  - Quick questions response callback
  - Added support for clear previous attributes
* Android
  - Updated to Android 3.2.8 native SDK
  - Added support for clear previous attributes
  
## v3.2.1-beta2
- Update native iOS SDK to 3.2.4.

## v3.2.1-beta1
- Update native Android SDK to 3.2.2.
- Update native Android bridge to 3.2.1-beta.
- Update native iOS SDK to 3.2.3.

## v3.1.0-beta4
- Update native Android SDK v3.1.1-beta3.
- Update native iOS SDK 3.1.0-beta8.

## v3.1.0-beta3
- Update Android SDK to v3.1.0-beta12 and bridge to v3.1.0-beta8.
- Update iOS SDK to v3.1.0-beta5.
- Updated native and C# files to accommodate native SDK changes.

## v3.1.0-beta2
- Rebuild package to include all iOS framework files.

## v3.1.0-beta1
- Update Android SDK and bridge to v3.1.0-beta5.
- Update iOS SDK to v3.1.0-beta2.
- Updated native and C# files to accommodate native SDK changes.

## v3.0.0-beta4
- Update Android SDK and bridge.

## v3.0.0-beta3
- Update iOS SDK to dismiss a banner when tapping outside the banner.

## v3.0.0-beta2
* Fixed JVM and Java support for Android.

## v3.0.0-beta1
### This is a breaking change!
* Upgrade the Android SDK to v3.0.0-beta1.
* Upgrade the iOS SDK to v3.0.0-beta2.
* SDK rewritten for stability, simplicity, and performance.
* Added ability for some realtime feature updates and bug fixes.
* Partial screen interstitials and banners.
* Removed the need to store placement objects.
* Improved error reporting.

## v2.5.19
* Upgrade the iOS SDK to v2.5.14.
* Upgrade the Android SDK to v2.5.17.
* SDKs have improved internal logging.

## v2.5.18
* iOS: No longer sending placement unavailable message when placement is being displayed.

## v2.5.17
* Update iOS SDK to 2.5.13 with orientation fix

## v2.5.16
* Update Android SDK to 2.5.16 with orientation fix
* Update iOS SDK to 2.5.12 with orientation fix

## v2.5.15
* Android changes:
- Undo force portrait mode
- Update SDK version string to 2.5.15

## v2.5.14
* Android changes:
 - Force portrait-mode in Survey Wall via manifest XML not via code - fixes a tablet issue.
 - Remove unnecessary PlacementUnavailable callback after the Survey Wall has been closed.
 - Handle edge-case if SDK is initialized more than once at the same time.
 - Update SDK version string to 2.5.14

## v2.5.13
* iOS framework updated to 2.5.11 with PrivacyInfo.xcprivacy file and code-signed.

## v2.5.12
* Update reward collection listener setter
* Android Bridge update to 2.5.6

## v2.5.11
* Fixed an issue with rewarding on SDK startup.
* Android Bridge update to 2.5.5

## v2.5.10
* Improved offers support.
* Android SDK 2.5.12
* iOS SDK 2.5.10

## v2.5.9
* Update to support offers
* Android SDK v2.5.11
* iOS SDK 2.5.9

## v2.5.8
* Remove erroneous setting of iOS deployment version from BuildPostprocessoriOS.cs.

## v2.5.7
* Removing accidental EDM inclusions.

## v2.5.6
* Upgrade the Android SDK to v2.5.8.

## v2.5.5
* Upgrade the iOS SDK to v2.5.8.
* Upgrade the Android SDK to v2.5.7.

## v2.5.4
* Upgrade the iOS SDK to v2.5.7.

## v2.5.3
* Upgrade the Android SDK to v2.5.5.
* Upgrade the iOS SDK to v.2.5.6.
* Fixed an error that prevented Google rewards from returning to C#.

## v2.5.2
* Upgrade the iOS SDK to v2.5.5.

## v2.5.1
* Replaced directory copy with replace.
* Corrected some bridge-to-c# message names.

## v2.5.0
* Embedded frameworks added for UnityPackage.
* Removed reliance on Cocoapods for iOS.
* Upgrade the Android SDK to v2.5.4.
* Upgrade the iOS SDK to v2.5.4.

## v2.4.2
* Fix for potential missed reward.
* Fix for offer staying unavailable after showing it.
* Navigation bar styling fix.
* Expose version in Unity bridge.

# v2.4.1
* Improved stability.
* Removed usage of deprecated iOS functions.
* Fixed an issue that caused a run-away cache.
* Fixed a compatibility issue with pure Swift projects.

# v2.4.0
* Upgrade the Android SDK to v2.4.0.
* Update the iOS SDK cocoapod version to v2.4.0.

# v2.3.1
* Upgrade the Android SDK to v2.3.1.
* Update the iOS SDK cocoapod version to v2.3.1u.

# v2.3.0
* Upgrade the Android SDK to v2.3.0.
* Update the iOS SDK cocoapod version to v2.3.0u.
* Change bridges for when custom parameters are passed to the SDK.
* Change bridges to handle new placement callbacks.

# v2.2.1
* Upgrade the Android SDK to v2.2.1.
* Update the iOS SDK cocoapod version to v2.0.21.

# v2.2.0
* Upgrade the Android SDK to v2.2.0.
* Update the iOS SDK cocoapod version to v2.0.20.
* Update bridges to include array-based reward callback.

# v2.1.3
* Upgrade the Android SDK to v2.0.15
* Upgrade the iOS SDK to v2.0.15
* Update postBuildProcess for iOS to update Podfile for v2.0.15 of SDK.

# v2.1.2
* Unity 2019 iOS compatibility fix
* Upgrade the iOS SDK to v2.0.11

# v2.1.1 (Not backward compatible)
* Moving all the classes to TapResearch namespace
* Managing all the dependencies with [External Dependency Manager for Unity](https://github.com/googlesamples/unity-jar-resolver)
* Introducing Custom Parameters

# v2.0.8
* Fix - Android secure url handling fix

# v2.0.7
* iOS 13 full screen window support
* Fix session identifier cookie storage

# v2.0.6
* Fix - iOS post processing scripts not executing on Unity2018

# v2.0.5
* Android - Support non secure urls

# v2.0.4
* More survey availablity
* Fix - Android 4.+ back button crashes
* Fix - Android crash when closing the unity app
* Fix - iOS initialize on Restart
* Fix - Android fix in app rewards

# v2.0.3
* Fix the callbacks status

# v2.0.2
* Support Pure Spectrum surveys

## v2.0.1
* Send a placement response when the SDK isn't ready
* Bug fixes

## v2.0.0
* Introducing TRPlacement to evaluate availability and to display the survey wall
* Introducing TRReward to handle in app rewards

## v1.4.0
* New method `bool IsSurveyAvailableForIdentifier(const char *offerIdentifier)`
* Fix android app lifecycle issues

## v1.3.9
* Android v1.4.0
* iOS v1.3.9
* Unity 2017 support
* New methods
  - `TapResearch.SetNavigationBarText ("<Navigation title text")`
  -	`TapResearch.SetNavigationBarTextColor ("<hex color string e.g #ffffff")`
  -	`TapResearch.SetNavigationBarColor ("<hex color string e.g #ffffff")`
* New survey status with placement identifier parameter
    - `TapResearch.OnSurveyAvailableWithPlacement`
    - `TapResearch.OnSurveyNotAvailableWithPlacement`
    - `TapResearch.OnSurveyModalOpenedWithPlacement`
    - `TapResearch.OnSurveyModalDismissedWithPlacement`



## v1.3.8
- Android v1.3.8

## v1.3.7
- Android v1.3.6
- iOS v1.3.7

## v1.3.6
- Android v1.3.5
- iOS v1.3.6

## v1.3.5
- Android v1.3.4

## v1.3.4
- iOS v1.3.4
- Android v1.3.3

**New Features**

- Adding the offer identifier to the rewards callback, please note the callback signature was chage to
~~~~c-sharp
  private void OnDidReceiveReward(int quantity, string transactionIdentifier, string currencyName, int payoutEvent, string offerIdentifier)
  {
      // Handle reward logic here
  }
~~~~
- Bug Fixes

## v1.3.3
- iOS can't show survey when passing an offer identifier

## v1.3.2
- iOS v1.3.1
- Android v1.3.2
- **New Features**
  - Multi currency support please note that the rewards callback signature was changed to
~~~~c-sharp
  private void OnDidReceiveReward(int quantity, string transactionIdentifier, string currencyName, int payoutEvent)
  {
      // Handle reward logic here
  }
~~~~
  - Multi offer support
  - Surveys availability callbacks

## v1.1.2
---
- iOS v1.2.1
- Android v1.2.3
  - Bug Fixes
  - New activity definition. See the unity integration guide for details.

## v1.1.1
---
- iOS v1.2.1
- Android v1.2.1 -- TRSurveyActivity now inherits from Activity.

## v1.1.0
---
- iOS v1.2.1
- Android v1.2.0
- In-app webviews! Your users will stay inside the app as they complete TapResearch surveys.
- Multi-language support
- Bug fixes
- **Important changes**:
  - Delegate callbacks
    - OnSurveyDialogDismissed no longer has a parameter -- OnSurveyDialogDismissed (bool cancelled) -> OnSurveyDialogDismissed ()
    - Added OnSurveyModalOpened ()
  - **Android** showSurvey() now starts a new activity -- remember to update your AndroidManifest.xml file. See the integration guide for further instructions.
