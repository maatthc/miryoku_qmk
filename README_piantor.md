#   My Piantor Miryoku layout

- Don’t connect or disconnect the TRRS cable when the keyboard is powered. Always disconnect the USB cable first.
- Flash the firmware on both Raspberry Pi Picos.
- Enter the bootloader mode by holding down the BOOTSEL button while reconnecting the board into USB port.

https://github.com/beekeeb/piantor
https://github.com/qmk/qmk_firmware/tree/master/keyboards/beekeeb/piantor

## Compile and Flash

### Install QMK
python3 -m pip install qmk

### Compile
qmk compile -c -kb beekeeb/piantor -km manna-harbour_miryoku

### Flash
qmk flash -c -kb beekeeb/piantor -km manna-harbour_miryoku

### Check debug logs
qmk console

### info

qmk info -kb beekeeb/piantor -km manna-harbour_miryoku

## Configuration

https://github.com/manna-harbour/miryoku_qmk/tree/miryoku/users/manna-harbour_miryoku#userspace

- users/manna-harbour_miryoku/custom_config.h
- users/manna-harbour_miryoku/custom_rules.mk
- keyboards/beekeeb/piantor/keymaps/manna-harbour_miryoku/config.h
- keyboards/beekeeb/piantor/keymaps/manna-harbour_miryoku/keymap.c

### Test

https://config.qmk.fm/#/test

### Symbols that correspond to keycodes available in QMK.
https://docs.qmk.fm/keycodes
