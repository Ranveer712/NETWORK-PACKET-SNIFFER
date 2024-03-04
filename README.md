# NETWORK-PACKET-SNIFFER

# Network Packet Sniffer

This project is a network packet sniffer implemented in C, providing a detailed analysis of incoming packets at various protocol layers. It captures and interprets Ethernet, IP, TCP, and UDP headers, offering insights into network traffic. The application runs in a Linux environment using raw sockets and logs packet details to a text file.

# Features:
Packet Types: Identifies and categorizes packets into TCP, UDP, and other protocols.
Detailed Analysis: Parses Ethernet, IP, and transport layer headers, displaying key information such as source/destination addresses, ports, and flags.
Logging: Outputs packet details to a log file for comprehensive network monitoring.

# Tech Stacks:
Programming Language: C
Libraries and Headers: stdio.h, malloc.h, string.h, signal.h, stdbool.h, sys/socket.h, linux/if_packet.h, netinet/in.h, netinet/if_ether.h, netinet/ip.h, netinet/udp.h, netinet/tcp.h, arpa/inet.h
Networking: Raw sockets for packet capture and analysis.
File Handling: File I/O for logging packet details.

# How to Use:
Compile:

bash
Copy code
gcc packet_sniffer.c -o packet_sniffer
Run as Root:

bash
Copy code
sudo ./packet_sniffer
View Logs:

Packet details are logged in the log.txt file.
Note:
Root Access: Ensure running the application with root privileges to capture raw packets.
Linux Environment: Developed and tested in a Linux environment.
Disclaimer:
This tool is designed for educational and research purposes. Use responsibly and adhere to legal and ethical standards when monitoring network traffic. The author is not responsible for any misuse or unlawful activities.
