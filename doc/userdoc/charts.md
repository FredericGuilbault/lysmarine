#Location

Charts must be stored in `/srv/charts/`

For convenience a link have been added in the /home/pi/ directory.



#Users
The applications that directly read charts are signalk and opencpn.

Tuktuk for it's part is retrieving the charts from the signalk server.   


#Formats

### Tuktuk & signalk
Only support tiling formats.


### Opencpn

Opencpn support a wild range of charts.
You can take a look at the list on opencpn website [here](https://opencpn.org/wiki/dokuwiki/doku.php?id=opencpn:opencpn_user_manual:charts:chart_formats)

_NOTE: opencpn 5.0.0 have added the support for tiling formats.
But due to the low capacity of the raspberry. It often crash._
