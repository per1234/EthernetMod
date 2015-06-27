Modified Arduino Ethernet Library
==========

Modified Arduino 1.0.x Ethernet Library. The standard Ethernet library has a remoteIP() function for UDP communication but not TCP. This modification of the stock library provides the remoteIP() function to EthernetClient so it can be used for TCP communication as well. This function returns the IP address of the connected remote TCP server. Thanks to Philgaskin on the Arduino forum: http://forum.arduino.cc/index.php?topic=82416.0


#### Installation
- Choose the correct branch for your Arduino IDE version. The currently selected branch is only compatible with Arduino versions 1.0.x.
- Download the most recent version of EtherEvent here: https://github.com/per1234/Ethernet/archive/Arduino-IDE-1.0.x.zip
- Extract the downloaded file
- Rename the extracted folder Ethernet
- Copy the Ethernet folder to the libraries folder under your sketchbook folder
- Reopen the Arduino IDE


#### Usage
`EthernetClient.remoteIP()` - See examples/ChatServer.ino for demonstration of using remoteIP.
- Returns: The IP address of the remote connection.
  - Type: IPAddress

For all the standard functions included in the library see the official Arduino Ethernet documentation: http://arduino.cc/en/reference/ethernet
The read() function in the Client class inherits from Stream so the stream functions are also available, see the Arduino Stream documentation: http://arduino.cc/en/Reference/Stream


#### License
This file is free software; you can redistribute it and/or modify it under the terms of either the GNU General Public License version 2 or the GNU Lesser General Public License version 2.1, both as published by the Free Software Foundation.

This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License along with this library; if not, write to the Free Software Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA
