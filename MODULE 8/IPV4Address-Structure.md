# The IPV4 Address Structure

- The 32 bit IPV4 address consists of two parts
    - Network part -> **Identifies the network on which the host is located**
    - Host part -> **Unique for each host on the network**

- Different networks can have the same **subnet mask (The subnet mask is used to identify the network on which the host is connected)** for eg, ***255.255.255.0***

- For example a host has an IPV4 address of **192.168.5.11 with a subnet mask of 255.255.255.0.**
    - Here 
        - **(192.168.5)** -> Network part
        - **(11)** -> Host part

    - Known as **Hierarchial addressing** because the network part identifies the network on which the host is located
    - Routers only need to know how to reach a network rather than knowing the location of each individual host


---


### Multiple Logical Networks On Same Physical Network

- With IPV4 we can also make multiple logical addresses on the same physical network by changing the network part

    - For example on a single physical network
        - **3 hosts have network portion (192.168.18)**
        - **2 hosts have network portion (192.168.5)**

    - In this example
        - We have **1 physical network**
        - But **2 logical IPV4 networks**
    
    - The host with the same network portion can communicate with each other
    - The host can communicate with the other hosts (with different network portions) through **routing**


- Another example of a hierarchical network is the telephone system. 
    - Telephone number, the country code, area code, and exchange represent the network address
    - The remaining digits represent a local phone number