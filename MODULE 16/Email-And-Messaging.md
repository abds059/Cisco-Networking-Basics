# Email And Messaging

## Email Clients And Servers

- Email is one of the most popular client/server applications on the internet
- Email servers run server software that enables them to interact with clients and with other email servers over the network

#### Process

- Each mail server receives and stores mail for users who have mailboxes configured on the mail server
- Each user with a mailbox must then use an email client to access the mail server and read these messages
- Many internet messaging systems use a web-based client to access email
- Examples of this type of client include Microsoft 365, Yahoo, and Gmail

#### Mailboxes Identification

Mailboxes are identified by the format: **user@c​ompany.domain**

- Various application protocols used in processing email include SMTP, POP3, and IMAP4

## Email Protocols

#### Simple Mail Transfer Protocol (SMTP)

- Used by email client to send msgs to local mail server
- Local server decides if msg is destined for local mailbox or for mailbox on any other email server
- If the server has to send the message to a different server, SMTP is used between those two servers as well
- SMTP requests are sent to port 25

#### Post Office Protocol (POP3)

- A server that supports POP clients receives and stores messages addressed to its users
- When the client connects to the email server, the messages are downloaded to the client
- By default, messages are not kept on the server after they have been accessed by the client.
- Clients contact POP3 servers on port 110

#### Internet Message Access Protocol (IMAP4)

- A server that supports IMAP clients also receives and stores messages addressed to its users
- However, unlike POP, IMAP keeps the messages in the mailboxes on the server, unless they are deleted by the user
- The most current version of IMAP is IMAP4 which listens for client requests on port 143

#### Note

- Many different email servers exist for the various network operating system platforms

## Text Messaging

- Most popular communication tool
- Text messaging software is built into many online applications, smartphone apps, and social media sites
- Real time communication
- Both clients can send msg simultaneously

## Internet Phone Calls

- Internet Telephone client uses peer-to-peer technology similar to text messaging
- IP telephony makes use of **Voice over IP (VoIP) technology**, which converts analog voice signals into digital data
- The voice data is encapsulated into IP packets which carry the phone call through the network

- When the IP phone software has been installed, the user selects a unique name
- This is so that calls can be received from other users
- Speakers and a microphone, built-in or separate, are required
- A headset is frequently plugged into the computer to serve as a phone

- Calls are made to other users of the same service on the internet, by selecting the username from a list
- A call to a regular telephone (landline or cell phone) requires using a gateway to access the **Public Switched Telephone Network (PSTN)** 
- Charges may apply on this type of call depending on service
- Protocols and destination ports used by internet telephony applications can vary based on the software
