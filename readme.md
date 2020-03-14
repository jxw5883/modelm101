# modelm101

This is a configuration for the QMK firmware for reversible conversion of IBM's Model M keyboards based off iw0rm3r's mainline config (common 101-key ANSI and 102-key ISO models).

Unlike the config on the QMK repo, the configuration is built for the Atmel ATmega32U4 controller, which you can easily use on a Teensy 2.0 or an Arduino Micro (not the Pro Micro).  

Specify pins you use for your keyboard matrix in `config.h` and build with the following commands.

If you're using an arduino micro, run:

    make converter/modelm101:converter_modelm101_layout_jxw5883:avrdude

If you're using a teensy, run:

    make converter/modelm101:converter_modelm101_layout_jxw5883:teensy
    
See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).
