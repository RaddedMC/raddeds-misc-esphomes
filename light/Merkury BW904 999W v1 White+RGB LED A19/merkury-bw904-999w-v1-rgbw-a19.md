# Merkury BW904 999W v1 White+RGB LED A19 (2018)
This configuration is for the Merkury BW904 999W White+RGB LED A19 smart bulb.
Some models of this bulb, with a 2018 or older manufacture date, have an **ESP8266** inside.
This is an A19 smart bulb with an RGB LED and a single channel white LED (RGBW).

More info for this device is available [here](https://templates.blakadder.com/merkury-MI-BW904-999W.html).

> [!WARNING]  
> The pinouts for the 2019 and later models of this bulb are different. Make sure your bulb is a [2018 or "v1"](https://templates.blakadder.com/merkury-MI-BW904-999W.html), not a ["v2"](https://templates.blakadder.com/merkury-MI-BW904-999W-v2.html) or ["v3"](https://templates.blakadder.com/merkury-MI-BW904-999W-v3.html).

> I have a 2019 model as well and will attempt to flash it in the future.


Components:
- SM16716 RGB Controller
    - Data: GPIO14
    - Clock: GPIO4
    - 3 channels, 1 chip
        - Red: Channel 2
        - Green: Channel 1
        - Blue: Channel 0
        - (A BGR configuration)

- Power supply
    - GPIO13

- Light PWM
    - GPIO5
    - PWM Frequency of 1000hz

- Status
    - This changes state when the device goes offline.

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
    - Rainbow:
        - A colour wheel effect.
        - From [C0ntroller](https://gist.github.com/C0ntroller/3125650c07c30f9ca6de439a730e0a97)
    
> [!INFO]
> I'm also working on adding the [WLED realtime control protocol](https://esphome.io/components/light/#wled-effect) effect.