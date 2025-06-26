# Virtual Terminals

## Telnet
```

Telnet provides a way to use a computer, connected via the network, to access a network device as if the keyboard and monitor were directly connected to the device.

```

- Telnet provides a standard method of emulating text-based terminal devices over the data network
- Both the protocol itself and the client software that implements the protocol are commonly referred to as Telnet
- Telnet servers listen for client requests on TCP port 23

## Virtual Terminal 

- Appropriately enough, a connection using Telnet is called a virtual terminal (vty) session, or connection
- Rather than using a physical device to connect to the server, Telnet uses software to create a virtual device that provides the same features of a terminal session with access to the server’s command line interface (CLI)


## Security Issues With Telnet

- After a Telnet connection is established, users can perform any authorized function on the server, just as if they were using a command line session on the server itself
- If authorized, they can 
    - Start and stop processes
    - Configure the device
    - Shut down the system

- Although the Telnet protocol can require a user to login, it does not support transporting encrypted data
- All data exchanged during Telnet sessions is transported as plaintext across the network
- This means that the data can be easily intercepted and understood

## SSH

- The Secure Shell (SSH) protocol offers an alternate and secure method for server access
- SSH provides the structure for secure remote login and other secure network services
- It also provides stronger authentication than Telnet and supports transporting session data using encryption
- As a best practice, network professionals should always use SSH in place of Telnet, whenever possible