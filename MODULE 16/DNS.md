# Domain Name System

## DNS Servers

- Internet only understands IP addresses
- For eg, a client wants to access (www.cisco.com)
    - Client request the IP address of cisco page from DNS server
    - DNS server looks for the IP address, finds it and returns it to the client
    - Host can now use this IP address to contact the web server for the cisco page

## Syntax Checker - The nslookup Command

- When you manually configure a device for network connectivity, we also include a DNS server address
- For home networks, this configuration is typically handled by DHCP running on the home router
- ISP provides the DNS server address to home router, and then the home router uses DHCP to send the configuration to all the devices connected to its network
- When we type the name for a website, such as www.cisco.com, 
    - The DNS client running on your device first asks the DNS server for the IP address, such as 172.230.155.162
    - Then sends out your HTTP request

- The command nslookup discovers the IP addresses for any domain name