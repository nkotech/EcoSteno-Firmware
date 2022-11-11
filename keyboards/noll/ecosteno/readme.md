Ecosteno
===

![Ecosteno](https://nolltronics.com/wp-content/uploads/2021/04/Noll-Steno-Front-Angle.jpg)

* Keyboard Maintainer: [Nathan Olivares](https://github.com/nkotech)
* Hardware Supported: Ecosteno v1.1.X with pink switches and V1.0.1X with blue switches
* Hardware Availability: [Nolltronics](https://nolltronics.com/product/ecosteno)

Make example for this keyboard (after setting up your build environment):

    make noll/ecosteno:default

Flashing example for this keyboard:

    dfu-util.exe -d 1eaf:0003 -a 2 -D "noll_ecosteno_default.bin"

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs). 

[Here's a quick video demonstrating how to flash firmware onto the ecosteno](https://youtu.be/dqeZ40PPEW4)

V1.1.X and V1.0.1X have different pinouts, but the only file this affects is config.h . It's set up to work with the newer 1.1.X boards, but all you have to do to build firmware for 1.0.1X boards is comment out the MATRIX_COL_PINS and MATRIX_ROW_PINS for the 1.1.X and uncomment the lines for the 1.0.1X.