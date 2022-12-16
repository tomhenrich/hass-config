## Automations
- **Barn Door Protocol**
    - If any of the exterior openings are left open for 10 minutes while the heat is on, the heat will turn off.
    - Once all the exterior openings are closed for 5 minutes, the heat will resume.
- **Garage Door**
   - Garage Door is set to automatically close every night at 11pm. Controlled directly through the MyQ app.
- **Check Monthly Data**
    - Helper value sets interval at which Pi Zero W polls for internet usage data from router
    - At the established intervals, automation triggers a REST request to update the source data on the Pi
    - A short delay allows the source data to be processed, then the HA sensor updates with that new data

## Timers
- If **Porch Light Timer** is on:
    - Porch Light will turn on at sunset, and will turn off 30 minutes before sunrise
- If **Living Room Light Timer** is on:
    - If either hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, then it will turn on at low brightness
    - If neither hallway motion sensor detects motion for 2 minutes after being triggered, then the living room light will turn back off
    - If the living room light is manually turned on or off (or made brighter or dimmer) in the meantime, then the motion sensors won't automatically turn it off
- Seasonal: If **Christmas Tree Timer** is on:
    - Two separate helper values are enabled to set ON and OFF times for Christmas Tree lights
    - Switch will turn on and off at assigned times
