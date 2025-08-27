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

#### **Task 2** &mdash; Layer 1 - Physical

This is the lowest layer in the model and the easiest to grasp, this layer references physical components of the hardware used in networking. The devices use electrical signals to transfer data between each other in a binary Numbering system (1's and 0's). An example of this can be Ethernet cables.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Physical

What is the name of the numbering system that is both 0's and 1's?
- [x] Binary

What is the name of the cables that are used to connect devices?
- [x] Ethernet Cables

<br>

#### **Task 3** &mdash; Layer 2 - Data Link

The Data Link Layer, focuses on the physical addressing of the transmission. It will receive a packet from the Network Layer, which includes the IP Address for the remote computer and will add in the Physical MAC Address of the receiving endpoint. Inside every network-enabled computer is a NIC, or Network Interface Card, which comes with a unique MAC Address to identify it.

MAC Addresses are set by the manufacturer and literally burnt into the card, hence why its like a fingerprint, it cannot be changed, It can however be spoofed. When information is sent across within the same Network (LAN), its actually the physical address that is used to identify where exactly to send the information even though the IP Address is still there. 

When you need to send data outside your LAN, the IP address is what identifies the correct destination network and host. In addition to the Data Link Layer, Its the job of the data link layer to present the data in a formation suitable for transmission.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Data Link

What is the name of the piece of hardware that all networked devices come with?
- [x] Network Interface Card

<br>

#### **Task 4** &mdash; Layer 3 - Network

This layer handles the routing and re-assembly of data. Routing simply determines the most optimal path the data should be sent. While some protocols determine the optimal path data should take to reach a device, we should only be aware of them at this stage. These protocols include OSPF, which stands for  Open Shortest Path First and RIP, Routing Information Protocol.

The factors by which a route is taken is determined by, what path is shortest, what path is the most reliable and which path has the faster physical connection.

As mentioned before, This layer deals with Ip Addresses such as 192.168.1.100, where as Layer 2 Data Link, deals with the physical MAC Address. Devices such as routers capable of delivering packets using IP Addresses are known as Layer 3 devices as they able to work with the third layer in the OSI Model.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Network

Will packets take the most optimal route across a network? (Y/N)
- [x] Y

What does the acronym "OSPF" stand for?
- [x] Open Shortest Path First

What does the acronym "RIP" stand for?
- [x] Routing Information Protocol

What type of addresses are dealt with at this layer?
- [x] IP Addresses

<br>

#### **Task 5** &mdash; Layer 4 - Transport

Layer 4 of the OSI Model transmits data across the network, when data is sent between devices, it follows one of two different protocols that are based upon several factors. These protocols are:

- TCP _Transmission Control Protocol_
- UDP _User Datagram Protocol_

TCP, or Transmission Control Protocol is designed with reliability and guarantee in mind. This means the protocol reserves a constant connection between the two devices for the amount of time it takes for the data to be sent and received. TCP also incorporates error checking into its design, this is how TCP can guarantee that data sent from the session layer has then been received and reassembled in the same order. 

TCP is used for situation such as File Sharing, Internet Browsing or Sending Emails, thus, because because these services require data to be accurate. Services such as streaming does not use TCP as a loss of data is simply pixels being lost, pixels also being a form of data.

#### Advantages of TCP:

- Guarantees the accuracy of data
- Capable of synchronizing two devices to prevent each other from being flooded with data.
- Performs a lot more processes for reliability.

#### Disadvantages of TCP:

- Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used.
- A slow connection can bottleneck another device as the connection will be reserved on the receiving computer the whole time.
- TCP is significantly slower than UDP because more work has to be done by the devices using this protocol.

UDP, or User Datagram Protocol is not as advanced as its brother TCP, there is no error checking, data sent using UDP, doesn't care if the data gets to its destination or not. There is also no synchronization between the devices.

#### Advantages of UDP:

- UDP is much faster than TCP.
- UDP leaves the application layer (user software) to decide if there is any control over how quickly packets are sent.
- UDP does not reserve a continuous connection on a device as TCP does.

#### Disadvantages of UDP:

- UDP doesn't care if the data is received.
- It is quite flexible to software developers in this sense.
- This means that unstable connections result in a terrible experience for the user.

UDP is useful in places where small pieces of data is being sent, an example being protocols used for discovering devices, ARP or DHCP or larger files such as video streaming.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Transport

