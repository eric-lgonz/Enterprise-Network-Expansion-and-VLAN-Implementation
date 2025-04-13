# Enterprise-Network-Expansion-and-VLAN-Implementation

In this project, I will demonstrate how to:

- Integrate a new switch block into an existing enterprise network using Cisco Packet Tracer, simulating
real-world brownfield network expansion
- Configure VLANs, trunks, Layer 3 routing, SVIs, EtherChannel, and first-hop redundancy protocols to support
resilient network growth
- Apply the access-distribution-core design model to optimize performance, scalability, and manageability in a
multi-layer enterprise environment

This project will be split into 6 parts, with each section focusing on a different phase of the enterprise network upgrade to keep things organized and easy to follow.

<h2>Technologies Used</h2>

- <a href="https://www.netacad.com/cisco-packet-tracer"> Cisco Packet Tracer<a/> (version 8.2.2)

<h2>What is Cisco Packet Tracer?</h2>

<a href="https://www.netacad.com/cisco-packet-tracer"> Cisco Packet Tracer<a/> is a comprehensive, widely used, and free network simulation software tool. It enables users to design, configure, and troubleshoot network topologies without the need for physical hardware. Cisco packet tracer offers realistic simulation and visualization for modern computer networks, making it ideal for simulating both greenfield and brownfield computer network environments. Feel free to check out their <a href="https://www.netacad.com/cisco-packet-tracer"> website<a/> for more information about Cisco Packet Tracer and its capabilities.

<h1>Part 1: Basic Ethernet and IP Networking</h1>

In this section, we will be starting off with the existing network topology below and will be adding the two LANs highlighted in blue.

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%201.png">

Let's start by setting up the devices, configuring their cabling and IP addressing. Then we can make sure the connections work by pinging the devices.

<h2>Device Setup</h2>

Some of the devices need their power supply to be set up before connecting them, such as the multilayer switches and the IP phone. We can connect each multilayer switch to power by clicking on the device, and then dragging the AC power adapter to them:

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%202.png">
<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%203.png">

We can do the same for the IP phone:

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%204.png">
<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%205.png">

<h2>Cabling</h2>

Now let's connect all the devices together with cables, except for the laptops, those will have a wireless connection. I will be using copper straight-through cables for connections between different kinds of devices (pc to switch), and copper cross-over cables for similar devices (switch to switch). To demonstrate how to connect the cables, here's how to set up the connection between PC0 and Switch0:

First click the connections icon on the bottom (the lightning bolt), and select on the type of cable you want to use:

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%206.png">
<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%207.png">

Then bring the cable to your starting device, choose the port to connect it on, and then do the same for the device with the other end of the cable:

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%208.png">
<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%209.png">

Afterwords, the connection will look like this:

<img src = "https://github.com/eric-lgonz/Enterprise-Network-Expansion-and-VLAN-Implementation/blob/main/assets/Part%201%20-%2010.png">

I will be configuring the rest of the connections according to this table:



After all of the cabling, this is how my topology should look:

_insert image_

<h2>IP Addressing</h2>

<h2>Verifying Connections</h2>
