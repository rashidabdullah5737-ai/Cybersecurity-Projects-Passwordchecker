# 🔐 Cybersecurity Projects Portfolio

This repository showcases two cybersecurity projects I completed to strengthen my skills in **ethical hacking**, **Linux security**, and **Python scripting**.

---

## 1️⃣ Password Cracker using John the Ripper

**Description:**  
Password security auditing in a controlled lab environment using **John the Ripper** on Kali Linux.  
Evaluated password strength, extracted hashes, and performed dictionary attacks.

**Tools & Technologies:**  
- Kali Linux  
- John the Ripper  
- rockyou.txt wordlist  
- Linux terminal  

**Methodology:**  
```bash
# Create test user
sudo adduser testuser

# Extract password hashes
sudo unshadow /etc/passwd /etc/shadow > hashes.txt

# Perform dictionary attack
john --wordlist=/usr/share/wordlists/rockyou.txt hashes.txt

# Show cracked passwords
john --show hashes.txt
