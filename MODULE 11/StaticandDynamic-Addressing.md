# Static And Dynamic Addressing

- IPv4 addresses can be assigned either statically or dynamically

## Static IPV4 Address Assignment

- Network Administrator must manually configure the network information for host. This includes:
    - **IP Address:** => This identifies the host on network
    - **Subnet Mask:** => Used to identifuy the network on which the host is connected
    - **Default Gateway:** => Used to identify the device that host uses to access the internet or any remote network

- #### Advantages
    - Useful for such devices hat needs to be accessible clients on the network
        - It would be good if their IP doesnot change
        - For eg, printers, servers, other networking devices

    - Provide **increased control of networking resources**

- #### Disadvantages
    - **Time consuming** to enter information on each host
    - Important to maintain an accurate list of which IPv4 addresses are assigned to which devices as these are permanent addresses and are not normally reused
    - During static addressing the host only performs basic error checks on the IPv4 address increasing chances of errors

## Dynamic IPV4 Address Assignment

- Assigns IPV4 addresses automatically
- Uses Dynamic Host Configuration Protocol (DHCP)
- Address is not permanently assigned but only leased for a particular period of time
- If the host is powered down or taken off the network, the address is returned to the pool for reuse
    - Helpful with mobile users that come and go on a network

## DHCP Servers

- When you enter a cafe or airport with a wireless hotspot, DHCP makes it possible for you to connect to the internet
    - Your laptop DHCP client contacts the local DHCP server via a wireless connection
    - DHCP server assignes an IPV4 address to your laptop

- A device can be a DHCP server as long as it is running the DHCP service software

- In most medium to large networks => DHCP server is a dedicated PC - based server

- In home networks
    - DHCP server may be located at an ISP
    - A host on the home network receives its IPV4 configuration directly from the ISP

- In case of wireless routers => Router serves as both the DHCP client and server
    - The wireless router acts as a client to receive its IPv4 configuration from the ISP 
    - Then acts as a DHCP server for internal hosts on the local network
    - The router receives the public IPv4 address from the ISP, and in its role as a DHCP server, it distributes private addresses to internal hosts
