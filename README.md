# Data-Logging-System-for-house-hold-battery-packs
Industrial Level Projects

## Overview

This project involves the design and implementation of a datalogging system for monitoring and managing household battery packs. The datalogging system is positioned between the inverter and 16 parallel-connected battery packs. The communication between the battery packs and the datalogger hardware is established using Modbus protocol, facilitated by an ESP32 microcontroller. The datalogger extracts data from the battery packs, decodes the Modbus reply, and utilizes the information to generate CAN messages with different protocols tailored for various inverters.

Furthermore, the extracted data is formatted into a JSON file and transmitted to the backend through MQTT protocol. The backend then facilitates the display of battery data on a mobile app developed by our company.


## Implementation Details

- The ESP32 microcontroller is programmed to interpret Modbus communication and decode reply data from battery packs.
- CAN messages are generated based on the decoded data, with different protocols for each inverter.
- Extracted data is formatted into a JSON file for easy storage and transmission.
- MQTT protocol is employed to send JSON data to the backend for further processing.
- The backend manages the storage, processing, and retrieval of battery data.
- The mobile app provides a user-friendly interface to display real-time battery information.

## Usage

1. **Datalogger Setup:**
   - Connect the datalogger hardware between the inverter and 16 parallel-connected battery packs.
   - Ensure proper Modbus communication setup.

2. **ESP32 Configuration:**
   - Flash the ESP32 with the provided firmware to handle Modbus communication and data processing.

3. **Inverter Configuration:**
   - Configure the datalogger to generate CAN messages with the specific protocols for each inverter.

4. **Backend Integration:**
   - Set up the backend to receive JSON-formatted data via MQTT and process it accordingly.

5. **Mobile App:**
   - Install the mobile app developed by our company to monitor and display battery data.
  
     
![1](https://github.com/temci024/Data-Logging-System-for-house-hold-battery-packs/assets/129023792/ede98c93-8d37-4519-afa1-06e0231fdcee)

