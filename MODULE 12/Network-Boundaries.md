# Network Boundaries

## Router As Gateways

- Router serves as bridges b/w networks
- Each router interface connects to a seperate network segment
- IPV4 address on a specific interface identifies which specific network is directly connected to that interface

#### Default Gateway

- For host to communicate with some other network they must know the **IP address of their router's interface => Default Gateway**
- Default Gateway can be configured by two ways;
    - By Static Configuration (Manually set on each host)
    - By DHCP (Automatically provided by DHCP)

#### DHCP Integration

- Wireless routers are configured as DHCP Host by default
- When wireless routers are configured to be DHCP servers, they provide 
    - Router's own internal IPV4 address as **Default Gateway**
    - Individual IPV4 addresses For each client device
    - Appropriate subnet mask

---

## Routers As Boundaries Between Networks

- The wireless router serves as the boundary between the local internal network and the external internet.

#### Internal Network Structure

- The wireless router creates an inside network consisting of all locally connected devices (via Ethernet or wirelessly)
    - Uses private IP addresses
    - Private IPs ensure that internet is not directly accessible
    - The Default Gateway (Router's IP) is usually the first available host address on the network

- Provides IP, subnet masks and Default Gateway addresses to clients either statically or through DHCP

#### External Network Connection

- Router serves as a DHCP client to the ISP
- Receives public IP address (routable on internet) from ISP's DHCP server
- This external address enables connectivity for all internal devices



