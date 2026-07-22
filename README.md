# STM32-Based Closed Loop DC-DC Buck Converter

A closed-loop DC-DC buck converter designed using an STM32 microcontroller for PWM generation and feedback control. The project regulates the output voltage by adjusting the PWM duty cycle based on ADC feedback.

---

## Overview

This project demonstrates the design and implementation of a digitally controlled buck converter capable of providing a regulated DC output voltage from a higher DC input.

The controller continuously monitors the output voltage using the STM32 ADC and adjusts the PWM duty cycle to maintain the desired output under varying load conditions.

---

## Features

- STM32-based PWM generation
- Closed-loop voltage regulation
- ADC-based voltage feedback
- Adjustable output voltage
- High-efficiency switching operation
- Over varying load conditions

---

## Software Used

- STM32CubeIDE
- STM32 HAL Library
- LTspice XVII
- KiCad (optional PCB design)

---

## Hardware Components

- STM32F103C8T6 (Blue Pill)
- N-Channel MOSFET
- Schottky Diode
- Inductor
- Output Capacitor
- Voltage Divider
- Load Resistor

---

## Working Principle

1. STM32 generates a high-frequency PWM signal.
2. PWM drives the MOSFET of the buck converter.
3. Output voltage is sampled using the ADC.
4. The controller compares the measured voltage with the reference voltage.
5. PWM duty cycle is updated to minimize the voltage error.
6. The process repeats continuously to maintain a stable output.

---

## Simulation

The converter was first simulated in LTspice to verify:

- Output voltage regulation
- Inductor current ripple
- Output voltage ripple
- Switching waveform
- Transient response

Simulation results closely matched the hardware implementation.

---

## Results

| Parameter | Value |
|-----------|---------|
| Input Voltage | 12 V |
| Output Voltage | 5 V |
| Switching Frequency | 50 kHz |
| Efficiency | ~90% |
| Control Method | Closed Loop PWM |

---

## Learning Outcomes

- Buck converter design
- PWM generation using STM32
- ADC interfacing
- Closed-loop control systems
- LTspice simulation
- Embedded systems programming

---

## Screenshots



---

## References

This project was developed as a learning exercise based on standard buck converter design principles and STM32 embedded control techniques. Open-source resources and reference designs were consulted during development.
