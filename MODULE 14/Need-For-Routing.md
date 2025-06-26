# The Need For Routing

## Routing

- Process of determining the best path to the destination

## Router

- Networking device connecting multiple Layer 3 IP networks

- **Switches use Layer 2 MAC address**
- **Routers use Layer 3 IP address**

- #### Forwarding Process

    - When a router receives a packet from a source
        - It de-encapsulates the ethernet frame to read the Layer 3 IP address
        - Anytime the network portion of source and destination doesnot match (destination is located on different subnet or network)
            - A router must forward the msg
            - For e.g, If a **host on network** wants to send a msg to a **host on network 5.5.5.0**
                - The router will **receive** the packet
                - **De-encapsulate** it to reads the destination IP address
                - Looks for the address in its **Routing Table** 
                - **Re-encapsulate** the packet back into a new frame
                - **Forward** the msg to its destination

- #### Note:
    - **Switches make their routing decision based on Layer 2 MAC address**



