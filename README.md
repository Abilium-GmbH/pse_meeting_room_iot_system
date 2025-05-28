# pse_meeting_room_iot_system -  PSE_Abilium_2025

## Project description
 
PSE_Abilium is an IoT module for the open source ERP system Odoo that enables the management and labeling of meeting rooms with e-Ink displays. The aim of the project is to avoid double bookings by displaying reservation information on an e-Ink display.

## Features

- **Calendar integration** : Seamless linking with the Odoo calendar system
- **Room reservation**: Easy assignment of rooms to calendar events
- **E-Ink display support**: Energy-saving display of current and upcoming room bookings
- **MQTT communication**: Reliable real-time data transfer between Odoo and the Raspberry Pi devices
- **Status update**: Automatic updating of displays when changes are made in the calendar

<iframe width="560" height="315" src="----" frameborder="0" allowfullscreen></iframe>

## Technical requirements

#### Server requirements

- Odoo v18.0
- Python
- MQTT broker
- Internet connection for communication between Odoo and the display devices

#### Display hardware

- Raspberry Pi
- E-Ink display
- Micro SD card
- Stable power supply
- WLAN connection

## Getting started

To use this module, you need to have [Odoo installed](https://www.odoo.com/de_DE/page/download?msockid=39f4aad28e496d093fcab8658f426c19).

After installing Odoo, download this module and place its contents into your Odoo `addons` directory.

Next, open Odoo, go to the Apps page, and install the `Abilium room booker` module. 


## Documentation

For more detailed guidance on installing and using this module, please refer to our [user manual](https://github.com/Abilium-GmbH/pse_meeting_room_iot_system/blob/dev_branch/dokumentation/Manual_Abilium_room_booker.pdf). 
Additionally, you can find documentation on the architecture[here](https://github.com/Abilium-GmbH/pse_meeting_room_iot_system/blob/dev_branch/dokumentation/MQTT_Documentation.md).


## Development and customization

The module can be easily extended to implement additional functions:
- Integration with presence sensors to detect unused reservations
- Extensions for other display types
