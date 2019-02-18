# OSI Model Layers

## Mnemonic
Mnemonic to easily remember the seven layers of the OSI Model.

- Physical
  - Please

- Data
  - Do

- Network
  - Not

- Transport
  - Throw

- Session
  - Sausage

- Presentation
  - Pizza
  
- Application
  - Away

## Layer 1 - Physical
The physical layer is where we start to convert our data into signals or vice versa

- Cables
- Physical/Electrical
- Pinouts
- Voltages
- Cable Specifications
- Network Interface Cards (NIC)
- More...

## Layer 2 - Data Link
The Data Link layer is where we gain access to our device(s) such as computers, mobile phones, IoT devices, etc. This layer is going to take the data sent from the Physical layer and package that data into bits or frames.

The Data Link layer also deals with our devices Media Access Control (MAC) address which is hardcoded into our devices NIC that gives each device its own unique address. NIC manufacturers are given a certain range of numbers to use in order to keep each MAC address unique to each NIC. Hypothetically, if we had two devices with the same MAC address we would potentially have connectivity issues with these devices.

- Gives access to physical device
- Converts data being sent out into frames
- Converts frames being received into raw data
- Media Access Control (MAC)
- Switches/Hubs

## Layer 3 - Network (IP Layer)
This layer allows us to take our data and send it over different networks depending the IP address, "Logical Address", that is mapped to a MAC address, "Physical Address".

- Referred to as IP Layer
- Transfers data from one-one or one-many networks
- Converts IP address, "Logical", to MAC address, "Physical", and vice versa
- Performs network routing functions, fragmentation, and reassembly
- Routers

## Layer 4 - Transport
The Transport layer helps manage and control which protocol the packets will be sent over, **Transmission Control Protocol (TCP)** or **User Datagram Protocol (UDP)**, and splits them into different packages. 

Intsead of sending large amounts of data at a time, say 1gb of data, packets are broken down, the size depends on the protocol used as they each have their own max packet size, and sent over the protocol in waves which makes the transfer of data more manageable and less likely to be corrupted which also depends on the protcol used. TCP is better at managing the packets and is less likely to be corrupted and UDP will stream packets and is more likely to lose packets but is faster than TCP.

TCP is better at managing packets and verifies that the packets are received, and assembled in the correct order but is slower because it needs to verify that the receiver has received the first packet before sending the next. This protocol is suited for sending and downloading files where all the data needs to be sent and received where corruption could ruin an entire download.

UDP is much faster and instead of taking time to manage the packets sent, UDP will send a constant stream of data from one end to the other. Things like, Zoom, Skype, YouTube, etc. use UDP to send data over as fast as possible with as little latency as possible. The reason this is faster is because unlike TCP, UDP will not wait for the receiver to verify that they have received the data and will continue to push more and more data as is needed. This protocol is suited for sending and receiving data where if some data might go missing this is not a problem.

- Management Control
- Transfer of Data
- Split Communications into Packages
- Protocol Types
  - Transmission Control Protocol (TCP): Verified
  - User Datagram Protocol (UDP): Not Verified

## Layer 5 - Session
The Session layer is where we establish, manage, and terminate connections between devices.

- Traffic Control
- Controls connections between devices
  - Establish Connections
  - Manage Connections
  - Terminate Connections

## Layer 6 - Presentation
Takes our packages and transform them in a way that our **Layer 7 Application** layer can read and display the data for humans.

- Translates Data
- Independant from differences in data representation
- Formats data: Encryption/Decryption

## Layer 7 - Application (Network Access)
The Application layer decides whether or not our applications are able to access the network we are trying to received data from and from what protocol: SMTP, HTTP(S), FTP, etc. It also identifies where or if at all we are able to connect to the network.

- Network Access
- Enables applications to access network
- Determines resources availability
- Synchronize communication
- Determines protcol we can receive data from
- Displays data to user

## Summary of Layers
- Layer 1 - Physical
  - Established a physical connection. If you can touch it this is Layer 1.

- Layer 2 - Data Link
  - Established a data link connection. Handles MAC address of device to make sure packets are being sent/received appropriately.

- Layer 3 - Network
  - Packages are given an IP address where they should be sent to.

- Layer 4 - Transport
  - Established protocol to send data over, TCP or UDP.

- Layer 5 - Sessions
  - Establish connections between multiple devices, how long to wait for a response, when to terminate connection.

- Layer 6 - Presentation
  - Encrypt outgoing data; Decrypt incoming data.

- Layer 7 - Application
  - Displays data (what the user can view).

## All Layer Explanation Examples
Here is a [post on r/computing](https://www.reddit.com/r/computing/comments/1o5cmp/eli5_osi_layer_model/) detailing the OSI Model in a simple way. There are multiple responses as well that give a different kind of explanation so if one doesn't make sense then read the next one.