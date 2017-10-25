# Power on and power off
## leave standby
Leaving standby is easy. Simply call 
```URL 
/raumserver/controller/leaveStandby?id=<RoomName>&scope=room
```

## enter standby
there are two ways of entering standby, because there are two ways how to send a Raumfeld device to the standby. 

### enterManualStandby
This sends the Raumfeld device to the standby the same ways as it does when you press the power button on the device while it is powered on. 

```URL
/raumserver/controller/enterManualStandby?id=<RoomName>&scope=room
```

In case you are using Spotify the next way is most probably your more relevant one. When you enter a manual standby the device has to be taken out of stanby prior to use Spotify Connect again because the zone disappears when you enter manual standby. 

### enterAutomaticStandby
Entering the eco-mode triggeres the same behaviour on the Raumfeld device you get when e.g. playback is paused and the time passed which you defined in the Raumfeld app under Settings > Room and Device Configuration > Speaker > Players in this Room: <Speakername> > Activate ECO automatically: After \<x\> Minutes.   

This is the way you may favour, at least in case you are using Spotify Connect. When your Raumfeld device is in the so called ECO mode you can still see it in the "available devices"-menu within the Spotify apps. 

```URL
/raumserver/controller/enterAutomaticStandby?id=<RoomName>&scope=room
```
