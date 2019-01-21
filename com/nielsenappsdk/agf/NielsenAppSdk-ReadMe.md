

Nielsen App Sdk Release Notes
******************************************************************************************************
Release 6.2.0.0 (01-21-2019)

- Fixed an issue causing crashes on certain Android devices using specific older Qualcomm chipsets with OEM modifications to OS 
- Implemented buildversion naming convention Help monitor SDK flavor (artifactory/Adobe Launch/standalone/etc) and market (AGF/Global)
- Location measurement has been removed from the SDK code. Location frameworks were there previously but disabled, now it’s fully removed to avoid confusion from noticing it being included at all
- Fixed the getOptoutStatus() api, so that user can call it in main thread
- Fixed the parsing error happening when clientid/vcid provided as empty in metadata. In case where clientid/vcid is not supplied, SDK will take default from config instead of using the blank value
- Align for FW detection with BSDK where for DCR use a variable nol_cmsIntrvlGp (value is 2) rather than nol_id3IntrvlGp(15). Detect forward event with >2 seconds of scrub for DCR instead of 15 seconds as currently

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
