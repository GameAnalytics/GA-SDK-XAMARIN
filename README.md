[![NuGet](https://img.shields.io/nuget/v/GameAnalytics.XAMARIN.SDK.svg)](https://www.nuget.org/packages/GameAnalytics.XAMARIN.SDK)
[![NuGet](https://img.shields.io/nuget/dt/GameAnalytics.XAMARIN.SDK.svg?label=nuget%20downloads)](https://www.nuget.org/packages/GameAnalytics.XAMARIN.SDK)

# GA-SDK-XAMARIN
GameAnalytics Xamarin SDK.

Documentation can be found [here](https://gameanalytics.com/docs/xamarin-sdk).

If you have any issues or feedback regarding the SDK, please contact our friendly support team [here](https://gameanalytics.com/contact).

Changelog
---------
<!--(CHANGELOG_TOP)-->
**5.1.1**
* added functionality to force a new user in a/b testing without having to uninstall app first, simply use custom user id function to set a new user id which hasn't been used yet

**5.1.0**
* added custom event fields feature

**5.0.0**
* Changed user identifier logic in preparation for Google changes to GAID. User id for a new install is now a randomised GUID. Existing installs that update SDK will continue using previous identifier logic. It is recommended to update as soon as possible to reduce impact on calculated metrics.

**4.3.8**
* it should now be possible to not show idfa consent dialog if you don't have any third party code that needs to use idfa (ios)
* prepared for google advertising identifier changes (will not use google advertising identifier when user has opted out) (android)

**4.3.7**
* added idfa consent status field to events

**4.3.6**
* updated client ts validator

**4.3.5**
* fixed dependencies for iOS (min. XCode 12 required)

**4.3.4**
* removed memory info from automatic crash reports

**4.3.3**
* corrected ad event annotation

**4.3.2**
* fixed removal of google play services dependencies
* improved user identifer flow for ios (ios)

**4.3.1**
* correction to ad event function names

**4.3.0**
* added ad event

**4.2.0**
* updated user identifier flow to prepare for iOS 14 IDFA changes (ios)

**4.1.1**
* fixed progression events with scores (android)

**4.1.0**
* exposed functions to get AB testing id and variant id

**4.0.2**
* added session_num to init request

**4.0.1**
* removed facebook, gender and birthyear methods
* added auto detect app version for build field option

**4.0.0**
* Remote Config calls have been updated and the old calls have deprecated. Please see GA documentation for the new SDK calls and migration guide
* A/B testing support added

**3.1.0**
* added enable/disable event submission function

**3.0.1**
* fixed business event validation

**3.0.0**
* added command center functionality

**2.4.0**
* added custom dimensions to design and error events
* added accept terms for sign up dialog

**2.3.10**
* bug fix for end session when using manual session handling

**2.3.9**
* session length precision improvement

**2.3.8**
* added bundle_id, app version and app build tracking
* added app signature and channel id (which app store was the app installed from)(android)
* added IMEI as fallback option for identifier when Google AID and Android ID is not available on the device (requires to add optional READ_PHONE_STATE permission)(android)

**2.3.7**
* fixed missing libraries

**2.3.6**
* possible to set custom dimensions and demographics before initialize

**2.3.5**
* bug fix to design events sent without value (android)

**2.3.4**
* * fixed user_id tracking for iOS 10 (ios, tvos)
* small fix related to manual session handling (android)

**2.3.3**
* added manual session handling
* fixed bug for client timestamp handling and session length in certain edge cases

**2.3.2**
* external storage read and write permissions are now optional (android)

**2.3.1**
* fixed nuget package for tvOS (tvos)

**2.3.0**
* added support for tvOS (tvos)
* fixed bug related to network changes for Android API level 23 and above (android)

**2.2.2**
* Minor bug fix for various event types (ios)
* Add-in has been updated to work with Xamarin 6.x (add-in)

**2.2.1**
* Google Play Services libraries updated to version 8.4.0 (android)

**2.2.0**
* feature for using a custom user id
* fix testflight issue with user id generation (ios)

**2.1.0**
* submit errors functionality added

**2.0.0**
* altered jailbreak check causing ios9 warning (ios)
* library / framework now compiled with bitcode (ios)
* restructuring to prepare for tvOS (ios)
* new java-only implementation (android)
* install size reduced (android)

**1.2.1**
* android.permission.WRITE_EXTERNAL_STORAGE not needed anymore (android)

**1.2.0**
* fixed tracking bug with ad opt out enabled (android)

**1.1.2**
* no network connection bug fix (android)

**1.1.1**
* fix related to connection changes (android)

**1.1.0**
* improved code structure (android)
* built library with Xcode7 (iOS 9.0)
* minor tweaks

**1.0.1**
* Xamarin SDK for V2 API
* iOS and Android support
* progression event
* business event validation
* resource event
* custom dimensions
