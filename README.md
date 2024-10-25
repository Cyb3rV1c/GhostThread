# GhostThread


**Description :**

An advanced Windows shellcode injection tool leveraging APC (Asynchronous Procedure Call) injection to execute encrypted payloads within target processes. 
GhostThread uses dynamic API resolution via hash-based function lookups, enhancing its stealth and evasion capabilities against static and dynamic analysis tools. 
This tool supports position independent code and employs XOR decryption to securely unmask and execute payloads. 


# Features

**[+] Obfuscation Techniques:** Employs XOR encryption to avoid signature-based detection.

**[+] APC Injection:** The injection process offers both alertable and suspended thread modes for executing payloads in a sacrificial thread.

**[+] API Hashing:**  Using dynamically resolved APIs via FNV-1a hashing,


# Getting Started

**Installation**


1. Clone the repository:
```
git clone https://github.com/Cyb3rV1c/GhostThread
```


# Usage

1. Add your shellcode in GhostThread.cpp (notice : make sure you encrypt your shellcode first with [Xor_Encryptor ](https://github.com/Cyb3rV1c/Phantom/tree/main/Xor_Encryptor) + add the same xor key)

2. Compile & Run.

***Notice***: Make sure your shellcode has the same architecture as the environment you'll execute it in.

# Example Output

**Execution** 
(I used MsfVenom payload messagebox for this example)

![exec](https://github.com/user-attachments/assets/3434667e-9fd6-461c-8c7c-91eda19073c3)


**Defender Static Evasion** 

![Def](https://github.com/user-attachments/assets/0dfdd730-b2eb-425f-8ec0-e34207e45d0e)





# Disclaimer
**This project is intended for educational and research purposes only.**

The code provided in this repository is designed to help individuals understand and improve their knowledge of cybersecurity, ethical hacking, and malware analysis techniques. It must not be used for malicious purposes or in any environment where you do not have explicit permission from the owner.
