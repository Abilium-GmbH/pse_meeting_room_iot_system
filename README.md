# Occupation Status Display System for Meeting Rooms

<p align="center">
<img src="https://github.com/user-attachments/assets/1c06c54e-1a5c-4198-8112-ee88094842c1" alt="settings_gif" width="600"/>
</p>

## Project description 
 
PSE_Abilium is an IoT module for the open source ERP system Odoo that enables the management and labeling of meeting rooms with e-Ink displays. The aim of the project is to avoid double bookings by displaying reservation information on an e-Ink display. 

Our custom Odoo module "Abilium Room Booker" is seamlessly integrated into the standard Odoo calendar, extending it with extra functionality to create meeting rooms and link them with raspberrys via MQTT. These rooms can then be booked in the familiar and userfriendly Odoo calendar UI, by selecting them when creating a meeting. Booked rooms are displayed on the raspberry E-ink displays and updated according to their occupation status in real-time!

## Features

- ### 📅 **Calendar integration** : Manage meeting rooms and raspberry connections from within the Odoo calendar system

  <img src="https://github.com/user-attachments/assets/62ad1ba0-e67c-4f6a-a06a-f17bbac030d5" alt="settings_gif" width="400"/>
- ### 🏢 **Room reservation**: Assign rooms to upcoming meetings in an intuitive way

  <img src="https://github.com/user-attachments/assets/ee419069-2993-48fd-b09c-ac4825420387" alt="size_filter_gif" width="400"/>
- ### 🖥️ **E-Ink display support**: Display current and upcoming room bookings in an energy-saving way
- ### 📡 **MQTT communication**: Transfers real-time data reliably between Odoo and the Raspberry Pi devices

  <img src="https://github.com/user-attachments/assets/5c7e17ae-d4c6-4200-98ea-c4be59f72a8a" alt="settings_gif" width="500"/>
- ### 🔄 **Status update**: Automatically updates the displays when changes are made in the calendar


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
Additionally, you can find documentation on the architecture [here](https://github.com/Abilium-GmbH/pse_meeting_room_iot_system/blob/dev_branch/dokumentation/MQTT_Documentation.md).


## Development and customization

The module can be easily extended to implement additional functions:
- Integration with presence sensors to detect unused reservations
- Extensions for other display types
