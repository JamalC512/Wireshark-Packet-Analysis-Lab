# Wireshark Packet Analysis Lab

## Project Overview

The Wireshark Packet Analysis Lab was a network forensics project where I investigated captured network traffic to better understand suspicious web activity. The project required me to analyze packets inside Wireshark, identify important network information, examine HTTP communication, and connect information from multiple packets to understand what happened during the captured activity.

Instead of only looking at individual packets, I worked through the packet capture as an investigation. I used different pieces of network information to identify the systems involved, examine the communication between them, and reconstruct a timeline of activity.

## Investigation Environment

The main tool used during this project was Wireshark. I worked with an existing packet capture containing network traffic that could be examined without interacting with a live production network.

The packet capture contained different types of network communication, so part of the investigation involved narrowing down the traffic and focusing on the packets that were relevant to the suspicious activity.

Some of the main concepts and technologies involved included:

- Wireshark
- Packet Captures
- TCP/IP
- HTTP
- IP Addresses
- MAC Addresses
- Network Protocols
- Wireshark Display Filters
- HTTP POST Requests
- Network Forensics

## Initial Packet Capture Analysis

I started the investigation by opening the packet capture in Wireshark and reviewing the traffic that had been recorded.

A packet capture can contain a large amount of information, so I had to determine which packets were useful to the investigation instead of trying to examine everything at the same time.

I reviewed packet information such as:

- Source IP addresses
- Destination IP addresses
- Source MAC addresses
- Destination MAC addresses
- Network protocols
- Source and destination ports
- Packet timestamps

Looking at this information helped me identify which systems were communicating and gave me a starting point for investigating the suspicious traffic.

## Using Wireshark Filters

One of the important parts of the project was using Wireshark filters to narrow down the packet capture.

Instead of manually searching through every packet, I could focus on specific types of network communication. This made it easier to locate traffic related to the investigation.

For example, filtering traffic by protocol allowed me to focus on HTTP communication when investigating web activity.

Using filters helped me understand why packet filtering is important during network investigations. Large packet captures can contain many unrelated connections, and narrowing the results makes it easier to identify useful evidence.

## Identifying Systems on the Network

During the investigation, I examined source and destination IP addresses to determine which systems were communicating with each other.

I also examined MAC addresses contained within the captured traffic. This gave me additional information about the devices involved in communication on the local network.

By comparing addressing information across multiple packets, I could better understand the direction of the traffic and determine which system was sending or receiving specific requests.

This strengthened my understanding of the difference between Layer 2 information such as MAC addresses and Layer 3 information such as IP addresses.

## Analyzing HTTP Traffic

A major part of the investigation focused on HTTP traffic.

I examined HTTP requests to better understand the communication between the client and web server. Looking at the HTTP traffic allowed me to see what type of web activity was taking place and identify requests that were relevant to the investigation.

Because HTTP operates at the application layer, analyzing it provided information beyond basic source and destination addresses. I was able to examine details associated with web requests and connect that information with the TCP/IP communication carrying the traffic.

## HTTP POST Analysis

I also examined HTTP POST traffic during the investigation.

POST requests are commonly used when information is submitted from a client to a web server. Examining this traffic helped me understand what information was being transmitted during the captured web activity.

I inspected the HTTP POST data contained within relevant packets and used that information as another part of the investigation.

This demonstrated why unencrypted HTTP traffic can create security concerns. Information transmitted through HTTP may be visible inside a packet capture because the application data is not protected by encryption in the same way that HTTPS traffic normally is.

## Following Network Activity

Instead of treating each packet as an isolated event, I compared information across multiple packets.

I looked at timestamps, IP addresses, protocols, and HTTP activity to understand how different packets were connected.

This helped me follow the communication between systems and understand the order in which different network events occurred.

Looking at the traffic this way was important because a single packet usually does not explain an entire incident. The larger picture becomes clearer when information from multiple packets is compared.

## Reconstructing the Timeline

After identifying the relevant network traffic, I used packet timestamps and communication details to reconstruct a timeline of the activity.

I compared when requests occurred, which systems were involved, and what type of HTTP communication was taking place.

By putting these events in order, I was able to develop a clearer picture of the actions that occurred during the captured session.

Timeline reconstruction helped turn the packet capture from a collection of individual packets into a sequence of network events that could be analyzed as part of an investigation.

## Identifying Suspicious Activity

By combining information from the packet capture, I was able to identify the network source associated with the suspicious web activity.

This required comparing several types of information instead of relying on only one packet or one network address.

The investigation involved connecting:

- IP address information
- MAC address information
- HTTP requests
- HTTP POST data
- Packet timestamps
- Communication between systems

Using these details together allowed me to better understand where the suspicious activity originated and what occurred during the captured network session.

## Network Forensics Process

This project helped me understand a basic network forensics workflow.

The process included:

1. Opening and reviewing the packet capture
2. Identifying the protocols contained in the traffic
3. Filtering the capture to reduce unrelated packets
4. Identifying source and destination systems
5. Examining IP and MAC addresses
6. Investigating HTTP communication
7. Inspecting HTTP POST data
8. Comparing timestamps and packet details
9. Reconstructing the sequence of activity
10. Identifying the source associated with the suspicious traffic

Following a process like this made the investigation more organized and helped me avoid looking at packets without a clear purpose.

## Security Concepts Demonstrated

This project covered several networking and cybersecurity concepts, including:

- Packet Analysis
- Network Forensics
- Network Traffic Analysis
- TCP/IP
- HTTP
- HTTP POST Requests
- IP Address Analysis
- MAC Address Analysis
- Protocol Analysis
- Packet Filtering
- Timeline Reconstruction
- Network Investigation
- Traffic Attribution

## Skills and Technologies

**Network Analysis**
- Wireshark
- Packet Captures
- Wireshark Display Filters
- Traffic Analysis

**Networking**
- TCP/IP
- HTTP
- IP Addresses
- MAC Addresses
- Network Protocols
- Client and Server Communication

**Cybersecurity**
- Network Forensics
- Suspicious Traffic Investigation
- HTTP POST Analysis
- Timeline Reconstruction
- Network Evidence Analysis

## What I Learned

The Wireshark Packet Analysis Lab helped me become more comfortable working with packet captures and investigating network traffic.

One of the biggest things I learned was that network investigations require more than finding one suspicious packet. I had to compare information across multiple packets and use IP addresses, MAC addresses, protocols, timestamps, and HTTP data together to understand what was happening.

I also gained more experience using Wireshark filters to narrow down traffic. This made it easier to focus on relevant packets and showed me how important filtering can be when working with a large amount of network data.

Analyzing HTTP and HTTP POST traffic also helped me understand why encryption is important when transmitting information across a network. Being able to inspect application data inside captured HTTP traffic demonstrated the security risks associated with sending sensitive information without encryption.

Overall, this project strengthened my skills in Wireshark, packet analysis, TCP/IP, HTTP analysis, network troubleshooting, network forensics, and cybersecurity investigation.

## Disclaimer

This project was completed using packet capture data in a controlled educational environment for cybersecurity and network forensics training.
