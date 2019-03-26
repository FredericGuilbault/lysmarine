## Signalk to opencpn

OpenCpn receive it's location data from signalk in nmea186 format over tcp  

### The path
```
 signalk-to-nmea0183 ===> opencpn
```
signalk-to-nmea0183 is a signalk plugin pre-configured to emit nmea0183 string over tcp on the port 10110.
Opencpn is configured to listen on this port for nmea0183 sentences.  

### debugging

 - Make sure signalk-to-nmea0183 plugin is enabled in the signalk admin panel.
 - Use `telnet localhost 10110` to validate that signalk emit nmea0183 sentences.
 - Check opencpn configuration.

If it still don't work open an issue at : 
 http://gitlab.com/lysmarine/lysmarine/issues/
