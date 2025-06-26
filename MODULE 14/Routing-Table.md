# The Routing Table

## Routing

- The process of forwarding the packets toward their destination network is called routing

## Communication In Same Network

- When a source host wants to send information to another host
    - It checks the IP address of the destination host with its subnet mask to determine if they both are on the same network
    - If true (same network) then
        - It looks for the destination MAC address in its ARP table
        - It directly forwards the msg through the switch

## Communication Between Different Network

- - When a source host wants to send information to another host
    - It checks the IP address with the destination host with its subnet mask to determine if they both are on same or different networks
    - If different networks
        - It looks for router's MAC address in its ARP table
        - Forward the msg to the router
        - The router receives the msg
        - Remove the Layer 2 (MAC address) headers
        - Looks for the destination address in its Routing table to determine the network on which the destination host is located
        - Re-encapsulate the packet into a new frame
            - In the layer 2 source MAC address inserts its own MAC address
            - For the destination MAC address uses its ARP cache to determine the MAC address associated with the IP address
            - Router then forward this packet to the destination host directly which receives and processes the packet

#### Note:

- In all cases we are assuming that whenever a device checks its ARP cache/table for an associated MAC address it already possese that address mapped to the IPV4 address
- If not then it will have to send an ARP request

## Routing Table Entries

- Routers move info from local to remote network for which they need routing tables
- Routing tables dont include the addresses of the individual hosts 
- They just contain the **addresses of networks and the best way to reach that network**
-  Routers use the routing tables to **determine which interface to use to forward a message to its intended destination**

#### Entries

- Entries can be made in the table in two ways
    - Dynamically updated by info received from other networks
    - Manually entered by network administrator

- If the router can't determine the best way to forward the msg it will drop it
    - To avoid this 
        - Network admin configure a static default route to avoid packet being dropped if destination network is not on routing table

    - **Default Route:** 
        - Interface through which the router forwards a packet containing an unknown destination IP network address
        - Usually connects to another router that can forward the packet towards its final destination network

## Default Gateway

- When a host needs to send a message to a remote network, it must use the router
- The host includes the IP address of the destination host within the packet just like before 
- However, when it encapsulates the packet into a frame, it uses the MAC address of the router as the destination for the frame - - In this way, the router will receive and accept the frame based on the MAC address

#### How does the source host determine the MAC address of the router? 
- A host is given the IPv4 address of the router through the default gateway address configured in its TCP/IP settings
- The default gateway address is the address of the router interface connected to the same local network as the source host
- All hosts on the local network use the default gateway address to send messages to the router
- When the host knows the default gateway IPv4 address, it can use ARP to determine the MAC address
- The MAC address of the router is then placed in the frame, destined for another network

#### Note:
- It is important that the correct default gateway be configured on each host on the local network
- If no default gateway is configured in the host TCP/IP settings, or if the wrong default gateway is specified, messages addressed to hosts on remote networks cannot be delivered