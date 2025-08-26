<section class="hero">
  <h6 align="Center">PS &mdash; 02</h6>
  <div align="center">
    <h2>
      Network Fundamentals
    </h2>
    <p>
      Within this <strong>Network Fundamentals</strong> section, we will be taking a look at <strong><a href="#what-is-networking">What is Networking</a></strong>, <strong><a href="#intro-to-lan">Intro to LAN</a></strong>, <strong><a href="#osi-model">OSI Model</a></strong>, <strong><a href="#packets--frames">Packets & Frames</a></strong> & <strong><a href="#extending-your-network">Extending your Network</a></strong>.
    </p>
  </div>
</section>

### What is Networking
#### **Task 1** &mdash; What Is Networking?

Networks are simply things connected. Two or more devices connected can be considered a network. Networks come in all shapes and sizes, such as:

- **PAN** 
  - _Personal Area Network_
- **LAN** 
  - _Local Area Network_
- **WLAN** 
  - _Wireless Local Area Network_
- **CAN** 
  - _Campus Area Network_
- **MAN** 
  - _Metropolitan Area Network_
- **WAN** 
  - _Wide Area Network_

**Answer the questions below** <br>
What is the key term for devices that are connected together.
- [x] Networks

<br>

#### **Task 2** &mdash; What Is The Internet?

The first iteration of the internet was within the ARPNET project, which was funded by the United States Defense Department. It wasn't until 1989, that the internet as we know it was invented by Tim Burners-Lee. 

The Internet is made up of many smaller networks all joined together. These smaller networks are called private networks, where as networks connecting these smaller networks are called public networks or the internet.

Networks can be one of two types:

- Private Network
- Public Network

**Answer the questions below** <br>
Who invented the World Wide Web?
- [x] Tim Burners-Lee

<br>

#### **Task 3** &mdash; Identifying Devices on a Network

To communicate and maintain order, devices must be both identifying & Identifiable on a network. Devices on networks are similar to humans in the fact that we have two ways of being identified, our name (IP Address) and our fingerprints (MAC Address).

Now we can change our name, but we cannot change our fingerprints. Devices work in the same way, it has two means of identification, with one being permeable. The IP Address being the permeable one.

#### IP Addresses

An IP Address or Internet Protocol Address can be used as a way of Identifying a host on a network for a period of time, whereby it can then be associated with another device without the IP Address changing. 

An IP Address is a set of numbers divided into four octets, This is an IP Address `192.168.1.1`, now lets break that down:

|Octet #1|Octet #2|Octet #3|Octet #4|
|:---:|:---:|:---:|:---:|
|192|168|1|1|
|0-255|0-255|0-255|0-255|

The Value of each octet will summarize to be the IP Address of the device on the network. Its calculated though a technique known as IP Addressing & Subnetting. What is important to understand here is that IP Addresses can change from device to device but cannot be simultaneously active more than once within the same network.

IP addresses follow a set of standards known as Protocols. Protocols are the backbone of networking and its what forces devices to communicate using the same language.

Devices can be on both a Private and Public network, and depending on where they are will determine what type of IP Address they will have, either a Private or Public IP Address.

|Device Name|IP Address|IP Address Type|
|:---|:---|:---:|
|DESKTOP-KJE57DF|192.168.1.77|Private|
|DESKTOP-KJE57DF|886.157.52.21|Public|
|CMNatic-PC|192.168.1.74|Private|
|CMNatic-PC|86.157.52.21|Public|

These two devices will be able to use their private IP Address to communicate with each other. However, any data sent to the internet from either of these devices will be identified by the same Public IP Address. A Public Ip Address is given by your ISP or Internet Service Provider.

There are to versions of IP Address, IPv4 & IPv6. The IPv4 Scheme has a numbering system of 2^32 which equates to 4.29 billion unique IP Addresses, which is a concern as more and more people are connecting to the internet. Here comes IPv6 which has a numbering scheme of 2^128, which equates to 340 trillion+ Unique IP Address, essentially solving that problem.

