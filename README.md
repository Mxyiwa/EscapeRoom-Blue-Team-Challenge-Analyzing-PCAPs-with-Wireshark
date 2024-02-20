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
- <b>2. What attack type was used to gain access to the system? (one word)</b>
<b>ANS: Brute-force Attack</b>
- <b>3. What was the tool the attacker possibly used to perform this attack?</b>
<b>ANS: Hydra</b>
- <b>4. How many failed attempts were there?</b>
<b>ANS: There were 52 failed attempts.</b>
- <b>5. What credentials (username: password) were used to gain access? Refer to shadow.log and sudoers.log.</b>
<b>ANS: manager: forgot</b>
- <b>6. What other credentials (username: password) could have been used to gain access and also have SUDO privileges? Refer to shadow.log and sudoers.log.</b>
<b>ANS: sean: spectre</b>
- <b>7. What tool is used to download malicious files on the system?</b>
<b>ANS: Wget</b>
- <b>8. How many files did the attacker download to perform malware installation?</b>
<b>ANS: 3</b>
- <b>9. What is the main malware MD5 hash?</b>
<b>ANS: 772b620736b760c1d736b1e6ba2f885b</b>
- <b>10. What file has the script modified so the malware will start upon reboot?</b>
<b>ANS: /etc/rc.local</b>
- <b>11. Where did the malware keep local files?</b>
<b>ANS: /var/mail</b>
- <b>12. What is missing from ps.log?</b>
<b>ANS: /var/mail/mail</b>
- <b>13. What is the main file that was used to remove this information from ps.log?</b>
<b>ANS: sysmod.ko</b>
- <b>14. Inside the Main function, what is the function that causes requests to those servers?</b>
<b>ANS: requestFile</b>
- <b>15. One of the IPs the malware contacted starts with 17. Provide the full IP.</b>
<b>ANS: 174.129.57.253</b>
- <b>16. How many files did the malware request from external servers?</b>
<b>ANS: 9</b>
- <b>17. What are the commands that the malware was receiving from attacker servers? Format: comma-separated in alphabetical order</b>
<b>ANS: NOP, RUN</b>














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
