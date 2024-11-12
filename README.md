## Building the Firmware

To build the firmware, follow these steps:

```bash
git clone https://github.com/QlDoors/minila-nano.git
git clone https://github.com/zmkfirmware/zmk.git
cd zmk
python3 -m virtualenv .venv --python=python3.7.5
source .venv/bin/activate
pip3 install -U west
west build -p -b dice_poker -- -DZMK_EXTRA_MODULES="/path/to/dice_poker" -DZMK_CONFIG="/path/to/dice_poker/config"
```

Replace `/path/to/dice_poker` with the actual path to the cloned dice_poker directory on your system.

## Keymap Editor

[https://nickcoutsos.github.io/keymap-editor/](https://nickcoutsos.github.io/keymap-editor/)