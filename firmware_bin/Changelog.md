# Changelog

## Release 0.91

### All models:
- Added support for 'Between (including)' as a trigger condition. This makes it possible to specify a range of values on which the trigger matches.
- Added the possibility to add authentication (http header) to the trigger request.
- Fixed an issue where triggers would not match float values if the JSON field was a string but the contents were a float value.
- Fixed an issue of incorrect handling of not connected sensors while rescanning.
- Fixed an issue where the autorun timer would incorrectly activate when the configuration was saved.
- Fixed an issue where the trigger would crash in case no json path was specified but the url was.

## Release 0.90

### All models:
- Initial beta release
