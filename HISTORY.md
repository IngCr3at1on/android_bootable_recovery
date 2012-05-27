### 03/02/2012
* Initial import of repo and wrapper corrections.

### 03/28/2012
* Version bump: changes power button from 'select' to 'back' (change made to device directory).

### 03/30/2012:
* Move reboot menu into advanced menu and change normal menu reboot option back to 'reboot system now'.
* Changed fastboot option to say 'fastboot bootloader' instead of just 'fastboot mode' to hopefully negate confusion.
* Version bump.

### 04/11/2012:
* Added custom UI color switch (allows users to change UI color from the advanced menu, currently only allows for 'red', 'cyan', 'lime' and 'orange').
* Removed potentially hazardous sdcard options (these were disabled but we don't need them anyway).
* Removed key test, we only have one key.
* Removed wipe battery stats, [read why you don't need to wipe your battery stats](https://plus.google.com/105051985738280261832/posts/FV3LVtdVxPT).
* Version bump (kf1.4)

### 04/12/2012:
* Fixed issue with blank text on first boot.
* Version bump (kf1.5)

### 04/18/2012:
* Removed sdcard/ and splash/ from format/mount options (sdcard is potentially dangerous when unmounted and could cause issues with dualboot systems, if someone would like me to add the format option back in just say so. As for splash; while I don't know of anything about it being dangerous I figured it would be best to eir on the side of caution).
* Moar Colors!!!
* Version bump (kf1.6)

### 05/11/2012
* Apply patch : Retouch Binaries (backported from ICS for 3.0 boot image compat), this requires the ICS 'system/extras/ext4_utils/' repo. (need to test full build to see if this causes any issues with the rom itself).
* Updated readme to reflect build requirements.
* Possibly fix signature verification status on boot (needs testing).
* Version bump (kf1.8)

### 05/12/2012
* Removes static tag from ensure_directory in nandroid.c for external use.
* Adds call to nandroid.h for ensure_directory.
* Added call to color switch in extendedcommands.c to ensure_directory (to resolve issues with the color switch on first boot {in the event 'sdcard/clockworkmod/' doesn't exist}).
* Cleaned up otherwise removed code from previous patch.
* Version bump: kf1.9
