# Trouble Shooting Commands

- Used to identify network problems
- Most of them are available on Command Line Interface (CLI)

- **ipconfig:** =>  Displays IP configuration information
- **ping:** => Test connections to other IP hosts
- **netstat:** => Displays network connections
- **tracert:** => Displays the route taken to destination
- **nslookup:** => Queries DNS server about website details (IP address)

## The ipconfig Command

- A device cannot communicate on the network or access the internet if
    - It doesnot receives an IP address
    - Or has an incorrect IP configuration

#### ipconfig

- The ipconfig command is used to display the current IP configuration information for a host
- Issuing this command from the command prompt displays the basic configuration information including
    - IP address
    - Subnet mask
    - Default gateway

#### ipconfig /all

-  Displays additional information including
    - MAC address
    - IP addresses of the default gateway
    - DNS servers

- Also indicates if 
    - DHCP is enabled
    - DHCP server address
    - Lease information

- If the host does not know the location of the DNS servers, it cannot translate names into IP addresses

#### ipconfig /renew And ipconfig /release

- If IP addressing information is assigned dynamically, the command ipconfig /release will release the current DHCP bindings
- ipconfig /renew will request fresh configuration information from the DHCP server
- A host may contain faulty or outdated IP configuration information
- A simple renewal of this information is all that is required to regain connectivity


- If, after releasing the IP configuration, the host is unable to obtain fresh information from the DHCP server, it could be that there is no network connectivity
- Verify that the NIC has an illuminated link light, indicating that it has a physical connection to the network
    - If this does not solve the problem, it may be an issue with the DHCP server or network connections to the DCHP server

## The ping Command

- To test network connectivity if IP configuration is correctly configured
- Can be followed by either an IP address or the name of a destination host
    - For e.g, 
            - The user pings the default gateway at 10.10.10.1 
            - Or pings ww​w.cisco.com

#### Process

- When a ping is sent to an IP address
    - A packet called **echo request** is sent across network to the specified IP address
    - The destianation host responds with **echo reply**
    - Connectivity is verified by the reply from the specific IP address
    - The ping is not successful if a message such as request timed out or general failure appears

- If a ping command is sent to a name, such as ww​w.cisco.com
    - A packet is first sent to a DNS server to resolve the name to an IP address
    - After the IP address is obtained, the echo request is forwarded to the IP address and the process proceeds
    - If a ping to the IP address succeeds, but a ping to the name does not, there is most likely a problem with DNS

#### Ping Results

- **Case 1:**
    - If ping commands to both the name and IP address are successful, but the user is still **unable to access the application**
        - Then the **problem** most likely resides in the **application on the destination host**
        - For example, the requested service is not running

- **Case 2:**
    - If neither ping is successful, then network connectivity along the path to the destination is most likely the problem
        - **If this occurs** => common practice is to **ping the default gateway**
            - If the ping to the default gateway is **successful** => the **problem** is **not local**
            - If the ping to the default gateway **fails** => the **problem** resides on **the local network**

- **Other Cases:**
    - In some cases, the ping may fail but network connectivity is not the problem.
    - A ping may fail due to 
        - **Firewall** on the sending or receiving device
        - **Router** along the path that is blocking the pings

#### Basic ping Command
- The basic ping command usually issues four echoes and waits for the replies to each one
- However, it can be modified to increase its usefulness