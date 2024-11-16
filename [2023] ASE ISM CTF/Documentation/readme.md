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
#### 0.1. Initial Setup - 🚩<kbd> flag{TesT_Fl@G} </kbd>🚩
---

## 1. Encoded
#### 1.1. TA TA TI TI TA - 🚩<kbd> 🚩ISMMASTERCURITY </kbd>🚩
- 📂Category: Encoded
- 🌐Official: https://ism.ase.ro/ctf/flag2.html
- ⚒️Tools: [Morse Code Translator](https://morsecode.world/international/translator.html), Chat GPT
- ⚔️Steps:
  	- Scan the QR Code -> Morse Code
  	- Chat GPT / Morse Code Translator
  	- Capture the Flag
---

#### 1.2. Simple App - 🚩<kbd> ISM_CTF_FLAG_IS_x1a </kbd>🚩
- 📂Category: Encoded
- 🌐Official: [ism_8d50e207f791ec66a2e4e1c851364715](https://ism.ase.ro/wp-content/uploads/2022/11/ism_8d50e207f791ec66a2e4e1c851364715.zip)
- ❓Hint: It’s all about strings / entity_iso_code”: “KP”
- ⚒️Tools:
- ⚔️Steps:
	- Download the .exe file.
 	- Detele the .exe extension -> Open the .txt file.
  	- Capture the Flag
---

#### 1.3. Quiz - 🚩<kbd> ctf21 </kbd>🚩
- 📂Category: Encoded
- 🌐Official: https://ism.ase.ro/ctf/flag2.html
- ⚒️Tools: CyberChef
- ⚔️Steps:
 	 - View Page Source -> function ascii_to_hexa(str)
 	 - CyberChef: On the number 6374663231 -> Apply From Hex (or Magic).
 	 - Capture the Flag
---

#### 1.4. Landscape 
- 📂Category: Encoded
- 🌐Official: http://ism.ase.ro/ctf/flag5.html
- ❓Hint: Do you see the image?
- ⚒️Tools:
- ⚔️Steps:
	- Download the landscape.png file

---

#### 1.5. Black Sheep
- 📂Category: Encoded
- 🌐Official: https://ism.ase.ro/ctf/flag8.html
- ❓Hint: Be strange or different / Which is different ?
- ⚒️Tools:
- ⚔️Steps:
  	- Downoad the .zip arhive -> Dezarchive -> Images 171 and 172 are different
---

#### 1.6. Apples - 🚩<kbd> ISM_HI </kbd>🚩
- 📂Category: Encoded
- 🌐Official: https://ism.ase.ro/ctf/flag7.html
- ❓Hint: The least one is Number One / The least significant bit
- ⚒️Tools: https://incoherency.co.uk/image-steganography/#unhide
- ⚔️Steps:
  	- Open the site Incoherency.co.uk -> Upload the image ->Unhide Image
  	- Capture the Flag
---

## 2. Web
#### 2.1. Hello World! - 🚩<kbd> ISM_FLAG_LETSSTART </kbd>🚩
- 📂Category: Web
- 🌐Official: https://ism.ase.ro/ctf/flag1.html
- ❓Hint:The source is the power
- ⚔️Steps:
	- Open the link -> View Page Source
 	- Capture the Flag
---

#### 2.2. Xerox - 🚩<kbd> ISM_FLAG_XEROXM </kbd>🚩
- 📂Category: Web
- 🌐Official: https://ism.ase.ro/ctf/flag3.php
- ❓Hint: Don’t be a brute, be smart / Defaults are valuable hints
- ⚔️Steps:
  	- Login: Username: admin / Password: 2222
  	- Capture the Flag
---

#### 2.3. Vlad
- 📂Category: Web
- 🌐Official: https://ism.ase.ro/wp-content/uploads/2022/11/file_6a91d5c13b99c7fd7fb04c68cf73eabd.zip
- ❓Hint: Extragi hash-ul arhivei (cu ce nu mai stiu, se gaseste pe net), faci o lista de posibile parole (sunt diverse programe pt asta, se gasesc pe net) si dupa folosind lista de parola spargi hash-ul cu hashcat sau johnTheRipper
- ⚒️Tools:
- ⚔️Steps:
	- Download the folder Arhive -> Extract Here
 	- Put the vlad.7z file and the vlad_run.py script in shared file.
  	- Open Kali Linux Machine
---

#### 2.4. The Beginning
---

## 3. Red Team CTF
#### 3.1. Jasons Cookies (JWT) - 🚩<kbd> ISMCTF{W34K_JWT_S3CR3T} </kbd>🚩
- 📂Category: Web
- 🌐Official:
- ❓Hint: Password: password123
---

#### 3.2. Path Finder 1
---

#### 3.3. Path Finder 2
---

#### 3.4. Path Finder 3
---

#### 3.5. Ping Pwn Party - 🚩<kbd> ISMCTF{l1br4ry-h1j4ck1ng-1s-c00l} </kbd>🚩
- 📂Category: Web
- 🌐Official:
- ❓Hint: Challenge de tip Command Injection
    - Comanda 'ping' folosita de protocolul ICMP, pentru a vedea daca poate comunica cu alte calculatoare dintr-o retea sau pe Internet.
- ⚔️Steps: 	1. Enter domain or IP adress: 127.0.0.1 -> Ping
---

#### 3.6. "Anonymous"?
---

#### 3.7. "Messages"
---

## 4. Network Capture
#### 4.1. Data Ninja Schemes (DNS - Wireshark) - 🚩<kbd> ISMCTF{L1K3_TH4T_DNS_3XF1L} </kbd>🚩
- 📂Category: Web
- 🌐Official:
- ❓Hint: Password zip file: ism_ctf_2023
---

#### 4.2. BabyShark
---

#### 4.3. Snake Files
---

## 5. Crypto
#### 5.1. Cookies - 🚩<kbd> ISM_THE_END </kbd>🚩
- 📂Category: Crypto
- 🌐Official: https://ism.ase.ro/ctf/flag10.php
- ⚒️Tools:[Decode.fr](https://www.dcode.fr/caesar-cipher)
- ⚔️Steps:
  	- Access the site: https://ism.ase.ro/ctf/flag10.php
  	- Right-Click -> Inspect -> Application -> Storage: Cookies: [https://ism.ase.ro](https://ism.ase.ro/)
  	- Name: Julius Caesar & Value:AOL%20MSHN%20PZ%20PZT_AOL_LUK -> Check: Show URL decoded: AOL MSHN PZ PZT_AOL_LUK
  	- Use Decode.fr -> Caesar Cipher Decoder: THE FLAG IS ISM_THE_END
  	- Capture the Flag
---

## 6. Reverse
#### 6.1. Notapdf
- Bitwise Operation Cipher (XOR)
- Magic Bytes - Semnatura Fisier
---
#### 6.2. Backup
---

## 7. Source Code
#### 7.1. SourceCodeSafari
---

## 8. Headache
#### 8.1. Flag X
---

#### 8.2. Flag Y
- Hint: LSB, Stegano, Decoder
---
