# Systemless Dalvik Xposed Framework

### This module is only for Android 4.2 to 4.4W!

You must select "Recovery (write zip to SD card, flash manually)" Installation mode in Xposed Installer, and click "Install/Update" button, then click "Cancel" before install this Magisk module.

The binaries are extract from Xposed Installer [https://repo.xposed.info/module/de.robv.android.xposed.installer](https://repo.xposed.info/module/de.robv.android.xposed.installer).

This module will never get any updates in the future, since @rovo89 has stopped development. This module is here for historical reasons.

For other Android version, check the Wiki: [https://github.com/ElderDrivers/EdXposed/wiki/Available-Android-versions](https://github.com/ElderDrivers/EdXposed/wiki/Available-Android-versions)

## Linker Patch

The app_process will trigger `Warning: linker: app_process has text relocations. This is wasting memory and is a security risk. Please fix.`.

This repo contains a fixed `linker` executable to remove this warning from stderr. 

The linker is extracted from UFI001C firmware. For other devices, you should extract the `/system/bin/linker` and patch it on your own.