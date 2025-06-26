# Broadcast Containment

## Broadcast Domains

- When a broadcast msg is sent
    - Broadcast is processed by every host in the network
    - Switches forward the msg to all connected hosts on teh same local network
    - For this reason, a local area network, a network with one or more Ethernet switches, is also referred to as a broadcast domain

- The number of hosts and the amount of network traffic that can be supported on the local network is limited by the capabilities of the switches used to connect them

- As the network grows and more hosts are added, network traffic, including broadcast traffic, increases

- To improve performance, it is often necessary to divide one local network into multiple networks, or broadcast domains

- Routers are used to divide the network into multiple broadcast domains

## Access Layer Communication

- On a local network a host only accepts a frame if
    - The MAC address corressponds to its own MAC address
    - Or the MAC address is a Broadcast MAC address

- For eg, a host PC1 will only receive a packet if the packet's destination address is 
    - Its own (PC1) MAC address
    - Or Broadcast MAC address

- Most network application however rely on only logical (IP) address to identify the location the servers and clients

- Problem arises if a sending host only has the logical IP address of the destination host

#### How does the sending host determine what destination MAC address to place within the frame?

- The sending host can use an IPv4 protocol called **Address Resolution Protocol (ARP)** to discover the MAC address of any host on the same local network

- IPv6 uses a similar method known as **Neighbor Discovery (ND)**.

## Address Resolution Protocol

- Applicable to devices in the same local network
- When a device has an IP address of a host and wants to know its MAC address
    - It sends an **ARP request (a broadcast)** to all the devices on the local network
    - All devices receive this frame and compare it with their IPV4 address
    - The device with the same IPV4 address sends out an **ARP reply (containing the MAC address of the device)** to the sender
    - The sender receives the msg and stores the IPV4 address and the received MAC address in a table called **ARP table**

#### Note:

- When the sending host has the MAC address of the destination host in its ARP table, it can send frames directly to the destination without doing an ARP request

