# IPV4 ISSUES

## Need For IPV6

- ### IPV6
    - 128 Bit Address space ~ 340 Undecillion possible addresses
    - **Internet Control Message Protocol Version 6 (ICMPV6)** includes **address resolution and address autoconfiguration** not found in ICMPV4

- All 5 RIRs have run out of IPV4 addresses

- NAT and private addresses proved vital in slowing down the depletion of IPV4

- However NAT is problematic for many applications, creates latency and has limititations severely impeeding peer-to-peer communications

- Mobile providers have been leading the way to IPV6 transition

## Internet Of Things (IOT)

- IOT refers to the network of physical objects (thing) that:

    - Have sensors, software, or embedded electronics
    - Can collect and exchange data over the internet
    - Operate autonomously or in coordination with other systems

- With an increasing internet population by the induction of IOTs, a limited IPv4 address space, issues with NAT and the IoT, the transition to IPv6 has become necessary

## IPV4 And IPV6 Coexistence

- There is no specific date to move to IPv6
- Both IPv4 and IPv6 will coexist in the near future and the transition will take several years
- The IETF has created various protocols and tools to help network administrators migrate their networks to IPv6
- The migration techniques can be divided into three categories:
    
    - #### Dual Stack
        - Allows IPV4 and IPV6 to exist in the same network segment
        - Dual stack devices run both of them simultaneously
        - Known as native IPv6
            - The customer network has an IPv6 connection to their ISP 
            - Able to access content found on the internet over IPv6

    - #### Tunneling 
        - Method of transporting an IPV6 packet over an IPV4 network
        - IPV6 packet is encapsulated inside an IPV4 packet, similar to other types of data

    - #### Translation
        - Network Address Translation 64 (NAT 64) allows IPV6 enabled devices to communicate with IPV4 enabled devices 
        - Uses a translation technique similar to NAT for IPV4
        - IPV6 packet translated to IPV4 packet
        - IPV4 packet translated to IPV6 packet

## Note: 
- Tunneling and translation are for transitioning to native IPv6 and should only be used where needed
- The goal should be native IPv6 communications from source to destination
