## Network Device Programming
***
Network Device Programming covers the concepts, principles, architecture, and implementation of network programming, with a focus on Software-Defined Networking (SDN). Students study the separation of the control plane and data/forwarding plane, SDN architecture, SDN controllers, OpenFlow, programmable switches, network automation, REST APIs, and network application development.
In this practical session, we will build a virtual network environment using Linux, Open vSwitch, Mininet, Python, and an SDN controller, and then develop a simple application or controller to programmatically handle configuration, monitoring, flow management, routing, traffic engineering, and network policies.


<b>1. Tabel Of Content</b>
|Chapter| Meeting |Section | Sub-Section Theory|Sub-Section Practice|
| --- | --- |--- | --- | --- |
| <p align="center">1</p> | <p align="center">1</p> |<b>Introduction to Network Device Programming</b> |Definition of network programming, Differences between manual configuration and programmable networking, Network devices and network operating systems, CLI vs. API, Network automation, Basic concepts of SDN, Motivation for SDN development [[read]](https://github.com/syaifulahdan/Netadmin/blob/main/Network_Administration_Tools/netadtools.md) | Install Ubuntu Linux and VirtualBox; introduction to Linux networking (ip, Ping, Traceroute, tcpdump); Python for simple network programming. [[read]](https://github.com/syaifulahdan/Netadmin/blob/main/Network_Administration_Tools/netadtools.md) |
| <p align="center">2</p> | <p align="center">2</p> | <b>Python Fundamentals for Network Programming</b> |Python for network administration, socket programming, IP addresses, TCP/UDP, client-server, JSON, REST API| Create Network Information Tools Programs, Program Functions (display hostname, IP address, Interface, Routing table, interface status, connectivity test) |
| <p align="center">3</p> | <p align="center">3</p> | <b>SDN Concepts and Architecture</b> |Traditional networking, Control plane, Data plane, Management plane SDN, Separation of control plane and forwarding plane, Centralized/logically centralized control, Programmability, Network abstraction|Mininet installation in a Linux environment, Introduction to Open vSwitch, Viewing OVS bridges and flows|  
| <p align="center">1-3</p> | <p align="center">4</p> | <b>Quiz</b> |1-3|1-3| 
| <p align="center">4</p> | <p align="center">5</p> | <b>OpenFlow</b> | OpenFlow, OpenFlow switch, Controller, Flow table, Match, Action Priority, Cookie, Timeout, Packet-In, Packet-Out, Flow-Mod, Statistics | View flows, add flows, delete flows, view statistics |
| <p align="center">5</p> |<p align="center">6</p> | <b>Mininet</b> |Network emulation, Virtual network, Mininet Host, Switch, Link, Controller, Topology| Create a host (h1, h2..), Create a switch (s1, s2..), Test connectivity (Pingall, nodes, net, dump) |
| <p align="center">6</p> | <p align="center">7</p> |<b>Mininet Topology Programming</b> |Mininet Python API, Custom topology, , Host, Switch, BandwidthDelay, Packet loss| Creating a topology in Python; configuring bandwidth, delay, packet loss, and topology. |
| <p align="center">1-6</p> | <p align="center">8</p> |<b>Midterm exam</b> | 1-7| 1-7|
| <p align="center">7</p>| <p align="center">9</p>| <b>SDN Controller</b> | Controller function, Controller architecture, Southbound API, Northbound API, Controller application, Reactive vs proactive forwarding, Controller scalability, Controller (Ryu / os-ken, ONOS, OpenDaylight, Faucet)| Running the controller and connecting (Mininet and Controller) |
| <p align="center">8</p> | <p align="center">10</p> |<b>SDN Programming: Forwarding</b> | Reactive forwarding, Proactive forwarding, MAC learning, Flow installation, Packet-In, Packet-Out | SDN Learning Switch: Creating a Controller Application (Packet-In, MAC Learning, Determining Output Port, Installing Flow Rules, Forwarding Packets) |
| <p align="center">9</p> | <p align="center">11</p> | <b>SDN Routing</b> | SDN-based routing, Shortest path, Topology Discovery, Link Cost, Dynamic routing | Creating an SDN Dynamic Router, Program: Network topology, Topology Discovery, Path calculation, flow installation, packet forwarding |
| <p align="center">10</p> | <p align="center">12</p> |<b>Network Monitoring</b> | Network telemetry, Flow statistics, Port statistics, Bandwidth monitoring, Latency, Packet loss, Network utilization |Create SDN Network Monitor, Dashboard/CLI displays: Packet count, byte count, bandwidth, port utilization, flow count |
| <p align="center">11</p> | <p align="center">13</p> |<b>SDN Security</b> | SDN security, Flow-based filtering, Access control, Traffic blocking, DDoS detection concept, Controller security, Southbound security, Single point of failure |Create SDN Firewall, Allow & Deny, TCP 80, TCP 443, ICMP, TCP 23, Selected IP|
| <p align="center">12</p> | <p align="center">14</p> |<b>Traffic Engineering</b> |Traffic engineering, Path Selection, Load Balancing, Congestion, Link Utilization, QoS, Bandwidth-aware routing | Developing an SDN Load Balancer / Traffic Engineering Application |
| <p align="center">13</p> | <p align="center">15</p> |<b>Network Automation dan REST API</b> |REST API, JSON, Network automation, API-based management, SDN northbound interface, Automation workflow |Students create a simple API: GET /switches, GET /flows, GET /statistics, POST /flow, DELETE /flow. |

<b>2. Prerequisite</b>

To support Network Programming laboratory activities, providing an adequate working environment is crucial for ensuring that every testing scenario runs optimally. This course requires a suite of complementary software tools—ranging from virtualization environments and operating systems, Software-Defined Networking (SDN)-based network emulators, and data traffic analysis tools to web/API development frameworks and version control systems. Each of these software components plays a specific role in ensuring the comprehensive implementation of network programming, simulation, and analysis workflows.

|No|Software| Function |URL |
| --- | --- | --- |--- | 
|<p align="center">1</p>| <p align="center">Linux Ubuntu</p> |Operating System | [https://ubuntu.com/download](https://ubuntu.com/download) |  
|<p align="center">2</p>| <p align="center">VirtualBox</p> |Virtual machine for running various operating systems | [https://www.virtualbox.org/](https://www.virtualbox.org/) |  
|<p align="center">3</p>| <p align="center">Python</p> |Network Programming | [https://www.python.org/](https://www.python.org/) |  
|<p align="center">4</p>| <p align="center">Mininet</p> |SDN Network Emulator |[https://mininet.org/](https://mininet.org/) |  
|<p align="center">5</p>| <p align="center">Open vSwitch</p> |Virtual SDN Switch |[https://www.openvswitch.org/](https://www.openvswitch.org/) |  
|<p align="center">5</p>| <p align="center">OpenFlow</p> |Southbound Protocol |[https://opennetworking.org/](https://opennetworking.org/) |  
