# CLient Server Interaction

## Web Server And Client IP Interactions

- A client wants to access a website (for e.g, learnip.com)
    - The cient enters the URL (https://www.learnip.com) in the web client browser (for e.g, chrome)
    - A **DNS lookup** is used to get the IP address associated with the URL
    - The IP address (for e.g, 172.16.10.50) is returned by the DNS server
    - Then a TCP connection is used to send the packet
        - TCP connection consist of
            - IP address of the web client (for e.g, 192.168.1.2)
            - TCP port assigned to web client (for e.g, 5507)
        - A TCP connection is formed by
            - **Source: 192.168.1.2:5507**
            - **Destination: 172.16.10.50:80**
        - The msg will be sent from the client to the server with this TCP connection
        - The server will reply by 
            - **Source: 172.16.10.50:80**
            - **Destination: 192.168.1.2:5507**


#### DNS Lookup 

- Sending a request to the DNS server in order to get back the IP address associated with the URL 

## URI, URN And URL

- Web resources and web services such as RESTFUL APIs are identified using **Uniform Resource Identifier (URI)**
- A URI is a string of characters that identifies a specific network resource

#### Uniform Resource Name (URN)

- Identifies only the namespace of the resource (webpage, document, image etc) without reference to the protocol

#### Uniform Resource Locator (URL)

- Defines network location of a specific resource on the network
- HTTP or HTTPS URLS are typically used with web browsers
- Other protocols FTP, SFTP, SSH and others can be used as a URL
- **For e.g,  A URL using SFTP might look like: sftp://sftp.example.com**

- **Parts Of URL**

    - **Protocol/Scheme =>  HTTPS or other protocols such as FTP, SFTP, mailto, and NNTP**
    - **Hostname => w​ww.example.com**
    - **Path and file name => /author/book.html**
    - **Fragment => #page155**

