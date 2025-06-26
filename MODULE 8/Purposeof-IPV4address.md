# Purpose Of IPV4 Address

```

Every packet sent across the internet has a source and destination IPv4 address. This information is required by networking devices to ensure the information gets to the destination and any replies are returned to the source.

```

## The IPV4 Address

```

A logical network address that identifies a particular host

```

- The host needs an IPV4 address to communicate on the internet and almost all LANs today

- **Must be properly configured and unique**

    - In the ***LAN for local communication***
    - In the ***world for remote communication***

- Through this the host communicates with other devices on the internet

- An IPV4 address is assigned to the **NIC (Network Interface Card)** installed on the device

    - Examples of **end user devices** with NIC card are
        
        - Workstations
        - Servers
        - Network printers
        - IP phones
        - ***Router interfaces providing connection to an IP network***
        

- Some servers have more than one NIC and all NIC will be assigned a seperate IPV4 address

## Octet And Dotted Decimal Notation

- IPV4 addresses are 32 bit in length

- ### Binary Representation of an IPV4 Address

    - **1010001101001011100100000000001**

    - For making it readable we divide the ***32 bits into 4 octets (8 - bit byte)***

        - **11010001.10100101.11001000.00000001**

    - #### Decimal Representation

    - We convert each octet into its decimal value for better readability

    - The above binary IPv4 becomes this dotted-decimal representation:
    
        - **209.165.200.1**