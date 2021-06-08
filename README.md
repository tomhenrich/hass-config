# Smart Home Documentation

## Controls
* Living Room Light
    * Turn on by 

## Automations

### Barn Door Protocol
If any of the exterior openings (Front or Back Door) are left open for 10 minutes while the heat is on, the heat will turn off.
Once all the exterior openings are closed for 5 minutes, the heat will resume.

### Timers
* If Porch Light Timer is on:
    * Porch Light will turn on 1 hour after sunset, and will turn off at 11pm
* If Living Room Light Timer is on:
    * If the upstairs hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, then it will turn on
    * If the upstairs hallway motion sensor doesn't detect motion for 2 minutes after being triggered, then the living room light will turn back off
    * If the living room light is manually turned on or off (or made brighter or dimmer) in the meantime, then the motion sensor won't automatically turn it off
