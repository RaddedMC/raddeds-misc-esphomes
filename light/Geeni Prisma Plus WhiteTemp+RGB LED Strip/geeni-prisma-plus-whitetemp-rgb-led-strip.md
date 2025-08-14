# Geeni Prisma Plus WhiteTemp+RGB LED Strip
This configuration is for the Geeni Prisma Plus WhiteTemp+RGB LED Strip. It has an **ESP8266** inside.
This is a single-channel RGBWW LED Strip.

More info for this device is available [here](https://templates.blakadder.com/geeni_GN-EW005-999S.html).

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