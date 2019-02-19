# Devices and Protocols in Relation to the OSI Model

## MAC Address
The **Media Access Control (MAC)** address works on the **Layer 2 - Data Link** layer on the **OSI Model**. **MAC** addresses are unique to all devices with a **Network Interface Card (NIC)**. The **MAC** address is also referred to as our computers **Physical Address** as opposed to the **Internet Protocol (IP)** address which is the **Logical Address** to our computer over a network. We can not handle routing over a network with a **MAC** address but we can point to specific devices with by their **MAC** address.

- Layer 2 - Data Link
- Stands for Media Access Control Address
- Physicial Computer Address
- Unique to all Devices

## IP Address
The **Internet Protocol (IP)** address works on the **Layer 3 - Network** layer on the **OSI Model**. The **IP** address is also referred to as our computers **Logical Address**. The **IP** address is also unique to our computer but can be changed. The **IP** address is mapped to our computers **MAC** address which is how data being sent over the internet knows which computer it needs to send the data to.

- Layer 3 - Network
- Stands for Internet Protocol (IP)
- Logicial Computer Address
- Unique but can be changed
- Specifies which computer data should be sent

## EUI 64
**EUI 64** is another name for **IPv6 Global Unicast** which is just a much larger set of binary digits we can use to create **IP** addresses and is also a unique **IP** address but for each device. Because this address is unique to each computer we are able to use the **EUI 64** address instead of the **MAC** address to send data over a network which also means the **EUI 64** address is not mapped to the **MAC** address like a normal **IPv4** address, typically just referred to as the **IP** address. Because we do not need to translate this address to the computers **MAC** address, when working with the **EUI 64** address we are considered to be working with the **Layer - 2 Network** layer.

- Layer 2 - Network
- Referred to as the IPv6 Glocal Unicast Address
- Unique to each device

## Frames
**Frames** are what we are referring to when our data has been split and packaged up into smaller pieces before sending it over a network.

- Layer 2 - Data Link

## Packet
**Packets** are our **Frames** but when working on the **Layer 3 - Network** layer.

- Layer 3 - Network

## Switch
**Switches** are devices we can use on our network to connect multiple devices on the same network which allows us to send and receive data in the same network without needing the computers specific **IP** address.

- Layer 2 - Data Link
- Maps to MAC address

## Router
Allows us to move (route) data across multiple networks using **IP** addresses. Routers can also be referred to as a **Layer 3 Switch**.

- Layer 3 - Network
- Referred to as a Layer 3 Switch
- Moves Data across Network

## Multi-Layer Switch
**Multi-Layer Switches** are devices that are able to perform switching functions but are also able to perform routing functions when necessarry.

- Layer 2 - Data Link
- Layer 3 - Network
- Can perform Switching Functions
- Can perform Routing Functions

## Hub
A **Hub** is like a **Switch** but instead of sending information to everyone on the network or a specific **MAC** address, a **Hub** will send the data to everyone connected on the network.

- Layer 2 - Data Link
- Passes Information to Everyone

## Encryption Device
Physical devices on our network that encrypts outgoing data and decrypts incoming data.

- Layer 6 - Presentation
- Formats Data

## Cable
Physical cables on our devices such as computers, routers, switches, etc.

- Layer 1 - Physical
- Handles Physical Data Transfer

## Network Interface Card (NIC)
A card with a unique **MAC** address assigned to it sitting on each device.

- Layer 1 - Physical

## Bridge
Provides a connection from point A to point B. This connection can be a phsycial connection like an ethernet cable or a wireless connection like WiFi.

- Layer 2 - Data Link
