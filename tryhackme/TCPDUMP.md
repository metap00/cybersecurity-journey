# TCPDUMP Lab

 - -i INTERFACE, filtering the interace you listen
 - -c COUNT, specify the amount of packets u list
 - -w FILE, saving a file
 - -r FILE, reading a file
 - -n to stop resolving friendly ip adresses
 - -nn to stop resolving port numbers
 - OPERATORS: and, or, not
   
 <img width="982" height="835" alt="image" src="https://github.com/user-attachments/assets/9c3556fe-5322-4d7e-a3f8-46f1ef78a058" />

 - greater LENGTH: Filters packets that have a length greater than or equal to the specified length
 - less LENGTH: Filters packets that have a length less than or equal to the specified length
 - Using pcap-filter, Tcpdump allows you to refer to the contents of any byte in the header using the following syntax proto[expr:size], where:
 - proto refers to the protocol. For example, arp, ether, icmp, ip, ip6, tcp, and udp refer to ARP, Ethernet, ICMP, IPv4, IPv6, TCP, and UDP respectively.
 - expr indicates the byte offset, where 0 refers to the first byte.
 - size indicates the number of bytes that interest us, which can be one, two, or four. It is optional and is one by default.

 TCP FLAGS:
 - tcp-syn TCP SYN (Synchronize)
 - tcp-ack TCP ACK (Acknowledge)
 - tcp-fin TCP FIN (Finish)
 - tcp-rst TCP RST (Reset)
 - tcp-push TCP Push

Tcpdump is a rich program with many options to customize how the packets are printed and displayed:

- q: Quick output; print brief packet information
- e: Print the link-level header
- A: Show packet data in ASCII
- xx: Show packet data in hexadecimal format, referred to as hex
- X: Show packet headers and data in hex and ASCII
