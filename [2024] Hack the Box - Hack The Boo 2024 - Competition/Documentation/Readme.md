# CTF WriteUps
**[[2024] Hack the Box - Hack The Boo 2024 - Competition]()**<br>
- 🏛️𝐎𝐫𝐠𝐚𝐧𝐢𝐳𝐞𝐫: Hack the Box
- 📅Date: 2024 October 24th - 26th
- 💪Mode: Individual
- 💻12 challenges across 6 categories
- ⚒️ Skills: Coding, Forensics, Web, Pwn, Reversing
- 🌐 Official: https://ctf.hackthebox.com/event/details/hack-the-boo-2024-competition-1813
---

## 1. Coding
### 1.1. Replacement- 🚩<kbd> </kbd>
- 📂Category: Coding- Python
- ⛑️Help: ChatGPT
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser
	- The code for flag is:
	```
	```
	- Capture the Flag
---
### 1.2. MiniMax - 🚩<kbd> HTB{aLL_maX3d_0uT_c19c50b4e007f2ac2460196592ea0ccc} </kbd>
- 📂Category: Coding- Python
- ⛑️Help: ChatGPT
- ⚔️Steps:
	- Spawn Docker -> Insert IP Address & IP in Browser
	- The code for flag is:
	```
	# Read the intercepted codes as a space-separated string and convert them to a list of floats
		codes = list(map(float, input().split()))

	# Identify the minimum and maximum values from the list
		min_value = min(codes)
		max_value = max(codes)

	# Print the minimum and maximum values, in the required order
		print(min_value)
		print(max_value)
	```
	- Capture the Flag