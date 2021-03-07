# Ado-SiCK-68

![sick68](https://github.com/heitorado/ado-sick68/blob/main/build_log/a_keyboard_is_born.JPG?raw=true)

The SiCK-68 is a custom 3D printed mechanical keyboard built from scratch without the price tag often associated with one. It uses the Tada68 layout but a Teensy 2.0 as microcontroller.

The Ado-SiCK-68 is a slightly modified version which includes:
- Modified bottom parts of 3D printed case to fit a RGB Led stripwith 55 LEDs on the inner walls [TODO] add thingiverse link of my remix
- QMK Configuration files with RBG enabled and keymaps to enable RGB effects and color control
- My QMK Configurator JSON file so you can easily update the Keymap
- [TODO] Wrist support since the keyboard got a bit taller
- [TODO] Custom sized keys printed in the [SA Keycap Profile](https://i1.wp.com/thekeeblog.com/wp-content/uploads/2020/10/gtderEvan.png). This makes the Keyboard even taller. I'm thinking on trying out some switches on the DSA profile to see which one feels better to type.
- [TODO] Build log with tips for people that, like me, are building their very first handwired keyboard.

## QMK Setup
In this repo I have added only the modified files for building my alternate version of the handwired sick-68 keyboard. So If you want to build this same version or just use the configuration files as a starting point for building your own, you have to copy the contents of this repo (the contents, not the repo itself!) inside the `keyboards/handwired/sick-68` folder. This will overwrite the default settings there (which are for an arduino pro micro, does not have RGB and has different keybindings for Layer 1) with my files, which will change the build to use a Teensy, enable RGB, etc. After you've done that you can run the make command specified below to generate the Hex file.

* Keyboard Maintainer (for this version, firmware only): [heitorado](https://github.com/heitorado)
* Hardware Supported: Teensy 2.0
* Hardware Availability: [files to print and documentation](https://www.thingiverse.com/thing:3478494)

Make example for this keyboard (after setting up your build environment):

    make handwired/sick68:ado

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).
