# UART LED Control

## Overview
This project shows basic UART communication between an STM32 microcontroller and a PC.

- Microcontroller receives single-character input via UART
- Echoes received message back to the terminal
- Controls an LED based on user input:
	- '1' -> LED ON
	- '0' -> LED OFF

## Hardware
- STM32 Nucleo-G0B1RE
- External LED and 470 Ohm resistor

## Wiring
- PA8 (D7) -> resistor -> LED -> GND

## Software
- STM32CubeMX and HAL
- UART (USART2, 115200 baud)
- GPIO output

## Learning Goals
- Basic UART RX/TX communication
- Blocking I/O with HAL (`HAL_UART_Receive`, `HAL_UART_Transmit`)
- Simple command handling via serial input
