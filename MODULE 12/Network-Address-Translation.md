# Network Address Translation

## NAT Definition

- The process used to convert private addresses to internet-routable addresses is called NAT
- With NAT, a private (local) source IPv4 address is translated to a public (global) address. The process is reversed for incoming packets
- The wireless router is able to translate many internal IPv4 addresses to the same public address, by using NAT

## Working Of NAT

- Router performs a function that keeps a table mapping the private IP to a public IP
- For eg, a host with IP address **(192.168.5.1)** is represented on the internet by a public IP **(200.100.58.50)**

    - Host sends a msg to an external server 
    - The **private IP (192.168.5.1)** travels upto the router
    - Router then uses the above table to translate this to **Public IP (200.100.58.50)**
    - The destination server will receive the Public address
    - When the server will respond back it will use the Public IP as the destination address 
    - The public IP will then be translated back to private IP at the router and will reach the desired destination

