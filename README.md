# Volumio plugin for RemotePi

This plugin is made for Volumio 2 and enables support for the RemotePi boards for Pi 3 B+/Pi 3 B and Pi 2/Pi 1 B+ from MSL Digital Solutions.

## Shutdown and cutting power
After activating the plugin the RemotePi board will get signaled as soon as Volumio is shut down via the GUI.
This allows the RemotePi board to cut power from the RasPi after the shutdown process has finished.

Further more the plugin detects the signal that is sent by the RemotePi board in case its hardware knob has been pressed or an IR power off signal from a remote control has been received.
The plugin then initiates the shutdown of Volumio and sends a signal back to the RemotePi. This allows the board to detect when Volumio's shutdown process has finished and cut the power afterwards.

## Set up IR receiver for LIRC
The plugin configures Volumio to load the necessary lirc-rpi overlay for the IR receiver of the RemotePi board. By default the gpio\_in\_pin parameter is set to 18.
But as RemotePi boards can be modified to use GPIO17 for the IR receiver instead of GPIO18 the plugin allows to set up the configuration accordingly.

**Note: The plugin will not install and setup LIRC!** This can be achieved by installing the IR remote controller plugin. Pay attention to get version 1.2.0 of the IR remote controller plugin. Earlier versions will override the gpio\_in\_pin setting with GPIO25.
