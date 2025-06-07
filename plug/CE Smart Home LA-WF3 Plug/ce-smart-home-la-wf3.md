# CE Smart Home LA-WF3 Plug
This configuration is for the CE Smart Home LA-WF3 Smart Plug. It has an **ESP8266** inside.
There are other products of different names that are compatible with this configuration.

More info for this device is available [here](https://templates.blakadder.com/ce_smart_home_LA-WF3.html). If your device looks like this, it is likely compatible with this configuration.

Components:
- Button
    - GPIO13
    - Pullup input, inverted
    - When pressed, will toggle the relay.
    - State exposed in Home Assistant

- Relay
    - GPIO12
    - State exposed and controllable in Home Assistant
    - When activated, turns on the Link/Blue LED.
    - When deactivated, turns off the Link/Blue LED.

- LED (Link / Blue)
    - GPIO4
    - Inverted
    - Set as the ESPHome status LED
    - State NOT exposed in Home Assistant

- LED (Power / Red)
    - GPIO5
    - Inverted
    - Only shows the state of the outlet
    - State NOT exposed in Home Assistant

- Status
    - This changes state when the device goes offline.