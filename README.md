# I2C Scanner with Arduino

This project is a simple program used to detect I2C devices connected to an Arduino. The program scans all possible I2C addresses and displays the addresses of detected devices via the Serial Monitor.

## Description

This code is designed to help users identify the I2C addresses of devices connected to an Arduino. It is especially useful when working with various I2C modules or sensors to determine the exact I2C address of each device.

## Key Features

- **I2C Device Detection**: The program scans I2C addresses from 1 to 119.
- **Serial Output**: The detected I2C device addresses are displayed in both decimal and hexadecimal format via the Serial Monitor.

## Required Components

- Arduino (Uno, Mega, or any other compatible model)
- I2C device (such as sensors, modules, etc.)
- Jumper wires

## How It Works

1. **Initialization**:

   - Serial communication is initialized with a baud rate of 115200.
   - The I2C bus is initialized using `Wire.begin()`.

2. **I2C Address Scanning**:
   - The program scans I2C addresses from 1 to 119.
   - If a device is found at a certain address, that address is displayed in the Serial Monitor in both decimal and hexadecimal formats.
   - After the scan is complete, the number of detected devices is displayed.

## How to Use

1. Connect the I2C device to the Arduino.
2. Upload this code to the Arduino.
3. Open the Serial Monitor in the Arduino IDE with a baud rate of 115200.
4. The program will scan I2C addresses and display the results in the Serial Monitor.

## Example Output

After the scan is complete, the Serial Monitor will display output like this:

## Notes

- Ensure that the I2C device is correctly connected to the SDA and SCL pins on the Arduino.
- The scan may take a few seconds to complete.
