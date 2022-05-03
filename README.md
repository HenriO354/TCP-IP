#   <center>TCP-IP</centre><br><br>
+   What are the differences between the OSI model and the TCP/IP model? 

**OSI Model TCP/IP** Model
It is developed by ISO (International Standard Organization) 	It is developed by ARPANET (Advanced Research Project Agency Network).
OSI model provides a clear distinction between interfaces, services, and protocols. 	TCP/IP doesn’t have any clear distinguishing points between services, interfaces, and protocols.
OSI refers to Open Systems Interconnection. 	TCP refers to Transmission Control Protocol.
OSI uses the network layer to define routing standards and protocols. 	TCP/IP uses only the Internet layer.
OSI follows a vertical approach. 	TCP/IP follows a horizontal approach.
OSI layers have seven layers. 	TCP/IP has four layers.
In the OSI model, the transport layer is only connection-oriented. A layer of the TCP/IP model is both connection-oriented and connectionless.
In the OSI model, the data link layer and physical are separate layers. In TCP, physical and data link are both combined as a single host-to-network layer.
Session and presentation layers are a part of the OSI model. 	There is no session and presentation layer in the TCP model.
It is defined after the advent of the Internet. 	It is defined before the advent of the internet.
The minimum size of the OSI header is 5 bytes. 	The minimum header size is 20 bytes.

+ How many layers do these two models have ?

![](assets/images/tcp-vs-osi.webp)

+ What do the acronyms TCP and IP refer to ?<br>
    TCP: is one of the main protocols in TCP/IP networks. Whereas the IP protocol deals only with packets, TCP enables two hosts to establish a connection and exchange streams of data. TCP guarantees delivery of data and also guarantees that packets will be delivered in the same order in which they were sent.<br>
    
    IP:  The Internet Protocol, as defined in IETF RFC 6864, which is the principal communications protocol in the IETF Internet protocol suite for specifying system address information when relaying datagrams across network boundaries.<br>

    The IP, as defined in IETF RFC 6864, is the principal communications protocol in the IETF Internet protocol suite for specifying system address information when relaying datagrams across network boundaries<br>
+ List the different layers of the TCP/IP model.

 <center>TCP/IP LAYERS</center>
    <ol>
        <li>Application Layer</li>
        <li>Transport Layer</li>  
        <li>Internet Layer</li>
        <li>Network Access Layer</li>
    </ol> <br>

+ Give some examples of protocols and indicate 
which one of TCP/IP model layer they refer to.
<table style="width:100%">
  <tr>
    <th><center>Layer</th>
    <th><center>Protocols</th>
  </tr>
  <tr>
    <td><center>Layer-4</td>
    <td><center>HTTP/RDP/SSH/SMTP</td> 
  <tr>
    <td><center>Layer-3</td>
    <td><center>TCP/UDP</td>
  </tr>
  <tr>
    <td><center>Layer-2</td>
    <td><center>(IP-v4/IP-v6)/ARP</td>
    
  </tr>
   <tr>
    <td><center>Layer-1</td>
    <td><center>ETHERNET/TOKEN RING</td>
    
  </tr>
</table><br>

+ Explain how a connection gets established, in other words, explain the "3-way handshake" process?

![3ways-handshake-2](assets/images/3ways-handshake-2.png)<br>
3 way Handshake Diagram

Step 1: In the first step,	the client establishes a connection with a server. It sends a segment with SYN and informs the server about the client should start communication, and with what should be its sequence number.

Step 2: In this step server responds to the client request with SYN-ACK signal set. ACK helps you to signify the response of segment that is received and SYN signifies what sequence number it should able to start with the segments.

Step 3: In this final step, the client acknowledges the response of the Server, and they both create a stable connection will begin the actual data transfer process.

+ Explain how a connection is terminated, in other words, explain the "4-way disconnect" process?

to terminate an established TCP connection, the following 4 TCP packets are needed to be exchanged. Which you can understand with the statements below:

1. Host A → Host B: FIN flag set.
2. Host B → Host A: ACK flag set.
3. Host B → Host A: FIN flag set.
4. Host A → Host B: ACK flag set.

These 4 steps are known as a TCP 4-way handshake, which is necessary to terminate a TCP connection. For the termination of the established TCP connection, the following steps are necessary for the process. Which are given down below:

Firstly, from one side of the connection, either from the client or the server the FIN flag will be sent as the request for the termination of the connection.

In the second step, whoever receives the FIN flag will then be sending an ACK flag as the acknowledgment for the closing request to the other side.

And, at the Later step, the server will also send a FIN flag as the closing signal to the other side.
In the final step, the TCP, who received the final FIN flag, will be sending an ACK flag as the final Acknowledgement for the suggested connection closing.

For a better understanding, you can take a look at the diagram below:

![3ways-handshake-2](assets/images)

+ Explain what are the "sequence number" and "acknowledgment number" in TCP.

+ What is the fundamental difference between TCP and UDP ?

+ What are TCP ports? How many of them are they?

+ What are the three main categories of TCP Ports (with there associated range)?

+ Provide three examples of well-know port numbers and tell to which Application layer protocol they refer to.

+ Explain the concept of TCP packets and how they are build over the layer flow.

