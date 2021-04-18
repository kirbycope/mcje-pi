# Minecraft Java Edition for the Raspberry Pi
This project suppliments the Minecraft instal you can do using PiApps. If you are unfamilar with that setup, see this [guide](https://flynnsforge.com/easily-install-minecraft-java-edition-on-the-raspberry-pi4/).

## What this script does
Installs [lwjgl](https://www.lwjgl.org/), [Optifine](https://www.optifine.net/home), and a graphics preset.

## What you should do first
1. Open terminal and run `sudo apt-get -y install xcompmgr libgl1-mesa-dri && sudo apt-get -y install libalut0 libalut-dev && sudo apt-get -y install mesa-utils`
1. Run `raspi-config`
1. Go to "Advanced" and enable the Fake Graphics driver
1. Save and reboot

## Running the script
Open terminal and paste in the following, `wget -qO- https://raw.githubusercontent.com/kirbycope/mcje-pi/main/install | bash` and then press [Enter]

## Running Minecraft
1. Run the Minecraft Launcher
1. Select "Edit Profile"
1. Check "JVM Arguments" 
   - If you chose 'Fastest' during the install, add `-Dorg.lwjgl.librarypath=/home/pi/lwjgl2arm32`
   - If you chose 'Latest' during the install, add `-Dorg.lwjgl.librarypath=/home/pi/lwjgl3arm32`
   - Change `pi` to your username if you changed it from the default
## Credits
How to setup Minecraft 1.8.9 on RaspPi2 - https://www.raspberrypi.org/forums/viewtopic.php?t=137279
How to setup any version of Minecraft on Pi4 - https://www.raspberrypi.org/forums/viewtopic.php?t=284448
Graphics Settings - @Megumir on https://discord.com/invite/jQCpfVK
