# Changelog

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
