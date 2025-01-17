---
layout: page
title: CHANGELOG
include_in_header: true
---

# Changelog

v0.18.0

* Added Vehicle Manager
* Added Ride Merging
* Support for Balance Input Configuration
* Display signal strength with BLE scan results
* Prefer GPS option is applied outside log viewer
* Improve BLE connectivity
* Other fixes

v0.17.1

* Fix average speed computation in share file summary
* Do not re-display connection dialog if dismissed
* Resetting BLE buffer if data alignment is lost
* Allow more time for initialization messages to be received
* Widen time & distance column of RideLogging listView
* Fix FOC wizard's battery amps text controllers
* Start BMS cell count from 1
* Display balancing cells with positive value and orange color
* Hiding BMS SoC when value equals 50% for Flexi users
* Using radio selection for Single, Dual, Quad ESC modes

v0.17.0

* Allow GPS speed and distance to be displayed in log
* Long press log entry to view quick statistics
* Display Fahrenheit temperatures in log viewer when enabled
* Fix wheel diameter conversion
* Fix initial Volts gauge value
* Other fixes and improvements
* Including Robogotchi 0.10.1 firmware

v0.16.1

* Fix max temperature realtime gauge (oops)
* Testing fix for backgrounded iOS disconnects

v0.16.0

* Added Help & Support dialog to the menu
* Implement syncstart command
* Display board avatar on map with chart selection
* Display max battery amps on map
* Improved dialog for selected map events
* Fix for known devices after importing data backup
* Improvements to the sync process
* Testing fix for backgrounded iOS disconnects

v0.15.1

* Fix battery remaining (sorry)
* Fix watt hours/distance on graph with imperial enabled
* Removed dismiss message from connection dialog

v0.15.0

* Added feature to export and import your FreeSK8 state
* Moved configuration tab to end of list
* Added UTC offset to log file header
* Display Icon in AppBar when performing Sync
* Fix flicker smart BMS cell data
* Fix flickering board avatar in configuration view
* Retry file if sync produces incorrect file size
* Fix logic for determining maximum ESC temp with multiple ESCs
* Fix long floating point values in input configuration
* Other fixes and improvements

v0.14.2

* Fix Android picture taking permission
* Fix long decimal values in log viewer
* Average speed computed when moving
* Fix battery remaining when charged >100%
* Make shared debug log easier to read
* Display Single, Dual or Quad with Wh/distance
* Ask to stop if logging when performing sync
* Address Flutter 2.0 depreciations
* Other improvements

v0.14.1

* All the same greatness as 0.14.0 without the failure to launch
* Fixed build issue causing Bluetooth to not work
* Updated project dependencies

v0.14.0

* Display Robogotchi priority alert status
* Display Robogotchi audio snooze duration
* Allow Robogotchi snooze duration to be set
* Show distance with ride log entries
* Fixes for decimal input using ','
* Fixes for sync with invalid contents
* Fix display of new telemetry packet
* Fix order of operations for Wh/time calculation
* Compute ESC speed and distance with log files
* Fixes for gear ratio and wheel diameter input
* Fixes for chart in log file viewer
* Update charting library
* Upgrade to Flutter 2.0
* Rename ESC Configurator to Motor Configuration
* Other fixes and improvements

v0.13.2

* Send and expect UTC time from Robogotchi
* Show map icon for current graph selection
* Requesting battery_level from ESC
* Cosmetic changes to Calendar view

v0.13.1

* Fix processing of duty cycle when parsing logs
* Display logged distance and energy consumption
* Fix length of battery and motor current values in real time data

v0.13.0

* Process GPS time synchronization from log files
* Create debug log that can be shared with developers
* Automatically include timezone with Robogotchi configuration
* Zoom ride map to route in log file viewer
* Fixes for disconnected device indication
* Change color interpolation for map polyline
* Other fixes and improvements

v0.12.1

* Fixes for opening log files
* Fix Connected dialog flashing on repeated requests
* Fix spelling in Robogotchi update dialog
* Show ability to change between List and Calendar views

v0.12.0

* Added TCP Bridge to provide ESC data to other applications
* Fix long decimal values seen in the ESC Configurator
* Fixes for switching between menu items
* Simplify the PPM Calibration routine
* Fixes for Real Time data view with Multi ESC enabled
* Display current initialization step in Connection dialog
* Added reset button to Speed Profiles
* Improvements to the Robogotchi Firmware update process
* Adjust padding in Input Configuration view

v0.11.0

* Added Robogotchi firmware updater
* Support for VESC FW5.2
* Fixes for mosfet and esc temperature delta processing
* Change in ESC packet processing if data alignment is lost

v0.10.0

