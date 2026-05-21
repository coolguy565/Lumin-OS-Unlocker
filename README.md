# Lumin OS Unlocker

You have likely arrived here from the main Lumin OS repository.

## How to Unlock
Simply get the Unlocker ZIP from releases. Extract to a folder named "USB0" on the Lumin OS directory.

You dont need to extract it directly to the Lumin OS directory, since USB0 is also a flat ZIP.

## How to Unlock 2
Launch launch.cmd from the Lumin OS folder, then enter the BIOS boot menu.

Select USB0, then when the unlock confirmation appears, select Y. If it stops at patch blocks ready, press enter.

It will automatically reboot, and voila! You have unlocked Lumin OS.

To install apps, move a .lapp file to USB0 and install it from the App Sideloader on the Lumin Desktop.


## But coolguy, how does it work?
Well, you can simply open USB0\boot\bootx64.cmd on Notepad to find out.

But heres my explanation.

The unlocker makes a backup of the kernel (lukrnl-backup.cmd),

And then patches the kernel by injecting additional lines using the symbols (flags on programming that point to places. If symbols didnt exist, we would have to guess, and thats really uncool).

It also installs App Sideloader and App Drawer by extracting them to data. The entries are already added from the kernel patches since the kernel is also userland.

## Screenshots
![Unlocked Desktop]()

Unlocked Lumin Desktop
