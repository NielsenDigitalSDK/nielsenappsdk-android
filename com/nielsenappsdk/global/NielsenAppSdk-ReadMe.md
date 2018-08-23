

Nielsen App Sdk Release Notes
******************************************************************************************************

Release 6.0.0.4 (5-24-2018)

- If the SDK build target is set to AGF then SDK will send the hello ping to “eu” and “eu-uat” for debug builds. No changes to the non AGF build the default sfcode will continue to be "sdk" and "cert" for debug build.
- The C1 parameter (NUID) will now be sent as encrypted DeviceID.
- New SessionID changes. The sessionID will contain 29 length random characters appended by timestamp.
- Support for multiple SDK instance without any limit.
- New log feature for CAT tool to retrieve the API level information from client apps. This ping will contain the eventType, parameters, SDK version, appid etc.
- Removed Viewability for this release.


Release 5.1.1.26 (7-31-2017)

- Genre parameter will be a part of DCR pings and the value is reflected as part of c44 parameter.
- Merged adModel and adLoadType flags
- Fix for stop event data carried to next session’s duration ping
- Fix for last playhead call that is not processed (when there is no time-gap between the last playhead and end call)

******************************************************************************************************