* Support for editing input configuration
* Re-enabled Pan and Zoom behavior on the ride log chart
* Added button for selecting connected ESC settings
* Estimate total time remaining in sync
* New rides can be sorted by watt hours consumed
* Displaying consumption in ride log viewer
* Show Robogotchi firmware version notification after initialization
* Allow connection to remain open if ESC is incompatible
* Color GPS route on map based on speed
* Other fixes and improvements

v0.9.0

* New logging file format
* Reduced sync time
* Estimate sync time remaining
* Swipe right in ride logging list view to share CSV
* Support for smart BMS on CAN ID 10 or 11
* Updated map icons
* Map centers on chart selection
* Display top speed and highest ESC temp on map
* Increase map size for larger devices
* Reduced points rendered on chart and map
* New secret "feature"
* Other fixes and improvements

v0.8.0

* Sharable fault reports
* Display faults observed since power up
* Chart in ride log viewer highlights faults
* Data popup in ride log displays fault code
* Faults are displayed on map when viewing ride log
* Map fault indicator will report fault code
* Faults observed report generated for each log
* Fix duplicate timers on iOS

v0.7.2

* Fix incorrect date bug in calendar view
* Fix hidden chart series selectors in Ride Log Viewer
* Send NACK if no message is received during sync
* Alert if Robogotchi is running unexpected firmware
* Stop Robogotchi status timer before initiating sync

v0.7.1

* Fix database schema when creating for the first time
* Fix missing DFU mode message
* Fix hidden connect button with large system font
* Fix flickering avatar in config tab on iOS
* Allow connection attempts to be aborted
* Showing connection attempt for all devices

v0.7.0

* Calendar view in logging tab (tap robot for old list view)
* Robogotchi status bar displayed on connection tab
* Fix discovered BLE devices grid to 2 items wide
* Fix missing selected CAN devices from Robogotchi config editor
* Sequentially communicate required data upon connection
* Testing SafeArea in RideLogViewer to reveal chart series selection
* Minor fixes and improvements

v0.6.4

* Will not attempt automatic reconnect
* Notify user when disconnected
* Display dialog when a connection attempt is in progress
* Larger area to dismiss keyboard in ESC Configurator
* Confirm before closing the ESC Configurator
* Minor fixes and improvements

v0.6.3

* Show file sync on user input instead of device response
* Send out syncstop message when user aborts file sync
* Storing relative path to log files and board avatars
* Increase height of RideLogChartOverlay
* Display app version in title (temporary)

v0.6.1

* Use the imperial units user preference in ESC Profiles
* Hide select series data on chart to reduce clutter
* Switch Log Auto Start Duty Cycle to eRPM in Robogotchi Configuration
* Minor fixes and improvements

v0.6.0

* Configurable Robogotchi alert thresholds
* Store board avatar(s) in Shared Preferences
* Board avatars can be selected from Gallery
* Smooth voltage input on real time data
* Disabled charting PanAndZoomBehvior for performance
* Minor fixes and improvements

v0.5.2

* Add SafeArea where appropriate for various manufacturer occlusions
* Capture state of ESC communication
* Restrict ESC Configurator access to connected & communicating devices
* Display message if Motor Configuration was not received

v0.5.0

* Added ESC Configurator for modification of settings
* Default all users to dark theme
* Reduced required user settings by requesting from ESC
* Minor UI changes and bug fixes

v0.4.1

* Fix applying ESC profile minimum and maximum watts
* Enforce negative value for Max Power Regen in ESC profile
* Added Robogotchi Configuration Editor
* Removed background location permission requirement
* Ride Log Viewer supports dual and quad ESC configurations
* Added confirmation before entering Robogotchi DFU mode

v0.3.0

* Editable ESC Profiles to control speed and power output
* Display DieBieMS discharge as red progress bar in cell grid
* Show DieBieMS State of Charge with current voltage
* Fix DieBieMS battery temperature decimal place
* Dart serializer for mc_configuration data structure
* Minor UI adjustments and fixes

v0.2.2

* Editing board details sets the cursor to the end of the text field
* Improved DieBieMS view
* Added DieBieMS cell comparison
* Evaluating asymmetric sigmoidal approximation for battery % remaining
* Positioned RideLogViewChartOverlay to fit better on those smol phones

v0.2.0

* New location package that does not execute in background
* DieBieMS Data Visualization
* Non linear battery curve to estimate % remaining

v0.1.1
* Sync without Erase will not show last file until you switch back to logging tab
* Sync with Erase while Logging is active will not erase files (could be robogotchi fw, see renee)
* Chart in ride log viewer not optimized for large number of points. Try mp_charts
* Duty Cycle gauge on Real Time tab may flicker the red highlight on and off
* Editing board settings may put the input cursor at the start of the entry
