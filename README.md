<h1>Building a Virtual Private Cloud (VPC)</h1>

This repository contains a walkthrough in building a Virtual Private Cloud (VPC) in AWS. 

Resources used:
- VPC

Region: us-west-2 (Oregon)

<h1>Objectives</h1>
The project aims to:
<ul>
  <li>Create an Amazon VPC</li>
  <li>Create a publc subnet</li>
  <li>Create an Internet Gateway</li>
</ul>
  <img src="AWS VPC/Architecture.jpg" alt="Architecture">

<h2>Stage 1: Create VPC</h2>
<p>A Virtual Private Cloud (VPC) in AWS (Amazon Web Services) is a logically isolated section of the AWS cloud where you can launch AWS resources, like EC2 instances, in a virtual network that you define. It gives you control over your virtual networking environment, including the selection of your IP address range, creation of subnets, and configuration of route tables and network gateways.<br><br>

  <img src="AWS VPC/VPC Creation.jpg" alt="VPC">
  
<h2>Stage 2: Create a Public Subnet</h2>
A subnet (short for "subnetwork") is a segment of a Virtual Private Cloud (VPC) in AWS that allows you to partition the VPC's IP address range into smaller, more manageable sections. Each subnet resides in a specific Availability Zone (AZ) within a VPC, and you can use it to organize and control the network flow for your resources, such as EC2 instances.
<br><br>
Subnet Creation process:
<li>Select VPC ID</li>
<li>Set up Subnet name</li>
<li>Select Availability Zone</li>
<li>Select VPC and subnet CIDR Block</li>
<li>Since this is a public subnet, we may enable auto-assign public IPv4 address.</li>
  <img src="AWS VPC/Subnet.jpg" alt="Subnet">

<h2>Stage 3: Create an Internet Gateway</h2>
An Internet Gateway (IGW) in AWS is a horizontally scaled, redundant, and highly available VPC component that allows communication between resources in your Virtual Private Cloud (VPC) and the internet. It serves as a bridge between your VPC and the internet, enabling your instances to receive inbound traffic from the internet and send outbound traffic to the internet.
Internet Gatewat creation process:
<li>Input Name tag</li>
<li>Attach the newly created Internet Gateway to the VPC</li>

  <img src="AWS VPC/Internet Gateway.jpg" alt="IAM user">

<h3>## Credits ##</h3>
Project was originally authored by <a href="https://community.nextwork.org/home">Nextwork</a>.
