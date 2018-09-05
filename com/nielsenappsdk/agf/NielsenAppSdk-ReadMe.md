

Nielsen App Sdk Release Notes
******************************************************************************************************
Release 6.1.0.1 (08-31-2018)

- Added new RTVOD feature.
- Davty enhancements for DTVR and DRM.
- Fix for static type independent of other types(content&ad).
- Fix for auto-stop called on DTVR when there is a type change on DCR with hybrid approach.
- Fix for sesid(c59) reporting as 0 when forward or backward slashes were present in the assetid with url encoded in the CMS mapping.

Release 6.0.0.4 (5-24-2018)

- If the SDK build target is set to AGF then SDK will send the hello ping to “eu” and “eu-uat” for debug builds. No changes to the non AGF build the default sfcode will continue to be "sdk" and "cert" for debug build.
- The C1 parameter (NUID) will now be sent as encrypted DeviceID.
- New SessionID changes. The sessionID will contain 29 length random characters appended by timestamp.
- Support for multiple SDK instance without any limit.
- New log feature for CAT tool to retrieve the API level information from client apps. This ping will contain the eventType, parameters, SDK version, appid etc.
- Removed Viewability for this release.

******************************************************************************************************