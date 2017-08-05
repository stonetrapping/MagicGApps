# MagicGApps 7.1.x ARM, ARM64



***
You may be asking yourself, "But... why?"

Well, first off, the targets are tweak freaks like me and those who own devices with limited system space.

This systemless implementation of GApps makes it easier to customize and update the included Google setup. 

For instance, ever seen that feature in Titanium Backup, "Integrate system app updates into ROM? Exactly. Now you can do that without writing to the system partition and then repack the module with the updated changes.

If you are into doing this sort of thing, [U]you must resize magisk.img[/U] to a value slightly larger than the sum of the files you want to integrate into /system, systemlessly before proceeding. To achieve that, run the following commands on terminal emulator:

`su
resize2fs /data/magisk.img xM`

Where "x" is the size in MegaBytes.

Example:

`resize2fs /data/magisk.img 200M`

This results on a magisk.img size of 200MB.

Don't worry if you added too much space. Magisk will shrink the image automatically upon next boot.

Moving on, you can add/replace/remove things from the package to suit your needs the easiest and fastest way possible (you will see some of these cool tweaks below). One more advantage: your ROM updates will be slightly faster, since GApps don't have to be backed up and restored afterwards every time you flash a new version of your ROM thanks to addon.d feature. AND my favorite, you can make regular backups of your magisk.img file to simplify future ROM setups even further!



***
PACKAGE SETUP

Full Google Framework

Core syncing APKs (i.e., Google Play Services, SetupWizard, Google Play Store)

Default permissions to prevent FCs

Google App, Google TTS + off-line voice data, Face Unlock and legacy LatinIME swype libs

Battery & data saving patches (hungry GApps removed from "power whitelist" -- /system/etc/sysconfig/google.xml)

Dynamic installer (single package for both ARM & ARM64)



***
Credits:

The Flash, BeansTown106, Surge1223, BaNkS, otonieru & others



***
XDA Thread: https://forum.xda-developers.com/apps/magisk/module-systemless-beansgapps-mini-7-1-x-t3611362

Well, first off, the targets are tweak freaks like me and those who own devices with limited system space. This systemless implementation of GApps makes it easier to customize and update the included Google setup. 

For instance, ever seen that feature in Titanium Backup, "Integrate system app updates into ROM? Exactly. Now you can do that without writing to the system partition and then repack the module with the updated changes. If you are into doing this sort of thing, [U]you must resize magisk.img[/U] to a value slightly larger than the sum of the files you want to integrate into /system, systemlessly before proceeding. To achieve that, run the following commands on terminal emulator:

`su
resize2fs /data/magisk.img xM`

Where "x" is the size in MegaBytes.

Example:

`resize2fs /data/magisk.img 200M`

This results on a magisk.img size of 200MB. Don't worry if you added too much space. Magisk will shrink the image automatically upon next boot.

Moving on, you can add/replace/remove things from the package to suit your needs the easiest and fastest way possible (you will see some of these cool tweaks below). One more advantage: your ROM updates will be slightly faster, since GApps don't have to be backed up and restored afterwards every time you flash a new version of your ROM thanks to addon.d feature. AND my favorite, you can make regular backups of your magisk.img file to simplify future ROM setups even further!



***
PACKAGE SETUP

Full Google Framework

Core syncing APKs (i.e., Google Play Services, SetupWizard, Google Play Store)

Default permissions to prevent FCs

Google App, Google TTS + off-line voice data, Facelock and legacy LatinIME swype libs

Battery & data saving patches (hungry GApps removed from "power whitelist" -- /system/etc/sysconfig/google.xml)

Dynamic installer (single package for both ARM & ARM64)



***
Credits:

The Flash, BeansTown106, Surge1223, BaNkS, otonieru & others



***
[XDA Thread](https://forum.xda-developers.com/apps/magisk/module-systemless-beansgapps-mini-7-1-x-t3611362)

[GitHub Repo](https://github.com/Magisk-Modules-Repo/MagicGApps)