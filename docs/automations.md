## Automations
- **Barn Door Protocol**
    - If either the front or back door is left open for 10 minutes while the heat is on, the heat will turn off.
    - Once both doors are closed for 5 minutes, the heat will resume.
- **Garage Door**
   - Garage Door is set to automatically close every night at 11pm. Controlled directly through the [MyQ app](https://www.myq.com/app).
- **Data Usage Refresh**
    - Helper value sets interval at which Pi Zero W polls the router for internet usage data
    - At the established intervals, automation triggers a REST request to update the source data on the Pi
    - A short delay allows the source data to be processed on the Pi, then the HA sensor updates with that new data

## Timers
- If **Porch: Light on Timer** is active:
    - Porch Light will turn on at sunset, and will turn off 30 minutes before sunrise
- If **Living Room: Night Light** is active:
    - If either hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, it will turn on at low brightness
    - If (after triggering the nightlight) neither hallway motion sensor detects motion for 2 minutes, the living room light will turn back off
    - If the living room light is manually turned on or off in the meantime, then the motion sensors won't automatically turn it off
- Seasonal: If **Christmas Tree Timer** is active:
    - Two separate helper values are enabled to set ON and OFF times for Christmas Tree lights
    - Switch will turn on and off at assigned times
