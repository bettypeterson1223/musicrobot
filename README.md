# Music Following Robot
This repository contains the code and setup instructions for a robot that detects and follows sound sources using microphones, digital filters, and motor control. The project integrates hardware and software components to implement autonomous navigation based on audio signals.

## Features
* Real-Time Sound Detection: Processes audio signals using high-pass and low-pass filters to isolate sound sources.
* Directional Movement: The robot moves forward, backward, left, or right based on the location of the sound source.
* Autonomous Navigation: Stops or rotates 180 degrees when sound is absent or originates from behind the robot.
* Custom Motor Control: Precise motor control for fluid movement using PWM signals.

## Hardware Requirements
* Microcontroller: Texas Instruments MSP432 LaunchPad or compatible microcontroller.
* Microphones: Two analog microphones connected to ADC channels (A14 and A15).
* Motors: Two DC motors with H-bridge motor drivers.
* Power Supply: 5V power supply for the microcontroller and motors.
* Other Components:
- Protoboard for soldering.
- Resistors and capacitors for filtering.
- LEDs for debugging and visual feedback.

 ## Setup Instructions
1. Hardware Assembly:
- Solder microphones and other components to the protoboard.
- Connect the microphones to ADC channels (P6.0 and P6.1).
- Connect motors to GPIO pins (P5.4, P5.5, P3.6, P3.7).
- Follow the wiring diagram to ensure proper connections.
2. Software Configuration:
- Clone this repository.
- Include the external libraries (SysTick.h, Clock.h) in the project directory.
- Open the finalcodeBPSF.c file in your IDE.
3. Compilation:
- Import the project into Code Composer Studio.
- Compile the code and resolve any dependency issues.
4. Deployment:
- Flash the compiled code onto the MSP432 microcontroller.
- Power up the system and verify functionality.


