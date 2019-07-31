# Node-Red-Contrib-Freebox
----

This module returns the list of all the devices connected on the Freebox network. It uses the Freebox API to get the list of connected devices.

```
{  
   "l2ident":{  
      "id":"55:B8:0A:7D:85:3C",
      "type":"mac_address"
   },
   "active":true,
   "id":"ether-55:b8:0a:7d:85:3c",
   "last_time_reachable":1564602810,
   "persistent":true,
   "vendor_name":"D-Link International",
   "host_type":"other",
   "primary_name":"Switch",
   "l3connectivities":[  
      {  
         "addr":"192.168.1.1",
         "active":true,
         "reachable":true,
         "last_activity":1564602810,
         "af":"ipv4",
         "last_time_reachable":1564602810
      }
   ],
   "reachable":true,
   "last_activity":1564602810,
   "primary_name_manual":true,
   "interface":"pub"
}
```


You need to enable a persistant storage in settings.js to allow this module to store the Freebox API token.

```
    contextStorage: {
        default: {
            module:"localfilesystem"
        },
    },
```