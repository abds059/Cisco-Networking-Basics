# Create A LAN

## LAN 

- Refers to a local network or a group of interconnected local networks under same administrative control
-  LANs can be 
    - A single local network installed in a home or small office
    - Interconnected local networks consisting of many hundreds of hosts, installed in multiple buildings and locations
    
- Common characteristics of LANs => typically use Ethernet or wireless protocols and they support high data rates

#### Intranet

- Refer to a private LAN that belongs to an organization
- Designed to be accessible only by the members of the organization, employees, or others with authorization

## Local And Remote Network Segments

- Within a LAN, it is possible 
    - To place all hosts on a single local network 
    - Or divide them up between multiple networks connected by a distribution layer device

- How this placement is determined depends on desired results

#### All Host In One Local Segment

- **Advantages of a single local segment:**

    - Appropriate for simpler networks
    - Less complexity and lower network cost
    - Allows devices to be **seen** by other devices
    - Faster data transfer - more direct communication
    - Ease of device access

- **Disadvantages of a single local segment:**

    - All hosts are in one broadcast domain which causes more traffic on the segment and may slow network performance
    - Harder to implement 
    - Harder to implement security

#### Host On A Remote Segment

- **Advantages:**

    - More appropriate for larger, more complex networks
    - Splits up broadcast domains and decreases traffic
    - Can improve performance on each segment
    - Makes the machines invisible to those on other local network segments
    - Can provide increased security
    - Can improve network organization

- **Disadvantages:**

    - Requires the use of routing (distribution layer)
    - Router can slow traffic between segments
    - More complexity and expense (requires a router)