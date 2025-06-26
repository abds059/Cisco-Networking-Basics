# DHCPV4 Configuration

- Host sends a packet => DHCP discover 
- Server responds with => DHCP Offer
- Host sends back => DHCP Request Packet
- Server sends back => DHCP Acknowledge

- #### DHCP Discover
    - DHCP Discover
    - Broadcast packet
    - MAC address
        - Destined for DHCP server

- #### DHCP Offer
    - Contains IP Address
    - Subnet Mask
    - Default Gateway Address

- #### DHCP Request
    - Host sends this to receive the IP offered by the DHCP 

- #### DHCP Acknowledge
    - Server sends acknowledge signal to host
    - Adds the host MAC on the MAC address table