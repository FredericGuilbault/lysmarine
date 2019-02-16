
# What is LysMarine
LysMarine a linuxOS based on the raspbian build script designed to run on a raspberry.

His goal is to provide a stable, lowcost navigation computer for boats.



# How it work
The operating is build via the `lysmarine-gen` tool and and made available in form of a image file to install on a SD card.
lys marine is made of :

## Desktop environment
 - Openbox
 - tint2
 - onboard
 - dbmenu
 - chromium
 - terminator
 - leafpad
 - obmenu

## The featured applications are
 - Signalk as communication protocol server
 - Opencpn and tuktuk as chart plotter
 - xygrips as weather app.

## Background software
 - signalk
 - gpsd
 - pypilot
 - kplex
 - openplotter




# Instruments connection
The raspberry provide multiple ways to connect and interact with instruments and sensors.
Signalk is the central point where all the data should go in and out.



# This is how it work for the supported devices
## USB GPS
```
physical GPS ===> udev rules ===> manage_gps.sh ===> gpsd ===> signalk
```
The list of supported gps dongle is based on the devices supported by the gpsd project.
The signalk server is pre-confured to receive 5 inputs form gpsd.

If you plug a GPS device and it does not work out-of-the-box The debugging procedure can be found here : __TODO__



## What to do in case of a supported device
_TODO_
