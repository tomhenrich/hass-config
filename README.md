# Smart Home Documentation

## Controls
- **Living Room Light**
    - Can be controlled by IKEA dimmer button mounted to the lamp, or:
    - Turn on/off: double-tap Entryway Light Switch up/down, or double-tap Dining Room Light Switch up/down
    - Make brighter: triple-tap Entryway Light Switch up/down, or triple-tap Dining Room Light Switch up/down
* **Main Bathroom Light** - single tap up will turn light on at previous level
    - Turn on to Low brightness: press small config button
    - Turn on to Medium brightness: double-tap up
    - Turn on to Full brightness: triple-tap up
* **Den Lights**
    - Controlled from the Den Tablet dashboard, or from the IKEA dimmer button mounted to Den Light 1
* **Good Night**
    - Double-tap the Main Bedroom Light Switch down
        - Turn off:
            - Kitchen Overhead Light
            - Dining Room Overhead Light
            - Bar Light
            - Living Room Light
            - Entryway Light
            - Den Lights
            - Main Bathroom Light
            - Main Bedroom Light
            - Deck Light
         - Turn on:
            - Outlet for Wyze camera in Living Room
            - Outlet for Wyze camera in Basement

## Automations
- **Barn Door Protocol**
    - If any of the exterior openings (Front or Back Door) are left open for 10 minutes while the heat is on, the heat will turn off.
    - Once all the exterior openings are closed for 5 minutes, the heat will resume.
- **Garage Door**
   - Garage Door is set to automatically close every night at 11pm. Controlled directly through the MyQ app.

## Timers
- If **Porch Light Timer** is on:
    - Porch Light will turn on at sunset, and will turn off 30 minutes before sunrise
- If **Living Room Light Timer** is on:
    - If either hallway motion sensor detects motion from sunset to sunrise, and the living room light is off, then it will turn on
    - If either hallway motion sensor doesn't detect motion for 2 minutes after being triggered, then the living room light will turn back off
    - If the living room light is manually turned on or off (or made brighter or dimmer) in the meantime, then the motion sensors won't automatically turn it off

## Devices

### Physical Devices

| Type         | Sub-Type       | Name                     | Connection  | Make/Model                 |
| ------------ | -------------- | ------------------------ | ----------- | -------------------------- |
| Button       | Dimmer         | Den Light Dimmer         | Zigbee      | IKEA Tradfri Dimmer        |
| Button       | Dimmer         | Living Room Light Button | Zigbee      | IKEA Tradfri Dimmer        |
| Button       | Dimmer         | Living Room Light Button | Zigbee      | IKEA Tradfri Dimmer        |
| Coordinator  | \-             | HUSBZB                   | \-          | Sigma Designs USB Adapter 
| Cover        | \-             | Garage Door              | Wi-Fi       | MyQ Liftmaster             |
| Fan          | \-             | Guest Room Ceiling       | RF          | Olibra RF Adapter          |
| Fan          | \-             | Master Bedroom Fan       | RF          | Olibra RF Adapter          |
| Fan          | \-             | Multipass Fan            | RF          | Olibra RF Adapter          |
| Light        | Bulb           | Den Light 1              | Zigbee      | Sengled E11-G13            |
| Light        | Bulb           | Den Light 2              | Zigbee      | Sengled E11-G13            |
| Light        | Bulb           | Living Room Light        | Zigbee      | Sengled E11-G13            |
| Media Player | \-             | Shield TV                | Ethernet    | NVIDIA Shield              |
| NAS          | \-             | Synology NAS             | Ethernet    | Synology DS420j            |
| Outlet       | Plug-In        | Bar Light                | Z-Wave      | Monoprice/Jasco            |
| Outlet       | Plug-In        | Monoprice Energy Outlet  | Z-Wave Plus | Monoprice HKZW-SO03        |
| Outlet       | Plug-In        | Monoprice Outlet 1       | Z-Wave      | Monoprice Plug-In          |
| Outlet       | Plug-In        | Washing Machine Outlet   | Z-Wave Plus | Monoprice HKZW-SO03        |
| Outlet       | Plug-In        | Wyze Basement            | Z-Wave      | Monoprice Plug-In          |
| Outlet       | Plug-In        | Wyze Ilium Outlet        | Zigbee      | SmartThings Outlet v4      |
| Outlet       | Plug-In        | ZigGuest                 | Zigbee      | SmartThings Outlet v4      |
| Sensor       | Doorbell       | Doorbell                 | Zigbee      | Echostar Bell              |
| Sensor       | Leak           | Washer Leak Sensor       | Zigbee      | Samsung Leak Sensor        |
| Sensor       | Motion         | Fibaro Motion            | Z-Wave      | Fibaro FGMS001             |
| Sensor       | Motion         | Fibaro Motion 2          | Z-Wave      | Fibaro FGMS001             |
| Sensor       | Multi          | Back Door                | Zigbee      | Samsung Multi-Sensor       |
| Sensor       | Multi          | Front Door               | Zigbee      | Samsung Multi-Sensor       |
| Sensor       | Open/Close     | Aqara Window Sensor 1    | Zigbee      | Aqara                      |
| Sensor       | Open/Close     | Aqara Window Sensor 2    | Zigbee      | Aqara                      |
| Sensor       | Open/Close     | Aqara Window Sensor 3    | Zigbee      | Aqara                      |
| Sensor       | Open/Close     | Chest Freezer            | Zigbee      | Visonic MCT-340 E          |
| Sensor       | Open/Close     | Chest Freezer 2          | Zigbee      | Visonic MCT-340 E          |
| Sensor       | Open/Close     | Master Bath Window       | Zigbee      | Visonic MCT-340 E          |
| Sensor       | Open/Close     | Multipass Window         | Zigbee      | \-                         |
| Sensor       | Temp/Humidity  | Dryer Sensor             | Zigbee      | Samsung Temperature Sensor |
| Sensor       | Temp/Occupancy | ecobee: Bedroom          | 915MHz      | ecobee                     |
| Sensor       | Temp/Occupancy | ecobee: Den              | 915MHz      | ecobee                     |
| Sensor       | Tilt           | Garage Door Sensor       | Z-Wave      | Monoprice ZG8101           |
| Standalone   | \-             | Bond Hub                 | Wi-Fi       | Bond                       |
| Switch       | Dimmer         | Dining Room Light Switch | Z-Wave Plus | Inovelli NZW31             |
| Switch       | Dimmer         | Master Bath Light        | Z-Wave      | Inovelli LZW31-SN          |
| Switch       | On/Off         | Deck Switch              | Z-Wave Plus | Inovelli NZW30             |
| Switch       | On/Off         | Entryway Light           | Z-Wave Plus | Inovelli NZW30 w/ Scenes   |
| Switch       | On/Off         | Master Bedroom Light     | Z-Wave Plus | Inovelli NZW30 w/ Scenes   |
| Switch       | On/Off         | Porch Light              | Z-Wave Plus | Inovelli NZW30             |
| Thermostat   | \-             | ecobee                   | Wi-Fi       | ecobee 3                   |
| UPS          | \-             | UPS                      | Ethernet    | NPC Back-UPS 650           |
