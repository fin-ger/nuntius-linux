Nuntius
===================================

##Introduction
Nuntius delivers notifications from your phone or tablet to your computer over Bluetooth.

Nuntius is an Open Source project from HolyLobster.

To use Nuntius you will need to install a companion tool on your phone or table and pair it via Bluetooth.

For more information on the project and the companion tools to install on the computer check https://github.com/holylobster

##The Icon
You may have questions on the icon. Nice shot.
In fact most of the Nuntius development time has been spent on the icon design concept.
If you have suggestions on how to improve it we are very open... but... we think it is hardly possible to do better than this.

##Some tips to debug
 * Launch the bluetooth dameon as "sudo  /usr/libexec/bluetooth/bluetoothd -d -n"
 * Using bluetoothctl
   * I had to set "agent on", "default-agent" and "trust 98:D6:F7:73:03:F1"
   * Having it running it will provide some information
 * /var/log/messages gives also some information about bluetoothd if you do not run it directly
 * run "sudo btmon > btmon.log" to get information from the devices that try to connect to the computer
   * This is very useful to see to which uuid is trying to connect and what kind of errors it gets

##Packages

* [Arch Linux (AUR)](https://aur.archlinux.org/packages/nuntius/)