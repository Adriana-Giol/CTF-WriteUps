# [2023] ASE ISM CTF
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: ASE ISM
- 📅Date: 2023 October 25th - 26th
- 💪Mode: Team
- 💻X challenges across X categories
- ⚒️Skills: Encoded, Web, Reverse, Crypto, Pass
- 🌐Official: [2022] https://ism.ase.ro/capture-the-flag-exercise/ism-ctf-2022-old/
- 🌐Official: [2023] https://atlas.ase.ro/ctf
	- Register -> Mail Institutional: @stud.ase.ro
	- Registration Code: ISM-CTF-20231125
	- Login -> JoinTeam
---

## 0. Red Team Challenges
#### 0.1. Initial Setup - 🚩<kbd> flag{TesT_Fl@G} </kbd>
---

## 1. Encoded
#### 1.1. TA TA TI TI TA - 🚩<kbd> ISMMASTERCURITY </kbd>
	- Official: https://ism.ase.ro/ctf/flag2.html
	- Tools: [Morse Code Translator](https://morsecode.world/international/translator.html), Chat GPT
	- Steps: 
		1. Scan the QR Code -> Morse Code
		2. Chat GPT / Morse Code Translator
		3. Capture the Flag
---
#### 1.2. Simple App - 🚩<kbd>ISM_CTF_FLAG_IS_x1a  </kbd>
	- Official: ism_8d50e207f791ec66a2e4e1c851364715
	- Hint: It’s all about strings / entity_iso_code”: “KP”
	- Steps:
		1. Download the .exe file.
		2. Detele the .exe extension -> Open the .txt file.
		3. Capture the Flag
---
#### 1.3. Quiz - 🚩<kbd> ctf21  </kbd>
	- Official: https://ism.ase.ro/ctf/flag2.html
	- Steps: 
		1. View Page Source -> function ascii_to_hexa(str)
		2. CyberChef: On the number 6374663231 -> Apply From Hex (or Magic).
		3. Capture the Flag
---
#### 1.4. Landscape - 🚩<kbd>  </kbd>
	- Official: http://ism.ase.ro/ctf/flag5.html
	- Hint: Do you see the image ?
	- Steps:
		1. Download the landscape.png file
		2. 
---
#### 1.5. Black Sheep - 🚩<kbd>  </kbd>
	- Official: https://ism.ase.ro/ctf/flag8.html
	- Hint: Be strange or different / Which is different ?
	- Tools: 
	- Steps:
		1. Downoad the .zip arhive -> Dezarchive -> Images 171 and 172 are different
		2. 
---
#### 1.6. Apples - 🚩<kbd> ISM_HI </kbd>
	- Official: https://ism.ase.ro/ctf/flag7.html
	- Hint: The least one is Number One / The least significant bit
	- Tools: https://incoherency.co.uk/image-steganography/#unhide
	- Steps:
		1. Open the site Incoherency.co.uk -> Upload the image ->Unhide Image
		2. Capture the Flag
---


## 2. Web
#### 2.1. Hello World! - 🚩<kbd> ISM_FLAG_LETSSTART  </kbd>
	- Official: https://ism.ase.ro/ctf/flag1.html
	- Hint: The source is the power
	- Steps:
		1. Open the link -> View Page Source
		2. Capture the Flag
---	
#### 2.2. Xerox - 🚩<kbd> ISM_FLAG_XEROXM </kbd>
	- Official: https://ism.ase.ro/ctf/flag3.php
	- Hint: Don’t be a brute, be smart / Defaults are valuable hints
	- Steps:
		1. Login: Username: admin  / Password: 2222
		2. Capture the Flag
---
#### 2.3. Vlad
	- Steps: 
		1. Download the folder Arhive -> Extract Here
		2. Put the vlad.7z file and the vlad_run.py script in shared file.
		3. Open Kali Linux Machine 
#### 2.4. The Beginning
---


## 3. Red Team CTF [Teo + Luca Stefan] 
#### 3.1. Jasons Cookies (JWT)- 🚩<kbd> ISMCTF{W34K_JWT_S3CR3T} </kbd>
	- Password: password123
#### 3.2. Path Finder 1 - 🚩<kbd>  </kbd>
#### 3.3. Path Finder 2 - 🚩<kbd>  </kbd>
#### 3.4. Path Finder 3 - 🚩<kbd>  </kbd>
#### 3.5. Ping Pwn Party - 🚩<kbd> ISMCTF{l1br4ry-h1j4ck1ng-1s-c00l} </kbd>
	- Hint: Challenge de tip Command Injection
		- Comanda 'ping' folosita de protocolul ICMP, pentru a vedea daca poate comunica cu alte calculatoare dintr-o retea sau pe Internet.
	- Steps:
		1. Enter domain or IP adress: 127.0.0.1 -> Ping
#### 3.6. "Anonymous"?
#### 3.7. "Messages"
---


## 4. Network Capture
#### 4.1. Data Ninja Schemes (DNS - Wireshark)- 🚩<kbd> ISMCTF{L1K3_TH4T_DNS_3XF1L} </kbd>
	- Password zip file: ism_ctf_2023
#### 4.2. BabyShark
#### 4.3. Snake Files
---

## 5. Crypto
#### 5.1. Cookies - 🚩<kbd> ISM_THE_END  </kbd>
	- Official: https://ism.ase.ro/ctf/flag10.php
	- Tools:[Decode.fr](https://www.dcode.fr/caesar-cipher)
	- Steps:
		1. Access the site: https://ism.ase.ro/ctf/flag10.php
		2. Right-Click -> Inspect -> Application -> Storage: Cookies: https://ism.ase.ro
		3. Name: Julius Caesar & Value:AOL%20MSHN%20PZ%20PZT_AOL_LUK -> Check: Show URL decoded: AOL MSHN PZ PZT_AOL_LUK
		4. Use Decode.fr -> Caesar Cipher Decoder: THE FLAG IS ISM_THE_END
		5. Capture the Flag 
		
---

## 6. Reverse
#### 6.1. Notapdf - 🚩<kbd>  </kbd>
	- Bitwise Operation Cipher (XOR)
	- Magic Bytes - Semnatura Fisier
#### 6.2. Backup
---


## 7. Source Code
#### 7.1. SourceCodeSafari  - 🚩<kbd>  </kbd>


## 8. Headache
#### 8.1. Flag X  - 🚩<kbd>  </kbd>
#### 8.2. Flag Y  - 🚩<kbd>  </kbd>
	- Hint: LSB, Stegano, Decoder
---
---
TOTAL: 26 / 35
