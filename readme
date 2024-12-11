# Multi-Servo Control System with CT6B Integration

This project demonstrates a multi-servo control system integrated with the CT6B radio transmitter. It provides seamless functionality for controlling servos via RC signals, enabling actions such as up-down motion, rolling, and pitching.

## Overview

The firmware is designed to control four servos connected to a microcontroller using input signals from the CT6B radio receiver. This system is ideal for robotics applications where precise motion control is required. The code includes:

- Servo initialization.
- Mapping RC inputs to servo angles.
- Smooth motion transitions.

## Components

The firmware consists of the following key components:

- **Servo Initialization**: Configures initial positions and movement ranges for the servos.
- **CT6B Input Handling**: Processes signals from the CT6B receiver channels.
- **Motion Control Logic**: Implements up-down, rolling, and pitching actions based on input signals.
- **Serial Debugging**: Outputs signal values for debugging and monitoring.

## Setup and Installation

### Prerequisites

- **Arduino IDE** (preferred).
- **Servo Library**: Ensure the Servo library is included in your Arduino environment.

### Hardware Requirements

- **Microcontroller**: Arduino-compatible board (e.g., Arduino Uno).
- **CT6B Radio Receiver**: For signal input.
- **Servos**: Four servos for motion control (connected to specified pins).
- **Power Supply**: Ensure adequate power for both servos and the microcontroller.

### Wiring Diagram

| Component           | Pin Configuration   |
|----------------------|---------------------|
| **Servo LF**         | Pin 6              |
| **Servo RF**         | Pin 5              |
| **Servo LB**         | Pin 4              |
| **Servo RB**         | Pin 3              |
| **CT6B Channel 1**   | Pin 7              |
| **CT6B Channel 2**   | Pin 8              |
| **CT6B Channel 3**   | Pin 9              |
| **CT6B Channel 4**   | Pin 10             |
| **CT6B Channel 5**   | Pin 11             |
| **CT6B Channel 6**   | Pin 12             |

### Installation Steps

1. Clone or download the firmware code into your Arduino environment.
2. Open the project in **Arduino IDE**.
3. Verify that the Servo library is installed.
4. Connect the components as per the wiring diagram.
5. Upload the code to your Arduino-compatible board.

## Usage

- **Initialization**: Servos are initialized to their default positions (down and up limits).
- **Up and Down Motion**: Controlled via Channel 6 input (mapped to predefined angles).
- **Rolling Motion**: Controlled via Channel 4 input.
- **Pitching Motion**: Controlled via Channel 3 input.
- **Debugging**: Monitor real-time channel values in the Serial Monitor.

## Configuration and Settings

- Servo angle limits are defined for each motion:
  - **Upside-Down Down Position**: `usuDP_*` variables.
  - **Upside-Down Up Position**: `usuUP_*` variables.
- Channel inputs are processed using `pulseIn()` for signal reading.
- Adjust the **angle mapping** in the `map()` function to match your specific servo range requirements.

## Troubleshooting

- **No Servo Movement**:
  - Check wiring and servo connections.
  - Verify signal inputs via Serial Monitor.
- **Incorrect Motion**:
  - Recalibrate the angle mapping in the `map()` function.
  - Ensure the CT6B transmitter is properly configured.
- **Signal Issues**:
  - Confirm the receiver is powered and transmitting signals.

## Files and Descriptions

| File               | Description                                      |
|--------------------|--------------------------------------------------|
| `main.ino`         | Contains the primary firmware logic and setup.   |
| `Servo.h`          | Standard Arduino library for servo control.      |
