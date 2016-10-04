# TapResearch-Unity-SDK
TapResearch Unity SDK v1.1.0

For additional information, please see the [TapResearch Unity SDK integration guide](https://www.tapresearch.com/docs/unity-integration-guide).

## v1.1.0
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

Other platforms:

[TapResearch Android SDK](https://github.com/TapResearch/TapResearch-Android-SDK)  
[TapResearch Android SDK integration guide](https://www.tapresearch.com/docs/android-integration-guide)

[TapResearch iOS SDK](https://github.com/TapResearch/TapResearch-iOS-SDK)  
[TapResearch iOS SDK integration guide](https://www.tapresearch.com/docs/ios-integration-guide)

[TapResearch JavaScript SDK integration guide](https://www.tapresearch.com/docs/javascript-integration-guide)
