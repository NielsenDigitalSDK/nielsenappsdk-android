Nielsen App Sdk Release Notes
******************************************************************************************************
Note: Starting Nielsen SDK 9.0.0.0 new modules/features are written in Kotlin language interoperable with existing java code. Please add Kotlin support dependency in your Java only app, to take advantage of these module/features as below: 

 org.jetbrains.kotlin:kotlin-stdlib 

Nielsen SDK 9.4.0.0 is compiled with Kotlin 1.8.0, please align Kotlin version in your app to avoid any incompatibility issues between app and sdk module. 

Release 9.4.0.0 (07-09-2024)

. Support for content tracking and no-tracking domains across sdk flavors and products.
. Upgraded SDK to use Java 11 and Kotlin 1.8.0.
. Other bug fixes and enhancements.

Release 9.3.0.0 (05-10-2024)

. Support for capturing user opt-out during initialization.

Release 9.2.0.0 (09-27-2023)

. DCR Static recognizing metadata with changed assetID for new impressions.
. Limiting ping retries during https failures.
. Other bug fixes and enhancements.

Release 9.1.0.0 (03-31-2023)

. DCR Static duration measurement for individual page section/assets.
. Support to enable Viewability feature by product (DCR, DTVR).
. Other bug fixes and enhancements.

Release 9.0.0.0 (10-07-2022)

. Viewability measurement for DTVR, DCR Content and DCR Ad products. 
. Audibility measurement for DTVR, DCR Content and DCR Ad products.
. Kotlin-Java interoperability implementation in SDK.
. Other bug fixes and enhancements.

Release 8.2.0.0 (03-21-2022)

. Support for EMM AGF AdID-less solution.
. Enabled SDK to capture network availability changes.
. Removed the usage of deprecated network classes.
. Other bug fixes and enhancements.

Release 8.1.0.0 (06-28-2021)

. Support for SDK build variants - AD/NoAD/NoID.
. Support to indicate ID used for AD build variant - AD ID vs Android ID.
. Support to capture Hashed email and UID.
. Support to collect SDK diagnostic data.
. Other bug fixes and enhancements.

Release 8.0.0.0 (10-05-2020)

. FPID and VendorID support.
. Support for Android apps running on ChromeOS.
. Support for Xamarin cross platform framework.
. Other bug fixes and enhancements.

Release 7.2.0.0 (05-18-2020)

. DTVR AQH and IVD requirements for End and pause timeout
. Support for Hybrid app webview measurement
. Support for Hybrid app react native webview measurement
. Support for react native measurement
. Other Bug Fixes and Enhancements

Release 7.1.0.0 (12-9-2019)

. Application background/foreground state auto-detection (AndroidX)
. Fixed forward rewind evdata containing negative values
. Offline viewing measurement enhancements
. Revisited precedence logic for sfcode parameter
. Using default value for incorrect adModel parameter
. Defaulting isLive parameter value on channel change

Release 6.2.0.0 (02-04-2019)

. Removal of Location Module from SDK Code.
. Fixed the getOptoutStatus() api, so that client can call it in main thread.
. Fixed the parsing error happening when clientid/vcid provided as empty in metadata.
. Align AppSDK for FW detection with BSDK for DCR measurement.
. Other enhancement and fixes.

Release 6.1.0.1 (08-31-2018)

. Added new RTVOD feature.
. Davty enhancements for DTVR and DRM.
. Fix for static type independent of other types(content&ad).
. Fix for auto-stop called on DTVR when there is a type change on DCR with hybrid approach.
. Fix for sesid(c59) reporting as 0 when forward or backward slashes were present in the assetid with url encoded in the CMS mapping.

Release 6.0.0.4 (5-24-2018)

. If the SDK build target is set to AGF then SDK will send the hello ping to “eu” and “eu-uat” for debug builds. No changes to the non AGF build the default sfcode will continue to be "sdk" and "cert" for debug build.
. The C1 parameter (NUID) will now be sent as encrypted DeviceID.
. New SessionID changes. The sessionID will contain 29 length random characters appended by timestamp.
. Support for multiple SDK instance without any limit.
. New log feature for CAT tool to retrieve the API level information from client apps. This ping will contain the eventType, parameters, SDK version, appid etc.
. Removed Viewability for this release.

For integration help, visit https://engineeringportal.nielsen.com/docs/DCR_&_DTVR
******************************************************************************************************