What does TCP stand for?
- [x] Transmission Control Protocol

What does UDP stand for?
- [x] User Datagram Protocol

What protocol guarantees the accuracy of data?
- [x] TCP

What protocol doesn't care if data is received or not by the other device?
- [x] UDP

What protocol would an application such as an email client use?
- [x] TCP

What protocol would an application that downloads files use?
- [x] TCP

What protocol would an application that streams video use?
- [x] UDP

<br>

#### **Task 6** &mdash; Layer 5 - Session

Once data has been formatted from the presentation layer, the session layer will then begin to create and maintain the connection to other computers for which the data is destined. When a connection is established, so is a session created, whilst the connection is active, so is the session.

The session layer is also responsible for closing the connection if it hasn't been used in while or if lost. Sessions can also contain checkpoints, where if the data is lost, only the newest pieces of data are required to be sent, saving bandwidth.

Sessions are unique, data cannot travel over different sessions.

**Answer the questions below** <br>
What is the name of this layer?
- [x] Session

What is the technical term for when a connection is successfully established?
- [x] Session

<br>

#### **Task 7** &mdash; Layer 6 - Presentation

The Presentation layers is where standardization starts to take place, because software developers can develop any software such as an email client differently to another email client, the data still needs to be handled in the same way, it doesn't matter how the software works.

This layer acts as a translator for data to and from the application layer. The receiving computer will also understand the data being sent. An example being, when sending an email, another computer will also understand how to display that email.

Security features such as HTTPS occur at this layer.

**Answer the questions below** <br>
What is the name of this Layer?
- [x] Presentation

What is the main purpose that this Layer acts as?
- [x] Translator

<br>

#### **Task 8** &mdash; Layer 7 - Application

The application layer is the layer in which protocols and rules are in place to determine how the user should interact with data sent or received. This is the layer that we are most familiar with, that being the GUI, or Graphical User Interface, this layer also contain other layers such as the DNS layer, or Domain Name System.

What is the name of this Layer?
- [x] Application

What is the technical term that is given to the name of the software that users interact with?
- [x] Graphical User Interface

<hr>

### Packets & Frames

#### **Task 1** &mdash; What are Packets and Frames

Packets and frames are small pieces data that when formed togather make up a larger piece of data. However they are two different things within the OSI model. The Packet is from layer 3 or Network layer of the OSI Model, which contain information such as the IP Header and payload. A Frame is from the Data Link layer or Layer 2 of the OSI Model and this encapsulates the Packet adding more data such as the MAC Address.

Using the analogy of mailing a letter through the post, the envelope is the frame which is used to move the contents, in this case the packet to another place. Once the recepient opens the envelop or frame, they will know where to forward the letter or packet, itself. This is known as encapsulation.

Packets are an efficient way of sending data across networked devices, Because this data is exchanged in small pieces, there is less chance of bottlenecking occuring across a network than large messages being sent at once. An example of this is when loading an image from a website, this image is not sent to your computer as a whole, but rather small pieces where it is reconstructed when it reaches your computer.

Networking is full of standards and protocols that act as a set of rules for how the packet is handled on a device. Continuing with the internet protocol example, a packet using this protocol will have a set of headers that contain additional information to the daya that is being sent across a network.

|Header|Description|
|:---:|:---:|
|Time to Live (TTL)|Sets an expiry timer, so that the packet does not clog up your network if it doesnt reach the host or escapes|
|Checksum|Provies integrity checking for protocols such as TCP/IP. If any data is changed, this value will be different from what was expected and therefore corrupt.|
|Source Address|The IP Address of the device that the packet is being **from** so that data knows where to **return to**|
|Destination Address|The Devices IP address the packet is being sent to so that the data knows where to travel next|

**Answer the questions below** <br>
What is the name for a piece of data when it does have IP addressing information?
- [x] Packet

What is the name for a piece of data when it does not have IP addressing information?
- [x] Frame

<br>

#### **Task 2** &mdash; TCP/IP (The Three-Way Handshake)

We recently had a look at the TCP/IP Model/Protocol, this protocol is very similar to the OSI Model however it only consists of four layers and is arguably just a summed up version of the OSI Model.

#### TCP/IP Model/Protocol

|Layers|
|:---:|
|Application|
|Transport|
|Internet|
|Network Interface|

