# IPV4 Unicast, Broadcast and Multicast

- **A source IP address is always a unicast address**
- **Destination IP address can be** 
    - ***Unicast***
    - ***Broadcast***
    - ***Multicast***

## IPV4 Unicast

- Unicast refers to one device sending a msg to anither device in **one-to-one communication**
- The destination IP address is a unicast address (msg goes to a single receipent)

- #### Range Of Unicast Host Addresses

    - **1.1.1.1 - 223.255.255.255**
    - However this range also includes some reserved special purpose addresses

## IPV4 Broadcast

- Destination address is either **1.1.1.1** or **255.255.255.255** (i.e, the msg is forwarded to all hosts except the source)
- **One-to-all communication**
- **IPV4** uses broadcast packets, however **IPV6 doesnot possess broadcast packets**

- ### Types Of Broadcasts

    - #### Directed Broadcast
        - Targets a specific network broadcast address
        - For example, a host on the 172.16.4.0/24 network sends a packet to 172.16.4.255

    - #### Limited Broadcast
        - For devices on the same local network
        - A limited broadcast is sent to 255.255.255.255

- ***By default, routers do not forward broadcasts.***

---

## IPV4 Multicast

- To send msg to a selected group of hosts
- IPV4 multicast addresses have a range from **224.0.0.0 to 239.255.255.255**
- Sends packet to all devices (except source) but the devices that are in the multicast group will only process the packet (others will discard)
- ***Hosts that receive particular multicast packets are called multicast clients.***
- ***The multicast clients use services requested by a client program to subscribe to the multicast group.***

- When an IPv4 host subscribes to a multicast group
    - The host processes packets addressed to this multicast address
    - Packets addressed to its uniquely allocated unicast address

- Routing protocols such as **OSPF use multicast transmissions** 
    - For example, routers enabled with OSPF communicate with each other using the reserved OSPF multicast address **224.0.0.5** 
    - Only devices enabled with OSPF will process these packets with 224.0.0.5 as the destination IPv4 address
    - All other devices will ignore these packets.
