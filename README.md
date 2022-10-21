# Smart Home Documentation

## Controls
- **Den Lights**
    - Controlled from the Den Tablet dashboard, or from the IKEA dimmer button mounted to Den Light 1
- **Guest Room Light**
    - Primary control is the RF remote for the ceiling fan, but can also be toggled on/off with the Light Button on the wall
- **Living Room Light**
    - Can be controlled by IKEA dimmer button mounted to the lamp, or:
    - Turn on/off: double-tap Entryway Light Switch up/down, or double-tap Dining Room Light Switch up/down
    - Make brighter: triple-tap Entryway Light Switch up/down, or triple-tap Dining Room Light Switch up/down
- **Main Bathroom Light** - single tap up will turn light on at previous level
    - Turn on to Low brightness: press small config button
    - Turn on to Medium brightness: double-tap up
    - Turn on to Full brightness: triple-tap up
- **Good Night**
    - Double-tap the Main Bedroom Light Switch down
        - Turn off:
            - Bar Light
            - Deck Light
            - Dining Room Overhead Light
            - Entryway Light
            - Kitchen Overhead Light
            - Living Room Light
            - Main Bathroom Light
            - Main Bedroom Light (Lamp, not Fan Light)
         - Turn on:
            - Outlet for Wyze camera in Living Room
            - Outlet for Wyze camera in Basement

## Automations
- **Barn Door Protocol**
    - If any of the exterior openings are left open for 10 minutes while the heat is on, the heat will turn off.
    - Once all the exterior openings are closed for 5 minutes, the heat will resume.
- **Garage Door**
   - Garage Door is set to automatically close every night at 11pm. Controlled directly through the MyQ app.

## Timers
- If **Porch Light Timer** is on:
    - Porch Light will turn on at sunset, and will turn off 30 minutes before sunrise
- If **Living Room Light Timer** is on:
    - If either hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, then it will turn on at low brightness
    - If neither hallway motion sensor detects motion for 2 minutes after being triggered, then the living room light will turn back off
    - If the living room light is manually turned on or off (or made brighter or dimmer) in the meantime, then the motion sensors won't automatically turn it off

## Devices

### Physical Devices

| Type         | Sub-Type       | Name                     | Connection  | Make/Model                 |
| ------------ | -------------- | ------------------------ | ----------- | -------------------------- |
| Sensor       | Multi          | Back Door                | Zigbee      | Samsung Multi-Sensor       |
| Outlet       | Plug-In        | Bar Light                | Z-Wave      | Monoprice/Jasco            |
| Standalone   | \-             | Bond Hub                 | Wi-Fi       | Bond                       |
| Printer      | \-             | Canon MX472              | Wi-Fi       | Canon                      |
| Sensor       | Open/Close     | Chest Freezer            | Zigbee      | Visonic MCT-340 E          |
| Sensor       | Open/Close     | Chest Freezer 2          | Zigbee      | Visonic MCT-340 E          |
| Switch       | On/Off         | Deck Switch              | Z-Wave Plus | Inovelli NZW30             |
| Light        | Bulb           | Den Light 1              | Zigbee      | Sengled E11-G13            |
| Light        | Bulb           | Den Light 2              | Zigbee      | Sengled E11-G13            |
| Button       | Dimmer         | Den Light Dimmer         | Zigbee      | IKEA Tradfri Dimmer        |
| Media        | TV             | Den TV                   | ADB         | Amazon Fire TV             |
| Switch       | Dimmer         | Dining Room Light Switch | Z-Wave Plus | Inovelli NZW31             |
| Sensor       | Doorbell       | Doorbell                 | Zigbee      | Echostar Bell              |
| NAS          | \-             | DS420j                   | Ethernet    | Synology DS420j            |
| Thermostat   | \-             | ecobee                   | Wi-Fi       | ecobee 3                   |
| Sensor       | Temp/Occupancy | ecobee: Bedroom          | 915MHz      | ecobee                     |
| Sensor       | Temp/Occupancy | ecobee: Den              | 915MHz      | ecobee                     |
| Switch       | On/Off         | Entryway Light           | Z-Wave Plus | Inovelli NZW30 w/ Scenes   |
| Sensor       | Motion         | Fibaro Motion 1          | Z-Wave      | Fibaro FGMS001             |
| Sensor       | Motion         | Fibaro Motion 2          | Z-Wave      | Fibaro FGMS001             |
| Sensor       | Multi          | Front Door               | Zigbee      | Samsung Multi-Sensor       |
| Appliance    | Washer         | GE Washer                | Wi-Fi       | GE Washing Machine         |
| Appliance    | Dryer          | GE Dryer                 | Wi-Fi       | GE Clothes Dryer           |
| Sensor       | Open/Close     | Front Window North       | Zigbee      | Comcast Window Sensor      |
| Sensor       | Open/Close     | Front Window South       | Zigbee      | Comcast Window Sensor      |
| Cover        | \-             | Garage Door              | Wi-Fi       | MyQ Liftmaster             |
| Sensor       | Tilt           | Garage Door Sensor       | Z-Wave      | Monoprice ZG8101           |
| Fan          | \-             | Guest Room Ceiling       | Bond        | Olibra RF Adapter          |
| Sensor       | Open/Close     | Guest Room Window        | Zigbee      | Comcast Window Sensor      |
| Coordinator  | \-             | HUSBZB                   | \-          | Sigma Designs USB Adapter  |
| Light        | Bulb           | Living Room Light        | Zigbee      | Sengled E11-G13            |
| Button       | Dimmer         | Living Room Light Button | Zigbee      | IKEA Tradfri Dimmer        |
| Switch       | Dimmer         | Master Bath Light        | Z-Wave      | Inovelli LZW31-SN          |
| Sensor       | Open/Close     | Master Bath Window       | Zigbee      | Visonic MCT-340 E          |
| Fan          | \-             | Master Bedroom Fan       | RF          | Olibra RF Adapter          |
| Switch       | On/Off         | Master Bedroom Lamp      | Z-Wave Plus | Inovelli NZW30 w/ Scenes   |
| Sensor       | Open/Close     | Master Bedroom Window N  | Zigbee      | Comcast Window Sensor      |
| Sensor       | Open/Close     | Master Bedroom Window S  | Zigbee      | Comcast Window Sensor      |
| Outlet       | Plug-In        | Monoprice Energy Outlet  | Z-Wave Plus | Monoprice HKZW-SO03        |
| Outlet       | Plug-In        | Monoprice Outlet 1       | Z-Wave      | Monoprice Plug-In          |
| Fan          | \-             | Multipass Fan            | RF          | Olibra RF Adapter          |
| Sensor       | Open/Close     | Multipass Window         | Zigbee      | \-                         |
| PC           | \-             | Pi Zero W                | Ethernet    | Raspberry Pi Zero W        |
| Button       | On/Off         | Plex Button              | Zigbee      | IKEA Tradfri Dimmer        |
| Switch       | On/Off         | Porch Light              | Z-Wave Plus | Inovelli NZW30             |
| UPS          | \-             | UPS                      | Ethernet    | NPC Back-UPS 650           |
| Sensor       | Leak           | Washer Leak Sensor       | Zigbee      | Samsung Leak Sensor        |
| Outlet       | Plug-In        | Wyze Basement            | Z-Wave      | Monoprice Plug-In          |
| Outlet       | Plug-In        | Wyze Ilium Outlet        | Zigbee      | SmartThings Outlet v4      |
| Outlet       | Plug-In        | ZigGuest                 | Zigbee      | SmartThings Outlet v4      |
