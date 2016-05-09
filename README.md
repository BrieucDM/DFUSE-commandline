DFU Commandline
=====

DFU Commandline allows the stm32 developers to program the device without using a JTAG/SWD ST-Link programmer devices.


Description
-----------------------

"DFU Commandline Master" project is intended to be used by stm32 programmers. 

ST released a modified version of DFU called DFUSE, it allows to program the STM32 through it's USB port

DfuFileMgr.exe converts a .hex file to a .dfu file following the DFUSE specification.

DfuSeCommand.exe then uploads the code into the target.

A tutorial and example is available in the archive.


How To Use
---------------------

1- First, Install the DFU driver located in the Driver folder.

2- Plug in your DFU device, make sure it's in DFU mode. If your driver is installed and
the device connected, you should see a DFU device in your device manager.

3- Your device is ready, now setup the IDE to load automatically the program.
You just need to adjust your compiler to execute the "load.bat" file after its compilation process is done.
Be sure the output HEX file name shall not have any spaces.

5- Congratulations Your IDE is now ready! Build your program and if the device is
plugged in the DFU mode, the loader will find and program it. Otherwise, it will
do nothing.


Calling the STM32 SystemMemory Bootloader from the user application firmware
-----------------------

To do this please refer to the following video from ST. Also you can use the "Blinky Sample" included in the project and  "CD00167594.pdf" file as a reference.

[Calling the STM32 SystemMemory Bootloader from your application](https://www.youtube.com/watch?v=cvKC-4tCRgw)

[Calling the STM32 SystemMemory Bootloader from the application firmware](https://www.youtube.com/watch?v=vQQ4yi4KXwU)

