# Bright 34205 White LED A19
This configuration is for the Bright 34205 White LED A19 smart bulb. It has an **ESP8266** inside.
This is an A19 smart bulb with a dimmable single channel white LED.

More info for this device is available [here](https://templates.blakadder.com/bright_741235077572.html).

Components:
- Light PWM
    - GPIO5
    - PWM Frequency of 1000hz

- Switch
    - GPIO13
    - I don't know what this does, so I skipped it in the config

Extra features:
- Restore mode:
    - When the light loses power, it will return to its previous brightness level.
- Effects:
    - Slow pulse:
        - The light fades on and off over an interval of 10 seconds.
    - Fast pulse:
        - The light fades on and off over an interval of 2 seconds.
    - Candlelight:
        - The default flicker effect. (1.5% intensity)
    - Sparkle:
        - The flicker effect at 10% intensity