IPv6 uses 128-bit addresses written in hexadecimal (8 groups separated by colons), while IPv4 uses 32-bit addresses written in decimal (4 groups separated by dots).

|IP Address Version|Example|
|:---:|:---:|
|IPv6|2001:0db8:85a3:0000:0000:8a2e:0370:7334|
|IPv4|192.168.1.1|

#### MAC Addresses

All devices on a network have a Physical Network Interface, Which is a microchip board found on the device's motherboard. This Network interface is assigned a unique address at the factory it was made. This is known as the MAC Address or Media Access Control Address. 

A MAC Address is a 12 character hexadecimal number, seperated by colons, these colons known as seperators. This es an example of a MAC Address, `a4:c3:f0:85:ac:2d`, Where the first 6 characters represent the company who built the device and the last 6 being a unique number given to, and burnt into that device.

|Vendor Unique Number|Device Unique Number|
|:---:|:---:|
|a4:c3:f0|85:ac:2d|

MAC Address can be faked or spoofed in a process known as spoofing, meaning someone can copy your MAC Address which can create some security risks as one device is pretending to be another. If you have a firewall which allows communication to and from a specific MAC Address, if a device were to pretend or spoof that MAC, the firewall would now think that it is receiving communication from the trusted device itself.

**Answer the questions below** <br>
What does the term "IP" stand for?
- [x] Internet Protocol

What is each section of an IP address called?
- [x] Octet

How many sections (in digits) does an IPv4 address have? 
-[x] 4

What does the term "MAC" stand for?
- [x] Media Access Control

<br>

#### **Task 4** &mdash; Ping (ICMP)

Ping which uses ICMP or Internet Control Message Protocol, is a fundamental network tool used to gauge the performance of a connection between devices, as in if the connection exists or is stable.

Ping can be performed against devices within your network or on websites, it comes installed on most OS, _Operating Systems_, such as Linux or Windows. The syntax for ping is `ping IP Address or website URL`, example `ping 8.8.8.8`.

**Answer the questions below** <br>
What protocol does ping use?
- [x] ICMP or Internet Control Message Protocol

What is the syntax to ping 10.10.10.10?
- [x] ping 10.10.10.10

<hr>

### Intro to LAN
#### **Task 1** &mdash; Introducing Lan Topologies

#### Local Area Network (LAN) Topologies

Within networking, when talking about topologies, we are speaking about the design or look of the network at hand. Over the years there have many various experimentation and  implementations of network designs. We will be looking at different topologies and its advantages and disadvantages.

#### The Star Topology

This is the most common lan topology found today due to its reliability and scalability, The premise of this topology is that devices individually connect to a central networking device such as a Switch or HUB. Any information sent to a device in this topology is sent via the central device to which it is connected.

**Advantages**
- More Scalable, its easy to add more devices as the demand for the network increases.
- Robust devices, prone to failure, although reduce to its robust nature.


**Disadvantages**
- Cost due to more cabling and dedicated networking devices, this making more expensive than any other topology. As the network scale, it requires more maintenance to keep the network functional.
- Troubleshooting faults can be harder.

#### BUS Topology

This type of device relies on a single connection, also known as a backbone cable, Think of it as a leaf on a tree, where the devices are the leaves that stem from a branch.


**Advantages**
- Easy to setup
- Cost Effective

**Disadvantages**
- Prone to network becoming slow and bottlenecking.
- Bottlenecking also results in difficult to troubleshoot instances, as  it becomes difficult to identify which device is experiencing issues with data all traveling along the same cable.

#### Ring Topology

The ring topology, also known as the token topology boasts some similarities. Devices such as computers are connected directly to each other to form a loop, meaning there is little cabling required and less dependence on dedicated hardware such as within the star topology.

A ring topology works be sending data across the loop until it reaches its destined device, it uses other devices along the loop to forward the data. A device will only send data along if it itself doesn't have data to send first.

