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
this is the port node-raumserver is available after it's start. 
## raumfeld 
### raumfeldHost
this option allows you to enter a static IP address one of you Raumfeld devices is available and node-raumserver can do it's discovery procedure. 0.0.0.0 means that the Raumfeld devices get autodetected by using [SSDP discovery](https://en.wikipedia.org/wiki/Simple_Service_Discovery_Protocol). 
### raumfeldHostRequestPort
### raumfeldManufacturerId
### raumfeldVirtualMediaPlayerModelDescription

### alivePingerIntervall
intervall used to check if host is alive with a "ping" on the last know ip

### ssdpDiscovertimeout
If the host is not found via bonjour the kernel tries to find it via ssdp for this amount of milliseconds. If it does not find the host it starts again with the the bonjour search. This will be done until a host ist found

### bonjourDiscoverTimeout
If the system is searching for the host it first uses the bonjour discovery. If host is not found within this amount of time there is a fallback to ssdp-discovery

### uriMetaDataTemplateFile
### rendererStateTriggerConfirmationTimout and zoneTriggerConfirmationTimout
are internal values which do not have any relation to finding/rediscovering the host
