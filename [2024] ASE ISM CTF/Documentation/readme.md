# [2024] ASE ISM CTF
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: ASE ISM
- 📅Date: 2024 October 23rd - 24th
- 💪Mode: Team
- 💻X challenges across X categories
- ⚒️Skills: Encoded, Web, Reverse, Crypto, Pass
- 🌐Official: [2024] 
- 🌐Official: [2023] https://atlas.ase.ro/ctf/
	- Register -> Mail Institutional: @stud.ase.ro
	- Registration Code: ISM-CTF-20231125
	- Login -> JoinTeam
- 🌐Official: [2022] https://ism.ase.ro/capture-the-flag-exercise/ism-ctf-2022-old/
---

## 0. Red Team Challenges Initialization
#### 0.1. Initial Setup - 🚩<kbd> flag{TesT_Fl@G} </kbd>🚩
---

## 1. Web
#### 1.1. INDEX.HTML - 🚩<kbd>  </kbd>🚩
---

## 2. Encoded
#### 2.1. QRCode - 🚩<kbd>  </kbd>🚩
---

## 3. Steganography
#### 3.1. Mr. Robot - 🚩<kbd>  </kbd>🚩
---

## 4. Crypto
#### 4.1. Web Secrets - 🚩<kbd>  </kbd>🚩
---
#### 4.2. TODO List - 🚩<kbd>  </kbd>🚩
---
#### 4.3. ASUS - 🚩<kbd>  </kbd>🚩
---

## 5. Recon
#### 5.1. Get Your File - 🚩<kbd>  </kbd>🚩
---
#### 5.2. R3c0N - 🚩<kbd>  </kbd>🚩
---

## 6. Forensics
#### 6.1. Capture The Intrusion - 🚩<kbd>  </kbd>🚩
---

## 7. Injection
#### 7.1. Admin is Here - 🚩<kbd>  </kbd>🚩
---
#### 7.2. Binary Exploitation - 🚩<kbd>  </kbd>🚩
---

## 8. Encoded
#### 8.1. Meta Universe - 🚩<kbd>  </kbd>🚩
---
#### 8.2. LSB - 🚩<kbd>  </kbd>🚩
---

## 9. Vulnscan
#### 9.1. EXPLOIT IT - 🚩<kbd>  </kbd>🚩
---

## 10. Pwn
#### 10.1. Sumset - 🚩<kbd>  </kbd>🚩
---
## 10. Reverse Engineering

#### 1.1. EXPLOIT IT - 🚩<kbd> 🚩ISMMASTERCURITY </kbd>🚩
- 📂Category: Vulnscan
- ⚒️Tools: Kali
- ⚔️Steps:
  	- Se pune fisierul de client.ovpn pe masina de Kali (Mode: Bridge Adapter)
  	- Se verifica daca merge netul :) `ping 10.1.5.102`
  	- Se scaneaza cu comanda  `nmap <10.1.5.102> -p-` <br>
  	  <img src = "https://github.com/Adriana-Giol/CTF-WriteUps/blob/main/%5B2024%5D%20ASE%20ISM%20CTF/Images/Exploit%20It-1.png" width = "auto" height="200px" align = "center"/> 
  	- Tot in Kali se deschide Firefox si se acceseaza `http://10.1.5.102:35622` si da click
  	-   <img src = "https://github.com/Adriana-Giol/CTF-WriteUps/blob/main/%5B2024%5D%20ASE%20ISM%20CTF/Images/Exploit%20It-2.png" width = "auto" height="200px" align = "center"/> 
  	- Se creaza fisierul exploit.sh cu fix codul care e aici https://www.exploit-db.com/exploits/50406
  	- Se face un targets.txt file in care sa fie scris doar  `http://10.1.5.102:35622`
  	- Se face fisierul exploit.sh executabil cu comanda `chmod +x ./exploit.sh`
  	- Se ruleaza comanda `sudo ./exploit.sh targets.txt /bin/sh  'cat /home/flag/flaguser’`
  	-   <img src = "https://github.com/Adriana-Giol/CTF-WriteUps/blob/main/%5B2024%5D%20ASE%20ISM%20CTF/Images/Exploit%20It-3.png" width = "auto" height="100px" align = "center"/> 
  	- Capture Th Flag
---
