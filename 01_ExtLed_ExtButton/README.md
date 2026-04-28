# External LED controlled by external Push Button

## Overview
Simple STM32 project:
- Button pressed -> LED ON
- Button released -> LED OFF
- UART debug message on state change

## Hardware
- STM32 Nucleo-G0B1RE
- Breadboard, wires
- LED and 470 Ohm resistor
- Push Button

## Wiring
- LED: PA9 -> resistor -> LED -> GND
- Button: PA8 -> button -> GND (internal pull-up)

## Software
- STM32CubeMX (for Pinout-Settings)
- HAL
- GPIO input/output
- UART (USART2, 115200 baud)
- State change detection (no debouncing)

## Learning Goals
- GPIO basics
- pull-up concept
- Embedded control loop
- UART debugging

