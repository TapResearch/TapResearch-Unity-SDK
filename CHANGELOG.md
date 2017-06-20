# Changelog

## v1.3.2
- iOS v1.3.1
- Android v1.3.2
- **New Features:**
  - Multi currency support please note that the rewards callback signature was changed to  
  ~~~~
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