There is only one direction data can travel across this topology, it is fairly easy to troubleshoot any faults, however, its not an effective way for data to travel across a network as it has to visit other devices first. They are also prone to bottlenecks such as within the BUS Topology, A cut in the cable or broken device will result in the entire  network breaking.

#### What is a Switch?

Switches are dedicated devices within a network that are designed to aggregate various other network capable devices using ethernet. These various devices plug into the switches port.

Switch are usually found in larger networks such as Businesses, Schools or similar sized networks, basically where there are many devices to connect to the network. Switch can connect a large number of devices by having ports of 4, 8 16, 24, 32 and 64 for devices to connect to.

Switches are more efficient than simpler devices such as hubs and repeaters. A repeater is used to regenerate a signal on a cable when the distance is too long and the signal weakens. A hub functions as a multi-port repeater, broadcasting the signal to all connected devices, whereas a switch forwards data only to the intended device, making it faster and more efficient.

Switches also keep track of what device is connected to which port, this way when they receive a packet, instead of repeating that packet to every port, like a hub would do, it just sends it to the intended target, thus reducing network traffic,

Both switches and Routers can be connected to one another. 

#### What is a Router?

Its a Routers job to connect networks and pass data between them, It does this through a process known as routing, hence a router. Routing is the label given to the process of data traveling across networks. Routing involves creating a path between networks, so that this data can be successfully delivered.

**Answer the questions below** <br>
What does LAN stand for?
- [x] Local Area Network

What is the verb given to the job that Routers perform?
- [x] Routing

What device is used to centrally connect multiple devices on the local network and transmit data to the correct location?
- [x] Switch

What topology is cost-efficient to set up?
- [x] Bus Topology

What topology is expensive to set up and maintain?
- [x] Star Topology

<br>

#### **Task 2** &mdash; A Primer on Subnetting

Subnetting is the term of splitting up a network into smaller, miniature networks within itself. Network Admins, can split up and assign different parts of a network using subnetting, to reflect which network belongs to which department, such as Accounting, Human resources and Finance.

Subnetting is achieved by splitting up the number of hosts that can fit within the network which is represented by a number called a subnet mask. Lets take the IP Address before 192.168.1.1

|Octer #1|Octer #2|Octer #3|Octer #4|
|:---:|:---:|:---:|:---:|
|192|168|1|1|
|255|255|255|0|

An IP Address is made up of four octets, the same goes for a subnet mask, which is represented as a number of four bytes or 32 bits, this ranging from 0 to 255.

Subnets use IP addresses in three different ways:

- Identify the network address
- Identify the host address
- Identify the default gateway

|Type|Purpose|Explanation|Example|
|:---|:---|:---|:---:|
|Network Address|This address identifies the start of the actual network and is used to identify a network's existence.|For example, a device with the IP address of 192.168.1.100 will be on the network identified by 192.168.1.0|192.168.1.0|
|Host Address|An IP address here is used to identify a device on the subnet|For example, a device will have the network address of 192.168.1.1|192.168.1.100|
|Default Gateway|The default gateway address is a special address assigned to a device on the network that is capable of sending information to another network |Any data that needs to go to a device that isn't on the same network (i.e. isn't on 192.168.1.0) will be sent to this device. These devices can use any host address but usually use either the first or last host address in a network (.1 or .254)|192.168.1.254|

In small networks, such as at home, you will be on one subnet, as there is an unlikely chance that you need more than 254 devices connected at one time. Though Businesses and Offices will have more devices and this is where subnetting takes place.

Subnetting provides a range of benefits, including:

- Efficiency
- Security
- Full control

**Answer the questions below** <br>
What is the technical term for dividing a network up into smaller pieces?
- [x] Subnetting

How many bits are in a subnet mask?
- [x] 32bits

What is the range of a section (octet) of a subnet mask?
- [x] 0-255

What address is used to identify the start of a network?
- [x] Network Address

