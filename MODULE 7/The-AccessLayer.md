# The Access Layer

- **Switch** builds a **MAC addresss table** 
- When a host sends a data, the switch reads the ***destination MAC address*** (at Layer 2) and checks that in its MAC address table
- If found the packet is sent to that MAC address

## How Switch Build MAC Address Table ?

- Initially the MAC address table is empty
- When a packet is received from the connected hosts, the switch checks the source MAC address against entries in its MAC address table
- If no matching entries **(unknown unicast)** are found the MAC address is inserted in the MAC Address Table
- Then the destination MAC address is checked against all entries on the MAC address table
    - If not found
        - The switch sends the packet to all hosts (except for the source host) 
        - Every host receives that data and checks (the destination host) against its own MAC address
            - If not found it ignores the rest of the frame
            - If found it de encapsulates the msg