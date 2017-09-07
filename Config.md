# Config options

## the file config/default.json
```JSON
{
    "raumserver": {
        "port" : 8080
    },
    "raumfeld": {   
        "raumfeldHost"              : "0.0.0.0", 
        "raumfeldHostRequestPort"   : 47365, 
        "raumfeldManufacturerId"    : "Raumfeld GmbH",
        "raumfeldVirtualMediaPlayerModelDescription" : "Virtual Media Player",
        "alivePingerIntervall"      : 2500,
        "ssdpDiscovertimeout"       : 5000,
        "bonjourDiscoverTimeout"    : 3000,
        "uriMetaDataTemplateFile"   : "lib/setUriMetadata.template",
        "rendererStateTriggerConfirmationTimout": 3500,
        "zoneTriggerConfirmationTimout": 6000
    }
}
```

## raumserver 
### port
this is the port raumserver is available on after start. 
## raumfeld 
### raumfeldHost
this option allows you to enter a static IP address one of you Raumfeld devices is available and node-raumserver can do it's discovery procedure. 0.0.0.0 means that the Raumfeld devices get autodetected by using [SSDP discovery](https://en.wikipedia.org/wiki/Simple_Service_Discovery_Protocol). 
### raumfeldHostRequestPort
### raumfeldManufacturerId
### raumfeldVirtualMediaPlayerModelDescription
### alivePingerIntervall
### ssdpDiscovertimeout
This is the value in milliseconds in which node-raumserver waits for the SSDP discovery reply of the device that should be discovered.  
### uriMetaDataTemplateFile
### rendererStateTriggerConfirmationTimout
### zoneTriggerConfirmationTimout
