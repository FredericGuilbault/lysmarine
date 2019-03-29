
## USB GPS
The list of supported gps dongle is based on the devices supported by the gpsd project.
5 path are pre-confured to receive GPS. More can be added manually if needed. If you need documentation for this plz open an issue at http://gitlab.com/lysmarine/lysmarine/issues/

### The path
```
physical GPS ===> physical USB port ===> udev rules ===> manage_gps.sh ===> gpsd(via systemd) ===> signalk
```

### Supported devices
|Device|Status|Notes|
|----|----|----|
| Prolific Technology, Inc. PL2303 Serial Port [linux module: pl2303]|Working| Reported by Frederic guilbault|
| ATEN International Co., Ltd UC-232A Serial Port [linux module: pl2303]|Unknown||
| PS-360 OEM (GPS sold with MS Street and Trips 2005) [linux module: pl2303]|Unknown||
| FTDI 8U232AM / FT232 [linux module: ftdi_sio]|Unknown||
| Cypress M8/CY7C64013 (Delorme uses these) [linux module: cypress_m8]|Unknown||
| Cypress M8/CY7C64013 (DeLorme LT-40)|Unknown||
| Garmin International GPSmap, various models (tested with Garmin GPS 18 USB)  [linux module: garmin_gps]|Unknown||
| Cygnal Integrated Products, Inc. CP210x Composite Device (Used by Holux m241 and Wintec grays2 wbt-201) [linux module: cp210x]|Unknown||
| Cygnal Integrated Products, Inc. [linux module: cp210x]|Unknown||
| u-blox AG, u-blox 5 (tested with Navilock NL-402U) [linux module: cdc_acm]|Unknown||
| u-blox AG, u-blox 6 (tested with GNSS Evaluation Kit TCXO) [linux module: cdc_acm]|Unknown||

### debugging
  Boot without having the device connected then plug it and fallow the debug chain bellow

 - If `ls /dev/ttyLYS*` Output a file. this mean that udev have reconised the device you plugged as a USB GPS.
 - In `tail /var/log/syslog` you should see a row like this one `This USB device is known as a GPS and will be connected to gpsd on port 2947?`. This would mean that `manage_gps.sh` have tried to start gpsd.
 - Try `systemctl status lysgpsd@0.service` and/or `ps aux | grep gpsd` to validate that gpsd daemon is running.
 - Check with `gpsmon 127.0.0.1:29470` that you receive NMEA data and have your position.
 - Restart signalk.    

 If it still don't work open an issue at :
  http://gitlab.com/lysmarine/lysmarine/issues/
