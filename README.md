<h1>jordans Nmap 👨🏿‍💻</h1>

<h2>Description</h2>
Project consists of a simple exercise on how nmap works  
<br />


<h2>tools Used</h2>

- <b>nmap🌎, metasploit framwork 🛡️</b> 

<h2>Environments Used </h2>

- <b>linux</b> 

<h2>nmap walk-through:</h2>

<p align="center">
check systems are alive: <br/>
<img src="https://github.com/user-attachments/assets/6628b572-19bf-4b9a-8101-e14b5c62f2b3"/> 
in this image i am checking the for comnticatons between devices using ifconfig and nmap -sP.ifconfig helps you determine your devices IP address,subnet mask and network interface detailes.
  using nmap -sP (ping scan) option helps check if other devices are connected to the same network by sending ICMP echo requests. 
<br />
<br />
scanning specific ports using Nmap -sS -p 80,443:  <br/>
<img src="https://github.com/user-attachments/assets/acdaa1f8-fab8-4735-9743-b67ccb305bb2"/> 
in this image it shows that i am doing a stealthy scan (SYN) on ports 80(HTTP) and 443 (HTTPS) of the target system.
-sS sends SYN packest to the target without completing the TCP handshake.in this case the port is closed and reponds with reset RST  
<br />
<br />
meta-slpoit frameworks openssh script: <br/>
<img src="https://github.com/user-attachments/assets/34e93314-6eca-4b38-95f7-9dbfc296e855"/> 
in this image it shows me using metasploit framework to search for openSSH exploits. 
<br />
<br />
openSSH script in use, nmap -TS -A -Y :  <br/>
<img src="https://github.com/user-attachments/assets/249f4f4a-0a33-4042-b9aa-03a5e3b242af"/> 
in this image we i am using ssh brute to test for potentail vulnerabilities in the second command ran (-T5 -A -oX) provides an aggressive and detalied scan with a structred output 
 <br />
<br />
namp vuln script:  <br/>
<img src="https://github.com/user-attachments/assets/4055bb35-5848-4305-bd7a-2f35360e335d"/> 
in this image i am using another script for port 80 vlunerbilities. nmap scans thet targed web server and checks for security issues 
 <br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
