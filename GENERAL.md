# Generalities

These are a few tips in order for you to hit the ground running when trying to spin up a new/related device (sub-)profile

## How to root

Assuming the bootloader is unlocked, there are solutions that are able to repack an original/stock boot.img, **from** the device,
using an application on the Android device. Ask your device team for details; some of these apps may or may not have a existing
reputation.

## EDID location

Check in the directories under `/sys/class/drm`. The exact sub-directory may differ across devices.
