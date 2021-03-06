# Changelog

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
