# AccessibilityAccessPad

AAPad is an 8 key macropad with a rotary encoder, an OLED Display. It also has 9 WS2812B Leds, and uses QMK firmware

It serves as a plug & play device integrated with the Windows accessibility toolkit in order to allow computer-illiterate users use of accessibility features (i.e. high contrast mode). 

## Features:
- Dual layer PLA case (hopefully made out of wood, later)
- Plexiglass window, displaying the diodes and silkscreened logo on the PCB (also my glasses )
- 128x32 OLED Display, to allow bystanders to assist the user whenever necessary
- EC11 Rotary encoder, for tactile feedback
- 9 WS2812B RGB LEDs. One for the accessibility icon, and the rest for backlighting
- 8 Keys (for functions, see below)

## Planned Features:
- [VIA](https://www.caniusevia.com/) support!
- Reactive backlight for each key

## CAD Model:
Everything fits together using 6 M3 Bolts and heatset inserts. 4 for the case, two for the PCB.

It has 2 separate printed pieces. The base, where the PCB is mounted, and the cover.

<img src=assets/IMAGE_CAD.png alt="3D Cad Model" width="500"/>

Made in Fusion360. First time using it!


## PCB
Here's my PCB! It was made in KiCad. The silkscreen(s) was imported from Canva. I also put a quote on the top right, because why not?

Schematic
<img src=assets/IMAGE_SCHEM.png alt="Schematic" width="300"/>

PCB
<img src=assets/IMAGE_PCB.png alt="PCB" width="300"/>

## Firmware Overview
This hackpad uses [QMK](https://qmk.fm/) firmware for everything. 

- The rotary encoder changes volume, press to mute

- The 8 keys currently act as functions/macros I preassigned in QMK.
    1. Text-to-Speech (TTS) Toggle
        - Reads aloud selected text on screen
    2. Zoom In
    3. Zoom Out
    4. Speech-to-Text Activation
        - Starts or stops dictation mode to convert speech into text
    5. Adjusts Cursor Speed
    6. Activates Computer speakers to announce a custom message (preset "I need assistance")
    7. High Contrast Mode Toggle
    8. Opens Accessibility Settings Window

- The OLED reads out the function of a button whenever it is pressed. The goal is so that any bystander who is called to assist the user may know what the device is suppose to be doing at any given input.

- *Note*: **Please suggest any new functions for each key!!** I have a very limited understanding of accessibility needs at the moment, though I hope my preset functions serve you well.

## BOM:
Here should be everything you need to make this hackpad

- 8x Cherry MX Style Switches
- 8x DSA Keycaps
- 6x M3x5x4 Heatset inserts
- 3x M3x16mm SHCS Bolts
- 9x 1N4148 DO-35 Diodes.
- 9x WS2812B LEDs
- 1x 0.91" 128x32 OLED Display
- 1x EC11 Rotary Encoder
- 1x XIAO RP2040
- 1x Case (2 printed parts, PLA)


## Extra stuff
Thanks so much for reading to the end, this is my first real hardware project. Stay tuned to my GitHub for more :\)\)

~ Adarsh
