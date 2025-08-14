# Generic ESP8266 Square Plug
This configuration is for Generic **ESP8266** Square Plugs.
It has been confirmed to work with the following models:
- Bright Smart Plug
- Globe Smart Plug 50000

More info for this device is available [here](https://templates.blakadder.com/bright_741235077565.html). If your device looks like this, it is likely compatible with this configuration.

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
    - Will always be ON when the device is restarted.

- LED
    - GPIO14
    - Inverted
    - Set as the ESPHome status LED
    - State NOT exposed in Home Assistant

- Status
    - This changes state when the device goes offline.