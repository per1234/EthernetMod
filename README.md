Modified Arduino Ethernet Library
==========

Modified Arduino 1.5+ Ethernet Library. The standard Ethernet library has a remoteIP() function for UDP communication but not TCP. This modification of the stock library provides the remoteIP() function to EthernetClient so it can be used for TCP communication as well. This function returns the IP address of the connected remote TCP server. Thanks to Philgaskin on the Arduino forum: http://forum.arduino.cc/index.php?topic=82416.0

#### Installation
- The library is available for download here: http://github.com/per1234/Ethernet
- Choose the correct branch for your Arduino IDE version. The currently selected branch is only compatible with Arduino versions 1.5 and up.
- Click the "Download ZIP" button.
- Extract the Ethernet-master folder from the downloaded zip file.
- Rename the folder Ethernet.
- Move the folder to the libraries folder under your Arduino sketchbook folder as configured in Arduino IDE File>Preferences>Sketchbook location.
- Restart the Arduino IDE if it is open.

#### Usage
`remoteIP(remoteIPbuffer)` - See examples/ChatServer.ino for demonstration of using remoteIP.
- Parameter: remoteIPbuffer - Create a 4 byte array: byte remoteIPbuffer[4]; this buffer will contain the remote IP address after the function is called.
  - Type: 4 byte array
- Returns: none

For all the standard functions included in the library see the official Arduino Ethernet documentation: http://arduino.cc/en/reference/ethernet
The read() function in the Client class inherits from Stream so the stream functions are also available, see the Arduino Stream documentation: http://arduino.cc/en/Reference/Stream

#### License

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public
License along with this library; if not, write to the Free Software
Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA