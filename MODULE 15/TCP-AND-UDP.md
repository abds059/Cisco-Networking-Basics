# TCP And UDP

## UDP

- Used in streaming and realtime communications
- No overhead
-  Packets take a path from the source to a destination
- A few packets may be lost but it is usually not noticeable

## TCP

- TCP packets take a path from the source to the destination
-  Each packet has a sequence number
- TCP breaks up a message into small pieces known as segments
- The segments are
    - Numbered in sequence  
    - Passed to the IP process for assembly into packets
- TCP keeps track of the number of segments that have been sent to a specific host from a specific application
- If the sender does not receive an acknowledgment within a certain period of time, it 
    - Assumes that the segments were lost 
    - And retransmits them
    - Only the portion of the message that is lost is resent, not the entire message