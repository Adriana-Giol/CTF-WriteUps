# [2024] Hack the Box - Hack The Boo 2024 - Practice
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: **Hack the Box**
- 📅Date: 2024 October 21st - 26th
- 💪Mode: Individual
- 💻15 challenges across 5 categories
- ⚒️ Skills: Reversing, Crypto, Coding, Web, Forensics
- 🌐 Official: https://ctf.hackthebox.com/event/1811
---

## 1. Reversing
### 1.1. Grave Robber - 🚩<kbd>HTB{br34k1n9_d0wn_th3_sysc4ll5} </kbd>
- 📂Category: Reversing - ELF Files
	- ELF is short for Executable and Linkable Format. It's a format used for storing binaries, libraries, and core dumps on disks in Linux and Unix-based systems.
- ⚒️Tools: VirtualBox, Kali VM
- ⛑️Help: [CTF Time](https://ctftime.org/writeup/26531)
- ⚔️Steps: 
	- Download the File (File Name: robber)
	- Open Virtual Box -> Kali Virtual Machine -> Place the file in Shared folder
	- In the terminal, navigate to the file path, then enter the following commands:
		- `cat roober` -  display the contents of files 
	- Capture the Flag
---

### 1.2. Crypt Of The Undead - 🚩<kbd> </kbd>
---

### 1.3. Spooky Pass - 🚩<kbd> HTB{un0bfu5c4t3d_5tr1ng5} </kbd>
- 📂Category: Reversing - ELF Files
	- ELF is short for Executable and Linkable Format. It's a format used for storing binaries, libraries, and core dumps on disks in Linux and Unix-based systems. 
- ⚒️Tools: VirtualBox, Kali VM
- ⛑️Help: [[Writeup Medium] TryHackMe: Reversing ELF](https://medium.com/@xiosec/tryhackme-reversing-elf-60ab96969e41)
- ⚔️Steps: 
	- Download the File (File Name: pass)
	- Open Virtual Box -> Kali Virtual Machine -> Place the file in Shared folder
	- In the terminal, navigate to the file path, then enter the following commands:
		- `file ./pass ` - returns information about file format and type.
		- `chmod +x pass` - add execute permission for the specified file
		- `./pass` - execute the file
  		- password: s3cr3t_p455_f0r_gh05t5_4nd_gh0ul5 (Open the file in Notepad -> The password is in plaintext)
	- Capture the Flag
---

## 2. Crypto
#### 2.1. Sugar Free Candies - 🚩<kbd> </kbd>
---
#### 2.2. Sekur Julius - 🚩<kbd>HTB{SECURITYOFATHOUSANDORSECURITYOFASINGLE} </kbd>
- 📂Category:Cryptography - Julius Caesar Cipher
- ⚒️Tools: [CrypTool](https://www.cryptool.org/en/ct2/downloads/) / [Cryptii](https://cryptii.com/pipes/caesar-cipher) / [Decode.fr](https://www.dcode.fr/caesar-cipher)
- ⚔️Steps: 
	- Download the Files (Files Name: output.txt, source.py)
	- Since the code in the file `source.py` shifts the letters in the same way as the Caesar Cipher, and the function is named julius_encrypt, we assume that the cipher used for encryption was the Julius Caesar Cipher. We use CrypTool to decrypt the code, and because the number of shifts in the source code is random, we will try multiple variations. We have determined that the number of shifts is 15.
	- Decrypted Text: WELCOMETOHACKTHEBOOTWOTHOUSANDTWENTYFOURTHISISAPROOFOFCONCEPTTOPROVEYOUTHATTHECAESARCIPHERISINSECURENOMATTERHOWMANYTIMESYOUAPPLYITTHESECURITYOFATHOUSANDDISTINCTSHIFTSISEVENTUALLYTHESAMEASTHATOFASINGLESHIFTENOUGHMUMBLINGTAKEYOURFLAGANDENJOYTHERESTOFTHECONTESTMAKESUREYOUWRAPTHEFOLLOWINGTEXTWITHTHEHTBFLAGFORMATSECURITYOFATHOUSANDORSECURITYOFASINGLE
	- Capture the Flag
---

#### 2.3. Brevi Moduli - 🚩<kbd> </kbd>
---
## 3. Coding
#### 3.1. Reversal - 🚩<kbd> </kbd>
#### 3.2. Addition - 🚩<kbd> </kbd>
#### 3.3. Oddly Even - 🚩<kbd> </kbd>
---
## 4. Web
#### 4.1. Phantom's Script - 🚩<kbd>  </kbd>
#### 4.2. Void Whispers - 🚩<kbd>  </kbd>
#### 4.3. Unholy Union - 🚩<kbd>  </kbd>
---
## 5. Forensisc
#### 5.1. Spooky Theme - 🚩<kbd>  </kbd>
#### 5.2. The Shortcut Haunting - 🚩<kbd>  </kbd>
#### 5.3. Forbidden Manuscript - 🚩<kbd>  </kbd>
---
---
