shell-script-unix-instruments
=============================

contains shell script and unix instruments to run ios automation test

for full project and original copy: https://github.com/jonathanpenn/AutomationExample

To run it, write in terminal
  $ ./run_automation.sh

Open run_automation.sh:

- Change the directory build path for your project
  BUILD_DIR=/tmp/iPropSGiOSiPhoneV2
  
- Change workspace or project name and scheme name to your project or workspace name
  To build the Xcode project:
  xcodebuild -workspace "workspace_name.xcworkspace" -scheme "scheme_name" -sdk iphonesimulator clean build \
  CONFIGURATION_BUILD_DIR=$BUILD_DIR \
  TARGETED_DEVICE_FAMILY=1
  
  or
  
  To build the Xcode workspace:
  xcodebuild -project "project_name.xcodeproj" -scheme "scheme_name" -sdk iphonesimulator clean build \
  CONFIGURATION_BUILD_DIR=$BUILD_DIR \
  TARGETED_DEVICE_FAMILY=1
  
- in unix_instruments part, change UIASCRIPT file to your test script
