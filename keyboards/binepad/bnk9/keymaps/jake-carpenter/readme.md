# Binepad BNK9 setup

## Compiling

### Install dependencies
```bash
# from the root of the qmk_firmware repository
make binepad/bnk9:jake-carpenter
```

If this fails, try to reinstall/setup QMK:

```bash
brew uninstall qmk/qmk/qmk
brew install qmk/qmk/qmk
qmk setup jake-carpenter/qmk_firmware
```

## Flashing

NOTE: Cannot be flashed from QMK toolbox.

1. Unplug the device
2. Press and hold the knob
3. Plug the device in while the knob is pressed
4. Run the QMK flash command:

```bash
qmk flash --keyboard binepad/bnk9 --keymap jake-carpenter
```
