# Communication Protocols

### **Protocols** -> Rules that govern how devices communicate.

Three things are essential for communication
- Method
    - Before communication begins we reach on an agreement on the method used

- Language
    - Before communication begins we reach an agreement on the language used

- Confirmation
    - Communication is successful when intended msg is received fully and confirmed

## Why Protocols Matter ?

- For devices to communicate together in a network they must share the same protocols (Like for eg, in a room full of people they must speak the same language to communicate).

- In both wired and wireless environment a local network is defined as an area in which all hosts share the same protocol

### Aspects Of Communication Over Local Network 

- #### Message Format
    - Msg should be in specific format before being sent
    - Msg format depend on
        - Type of msg
        - Channel used for delivery of msg

- #### Message Size
    - Rules that govern the size of pieces transmitted are very strict
    - Often longer msgs are broken into smaller pieces in order to ensure reliable delivery

- #### Timing
    - Many network communication functions are dependent on timing
    - Timing also determines the speed at which bits are transmitted across the network
    - The timing affects
        - When an individual host can send data 
        - Total amount of data that can be sent in one transmission

- #### Encoding
    - The msgs are first converted into bits by sender host
    - Each bit is encoded then into patterns of sound, light waves or electrical impulses depending on the network
    - The destination host then decodes this signal to interpret the msg

- #### Encapsulation
    - Each msg transmitted on the internet must contain a header that identifies the source and destination hosts. Without this the msg wont be delivered.
    - ***Encapsulation*** is the method of adding this information to the pieces of data that make up the msg
    - In addition to addressing, there maybe more information in the header that ensures the msg is delivered to the correct application on the destination host

- #### Message Pattern
    - Some msg require an acknowledgement before the next msg is sent
    - This type of request/response method is a common example of many networking protocols
    - However, there are other types of msgs that maybe just streamed across the network without concern as to whether they reach the destination
