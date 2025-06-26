# MAC And IP

## Destination On Same Network

- When host wants to send data to another host on the same network, it must know
    - Destination MAC address -> Layer 2 Physical Address (Used to send packets across same IP network or remote network)
    - Destination IP address -> Layer 3 Logical Address (Used for NIC to NIC communication on same ethernet network)

- Layer 2 physical address is used to deliver the data link frame with the encapsulated IP packet from one NIC to another NIC on same network
- If destination IP address is on the same network then destination MAC address will be of the destination device

## Destination On Remote Network

- When Destination IP address is on a remote network the destination MAC address will be the address of the default gateway
- For eg PC1 wants to send data to PC2 which is on a remote network

    - Destination addresses will include
        - MAC address of the router
        - IPV4 address of PC2
    
    - When the data reaches the router (Destination MAC address)

        - Router will **de-encapsulate the packet** and obtain the Layer 3 IP information by striping the layer 2 information (MAC addresses)

        - Based on the IPV4 information it will determine
            - The **best way to forward the packet**
            - Determine the next hop-device

        - **Encapsulate the packet** in a new data link frame for outgoing device

- If the next device is not the destination device => The destination MAC address will be of that particular device

-  If the next-hop device is the final destination => The destination MAC address will be that of the device Ethernet NIC

- How are the IP addresses of the IP packets in a data flow associated with the MAC addresses on each link along the path to the destination? 

    - For IPv4 packets, this is done through a process called **Address Resolution Protocol (ARP)**
    - For IPv6 packets, the process is **ICMPv6 Neighbor Discovery (ND)**