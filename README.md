

<p align="center">

![WireShark](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/20c4b0a9-bf01-4bad-b4e2-6aa19385ae9a)

</p>

<h1>Inspect-network-traffic</h1>
This tutorial outlines how Wireshark uses OSI layers to break down packets and how to use these layers for analysis..<br />


<h2>Technology Used</h2>

- WireShark v3.2.3


<h2>Operating Systems Used </h2>

- Ubuntu

<h2>High-Level Deployment and Configuration Steps</h2>

- Open PCAP file
- Packet dissection
  

<h2>Importing File and Dissection Steps</h2>

<p>

![Screen Shot 2024-04-17 at 8 15 34 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/14d79504-51c4-45f8-b029-f2930713fdc2)
/p>
<p>
Initially I loaded a packet capture (PCAP) file.
</p>
<br />

<p>

![Screen Shot 2024-04-17 at 8 46 25 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/06529648-5c67-4cee-b664-c373d941cc4e)

</p>
<p>
Packets consist of 5 to 7 layers based on the OSI model. I selected an HTTP packet to dissect. The Frame (Layer 1): This will show you what frame/packet you are looking at and details specific to the Physical layer of the OSI model.
</p>
<br />

<p>

![Screen Shot 2024-04-17 at 8 52 14 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/ebd6b3db-6532-4f4d-82e2-6c86b83f30fe)

</p>

<p>
Source [MAC] (Layer 2): This will show you the source and destination MAC Addresses; from the Data Link layer of the OSI model.
</p>
<br />
</p>

![Screen Shot 2024-04-17 at 8 55 17 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/fc6b01ea-ecd7-4e3f-83dc-b07b05654f26)

</p>
<p>

Source [IP] (Layer 3): This will show you the source and destination IPv4 Addresses; from the Network layer of the OSI model.
</p>
<br />
</p>

![Screen Shot 2024-04-17 at 8 58 10 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/5e905e1e-3017-490a-b10f-44c0f3dbfdb9)
</p>
<p>

Protocol (Layer 4): This will show you details of the protocol used (UDP/TCP) and source and destination ports; from the Transport layer of the OSI model.

</p>
<br />

<p>

![Screen Shot 2024-04-17 at 9 05 38 PM](https://github.com/kennyfrantz/Inspect-network-traffic/assets/163783743/abd7ceae-ccbb-47f7-b28a-ba869965a1cf)

</p>
<p>

Application Protocol (Layer 5): This will show details specific to the protocol used, such as HTTP, FTP,  and SMB. From the Application layer of the OSI model.
