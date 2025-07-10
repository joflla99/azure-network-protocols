Azure Network Protocols
<p align="center"> <img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/> </p>
Network Security Groups (NSGs) and Traffic Inspection Between Azure Virtual Machines
This project explores how network traffic flows between Azure Virtual Machines (VMs) and how to inspect and control that traffic using Network Security Groups (NSGs) and Wireshark. It demonstrates how different protocols behave, how traffic is filtered, and how network security can be enforced in a cloud environment.

📺 Video Demonstration
YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups
(Link will take you to a demonstration of traffic inspection and NSG configurations in real time.)

🧰 Environments and Technologies Used
Microsoft Azure – Virtual Machines / Compute

Remote Desktop Protocol (RDP)

Command-Line Tools – ping, tracert, curl, etc.

Protocols Observed – SSH, RDP, DNS, HTTP/S, ICMP

Wireshark – Network protocol analyzer

🖥️ Operating Systems Used
Windows 10 (21H2)

Ubuntu Server 20.04

📝 High-Level Steps
Deploy Azure Virtual Machines (Ubuntu & Windows)

Configure NSGs to Allow/Block Traffic

Use Remote Desktop to Connect and Transfer Data

Capture and Analyze Traffic with Wireshark

🔍 Actions and Observations
📷 Network Traffic Capture Example
<img width="1324" height="787" alt="image" src="https://github.com/user-attachments/assets/259467ae-46c5-453a-b519-e94794005f44" />

In this section, various network protocols were triggered (e.g., ICMP, HTTP) between the VMs to observe how traffic appears in Wireshark. NSG rules were modified in real-time to test access control behavior.

📷 NSG Rule Adjustment and Testing
<img width="760" height="678" alt="image" src="https://github.com/user-attachments/assets/6e94fab2-7ef3-4f3e-a27c-20fd35231a0f" />

As NSG inbound and outbound rules were updated, we validated changes by re-initiating connections (e.g., blocked SSH vs. allowed RDP). The impact was immediately visible through both failed connections and packet drops in Wireshark.

📷 Final Capture and Summary
<img width="1884" height="889" alt="image" src="https://github.com/user-attachments/assets/a3ff2b0e-36d5-4853-aedc-ec050b4396be" />

A summary capture demonstrates how NSGs can effectively restrict unauthorized traffic. Logs and packet details show protocol types, source/destination IPs, ports, and behavior before/after rule changes.

✅ Summary
This lab provided hands-on experience with:

Deploying and connecting Azure VMs across platforms

Capturing network traffic to understand protocol behavior

Modifying NSGs to control traffic flow and security

Using Wireshark for deep traffic inspection and validation
