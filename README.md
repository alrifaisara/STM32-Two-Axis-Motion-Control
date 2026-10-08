# STM32 2-Axis Motion Control System
<img width="1540" height="1170" alt="image" src="https://github.com/user-attachments/assets/63204b3f-d9f1-4338-b631-e06e835b6cc9" />


A two-axis embedded motion-control system developed using an **STM32F401 microcontroller** and stepper motors. The system combines motor-driver communication, analog input control, external interrupts, and limit-switch protection to provide controlled and safe bidirectional motion.

**Project Duration:** May 2026 – August 2026

---

## Overview

This project was completed as part of a two-person university engineering team.

The system independently controls two stepper-motor axes using an STM32F401 microcontroller. Stepper-motor drivers are interfaced through SPI, while ADC inputs are used as part of the motor-control logic.

External interrupts and limit switches are used for boundary detection and machine-safety behaviour. When a physical limit is reached, the controller prevents the corresponding motor from continuing farther into that boundary while still allowing motion in the opposite direction.

Both team members collaborated throughout the full development process, including embedded programming, hardware integration, testing, debugging, and system design.

---

## Key Features

- Independent control of two stepper-motor axes
- STM32F401 microcontroller
- SPI communication with stepper-motor drivers
- ADC-based variable motor control
- GPIO configuration and digital I/O
- External interrupt handling
- Limit-switch boundary detection
- Direction-aware safety logic
- Controlled bidirectional motion
- Hardware/software integration
- Embedded-system debugging and testing

---

## Technologies

### Hardware

- STM32F401 microcontroller
- Stepper motors
- Stepper-motor drivers
- Limit switches
- Potentiometer / analog input
- Supporting electronic hardware

### Software & Embedded Systems

- C / C++
- STM32
- SPI
- ADC
- GPIO
- External interrupts
- Stepper-motor control

---

## System Operation

The STM32 acts as the central controller for both motion axes.

Each stepper motor is controlled through a dedicated motor driver communicating with the STM32 through **SPI**.

Analog inputs are read using the STM32's **ADC** and used to provide variable motor-control input.

The system also monitors physical limit switches connected through GPIO pins. These switches are handled using **external interrupts**, allowing the controller to respond immediately when an axis reaches its mechanical travel limit.

The control logic prevents the motor from continuing farther into an activated limit while still allowing movement in the opposite direction.

This provides both responsive motion control and basic machine-safety functionality.

---

## Limit-Switch Safety Logic

A key part of the project was implementing safe movement at the physical boundaries of each axis.

The control logic:

1. Detects limit-switch activation using external interrupts.
2. Identifies the affected axis.
3. Determines the current direction of motion.
4. Prevents movement farther into the activated limit.
5. Allows motion away from the limit.
6. Maintains independent motion and safety states for both axes.

This prevents the motors from continuously driving against the mechanical boundaries of the system.

---

## My Contributions

As part of a two-person team, I contributed across the full development of the system, including:

- STM32 firmware development in C/C++
- GPIO configuration
- External interrupt implementation
- Limit-switch handling
- Boundary-protection logic
- SPI communication with stepper-motor drivers
- ADC-based motor-control input
- Bidirectional motion-control logic
- Hardware wiring and integration
- System testing
- Debugging hardware/software interactions
- Validating safe motor behaviour

Both team members worked collaboratively across the entire project rather than dividing the system into completely separate individual components.

---

## Engineering Skills Demonstrated

This project strengthened my experience in:

- Embedded systems
- Microcontrollers
- Stepper-motor control
- Hardware/software integration
- Interrupt-driven programming
- SPI communication
- ADC input handling
- GPIO
- Sensor and switch integration
- Real-time control behaviour
- Debugging
- Machine-safety logic
- Team-based engineering development

---

## Demo

A demonstration of the completed system is available through my engineering portfolio:

**Portfolio:**  
https://saraalrifai.netlify.app/

