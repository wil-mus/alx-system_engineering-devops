#Firewall

The term firewall originally referred to a wall intended to confine a fire within a line of adjacent buildings.[4] Later uses refer to similar structures, such as the metal sheet separating the engine compartment of a vehicle or aircraft from the passenger compartment. The term was applied in the late 1980s to network technology[5] that emerged when the Internet was fairly new in terms of its global use and connectivity.[6] The predecessors to firewalls for network security were routers used in the late 1980s. Because they already segregated networks, routers could apply filtering to packets crossing them.[7]

Before it was used in real-life computing, the term appeared in the 1983 computer-hacking movie WarGames, and possibly inspired its later use.[8]

#Types
See also: Computer security and Comparison of firewalls
Firewalls are categorized as a network-based or a host-based system. Network-based firewalls are positioned between two or more networks, typically between the local area network (LAN) and wide area network (WAN),[9] their basic function is to control the flow of data between connected networks. They are either a software appliance running on general-purpose hardware, a hardware appliance running on special-purpose hardware, or a virtual appliance running on a virtual host controlled by a hypervisor. Firewall appliances may also offer non firewall functionality, such as DHCP[10][11] or VPN[12] services. Host-based firewalls are deployed directly on the host itself to control network traffic or other computing resources.[13][14] This can be a daemon or service as a part of the operating system or an agent application for protection.



##Packet filter
The first reported type of network firewall is called a packet filter, which inspects packets transferred between computers. The firewall maintains an access-control list which dictates what packets will be looked at and what action should be applied, if any, with the default action set to silent discard. Three basic actions regarding the packet consist of a silent discard, discard with Internet Control Message Protocol or TCP reset response to the sender, and forward to the next hop.[15] Packets may be filtered by source and destination IP addresses, protocol, source and destination ports. The bulk of Internet communication in 20th and early 21st century used either Transmission Control Protocol (TCP) or User Datagram Protocol (UDP) in conjunction with well-known ports, enabling firewalls of that era to distinguish between specific types of traffic such as web browsing, remote printing, email transmission, and file transfers.[16][17]

The first paper published on firewall technology was in 1987 when engineers from Digital Equipment Corporation (DEC) developed filter systems known as packet filter firewalls. At AT&T Bell Labs, Bill Cheswick and Steve Bellovin continued their research in packet filtering and developed a working model for their own company based on their original first-generation architecture.[18] In 1992, Steven McCanne and Van Jacobson released a paper on BSD Packet Filter (BPF) while at Lawrence Berkeley Laboratory.[19][20]

##Connection tracking

Flow of network packets through Netfilter, a Linux kernel module
Main article: Stateful firewall
From 1989–1990, three colleagues from AT&T Bell Laboratories, Dave Presotto, Janardan Sharma, and Kshitij Nigam, developed the second generation of firewalls, calling them circuit-level gateways.[21]

Second-generation firewalls perform the work of their first-generation predecessors but also maintain knowledge of specific conversations between endpoints by remembering which port number the two IP addresses are using at layer 4 (transport layer) of the OSI model for their conversation, allowing examination of the overall exchange between the nodes.[22]
