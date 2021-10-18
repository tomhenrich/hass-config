# Smart Home Documentation

## Controls
* **Living Room Light**
    * Can be controlled by IKEA dimmer button mounted to the lamp, or:
    * Turn on/off: double-tap Entryway Light Switch up/down, or double-tap Dining Room Light Switch up/down
    * Make brighter: triple-tap Entryway Light Switch up/down, or triple-tap Dining Room Light Switch up/down
* **Main Bathroom Light** - single tap up will turn light on at previous level
    * Turn on to Low brightness: press small config button
    * Turn on to Medium brightness: double-tap up
    * Turn on to Full brightness: triple-tap up
* **Den Lights**
    * Controlled from the Den Tablet dashboard, or from the IKEA dimmer button mounted to Den Light 1
* **Good Night**
    * Double-tap the Main Bedroom Light Switch down
        * Turn off:
            * Kitchen Overhead Light
            * Bar Light
            * Living Room Light
            * Entryway Light
            * Den Lights
            * Main Bathroom Light
            * Main Bedroom Light
         * Turn on:
            * Outlet for Wyze camera in Living Room
            * Outlet for Wyze camera in Basement
         * Close:
            * Garage Door

## Automations
* **Barn Door Protocol**
    * If any of the exterior openings (Front or Back Door) are left open for 10 minutes while the heat is on, the heat will turn off.
    * Once all the exterior openings are closed for 5 minutes, the heat will resume.
* **Garage Door**
   * Garage Door is set to automatically close every night at 11pm. Controlled directly through the MyQ app.
* **Den Tablet Charging** - don't leave the dashboard tablet continuously charging 24/7
   * Den tablet power outlet will turn on if it has been off for 1 hour
   * Den tablet power outlet will turn off if it has been on for 3 hours

## Timers
* If **Porch Light Timer** is on:
    * Porch Light will turn on 1 hour after sunset, and will turn off at 11pm
* If **Living Room Light Timer** is on:
    * If either hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, then it will turn on
    * If either hallway motion sensor doesn't detect motion for 2 minutes after being triggered, then the living room light will turn back off
    * If the living room light is manually turned on or off (or made brighter or dimmer) in the meantime, then the motion sensors won't automatically turn it off
