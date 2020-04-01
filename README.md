Adafruit-GPIO-Halt
==================

Press-to-halt program for headless Raspberry Pi. Similar functionality to the rpi_power_switch kernel module from the fbtft project, but easier to compile (no kernel headers needed).

I made a slight modification to point the button press to a script, which can then be customized as needed. (Used in RetroPie)

To install, just install normally through the Arcade Bonnet installed, selecting the pin you would like to use. (NOTE: GPIO 2 & 3 will cause bonnet controlls not to respond)

Then run
```git clone https://github.com/bizzar721/Adafruit-GPIO-Halt/
cd Adafruit-GPIO-Halt
make
sudo make install```

Replace `/usr/local/bin/gpio-halt` with the newly created `gpio-halt`

Create `shutdown.sh`, place in `home/pi/RetroPie/` and make executable with `chmod +x /home/pi/RetroPie/shutdown.sh`
