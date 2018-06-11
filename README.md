# Wireshark-TCP-and-UDP-Tracing
capture TCP sequences on WireShark and Trap a UDP message with Wireshark and measure the time it takes to form a connection and send a file and disconnect.
This lab has three parts:

PART 1

The object of this part of the lab is to capture TCP sequences on WireShark and understand the TCP changes especially the handshake and the sequencing.

a) Send a large file from any system on one bench to a server on another bench using FTP. You should send a file large enough to send at least 10 TCP packets.
b) Using Wireshark you need to capture the packets and analyze the TCP portion of at least 5 packets concentrating on:
- The syn message (the first message)
- The sequence number 
- The flags
- The Ack
- Window size
- The fin (make sure to capture the last packet)

See if you can see how the different layers relate to each other e.g. the sequence number fror TCP and the fragment offset in IP 

PART 2:

Trap a UDP message with Wireshark and determine all of the fields. Notice that it is much simpler than TCP. Please note the differences in both the header format and in the way you would see UDP being used.

PART 3:

We need to be able to measure latency. TTCP is a tool that allows us to do that. TTCP is installed in the network lab and is also a free download. Use TTCP (Test TCP is a free download) to measure the time it takes to form a connection and send a file and disconnect.

- Test this under several different network loads


QUESTION AND ANSWER:

Answer the following questions as part of your report:

- Identify the port numbers for the following applications. 
a. Telnet 
b. HTTP (Hypertext Transfer Protocol) 
c. FTP (File Transfer Protocol) 
d. DNS (Domain Name Server) 
e. DHCP(Dynamic Host Control Protocol) 

- Define the purpose of a connection oriented protocol. Give an example

- What three packets are exchanged between two hosts when establishing a TCP connection? (use your traces to form the proper responses - provide live examples)

- What is a connectionless protocol? Give an example. How is it different from a connection oriented protocol?

- How does tcp improve the ability of IP to send really really large files...show me the math. (calculate the max packet that IP can send and multiply by the maximum fragments...compare that to what TCP can do)

- What is FTP (application) Why is it important? How does it relate to TCP?

- Explain in your own words the sequencing of the sliding window in TCP. Use some examples and draw the buffers.
