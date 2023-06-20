# IoT Automatic Water Dispenser

Welcome to the IoT Automatic Water Dispenser project! This project aims to build a device that can automatically dispense water based on predefined settings and user commands using Internet of Things (IoT) technology. This README file will guide you through the process of building and setting up the automatic water dispenser.

## Table of Contents

1. [Introduction](#introduction)
2. [Components](#components)
3. [Hardware Setup](#hardware-setup)
4. [Software Setup](#software-setup)
5. [Usage](#usage)
6. [Contributing](#contributing)


## Introduction

The IoT Automatic Water Dispenser is designed to provide convenient and automated water dispensing. Automatic water dispensers for commercial settings are intended to give staff, clients, and visitors a simple and dependable source of drinking water. They are typically used in public spaces like workplaces, schools, hospitals, and other places where many people might need access to clean water. Automatic water dispensers for industrial settings frequently include features like filtration systems, temperature controls, and adjustable flow rates to satisfy the individual demands of different users. They also always deliver a steady supply of fresh, clean water.

## Components

To build the IoT Automatic Water Dispenser, you will need the following components:

- Microcontroller board ( Arduino )
- Water pump
- Water level sensor
- Relay module
- Power supply
- Jumper wires
- Tubing and fittings
## Hardware Setup

1. Connect the water pump to the microcontroller board. Use the relay module to control the power supply to the pump.
2. Connect the water level sensor to the microcontroller board. This sensor will detect the water level and send signals to the microcontroller.
3. Connect the power supply to the microcontroller board, water pump, and relay module.
4. Set up the tubing and fittings to connect the water source to the pump and the dispenser outlet.

## WORKING PROCEDURE:
The general steps involved in the working of this IoT project:

1.The ultrasonic sensor detects the presence of a water container and sends a signal to the Arduino Uno R3.

2.The Arduino Uno R3 activates the water pump via the relay module to begin dispensing water into the container.

3.The LM393 sound sensor module monitors the sound waves produced by the falling water and sends a signal to the Arduino Uno R3.

4.The Arduino Uno R3 uses the analog input pin to measure the voltage output from the sound sensor module, which corresponds to the intensity of the sound waves.

5.As the water container fills up with water, the sound waves produced by the falling water will have a lower intensity and therefore produce a lower voltage output from the sound sensor module.

6.The Arduino Uno R3 uses a threshold value to determine when the container is full, based on the voltage output from the sound sensor module.

7.When the container is full, the Arduino Uno R3 sends a signal to the relay module to deactivate the water pump and stop dispensing water.

8.The Arduino Uno R3 continues to monitor the ultrasonic sensor and the sound sensor module, and the cycle repeats when the container is empty again.

Note that this is a general overview of the working of the water dispenser prototype. The specific implementation details, such as the threshold value for detecting a full container or the cloud server and mobile app integration, may vary depending on your specific project requirements.

## CONNECTION PROCEDURE: 

1.Connect the LM393 sound sensor module to the breadboard. Connect VCC to the 5V power supply, GND to the ground, and OUT to any digital input pin on the Arduino Uno R3 (for example, pin 2).

2.Connect the ultrasonic sensor (HC-SR04) to the breadboard. Connect VCC to the 5V power supply, GND to the ground, TRIG to any digital output pin on the Arduino Uno R3 (for example, pin 4), and ECHO to any digital input pin on the Arduino Uno R3 (for example, pin 3).

3.Connect the relay module to the breadboard. Connect VCC to the 5V power supply, GND to the ground, and IN to any digital output pin on the Arduino Uno R3 (for example, pin 5).

4.Connect the water pump to the relay module. Connect the positive (+) wire of the water pump to the NO (normally open) pin of the relay module, and connect the negative (-) wire of the water pump to the ground.

5.Connect a 12V power supply to the relay module. Connect the positive (+) wire of the power supply to the COM (common) pin of the relay module, and connect the negative (-) wire of the power supply to the ground.

6.Connect a separate 5V power supply to the Arduino Uno R3. Connect the positive (+) wire of the power supply to the VIN pin on the Arduino Uno R3, and connect the negative (-) wire of the power supply to the ground.

7.Connect a resistor (for example, a 10k ohm resistor) between the TRIG pin of the ultrasonic sensor and the positive (+) rail on the breadboard. This will help to protect the ultrasonic sensor.

8.Finally, upload the Arduino code to the board and test the water dispenser prototype.

Note that this is a basic guide and the specific connections may vary depending on the specific components you are using. Always consult the datasheets and documentation for your components to ensure proper wiring and safety precautions.

## Contributing

We welcome contributions to the IoT Automatic Water Dispenser project. If you would like to contribute, please follow the guidelines outlined in the project repository.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Happy building and enjoy using the IoT Automatic Water Dispenser! If you have any questions or need further assistance, please refer to the project documentation or reach out to the project maintainers.
