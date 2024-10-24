# [2024] Hack the Box - Hack The Boo 2024 - Practice
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: **Hack the Box**
- 📅Date: 2024 October 21st - 26th
- 💪Mode: Individual
- 💻18 challenges across 6 categories
- ⚒️ Skills: Reversing, Crypto, Coding, Web, Forensics, Pwn
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

### 1.2. Crypt Of The Undead - 🚩<kbd> HTB{und01ng_th3_curs3_0f_und34th} </kbd>
- 📂Category: Reversing - ELF Files
- ⚒️Tools: VirtualBox, Kali VM
- ⚔️Steps: 
	- Download the File (Files Name: crypt, flag.txt.undead)
 	- Remove the `.undead` extension from the encrypted file. 
	- Open Virtual Box -> Kali Virtual Machine -> Place the file in Shared folder
	- In the terminal, navigate to the file path, then enter the following commands:
		- `file ./crypt ` - returns information about file format and type.
		- `chmod +x crypt` - add execute permission for the specified file
		- `./crypt flag.txt` - execute the file
  		- The flag will be find in the flag.txt.undead 
	- Capture the Flag
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
#### 3.1. Reversal - 🚩<kbd>HTB{r3VerS4l?_wElL_1_n3vEr_6b7f117b380e3074d93a2bfe86e932ff} </kbd>
- 📂Category: Coding - Python
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser
 	- The code to reverse a string is:
	```
 	# take in the string
	n = input()
	
	# calculate answer
	answer = n[::-1]  # reverse the string
	
	# print answer
	print(answer)
 	```
 	- Capture the Flag
---
#### 3.2. Addition - 🚩<kbd> HTB{aDd1nG_4lL_tH3_waY_992570f022ab751823ad3ba2a0761a52} </kbd>
- 📂Category: Coding - Python
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser
 	- The code to add two numbers is:
	```
 	# take in two numbers
	a = int(input())  
	b = int(input())  
	
	# calculate answer
	answer = a + b 
	
	# print answer
	print(answer)
 	```
 	- Capture the Flag
---
#### 3.3. Oddly Even - 🚩<kbd>HTB{15_iT_0dD_oR_Is_iT_n0t?_55a5b52d9d858a2d1832499ba93ccb2f} </kbd>
- 📂Category: Coding - Python
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser
 	- The code to print "odd" for odd numbers and "even" for even numbers:
	```
 	# take in the number
	n = int(input())
	
	# calculate answer
	if n % 2 == 0:
	    answer = "even"
	else:
	    answer = "odd"
	
	# print answer
	print(answer)
 	```
 	- Capture the Flag
---
## 4. Web
#### 4.1. Phantom's Script - 🚩<kbd> HTB{xSS-1S_E4SY_wh4t_d0_y0u_th1nk?_21fa18a001db4e7d21af4934c7b5c28e} </kbd>
- 📂Category: Web -  XSS Vulnerability
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser -> Wait 10 secounds
 	- In the Search Box insert `<script>alert('Boo!');</script>`
 	- Capture the Flag
---

#### 4.2. Void Whispers - 🚩<kbd>  </kbd>
#### 4.3. Unholy Union - 🚩<kbd>  </kbd>
---
## 5. Forensisc
#### 5.1. Spooky Theme - 🚩<kbd>  </kbd>
#### 5.2. The Shortcut Haunting - 🚩<kbd>  </kbd>
---

#### 5.3. Forbidden Manuscript - 🚩<kbd> JHTB{f0rb1dd3n_m4nu5cr1p7_15_1n_7h3_w1ld} </kbd>
- 📂Category: Forensics - PCAP Files
- ⚒️Tools: VirtualBox, Kali VM, [CyberChef](https://gchq.github.io/CyberChef/#recipe=From_Hex('Auto')&input=Rmo0YTQ4NTQ0MjdiNjYzMDcyNjIzMTY0NjQzMzZlNWY2ZDM0NmU3NTM1NjM3MjMxNzAzNzVmMzEzNTVmMzE2ZTVmMzc2ODMzNWY3NzMxNmM2NDdk&oeol=CR)
- ⛑️Help: [CTF Andrew Roderos](https://andrewroderos.com/how-to-solve-my-pcap-ctf-challenges/)
- ⚔️Steps: 
	- Download the File (File Name: capture.pcapng)
	- Open Virtual Box -> Kali Virtual Machine -> Place the file in Shared folder
	- In the terminal, navigate to the file path, then enter the following commands:
		- `strings capture.pcapng` -  display the contents of files
  		- Find the tag /flag and the HEX String is the FLAG in Hexadecimal Format. 		 `Fj4a4854427b66307262316464336e5f6d346e753563723170375f31355f316e5f3768335f77316c647d` 
	- Capture the Flag
---
## 6. Pwn
#### 6.1. Mathematricks - 🚩<kbd>  </kbd>
#### 6.2. El Teteo - 🚩<kbd>  </kbd>
#### 6.3. Que onda - 🚩<kbd>  </kbd>
---
---
