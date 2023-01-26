# install platformio
python3 -c "$(curl -fsSL https://raw.githubusercontent.com/platformio/platformio/master/scripts/get-platformio.py)"

export PATH=$PATH:$HOME/.local/bin

ln -s ~/.platformio/penv/bin/platformio ~/.local/bin/platformio
ln -s ~/.platformio/penv/bin/pio ~/.local/bin/pio
ln -s ~/.platformio/penv/bin/piodebuggdb ~/.local/bin/piodebuggdb

# install lib_deps
`pio pkg install --library "mcci-catena/MCCI LoRaWAN LMIC library@^4.1.1"`