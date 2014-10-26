# Garmin Edge 510 Restoration

This guide was written after my Edge 510 corrupted its filesystem, turning directories into broken file entries and preventing any further rides from being recorded.

## Requirements

* Garmin Edge 510 device
* [Garmin Express](http://software.garmin.com/en-US/express.html) to perform software updates.
* The `edge-510-filesystem.zip` file stored alongside this file.

## Instructions (Macintosh OS X)

1.  Plug the Garmin Edge 510 into your computer using the USB cable.
2.  Decompress the `edge-510-filesystem.zip` archive to the location of your choice.
3.  Open "Disk Utility" (`/Applications/Utilities/Disk Utility.app`).
4.  In the left-hand menu of the "Disk Utility" application select the partition labeled "GARMIN"
    ![Disk Utility selection screenshot](http://i.imgur.com/wklQBag.png)
5.  Click on the tab labeled "Erase" (between "First Aid" and "RAID"). Select "MS-DOS (FAT)" as the format and enter "GARMIN" (all capitalized) for the name. Press the "Erase..." button to erase the disk. This may take a long time (many minutes) as the device's flash memory is very low-speed.
    ![Disk Utility erase screenshot](http://i.imgur.com/KbRdRW5.png)
6.  Open the `edge-510-filesystem` folder that was created by step 2. Copy the contents of the folder (*NOT* the folder itself) into the directory. This may also take a long time to complete.
7.  Verify that the contents of the "GARMIN" device look like this now:
    ![Finder view of GARMIN](http://i.imgur.com/XDr7JhB.png)
8.  Disconnect the Edge 510 and reboot it. Wait for the device to reboot fully and verify that it brings up the default "RIDE" screen.
9.	Plug the Edge 510 back into the computer.
10. Run Garmin Express and allow it to update the firmware on the Edge 510.
11. Disconnect the Edge 510 and reboot it again. If the firmware required updating the device will show a progress bar and indicate that it is performing the update.
12. To verify that the device is recording properly, press the **Start/Stop** button and let a ride run for a few seconds. Press it again to stop, save the ride, and then tap on the folder icon on the main "RIDE" screen. Then tap on "Rides", followed by "Last Ride", followed by "Summary" once the ride has loaded. Confirm that there is time recorded.