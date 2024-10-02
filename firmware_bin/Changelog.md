# Changelog

## Release 1.10

### All models with temperature sensors:
- Added support for a 24-hour temperature history graph displaying 'Circuit 1 flow', 'Circuit 1 return', 'Activation', and 'Hysteresis'. For the 'Activate when &Delta;T below' and 'Activate when &Delta;T above' pump activation modes, the '&Delta;T' value is also shown. Part of the background changes during periods when the pump is running.
- Improved temperature sensor detection with enhanced reliability in identifying and managing sensors.

### All models:
- Added Quatt heat pump autodetect functionality, which simplifies the trigger setup process by automatically detecting Quatt devices on the network.
- Moved 'Temperature sensor rescan' and 'Restart/Reset device' to the new 'System tools' section.
- Added 'Manual auto run' functionality for manual pump operation for a set time, typically used for testing or maintenance.
- Improved request memory management by eliminating the need for an additional buffer, resulting in more efficient resource utilization during requests and reducing potential memory overhead.
- Removed the 6 KB limit for non https trigger requests, allowing for larger payloads. However, caution is advised to use excessively large payloads due to the memory constraints of embedded devices.

## Release 0.95

### All models:
- Added support for the new SPC-SC model, a socket version of the SPC without temperature sensors.
- Changed the URL of <i>Download a firmware file</i> on the <i>Update</i> page so that it opens the location of the firmware files for the current model and hardware ID.

## Release 0.94

### All models:
- Added a detailed logbook entry in case the pump was triggered and the JSON trigger returned an error.
- Resolved an issue where negative activation was not permitted, even though it is valid in certain cases for the 'Activate when &Delta;T below' pump activation mode.
- Resolved an issue where triggers would not match float values if the JSON field was a string but the contents was a float value.

## Release 0.93

### All models:
- Added 'Activate when &Delta;T above' and 'Activate when &Delta;T below' as pump activation mode.
- Added pump activation reason to the SPC page and as a Home Assistant sensor (autodiscovery).
- Added a logbook capturing events related to the pump's start and stop times.
- Added support for 'Outside (including)' as a trigger condition. This enables matching the trigger outside a range of values.
- Added 'Uptime' as a diagnostic sensor for Home Assistant (autodiscovery), containing the number of seconds the device has been powered on.
- Added units where applicable to the configuration items on the configuration pages.
- Resolved an issue where the hysteresis was not taken into account when deactivating the pump. 
- Resolved an issue where the new firmware check was not invoked under all conditions.

## Release 0.92

### All models:
- Added led blinking to indicate that the device is in access point mode (configure WiFi network).
- Added option to specify default pump behavior when JSON trigger returns an error.
- Added link to the changelog on the update page.
- Changed Quatt example on the trigger page to use qc.supervisoryControlMode 
- Resolved an issue where the 'Between (including)' as a trigger condition was not persisted between restarts.
- Resolved an issue where the refresh page timer would run out before the update of the firmware was completed.

## Release 0.91

### All models:
- Added support for 'Between (including)' as a trigger condition. This makes it possible to specify a range of values on which the trigger matches.
- Added the possibility to add authentication (http header) to the trigger request.
- Resolved an issue where triggers would not match float values if the JSON field was a string but the contents was a float value.
- Resolved an issue of incorrect handling of not connected sensors while rescanning.
- Resolved an issue where the autorun timer would incorrectly activate when the configuration was saved.
- Resolved an issue where the trigger would crash in case no json path was specified but the url was.

## Release 0.90

### All models:
- Initial beta release
