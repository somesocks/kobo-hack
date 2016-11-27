kobo-hack
=========

A repository for building tools for the Kobo Aura(non HD)


Usage
-----

Ensure you have `arm-linux-gnueabihf` compiler suite installed somewhere and available in your `PATH`.
If you're on Arch Linux, you can use https://aur.archlinux.org/packages/arm-linux-gnueabihf-gcc


Run `make` in the top directory. 
If all goes well, a file called `KoboRoot.tgz` will have been made inside the 'build' directory.


To apply the update, copy the `KoboRoot.tgz` file to the `.kobo` folder on the Kobo device. 
As soon as you eject the Kobo, it will reboot and start applying the update.


After the update has completed, when WiFi is connected, 
and the device is powered on (so it cannot be 'Sleeping' or 'Powered off'), 
you can `telnet` to the device's IP.  The IP can be found in `Settings->Device information`.
