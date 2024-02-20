<h1>EscapeRoom Blue Team Challenge — Analyzing PCAPs with Wireshark</h1>

<h2>Description</h2>
<b>
 This lab is the walkthrough of my approach to solving the “EscapeRoom” CTF by The Honeynet Project on the Cyberdefenders website. The goal is to perform a series of analyses of the PCAP files provided by the Cyberdefenders platform and answer a series of questions about my analysis.
</b>

## Challenge Scenario
<b>As a SOC Analyst, you are part of a company that specialises in hosting web applications through KVM-based Virtual Machines. Over the weekend, one of the Virtual Machines went down, and the site administrators began to panic as they feared this might be the result of malicious activity. They were able to extract a few logs from the compromised environment in hopes that you could investigate and determine what happened.
</b>
<br />

<h2>Link to hands on step-by-step guide on how to perform this project</h2>

- <b>https://medium.com/@muyiwafadare/escaperoom-blue-team-challenge-analyzing-pcaps-with-wireshark-648d6b57a0c4</b>


## Technologies & OS Used

- <b>MacOS {Host Device}</b>
- <b>Parallels VM</b>
- <b>Kali Linux</b>
- <b>Wireshark</b>
- <b>Ghidra</b>
- <b>ZUI (Brim Security)</b>
- <b>UPX (Ultimate Packer for eXecutables)</b>

## Challenge Questions with Answers

- <b>1. What service did the attacker use to gain access to the system?</b>
<b>ANS: SSH</b>


<h2>Attacks from Luxembourg, Germany and, Belgium coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://imgpile.com/images/hoXc8X.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 5 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://imgpile.com/images/hoXba3.png" height="100%" width="100%" alt="Image Analysis Dataflow"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
