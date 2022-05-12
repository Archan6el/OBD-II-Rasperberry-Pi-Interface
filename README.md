# OBD-II-Rasperberry-Pi-Interface
Code in Python to interface a Raspberry Pi 4 with a Bluetooth OBD II Adapter to retrieve data and display values on a GUI using pygame

This code is free to be expanded upon and improved by others!

Connecting to the Bluetooth OBD II Adapter through the Raspberry Pi can be a hassle. This is a good reference, and provides the Linux commands done to do so:
https://www.hackster.io/tinkernut/raspberry-pi-smart-car-8641ca

When it comes to actually extracting the data from the OBD II Adapter, that can be a hassle as well. The adapter can be finnicky and can choose to provide commands, and sometimes will choose not to. An easy solution is to use a while loop that constantly queries with the adapter until the amount of supported commands returned is greater than 100, which you can see by used in "CarInterface.py"
