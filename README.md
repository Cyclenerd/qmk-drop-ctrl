# Massdrop CTRL Keymap

![CTRL](https://massdrop-s3.imgix.net/product-images/massdrop-ntkl-mechanical-keyboard/FP/W6zvr0cTR4KVDY5z8rwp_AI7B6588%20copy%20page.jpg?auto=format&amp;fm=jpg&amp;fit=max&amp;w=700&amp;h=467&amp;dpr=1&amp;q=80)

The Massdrop CTRL is a TKL mechanical keyboard featuring dual USB-C connectors, an integrated Hi-Speed USB 2.0 hub, and fully customizable RGB backlighting and underlighting.

Keyboard Maintainer: [Massdrop](https://github.com/massdrop)  
Hardware Supported: Massdrop, Inc. CTRL PCBs utilizing Microchip&#39;s ATSAMD51J18A MCU and USB2422 2-Port USB 2.0 Hi-Speed Hub Controller, and ISSI&#39;s IS31FL3733 LED Drivers.  
Hardware Availability: [Massdrop CTRL Mechanical Keyboard](https://www.massdrop.com/buy/massdrop-ctrl-mechanical-keyboard)

This custom keymap is based on the [Endgame keymap](https://github.com/qmk/qmk_firmware/tree/master/keyboards/massdrop/ctrl/keymaps/endgame).

## Install

With QMK CLI:
```shell
# Setting Up Your QMK Environment
sudo apt install -y git python3-pip
# Install the QMK CLI
python3 -m pip install --user qmk
# Setup
qmk setup
# Compile firmware with default keymap
qmk compile -kb massdrop/ctrl -km default
```

Without QMK CLI:
```shell
git clone --recurse-submodules https://github.com/qmk/qmk_firmware.git
cd qmk_firmware
util/qmk_install.sh
make massdrop/ctrl:default
```

[Need more help?](https://github.com/qmk/qmk_firmware/blob/master/docs/newbs_getting_started.md)

## Add Custom Keymap

```shell
# Clone this repo
git clone https://github.com/Cyclenerd/qmk-drop-ctrl.git
# Link custom keymap to QMK firmware
ln -s /mnt/c/Users/Nils/Projects/qmk-drop-ctrl/ qmk_firmware/keyboards/massdrop/ctrl/keymaps/nils
# Compile custom keymap
qmk compile -kb massdrop/ctrl -km nils
```

## Flash

Flash `massdrop_ctrl_nils.bin` (in root folder `qmk_firmware`) with [QMK Toolbox](https://github.com/qmk/qmk_toolbox).