What address is used to identify devices within a network?
- [x] Host Address

What is the name used to identify the device responsible for sending data to another network?
- [x] Default Gateway

<br>

#### **Task 3** &mdash; ARP

Devices can have 2 Identifiers, a MAC and IP Address, ARP or the Address resolution Protocol, is the technology that is responsible for allowing devices to identify themselves on a network.

ARP, Allows a device to associate their MAC Address to an IP Address, furthermore, each device  on a network will keep a log of the MAC Address associated to other devices.

When devices wish to communicate with another, they will send a broadcast to the entire network searching for the specific device,

#### How does ARP Work?

Each device within a network has a ledger to store information on, which is called a cache. With Arp this cache store identifiers of other devices on the network. To map these to identifiers together, the IP and MAC, ARP sends two types of messages:

- ARP Request
- ARP Reply

When an ARP Request is sent, a message is broadcasting on the network to other devices asking, what MAC address owns this IP Address. When the other devices receives that messages, they will only respond if they own that IP Address and then will send back an ARP Reply with its MAC Address.

**Answer the questions below** <br>
What does ARP stand for?
- [x] Address Resolution Protocol

What category of ARP Packet asks a device whether or not it has a specific IP address?
- [x] ARP Request

What address is used as a physical identifier for a device on a network?
- [x] MAC Address

What address is used as a logical identifier for a device on a network?
- [x] IP Address

#### **Task 4** &mdash; DHCP

DHCP, which stands for Dynamic Host Configuration Protocol, is used to automatically give a device a IP Address if said device was not given one manually. This is done by using the DHCP Server.

This is done by when a device connects to a network, it sends out a request known as  DHCP Discover to see if any DHCP servers are on the network. 

The DHCP server then replies back with an IP Address known as a DHCP Offer. The device then sends out a reply confirming it wants the offered IP Address in the form of DHCP Request. The DHCP Server then replies with a DHCP ACK to acknowledge this request and the device can now start using that IP Address.

Lets break down the DHCP Protocol:

- DHCP Discover
- DHCP Offer
- DHCP Request
- DHCP ACK

**Answer the questions below** <br>
What type of DHCP packet is used by a device to retrieve an IP address?
- [x] DHCP Discover

What type of DHCP packet does a device send once it has been offered an IP address by the DHCP server?
- [x] DHCP Request

Finally, what is the last DHCP packet that is sent to a device from a DHCP server?
- [x] DHCP ACK

<hr>

### OSI Model

#### **Task 1** &mdash; What is the OSI Model?

The OSI Model, stands for the **Open Systems Communication** _reference_ model. Reference model, being that it was never implemented in the real world, instead the **TCP/IP** model is being used. 

However, the OSI Model is a great way of presenting how data flows on a network. Take it as a guide as to how networks operate. Below is a table showcasing the OSI Model. Something to remember is that the OSI Model breaks downs the complex tasks of computer to computer communication in 7 layers and that layers 7 to 4 are know as the **Host Layers** and 3 to 1 the **Media Layers**.

What is important to take note of is that at every layer data travels through, a specific process takes place, where a piece of data is added. This process is known as **encapsulation**. Think of
it as, when a file _(or any data)_ is sent from one device to another, it doesn’t travel as-is.

Instead, as the data goes down the OSI layers _(from the application layer down to the physical layer)_, each layer adds its own “header” _(and sometimes a footer)_ with extra information.

This is like wrapping your data in several envelopes:
- Application layer → your message _(the raw data)_.
- Transport layer → adds port numbers _(so the right app gets it)_.
- Network layer → adds IP addresses _(so it knows where to go)_.
- Data link layer → adds MAC addresses and error-check info.
- Physical layer → turns it into electrical signals, light pulses, or radio waves.


