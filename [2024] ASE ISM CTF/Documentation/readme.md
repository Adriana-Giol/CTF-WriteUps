# [2024] ASE ISM CTF
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: ASE ISM
- 📅Date: 2024 October 23rd - 24th
- 💪Mode: Team
- 💻X challenges across X categories
- ⚒️Skills: Encoded, Web, Reverse, Crypto, Pass
- 🌐Official: [2024] https://atlas.ase.ro/ctf/
	- Register -> Mail Institutional: @stud.ase.ro
	- Registration Code: ISM-CTF-20231125
	- Login -> JoinTeam
- 🌐Official: [2022] https://ism.ase.ro/capture-the-flag-exercise/ism-ctf-2022-old/
---

## 0. Red Team Challenges Initialization
#### 0.1. Initial Setup - 🚩<kbd> flag{TesT_Fl@G} </kbd>🚩
---

## 1. Web
#### 1.1. INDEX.HTML - 🚩<kbd> FLAG{SourcePower@@ISMCTF} </kbd>🚩
- 📂Category: Web
- ⚔️Steps:
  	- Open the .zip file -> open index.html -> Developer Tools -> View Page Source
  	- Take the text from all of `document.write(' ')` and put together.
  	- Capture the Flag
---

## 2. Encoded
#### 2.1. QRCode - 🚩<kbd> FLAG{caesar##ISM_CTF} </kbd>🚩
- 📂Category: Encoded
- ⚒️Tools: [QR Code Scanner](https://webqr.com), [Decode.fr - Caesar Cipher](https://www.dcode.fr/caesar-cipher)
- ⚔️Steps:
  	- Use the QR Code Scanner and take the string.
  	- The string will be decrypted with Decode.fr (Caesar Cipher).
  	- Capture the Flag
---

## 3. Steganography
#### 3.1. Mr. Robot - 🚩<kbd>  </kbd>🚩
---

## 4. Crypto
#### 4.1. Web Secrets - 🚩<kbd>  </kbd>🚩
---
#### 4.2. TODO List - 🚩<kbd> FLAG{ISM_CTF_vin3g@r} </kbd>🚩
 📂Category: Crypto
- ⚒️Tools: [CyberChef - Vigenere Decode](https://webqr.com)
- ⚔️Steps:
  	- Open the index.html file -> Developer Tools -> View Page Source.
  	- In `document.cookie` we have the encrypted flag, and we have as hint `go to store to buy vinegar`.
  	- Use Cyber Chef - Vigenere Decode on `input = XEOX{MKF_QKJ_nbb3x@v}` and `key = store`.
  	- Capture the Flag.
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
#### 8.1. Meta Universe - 🚩<kbd> {ISMCTF1123abcd} </kbd>🚩
- 📂Category: Encoded
- ⚒️Tools: [Metadata2Go](https://www.metadata2go.com), [CyberChef - From Base64](https://cyberchef.org/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=ZTBsVFRVTlVSakV4TWpOaFltTmtmUT09)
- ⚔️Steps:
  	- Download the zip.
  	- Import all the 3 files in Metadata2Go.
  	- In the metdata of the second picture (A_breathtaking_coastal_landscape_featuring_towerin.jpg) can see a Base64 string.
  	- Put the Base64 string in CyberChef.
  	- Capture the Flag.
---
#### 8.2. LSB - 🚩<kbd>  </kbd>🚩
---

## 9. Vulnscan
#### 9.1. EXPLOIT IT - 🚩<kbd> 🚩ISMMASTERCURITY </kbd>🚩
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

## 10. Pwn
#### 10.1. Sumset - 🚩<kbd>  </kbd>🚩
---

## 11. Crypto
#### 11.1. How to Crypto v1 - 🚩<kbd>  </kbd>🚩
---
#### 11.2. How to Crypto v2 - 🚩<kbd> ISMCTF{W0uld_Y0U_l1k3_4_w13n34_w1th_Y0u4_m34l?__} </kbd>🚩
- 📂Category: Crypto
- ⚒️Tools: [Decode.fr - RSA Cipher Decoder](https://www.dcode.fr/rsa-cipher)
- ⚔️Steps:
  	- Take the number and put in in Decode.fr - RSA Cipher Decoder.
  	- Capture the Flag
---

#### 11.3. How to Crypto v3 - 🚩<kbd>  </kbd>🚩
---
#### 11.4. Cryptography Mastery - 🚩<kbd>  </kbd>🚩
---

## 12. Revere Engineering, Crypto
#### 12.1. Feisty Revenge - 🚩<kbd>  </kbd>🚩
---

## 13. Revere Engineering
#### 13.1. Feisty - 🚩<kbd> ISMCTF{L00k_a7_Y0u_r3V3r51ng_f31stel_N3tw0rk5}  </kbd>🚩
- 📂Category: Reverse Enginnering
- ⚒️Tools: [Cyber Chef - From Hex](https://cyberchef.org/#recipe=From_Hex('None')&input=NDk1MzRENDM1NDQ2N0I0QzMwMzA2QjVGNjEzNzVGNTkzMDc1NUY3MjMzNTYzMzcyMzUzMTZFNjc1RjY2MzMzMTczNzQ2NTZDNUY0RTMzNzQ3NzMwNzI2QjM1N0Q)
- ⚔️Steps:
  	- Take the number and put in in Cyber Chef - From Hex.
  	- Capture the Flag
---
#### 13.2. Reversing Mastery - 🚩<kbd>  </kbd>🚩
---


