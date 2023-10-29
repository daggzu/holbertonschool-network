# Networking Basics #0 Learning!

## Learning Objectives:

## OSI Model
### What is it? / How many layers it has? / How is it organized?

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a communication system into
seven different layers. It was developed by the International Organization for Standardization (ISO) in the late 1970s.

Each layer in the OSI model has a specific role and set of functions, and they work together to facilitate communication between
different devices and systems in a network. The layers are as follows:

1. Physical Layer: This layer deals with the physical transmission of data over the network, including the electrical, mechanical, and
physical aspects of communication.

2. Data Link Layer: It provides reliable and error-free transmission of data frames between two directly connected nodes. It also
handles flow control and error detection.

3. Network Layer: This layer is responsible for addressing, routing, and logical transmission of data packets across different networks.
It determines the best path for data transmission.

4. Transport Layer: It ensures reliable and error-free end-to-end data delivery between hosts. It manages the segmentation and
reassembly of data, as well as flow control and error recovery.

5. Session Layer: This layer establishes, manages, and terminates communication sessions between applications. It also provides
synchronization and dialog control.

6. Presentation Layer: It is responsible for data formatting, encryption, and compression. It ensures that data from the application
layer is properly formatted for transmission.

7. Application Layer: This layer interacts directly with the end-user and provides network services to applications. It includes
protocols for various applications such as email, file transfer, and web browsing.

The OSI model provides a standardized framework for understanding and designing network communication protocols. It allows different
systems to communicate with each other by using compatible protocols at each layer.


## What is a LAN?
### Typical Usage. / Typical Geographival Size.

LAN (Local Area Network) is a network that connects devices within a limited geographical area, such as a home, office building, or
school. It allows devices like computers, printers, and servers to communicate and share resources with each other.

LANs are typically owned and controlled by a single organization or individual. They use wired or wireless connections to establish a
network infrastructure. Ethernet is the most common technology used for wired LAN connections, while Wi-Fi is often used for wireless
LANs.

The main take-away, LANs are designed to facilitate local communication and resource sharing, making them essential for small to
medium-sized networks in various settings.

## What is a WAN?
### Typical Usage. / Typical Geographival Size.

A WAN (Wide Area Network) is a type of network that spans a large geographical area, connecting multiple LANs and other networks
together. Unlike LANs, which are confined to a specific location, WANs can cover vast distances and connect devices across cities,
countries, or even continents.

WANs are typically used to facilitate communication and data transfer between different locations of an organization. They utilize
various technologies, such as leased lines, satellite links, and internet connections, to establish connections between distant sites.

The main take-away, WANs play a crucial role in enabling global communication, data sharing, and access to centralized resources for
organizations with geographically dispersed locations. They allow for efficient collaboration and information exchange across wide
distances.

## What is the Internet?
### What is an IP address? / What are the 2 types of IP address? / What is *localhost*? / What is a subnet? /Why IPv6 was created?

The **internet** is a global network of interconnected computers and devices that communicate with each other using a standardized set of
protocols. It is a vast network that spans the globe, allowing users to access and share information, communicate, and utilize various
online services.

An **IP address** (Internet Protocol address) is a unique numerical label assigned to each device connected to a computer network that
uses the Internet Protocol for communication. It serves two main functions:

1. Device Identification: An IP address uniquely identifies a device on a network. It allows other devices to locate and communicate
with it. Similar to a phone number or a street address, an IP address helps route data to the correct destination.

2. Network Addressing: IP addresses also enable devices to send and receive data packets across networks. They provide a way for devices
to identify the source and destination of data transmissions.

IP addresses are typically represented in either IPv4 (Internet Protocol version 4) or IPv6 (Internet Protocol version 6) format. IPv4
addresses consist of four sets of numbers separated by periods (e.g., 192.168.0.1), while IPv6 addresses use a longer hexadecimal format
(e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

**IPv6** (Internet Protocol version 6) was created to address the limitations of IPv4 (Internet Protocol version 4) and to meet the
increasing demand for IP addresses. Few main reasons for the development of IPv6 wwas, like previously mentioned, to increase the scale
of IP addresses being handle, with that improve the security by implementing features such as IPsec (Internet Protocol Security). In
addition, improving network traffic and better management of date, and making this implementation be long lansting with the ability to
adapt to future demands and increasing growth of users.

The term **localhost** is commonly used when developing and testing web applications or networking software. By running a web server or
other services on the localhost, developers can access and debug their applications locally before deploying them to a remote server. It
provides a convenient way to test and troubleshoot software without the complexities of a network environment.

When a program or application on a device communicates with the localhost, it is essentially sending and receiving data within the same
device. It allows programs to test and access services running on the device without the need for an external network connection.

A **subnet**, short for subnetwork, is a division of an IP network into smaller, more manageable segments. It allows for efficient
network management, improved security, and optimized routing of network traffic.

Subnetting is a fundamental concept in IP networking and is widely used to design and manage complex networks. It helps in organizing
and optimizing network infrastructure to meet the specific needs of an organization.


## TCP/UDP
### What are the 2 mainly used data transfer protocols for IP (transfer level on the OSI schema)? / What is the main difference between
### TCP and UDP? / What is a port? / Memorize SSH, HTTP and HTTPS port numbers. / What tool/protocol is often used to check if a device
### is connected to a network?

The two commonly used data transfer protocols for IP at the transport layer of the OSI model are TCP (Transmission Control Protocol) and
UDP (User Datagram Protocol).

**TCP** is a connection-oriented protocol that provides reliable, ordered, and error-checked data delivery. It establishes a connection
between the sender and receiver, ensures data integrity, and handles congestion control and flow control. TCP is commonly used for
applications that require guaranteed delivery of data, such as web browsing, email, file transfer, and streaming media.

**UDP**, on the other hand, is a connectionless protocol that offers a simpler, lightweight approach to data transmission. It does not
establish a connection or provide reliability mechanisms like TCP. UDP is often used for applications that prioritize speed and
efficiency over guaranteed delivery, such as real-time streaming, online gaming, DNS (Domain Name System), and VoIP (Voice over IP)
services.

In terms of main differences, TCP provides reliable, ordered, and connection-oriented data transmission, while UDP offers faster
connectionless, and unreliable transmission. The choice between TCP and UDP depends on the specific requirements of the application and
the trade-offs between reliability and speed.

A **port** refers to a communication endpoint in an operating system. It is a numerical identifier that allows different processes or
services on a device to send and receive data over a network.

Ports are part of the TCP/IP protocol suite and are used in conjunction with IP addresses to establish connections between devices. They
provide a way for multiple applications or services to operate simultaneously on a single device, each using a unique port number.

The default port numbers for **SSH**, **HTTP**, and **HTTPS** are as follows:

1. SSH (Secure Shell):
   - Port number: 22

2. HTTP (Hypertext Transfer Protocol):
   - Port number: 80

3. HTTPS (HTTP Secure):
   - Port number: 443

These port numbers are widely used and recognized as the default ports for these protocols. However, it's important to note that these
protocols can be configured to use different port numbers if desired.

Tool/protocol to check if a device is connected to a network is **ICMP** (Internet Control Message Protocol). ICMP is a network protocol
that allows devices to send and receive control messages to check connectivity, diagnose network issues, and exchange error messages.

The most commonly used ICMP tool is the "ping" command. It sends an ICMP Echo Request message to a specific IP address and waits for an
ICMP Echo Reply message. If the device receives the Echo Reply, it confirms that the device is connected and reachable on the network.
