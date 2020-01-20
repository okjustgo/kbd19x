# kbd19x
Instructions, tools, links and hex files for flashing kbdfans kbd19x. Mainly for personal use. 

# How to flash kbd19x
1. Download QMK Toolbox https://qmk.fm/toolbox/
1. Use QMK Configurator https://config.qmk.fm/#/kbdfans/kbd19x/LAYOUT_ansi
1. Setup your keybinds in the configurator
1. Compile/Download firmware from config.qmk.fm
1. Put Keyboard in flash mode by holding "Esc" while plugging in the keyboard
    - You should see `*** DFU device connected: Atmel Corp. ATm32U4DFU`
1. Load hex file into QMK toolbox and Flash
    - If having trouble with drivers and getting "no devices found" you may need to fix the driver
    - Use Zadig https://zadig.akeo.ie/ and libusb-win32

# Technical info for KBD Fans kbd19x
- Controller atMega32u4

# Issues we had
- The most difficult part of determining the layout is how to deal with the absence of the standard insert/delete/home/end/pgup/pgdwn cluster. We ended up sacrificing pause, scroll lock, insert, rt ctrl, rt gui/menu.
- In our layout print screen, and delete keys were important
- For a more advanced layout, switching the "\" and "backspace" keys, going with a 1 unit "\" would allow the addition of the delete key above backspace. 

