# ADC Controlled PWM LED

This project demonstrates how an analog voltage from a potentiometer can be converted into a PWM duty cycle to control the brightness of an LED.

Project focus:
- ADC configuration and usage
- PWM generation with hardware timers
- analog signal processing
- signal scaling
- threshold handling

## Hardware
- STM32 Nucleo-G0B1RE
- breadboard
- potentiometer connected to ADC1_IN0 (PA0)
- green LED connected to TIM1_CH1 (PA8)
- UART serial connection for debugging

## Notes
In order to be able to turn off the LED completely and reliably, I chose a lower threshold of 500 as ADC input. Such a high lower threshold was chosen to compensate for an ADC offset, likely caused by inexpensive hardware.

## Images
### Potentiometer Position Low
![LED off](Docs/images/01_LED_OFF.jpeg)

### Potentiometer Position Medium-Low
![LED low](Docs/images/02_LED_low.jpeg)

### Potentiometer Position Medium-High
![LED medium](Docs/images/03_LED_medium.jpeg)

### Potentiometer Position High
![LED high](Docs/images/04_LED_high.jpeg)