#### OSI Model Table
|Data|Layer #|Layer Name|Phrase|
|:---|---:|:---|:---|
|**DATA**|_Host_ **7**|**Application Layer** <br> _Network Process to Application_|**A**way|
|**DATA**|_Host_ **6**|**Presentation Layer** <br> _Data Representation & Encryption_|**P**izza|
|**DATA**|_Host_ **5**|**Session Layer** <br> _Interhost Communication_|**S**ausage|
|**SEGMENT**|_Host_ **4**|**Transport Layer** <br> _End to End Connection & Reliability_|**T**hrow|
|**PACKET**|_Media_ **3**|**Network Layer** <br> _Path Determination & IP (Logical Addressing)_|**N**ot|
|**FRAME**|_Media_ **2**|**Data Link Layer** <br> _MAC and LLC (Physical Addressing)_|**D**o|
|**BIT**|_Media_ **1**|**Physical Layer** <br> _Media, Signal & Binary Transmissions_|**P**lease|

> 💡 **Note:** _There is a saying you can use to help remember the different layers within the OSI Model, that being, "**P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way"_.

Even though this is about the **OSI Model**, its good to know how the data would essentially flow from one device to another, then also taking a quick look at the **TCP/IP Model** and comparing that side by side with the OSI Model. 

Firstly, Lets look at how the OSI Model will flow if one device sent an email as an example to another. 

#### OSI Model Flow Example
|Computer #1||||Computer #2|
|:---:|:---:|:---:|:---:|:---:|
|Application Layer|&darr;||&uarr;|Application Layer|
|Presentation Layer|&darr;||&uarr;|Presentation Layer|
|Session Layer|&darr;||&uarr;|Session Layer|
|Transport Layer|&darr;||&uarr;|Transport Layer|
|Network Layer|&darr;||&uarr;|Network Layer|
|Data Link Layer|&darr;||&uarr;|Data Link Layer|
|Physical Layer|&rarr;|&rarr;|&rarr;|Physical Layer|


#### TCP/IP Model Table
Next is a quick look at the TCP/IP Model, which only consists of four layers and how both the OSI and TCP/IP models compare.

|Layers|
|:---|
|**Application** Layer <br> _FTP, NFS, SNMP, SMTP, HTTP, POP3_|
|**Transport** Layer <br> _TCP/UDP_|
|**Internet** Layer <br> _IP, ARP_|
|**Network Interface** Layer <br> _Ehternet, Token Ring_|

#### Model Comparison
|TCP/IP||OSI Model|
|:---|:---:|:---|
|**Application** Layer|&larr;|**• Application** Layer <br> **• Presentation** Layer <br> **• Session** Layer|
|**Transport** Layer|&larr;|**• Transport** Layer|
|**Internet** Layer|&larr;|**• Network** Layer|
|**Network Interface** Layer|&larr;|**• Data Link** Layer <br> **• Physical** Layer|

**Answer the questions below** <br>
What does the "OSI" in "OSI Model" stand for?
- [x] Open Systems Communication

How many layers (in digits) does the OSI model have?
- [x] 7

What is the key term for when pieces of information get added to data?
- [x] Encapsulation

<br>

#### **Task 2** &mdash;Layer 1 - Physical

This is the lowest layer in the model and the easiest to grasp, this layer references physical components of the hardware used in networking. The devices use electrical signals to transfer data between each other in a binary Numbering system (1's and 0's). An example of this can be Ethernet cables.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Physical

What is the name of the numbering system that is both 0's and 1's?
- [x] Binary

What is the name of the cables that are used to connect devices?
- [x] Ethernet Cables



<br>

#### **Task 3** &mdash;Layer 2 - Data Link

<br>

#### **Task 4** &mdash;Layer 3 - Network

<br>

#### **Task 5** &mdash;Layer 4 - Transport

<br>

#### **Task 6** &mdash;Layer 5 - Session

<br>

#### **Task 7** &mdash;Layer 6 - Presentation

<br>

#### **Task 8** &mdash;Layer 7 - Application

<br>


<hr>

### Packets & Frames

<hr>

### Extending your Network
