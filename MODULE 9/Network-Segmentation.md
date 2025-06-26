# Network Segmentation

## Broadcast Domains And Segmentation

- Just like an email sent to everyone at your school or work, a broadcast in networking is a message sent to all devices on a local network (LAN)

- Often used for communication where the sender doesn’t know the exact recipient (yet)

- In an Ethernet LAN, devices use broadcasts and the Address Resolution Protocol (ARP) to locate other devices

- #### Address Resolution Protocol (ARP)

    - Sent when a device knows the IPv4 address but needs the MAC address

    - ARP sends a Layer 2 broadcast to a known IPV4 address to discover the MAC address of that device

- #### Dynamic Host Configuration Protocol (DHCP)

    - Used when a new device connects and needs an IPv4 address

    - Sends broadcast on a local network to locate a DHCP server

- Switches propagate broadcasts out all interfaces except the interface on which it was received

- Routers do not propagate broadcasts

- When a router receives a broadcast, it does not forward it out other interfaces

## Problems With Large Broadcast Domains

- #### Broadcast Domain
    - The area in a network where broadcast packets can reach all devices

- In a large LAN (e.g., 400 users in LAN 1), all hosts share the same broadcast domain

- **Issue: Broadcast and ARP requests are received and processed by all devices**

    - This leads to:
        - Slower network performance
        - Increased CPU load on devices
        
- **Solution: To split the network into smaller broadcast domains through Subnetting**

- **Subnetting**
    - Breaks one large network into smaller sub networks or subnets
    - Each subnet becomes its own broadcast domain

## Reasons For Subnetting Networks

- Subnetting 
    - Reduce overall network traffic
    - Improves network performance
    - Enables administrator to implement security policies
    - Reduces the no of devices affected by abnormal broadcast traffic due to misconfigurations, hardware/software problems, or malicious intent

- #### Various Ways To Using Subnetting

    - **Location:**
    - **Group or Function**
    - **Device Type**

