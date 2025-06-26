# Network Communication Models

```
Protocols help govern communication between two devices. A computer msg usually comprises of several protocols. For eg, a msg contains the following protocols

- Ethernet -> governs network interface card to network interface card in the same network

- IP (Internet Protocol) -> Governs communication from original source all the way to final destination

- TCP (Transmission Control Protocol) -> Makes sure that the msg reaches its destination reliably

- HTTP (Hyper Text Transfer Protocol) -> Governs the exchange or transfer of HTML

```

## Network Protocols Stack

The interaction between the different protocols on a device can be illustrated as a protocol stack. A stack illustrates the protocols as a layered hierarchy, with each higher-level protocol depending on the services of the protocols shown in the lower levels. The separation of functions enables each layer in the stack to operate independently of others.


### Types Of Models 

The **protocol model** and **reference model** are both frameworks used in networking, but they serve different purposes. Here’s how they differ:  

#### 1. **Protocol Model**

   - A **protocol model** is based on the actual implementation of network protocols.

   - It defines how different protocols interact and function within a network.

   - Example: **TCP/IP Model** is a protocol model because it is based on real-world protocols like TCP, IP, HTTP, FTP, etc.

   - It focuses on **practical communication** rather than theoretical structure.
   - Layers are designed to match the existing **protocols and technologies**.

#### 2. **Reference Model**
   
   - A **reference model** is a conceptual framework that provides a standard **guideline** for network communication.
   
   - It does not depend on specific protocols but defines how data should be logically transmitted.
   
   - Example: **OSI Model** is a reference model that defines **seven layers** (Physical, Data Link, Network, etc.).
   
   - It serves as a **theoretical framework** for understanding and designing network systems.
   
   - It helps in developing **new protocols** that fit into a structured hierarchy.

### **Key Differences:**
| Feature            | Protocol Model (TCP/IP) | Reference Model (OSI) |
|--------------------|-----------------------|----------------------|
| Purpose           | Implementation-based | Theoretical framework |
| Layers Defined by | Real-world protocols | Conceptual guidelines |
| Example           | TCP/IP Model | OSI Model |
| Usage            | Practical, used in networking today | Used for learning and protocol development |
| Flexibility      | Rigid, follows existing protocols | Flexible, can be modified |

### **Conclusion:**

- **Protocol Model** is used for actual communication and implementation.  

- **Reference Model** is used as a guide to understand and design network architectures.

### TCP/IP Model
Common reference of the internet model. It defines four categories of function that must occur for a communication to be successful.
    
- **Application** -> Represents data to the user plus encoding and dialog control

- **Transport** -> Supports communication b/w various devices across diverse networks

- **Internet** -> Determines the best path through the network

- **Network Access** -> Controls the hardware devices and media that makes up the network

## OSI Reference Model

- Created by **Open Systems Interconnection** (OSI) project at **International Organization Of Standardization** (ISO).

- Used for network data design, operation specifications and troubleshooting.

- It consists of seven layers

### 7. Application Layer

- Contains protocols used for process to process communication

- In simple words provides network services to end users (like browsers, email, file transfer)

### 6. Presentation Layer

- Provides for common representation of data transfereed b/w application layer services


### 5. Session Layer

- Provides services to presentation layer to organize its dialogue and to manage data exchange

### 4. Transport Layer

- Defines services to reassemble, segment and transfer data for individual communication b/w end devices

### 3. Network Layer

- Provides services to exchange individual pieces of data b/w identified end devices.

### 2. Data Link Layer

- Describes method for transfer data b/w devices over a common media (directly connected devices)

### 1. Physical Layer

- Describes electrical, mechanical, functional and procedural means to activate, maintain and deactivate physical connections for a bit transmission to and from a network device.

### Comparision b/w OSI And TCP/IP Models

- The TCP/IP model only discusses networking functions specific to the protocols used in the TCP/IP protocol suite.

- For eg, in **Network Access Layer** the TCP/IP model doesnot specify which protocols to use when transmitting over a physical medium nor does it specify the method of encoding signals for transmission.

- The mapping of different layers between both models is as follows:
   
   - **Physical and data link layers**  correspond to **Network Access Layer**.
   
   - **Network layer** correspond to **Internet layer**. 

   - **Transport layer** maps to **Transport layer**.

   - **Application, Presentation and session layers** map to **Application layer**.
