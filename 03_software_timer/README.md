# Software Timer LED

## Overview
This project explores non-blocking timing on an STM32 using a simple software timer approach.
- LED toggles every 500 ms
- no use of `HAL_Delay()`
- timing based on `HAL_GetTick`

## Hardware
- STM32 Nucleo-G0B1RE
- breadboard
- LED and 470 Ohm resistor

## Wiring
- PA9 (D8) -> resistor -> LED -> GND

## Software
- STM32CubeMX + HAL
- GPIO output
- Software timer using system tick

## Learning
- Basic understanding of non-blocking programming
- Basic event-driven design
- Foundation for multitasking systems