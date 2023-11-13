# Changelog

## Release 0.92

### All models:
- Added led blinking to indicate that the device is in access point mode (configure WiFi network).
- Added option to specify default pump behavior when JSON trigger returns an error.
- Added link to the changelog on the update page.
- Changed Quatt example on the trigger page to use qc.supervisoryControlMode 
- Fixed an issue where the 'Between (including)' as a trigger condition was not persisted between restarts.
- Fixed an issue where the refresh page timer would run out before the update of the firmware was completed.

## Release 0.91

### All models:
- Added support for 'Between (including)' as a trigger condition. This makes it possible to specify a range of values on which the trigger matches.
- Added the possibility to add authentication (http header) to the trigger request.
- Fixed an issue where triggers would not match float values if the JSON field was a string but the contents was a float value.
- Fixed an issue of incorrect handling of not connected sensors while rescanning.
- Fixed an issue where the autorun timer would incorrectly activate when the configuration was saved.
- Fixed an issue where the trigger would crash in case no json path was specified but the url was.

## Release 0.90

### All models:
- Initial beta release
