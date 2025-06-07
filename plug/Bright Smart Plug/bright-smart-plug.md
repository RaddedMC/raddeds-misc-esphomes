# Bright Smart Plug
This configuration is for the Bright Smart Plug, which has an **ESP8266 chip**.
It is a very simple smart plug. There are many others of a similar design.
More info for this device is available [here](https://templates.blakadder.com/bright_741235077565.html).

Components:
- Button
    - GPIO14
    - Pullup input, inverted
    - When pressed, will toggle the relay.
    - State exposed in Home Assistant

- Relay
    - GPIO12
    - State exposed and controllable in Home Assistant
    - When activated, turns on the LED.
    - When deactivated, turns off the LED.

- LED
    - GPIO14
    - Inverted
    - Set as the ESPHome status LED
    - State NOT exposed in Home Assistant