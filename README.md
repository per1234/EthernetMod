Modified Arduino Ethernet Library
==========

The stock Arduino IDE 1.6.2 Ethernet library with remoteIP() function added to EthernetClient. This function returns the IP address of the connected remote TCP server. Thanks to Philgaskin on the Arduino forum: http://forum.arduino.cc/index.php?topic=82416.0

#### Installation
- Download Ethernet library - Click the "Download ZIP" button(or "Clone in Desktop" if you have GitHub Desktop installed)
- Extract the Ethernet-master folder from the downloaded zip file
- Rename the folder Ethernet
- Move the folder to your arduino sketchbook\libraries folder
- Restart the Arduino IDE if it is open.

#### Usage
`remoteIP(remoteIPbuffer)` - see examples/ChatServer.ino for demonstration of using remoteIP
- Parameter: remoteIPbuffer - create a 4 byte array: byte remoteIPbuffer[4]; this buffer will contain the remote IP address after the function is called
  - Type: char array
- Returns: none

Arduino Ethernet documentation: http://arduino.cc/en/reference/ethernet
The read() function in the Client class inherits from Stream so the stream functions are also available:
Arduino Stream documentation: http://arduino.cc/en/Reference/Stream