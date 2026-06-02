This Project is an attempt to make my Mom life a bit easier.

The general idea of the project is as follows.

The irrigation system will have 1 Main Unit(MU) and roughly 6-7 node (N)

It realy doesn't matter how many node we need really since all node will be using the same code and will communicate with the MU to get its' own settings and operation time.

The MU will do a few things, first is that it will displace a localhost website that display settings, connected node (renamable), and it will have an "embedded" front and back-end.

Front-end is per usual, we simply display some static element such as button. Since this is the first commit, I would say that the only way I can redirect to another page (for settings) is to write another .html. But we'll see.

The settings page will have some dynamic element to it such as extendable container to display more device connected and for connection.

The back-end will be handle by Python such as Bluetooth connection/scanning, setting up Wifi for each ESP32 node (don't know how to do it yet). And managing which node to turn on or off depending of how each node perform.

Then the is the database side. Not too complicated, simply some PostgreSQL to store the information of each ESP32 node, such as its' setting (each node also store its' own setting to reduce the need for communication), IP address, and names, as well as time, and water pressure or volume settings.

On the small scale of thing, we simply will implement a BT only version first before adding Wifi for remote control.

So, our task right now is writing up a dynamic container for device connection, and potentially an (i) button to redirect the UI straight to individual device settings.

Then we will do some Physics calculation on Water Pressure, Volume and Time, since I haven't had any ideas what type of irrigation system to do yet. So these settings will be push-back after irrigation design (including pressure sensor, solenoid valve, solar power, and so more stuff), but we'll see.