As data moves through the TCP/IP models layers, similar to the OSI model, data is **encapsulated**, the reverse of this is **decapsulation**. The defining feature of TCP/IP is that it is **connection-based**, this meaning that TCP establishes a connection between both a client and a device acting as a server **before** data is sent. Due to this, TCP guarentees that any data sent will be received on the other end. This process is known as the **Three-way Handshake**


TCP Packets contain various sections of information known as headers that are added from encapsulation.

|Header|Description|
|:---:|:---:|
|Source Port|This value is the port opened by the sender to send the TCP packet from. This value is chosen randomly (out of the ports from 0-65535 that aren't already in use at the time).|
|Destination Port|This value is the port number that an application or service is running on the remote host (the one receiving data); for example, a webserver running on port 80. Unlike the source port, this value is not chosen at random.|
|Source IP|This is the IP address of the device that is sending the packet.|
|Destination IP|	This is the IP address of the device that the packet is destined for.|
|Sequence Number|When a connection occurs, the first piece of data transmitted is given a random number. We'll explain this more in-depth further on.|
|Acknowledgement Number|After a piece of data has been given a sequence number, the number for the next piece of data will have the sequence number + 1. We'll also explain this more in-depth further on.|
|Checksum|This value is what gives TCP integrity. A mathematical calculation is made where the output is remembered. When the receiving device performs the mathematical calculation, the data must be corrupt if the output is different from what was sent.|
|Data|This header is where the data, i.e. bytes of a file that is being transmitted, is stored.|
|Flag|This header determines how the packet should be handled by either device during the handshake process. Specific flags will determine specific behaviours, which is what we'll come on to explain below.|

|Step|Message|Description|
|:---:|:---:|:---:|
|1|SYN|A SYN message is the initial packet sent by a client during the handshake. This packet is used to initiate a connection and synchronise the two devices together |
|2|SYN/ACK|This packet is sent by the receiving device (server) to acknowledge the synchronisation attempt from the client.|
|3|ACK|The acknowledgement packet can be used by either the client or server to acknowledge that a series of messages/packets have been successfully received.|
|4|DATA|Once a connection has been established, data (such as bytes of a file) is sent via the "DATA" message.|
|5|FIN|This packet is used to cleanly (properly) close the connection after it has been complete.|
|#|RST|This packet abruptly ends all communication. This is the last resort and indicates there was some problem during the process. For example, if the service or application is not working correctly, or the system has faults such as low resources. |

Any sent data is given a random number sequence and is reconstructed using this number sequence and incrementing by 1. Both computers must agree on the same number sequence for data to be sent in the correct order. This order is agreed upon during three steps:

1. SYN - Client: Here's my Initial Sequence Number(ISN) to SYNchronise with (0)
2. SYN/ACK - Server: Here's my Initial Sequence Number (ISN) to SYNchronise with (5,000), and I ACKnowledge your initial number sequence (0)
3. ACK - Client: I ACKnowledge your Initial Sequence Number (ISN) of (5,000), here is some data that is my ISN+1 (0 + 1)

|Device|Initial Number Sequence (ISN)|Final Number Sequence|
|:---:|:---:|:---:|
|Client (Sender)|0|0+1=1|
|Client (Sender)|1|1+1=2|
|Client (Sender)|2|2+1=3|

#### TCP Closing a Connection

TCP will close a connection once a device has determined that the other device has successfully received all of the data. Because TCP reserves system resources on a device, its best practice to close TCP Connections as soon as possible. To initiate a Closure of a TCP, the device will send a **FIN** packet to the other device, of course with TCP the other device will also have to acknowledge this packet.

**Answer the questions below** <br>
What is the header in a TCP packet that ensures the integrity of data?
- [x] Checksum

Provide the order of a normal Three-way handshake (with each step separated by a comma)
- [x] SYN,SYN/ACK,ACK

<br>

#### **Task 3** &mdash; Practical Handshake

This is a table version of the practical lab on THM, between to people called **Human TCP Connection**

Help Alice and Bob communicate by re-assembling the TCP handshake in the correct order in the static lab attached to this task!

|Alice|||Bob|
|:---:|:---:|:---:|:---:|
|SYN: Can you hear me Bob?|&rarr;|||
|||&larr;|SYN/ACK: Yes, I can hear you!|
|ACK: Okay Great|&rarr;|||
|DATA: Cheesecake on sale!|&rarr;|||
|||&larr;|ACK:I hear ya!|
|FIN/ACK: I'm all done|&rarr;|||
|||&larr;|FIN/ACK:Yeah, Me too!|
|ACK: Okay, Goodbye|&rarr;|||

**Answer the questions below** <br>
What is the value of the flag given at the end of the conversation?
- [x] THM{TCP_CHATTER}

<br>

#### **Task 4** &mdash; UDP/IP


The User Datagram Protocol, or UDP is a stateless protocol, meaning it doesnt do a Three-way hanshake, there is no synchronization between devices. UDP Is used in scenarios where losing data or connection is not an end all, such as video streaming or voice chat.

UDP Packets are simpler than that of TCP and thus has fewer headers as shown in the table below:

|Header|Description|
|:---:|:---:|
|Time to Live (TTL)|This field sets an expiry timer for the packet, so it doesn't clog up your network if it never manages to reach a host or escape!|
|Source Address|The IP address of the device that the packet is being sent from, so that data knows where to return to.|
|Destination Address|The device's IP address the packet is being sent to so that data knows where to travel next.|
|Source Port|This value is the port that is opened by the sender to send the UDP packet from. This value is randomly chosen (out of the ports from 0-65535 that aren't already in use at the time).|
|Destination Port|This value is the port number that an application or service is running on the remote host (the one receiving the data); for example, a webserver running on port 80. Unlike the source port, this value is not chosen at random.|
|Data|This header is where data, i.e. bytes of a file that is being transmitted, is stored.|

Headers not included here are **Sequence Number**, **Acknowledgement Number**, **Checksum** & **Flag**.

**Answer the questions below** <br>
What does the term "UDP" stand for?
- [x] User Datagram Protocol

What type of connection is "UDP"?
- [x] Stateless

What protocol would you use to transfer a file?
- [x] TCP

What protocol would you use to have a video call?
- [x] UDP

<br>

#### **Task 5** &mdash; Ports 101

Perhaps aptly titled by their name, ports are an essential point in which data can be exchanged. Think of a harbour and port. Ships wishing to dock at the harbour will have to go to a port compatible with the dimensions and the facilities located on the ship. When the ship lines up, it will connect to a port at the harbour. Take, for instance, that a cruise liner cannot dock at a port made for a fishing vessel and vice versa.

Ports enforce where what can park, networking devices also use ports to engorce strict rules when communicating with one another. When a connection has been has been established, and data sent or received will be sent through these ports. Ports can range from 0-65535.

Due to ports ranging to such a high number, there can run a risk of losing tracak of what application is using what port. Thankfully we associate application, software and behaviours with a standard set of rules. Meaning, enforcing that any web browser data is sent over port 80, Software Developers can design a web browser such as Google Chrome or Firefox to interpret the data the same way as one another. This means that all web browser now share a common rule.

While the stand rule for web data is port 80, there are a few other protocols that have been allocated a standard rule. Any port that is within 0 and 1024, is known as a common port.

|Protocol|Port Number|Description|
|:---:|:---:|:---:|
|File Transfer Protocol (FTP)|21|This protocol is used by a file-sharing application built on a client-server model, meaning you can download files from a central location.|
|Secure Shell (SSH)|22|	This protocol is used to securely login to systems via a text-based interface for management.|
|HyperText Transfer Protocol (HTTP)|80|This protocol powers the World Wide Web (WWW)! Your browser uses this to download text, images and videos of web pages.|
|HyperText Transfer Protocol Secure (HTTPS)|443|This protocol does the exact same as above; however, securely using encryption.|
|Server Message Block (SMB)|445|This protocol is similar to the File Transfer Protocol (FTP); however, as well as files, SMB allows you to share devices like printers.|
|Remote Desktop Protocol (RDP)|3389|This protocol is a secure means of logging in to a system using a visual desktop interface (as opposed to the text-based limitations of the SSH protocol).|

Even though these protocols follow a standard, you can administer applications that interact wth these protocols on a different port other than what is the standard, an example being you can run a web server on port 8080 instead of port 80. Note, however, applications will presume that the standard is being followed, so you will have to provide a colon (:) along with the port number.

<hr>

### Extending your Network

#### **Task 1** &mdash; Introduction to Port Forwarding

Port forwarding is essential for connecting applications and services to the internet. Without it, applications and services such as web servers are only available to devices within the same direct network, thus, known as the Intranet. Port forwarding opens specifics ports. Port forwarding is configured at the router of a network.

**Answer the questions below** <br>
What is the name of the device that is used to configure port forwarding?
- [x] Router

<br>

#### **Task 2** &mdash; Firewalls 101

A firewall is a device within a network responsible for determining what traffic is allowed to enter and exit. An Admin can configure a firewall to **Permit** or **Deny** traffic from entering or existing a network based on various factors such as:

- Where the traffic is coming from?
    - _Has the firewall been told to accept/deny traffic from a specific network?_
- Where is the traffic going to?
    - _Has the firewall been told to accept/deny traffic destined for a specific network?_
- What port is the traffic for?
    - Has the firewall been told to accept/deny traffic destined for port 80 only?
- What protocol is the traffic using?
    - _Has the firewall been told to accept/deny traffic that is UDP, TCP or both?_

Firewalls comes in all shapes and sizes, it ranges from dedicated hardware such as IPS or Intrusion Prevention Systems, to Software such as [Snort](https://www.snort.org/). Firewalls can be categorised into 2 to 5 categories.

The two primary categories are:

|Firewall Category|Description|
|:---:|:---:|
|Stateful|This type of firewall uses the entire information from a connection; rather than inspecting an individual packet, this firewall determines the behaviour of a device based upon the entire connection.

This firewall type consumes many resources in comparison to stateless firewalls as the decision making is dynamic. For example, a firewall could allow the first parts of a TCP handshake that would later fail.

If a connection from a host is bad, it will block the entire device.|
|Stateless|This firewall type uses a static set of rules to determine whether or not individual packets are acceptable or not. For example, a device sending a bad packet will not necessarily mean that the entire device is then blocked.

Whilst these firewalls use much fewer resources than alternatives, they are much dumber. For example, these firewalls are only effective as the rules that are defined within them. If a rule is not exactly matched, it is effectively useless.

However, these firewalls are great when receiving large amounts of traffic from a set of hosts (such as a Distributed Denial-of-Service attack)|

**Answer the questions below** <br>
What layers of the OSI model do firewalls operate at?

For this answer, just provide the numbers in ascending order, separated by an ampersand (&) I.e: 4 & 5
- [x] 3 & 4

What category of firewall inspects the entire connection?
- [x] Stateful

What category of firewall inspects individual packets?
- [x] Stateless

<br>

#### **Task 3** &mdash; Practical - Firewall

This is practical held on THM, no notes here apart from the answer to the question asked.

**Answer the questions below** <br>
What is the flag?
- [x] THM{FIREWALLS_RULE}

<br>

#### **Task 4** &mdash; VPN Basics

A VPN or Virtual Private Network is a technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the internet, this is known as a **tunnel**, devices connected within this tunnel form their own private network. A VPN can allow two offices to be connected.

VPN's allow networks in different geographical locations to be connected, they Offer Privacy and anonymity. VPN technology has improved, we can explore some existing technologies below:

|VPN Tacknology|Description|
|:---:|:---:|
|PPP|This technology is used by PPTP (explained below) to allow for authentication and provide encryption of data. VPNs work by using a private key and public certificate (similar to SSH). A private key & certificate must match for you to connect.

This technology is not capable of leaving a network by itself (non-routable).|
|PPTP|The Point-to-Point Tunneling Protocol (PPTP) is the technology that allows the data from PPP to travel and leave a network. 

PPTP is very easy to set up and is supported by most devices. It is, however, weakly encrypted in comparison to alternatives.|
|IPSec|Internet Protocol Security (IPsec) encrypts data using the existing Internet Protocol (IP) framework.

IPSec is difficult to set up in comparison to alternatives; however, if successful, it boasts strong encryption and is also supported on many devices.|

**Answer the questions below** <br>
What VPN technology only encrypts & provides the authentication of data?
- [x] PPP

What VPN technology uses the IP framework?
- [x] IPSec

<br>

#### **Task 5** &mdash; What is a Router?

Its a routers job to connect networks and pass data between them, it does this by using **routing**. Routing is the label given to the process of data travelling across networks. Routing involves creating a path between networks so that this data can be successfully delivered. Routing also determines the shortest path, remember **OSPF**.

There is more on this topic but its already been covered earlier, no need to repeat it.

**Answer the questions below** <br>
What is the verb for the action that a router does?
- [x] Routing

What are the two different layers of switches? Separate these by a comma I.e.: Layer X,Layer Y
- [x] Layer 2,Layer 3
