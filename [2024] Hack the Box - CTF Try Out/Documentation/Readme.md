# [2024] Hack  the Box - CTF Try Out
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: Hack the Box
- 📅Date: 2024 October 19th - Present
- 💪Mode: Individual
- 💻15 challenges across 8 categories
- ⚒️ Skills:Warmup, Web, Forensics, Reversing, Misc, Crypto, Hardware, Pwn 
- 🌐 Official: https://ctf.hackthebox.com/event/details/ctf-try-out-1434

---
## ✔️1. Warmup
#### 1.1. Welcome to CTF - 🚩<kbd>HTB{onboard1ng_f14q} </kbd>
- 📂Category: Warm-up
- ⚔️Steps: 
    - Spawn Docker and click on "Play through the browser"
    - Capture the Flag
      
---
## 2. Web

---
## 3. Forensics

---
## ✔️4. Reversing
#### 4.1. Loot Stash - 🚩<kbd> HTB{n33dl3_1n_a_l00t_stack} </kbd>
- 📂Category: Reversing - ELF File
- ⚔️Steps: 
	- Download the File (File Name: stash)
 	- Open the file with Notepad and search for "HTB" keyword. The flag will be in plaintext.
  	- Capture the Flag 
   
---
## ✔️5. Misc
#### 5.1. Character - 🚩<kbd> HTB{tH15_1s_4_r3aLly_l0nG_fL4g_i_h0p3_f0r_y0Ur_s4k3_tH4t_y0U_sCr1pTEd_tH1s_oR_els3_iT_t0oK_qU1t3_l0ng!!} </kbd>
- 📂Category: Misc
- ⚔️Steps: 
	- Open Virtual Box -> Kali Virtual Machine -> Open the terminal -> insert the command `nc 94.237.60.154 57204`
 	- The program will ask for the index of the string - Interval [0-103]
  	- Capture the Flag
  	  
---

#### 5.2. Stop, Drop and Roll - 🚩<kbd> HTB{1_wiLl_sT0p_dR0p_4nD_r0Ll_mY_w4Y_oUt!} </kbd>
- 📂Category: Misc
- ⛑️Help: Chat GPT
- ⚔️Steps: 
	- Open Virtual Box -> Kali Virtual Machine -> Open the terminal -> Place the file in Shared folder
 	- TIn Shared folder creat the `game.py` file:
		```
			 	import socket
				import re
				
				# Setări de conexiune - noua adresă și port
				host = '94.237.63.215'
				port = 42376
				
				# Mapează scenariile la răspunsurile respective
				responses = {
				    "GORGE": "STOP",
				    "PHREAK": "DROP",
				    "FIRE": "ROLL"
				}
				
				# Funcție pentru a genera răspunsurile necesare
				def generate_response(message):
				    # Extrage scenariile din mesaj
				    scenarios = re.findall(r"(GORGE|PHREAK|FIRE)", message)
				    # Convertește fiecare scenariu în răspunsul corespunzător
				    response = '-'.join([responses[scenario] for scenario in scenarios])
				    return response
				
				# Conectează-te la server
				with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
				    s.connect((host, port))
				    
				    # Citire inițială a mesajului de întâmpinare
				    data = s.recv(1024).decode()
				    print(data)
				
				    # Trimite răspunsul de start
				    s.sendall(b"Y\n")
				    
				    while True:
				        # Citește mesajul de la server
				        data = s.recv(1024).decode()
				        print("Server:", data)
				        
				        # Verifică dacă mesajul conține scenarii și generează răspunsul corespunzător
				        if any(word in data for word in responses.keys()):
				            response = generate_response(data)
				            print("Trimite:", response)
				            s.sendall((response + "\n").encode())
				        
				        # Verifică dacă mesajul conține flag-ul și îl afișează
				        flag = re.search(r"FLAG{[^}]+}", data)
				        if flag:
				            print("Flag găsit:", flag.group(0))
				            break
				        
				        # Dacă jocul se termină fără flag, ieși din buclă
				        if "GAME OVER" in data or not data:
				            print("Joc terminat fără flag.")
				            break
		```
 	- In the terminal, navigate to the file path, then enter the following commands:
		- `python3 --version`  - instalare python
	   	- `python3 game.py` - execute the script using python
  	- Capture the Flag  

---
## ✔️6. Crypto
#### 6.1. Dynastic - 🚩<kbd> HTB{DID_YOU_KNOW_ABOUT_THE_TRITHEMIUS_CIPHER?!_IT_IS_SIMILAR_TO_CAESAR_CIPHER} </kbd>
- 📂Category: Cryptography - Trithemius Cipher
- ⛑️Help: Chat GPT
- ⚔️Steps: 
	- Download the Files (Files Name: output.txt, source.py)
  	- Open Virtual Box -> Kali Virtual Machine -> Place the file in Shared folder
	- In Shared folder creat the `decrypt.py` file:
   
         ```
	           # Decryption Code
	              def to_identity_map(a):
	                  return ord(a) - 0x41
	              
	                def from_identity_map(a):
	                    return chr(a % 26 + 0x41)
	                
	                def decrypt(encrypted_message):
	                    decrypted = ''
	                    for i in range(len(encrypted_message)):
	                        ch = encrypted_message[i]
	                        if not ch.isalpha():
	                            decrypted += ch  # Non-alpha characters remain unchanged
	                        else:
	                            chi = to_identity_map(ch)  # Get the encrypted character's identity
	                            # Reverse the encryption by subtracting the index
	                            original_ch_index = (chi - i) % 26
	                            decrypted += from_identity_map(original_ch_index)  # Get the original character
	                    return decrypted
	                
	                # Encrypted message from the output.txt
	                encrypted_message = "DJF_CTA_SWYH_NPDKK_MBZ_QPHTIGPMZY_KRZSQE?!_ZL_CN_PGLIMCU_YU_KJODME_RYGZXL"
	                decrypted_message = decrypt(encrypted_message)
	                
	                print(decrypted_message)
         ```
  - In the terminal, navigate to the file path, then enter the following commands:
      - `python3 --version`  - instalare python
      - `python3 decrypt.py` - execute the script using python
  - Decrypted Text:
     DID_YOU_KNOW_ABOUT_THE_TRITHEMIUS_CIPHER?!_IT_IS_SIMILAR_TO_CAESAR_CIPHER
  - Capture the Flag
 
---
## 7. Hardware

---
## 8. Pwn
---
