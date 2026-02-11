<h1>pfSense Firewall Home Lab</h1>

<h2>Description</h2>
This project was created to simulate a real world firewall environment using <b>pfSense</b> inside <b>VirtualBox</b>. The goal was to gain hands on experience with WAN vs LAN segmentation, firewall rule creation, traffic monitoring, and blocking malicious activity, similar to how perimeter defense works in real enterprise networks. <br /> <br />
To accomplish this, I deployed a <b>pfSense firewall</b> VM with two network interfaces (<b>WAN</b> and <b>LAN</b>), connected an internal <b>Ubuntu</b> machine on the LAN, and used <b>Kali Linux</b> on the WAN side to simulate an attacker. I then generated malicious traffic (SYN flood), observed it in packet captures, blocked it using pfSense firewall rules, and verified the results through logs and traffic reduction.

<br />

<h2>Tools and Technologies Used</h2>
<b>pfSense</b> <br />
<b>Oracle VirtualBox</b> <br />
<b>Kali Linux</b> <br />
<b>Ubuntu Desktop</b> <br />
<b>Wireshark</b> <br />
<b>hping3</b> <br />

<h2>Environments Used</h2>
<b>pfSense VM</b> (Firewall / Router) <br />
<b>Ubuntu VM</b> (Internal LAN Endpoint) <br />
<b>Kali Linux VM</b> (External WAN Attacker) <br />

<h2>Project Overview</h2>
This project focused on: <br />
Configuring pfSense WAN and LAN interfaces in VirtualBox <br />
Enabling access to the pfSense Web GUI and validating connectivity <br />
Setting up DHCP on the LAN interface so internal devices receive an IP automatically <br />
Testing internal connectivity with ping and DNS to confirm routing works <br />
Simulating an external attack from Kali (TCP SYN flood using hping3) <br />
Monitoring traffic on Ubuntu using Wireshark to confirm the attack is visible <br />
Creating a pfSense firewall rule to block malicious WAN traffic (with logging enabled) <br />
Verifying the block worked using pfSense firewall logs and reduced traffic in Wireshark <br />

<h2>Key Takeaways</h2>
Gained hands on experience setting up a firewall with WAN vs LAN segmentation <br />
Learned how to create allow/block rules and see the impact immediately <br />
Observed what a SYN flood attack looks like in Wireshark packet captures <br />
Practiced using pfSense firewall logs to validate blocked traffic and rule effectiveness <br />
Improved understanding of basic network defense and perimeter firewall concepts <br />

<h2>Disclaimer</h2>
⚠️ This project was completed in a lab environment for educational purposes only. All systems were virtualized and isolated from production networks.

<h2>Documentation</h2>
A full step by step walkthrough of the lab setup, pfSense configuration, attack simulation, rule creation, testing steps, and screenshots is documented and attached to this repository.
<a href="https://docs.google.com/document/d/1StgSRTYsTPF1fkkwZLgZyu8t2A--2D47A08nV3w0b7M/edit?usp=sharing">pfSense Firewall setup</a>
