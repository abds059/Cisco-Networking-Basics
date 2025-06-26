# Client And Servers

- In modern networks
    - Computer hosts can act as a client , a server or both (depending on the software installed on it)
        - **Servers** are those that have software installed that enable them to provide info to other hosts on the network. Each server requires a seperate server software.
            - Web server software
            - File server software
            - Email server software

        - **Clients** are computer hosts that have software installed that enables the host to request & display information obtained from server
            - Example of client server is a ***web browser*** (Chrome, Edge, Safari, Firefox)
                - Client requests a webpage(eg, www.cisco.com)
                - Server responds back with the webpage (i.e, in this case cisco webpage)
            - Email Client software like ***Microsoft Outlook***
                - To access email on the server 
                - Client can both send & receive msgs through the server

## ***What Are Hosts***
```

All computers connected to a network that participate in network communication are called hosts. They can act as clients, servers or both depending on software installed
    
```

## Client And Server Roles

- ### Web server
    - **Server** -> Runs web server software
    - **Client** -> Uses browser software like chrome to access web pages on the server

- ### Email Server
    - **Server** -> Runs email server software
    - **Client** -> Uses mail client software like Microsoft Outlook to access email on server

- ### File Server
    - **Server** -> Stores corporate and user files in a central location
    - **Client** -> Uses client software like windows file explorer to access these files

## Peer To Peer Networks
```
    - Client and server softwares usually run on different hosts
    - But its also possible to run them on same computers
    - In small businesses and homes many computer function as both clients and servers at same time
    - When computer hosts run both client and servers on same time then this type of network is called "P2P (Peer to Peer) Network"

```

- **Simplest P2P connection** 
    - Two computers connected to each other either wired or wireless connection
    - Both can use this to exchange data and services acting as client or server as necessary

- To create a larger network we need a ***switch*** to connect multiple PC's

### Advantages 
- Easy setup
- Low costs (cuz network devices and dedicated servers not req usually)
- Can be used for simple tasks such as printer sharing and file transfer

### Disadvantages
- Not centralized
- Not scalable
- Insecure
- All devices can act as client and server which lowers performance of hosts

## Peer To Peer Applications
 ```
    - Allows a device to act as both client and a server within the same communication.
    - Require each end device to run a UI and background service.
    - Some uses a hybrid system where resource sharing are decentralized but indexes that point to source locations are stored in the same centeralized directory. Here each peer access an index server to get the location of resource stored on another peer.

```

- A single server can run multiple server applications
- Similarly a single client host can run mutiple client applications