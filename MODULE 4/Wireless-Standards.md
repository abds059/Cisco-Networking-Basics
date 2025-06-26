# Wireless Standards

## Wi-Fi Networks

- A no of standards have been introduced to ensure that wireless devices can communicate
- They specify RF spectrum used, data rates, how information is transmitted and more
- ***IEEE (Institute Of Electrical And Electronics Engineers)*** is responsible for creation of wireless technical standards

### IEEE 802.11 Standard

    - Governs the WLAN environment
    - Ammendments to this standard provides characterstics for different standards of wireless communication
    - Wireless standards for LAN use 2.4GHz to 5GHz frequency bands
    - Collectively these technologies are referred to as Wi-Fi

- ***Wi-Fi Alliance*** is responsible for testing wireless LAN devices from different manufacturers 

## Wireless Settings

- Network Mode
    - Determine type of technology that must be supported
    - For eg, **802.11b, 802.11g, 802.11n or Mixed Mode**

- Network Name (SSID)
    - Used to identify **WLAN**
    - All devices that wish to participate in the WLAN must have same **SSID**

- Standard Channel
    - Specifies the channel over which communication will occur
    - By default, set to **Auto** to allow Access Point (AP) to determine optimal channel to use

- SSID Broadcast
    - SSID (Service Set Identifier)
    - Determines if SSID will be broadcast to all devices within the range (By default set to **Enabled**)

### Network Mode

- 802.11 protocol can provide increased throughput based on the wireless network environment
- If all devices connect to the same 802.11 standard then ***max speed*** can be obtained for that standard
- If access point is configured to accept only one 802.11 standard, devices that donot use that standard cannot connect to the access point

- #### MIXED MODE 

    - A mixed mode wireless network environment can include all devices that have any existing Wi-Fi standards
    - Provides easy access to older devices that need wireless connection but donot support latest standards


- #### SSID 
    - When building a wireless network it is necessary that the wireless components connect to the correct WLAN. This is done through SSID
    - SSID is case sensitive, alpha-numeric string containing upto 32 characters
    - Sent in headers of all frames transmitted over the WLAN
    - Used to tell wireless device (also called WTA's (wireless Stations)) which WLAN they belong to and with which other devices they can communicate
    

#### SSID Broadcasting

- Wireless routers broadcast their SSID's ***by default*** to allow other devices and clients to discover the name of the wireless network

- When disabled you must enter the the SSID manually on wireless devices
   
 - **Disabling**
        - Makes it more difficult for legitimate clients to find the wireless network
        - Not sufficient enough to prevent unauthorized access
        - As an alternative all wireless networks should use the strongest available encryption
