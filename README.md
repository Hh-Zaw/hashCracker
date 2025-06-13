# hash-cracker
Python-based hash cracking tool for password recovery and security assessments

# Hash Cracker 🔓
A fast, multi-threaded hash cracking tool for ethical hacking and security assessments.

## 🚀 Features
### Hash Cracking
- Multi-threaded for fast cracking
- Dictionary and brute force attacks
- Multiple hash algorithms (MD5, SHA1, SHA256, SHA512)
- Password variation generation
- Real-time progress tracking
- Clean output format

## 📋 Requirements
- Python 3.6+
- Standard library only (no external dependencies)

## 🔧 Installation
```bash
git clone https://github.com/Hh-Zaw/hash-cracker.git
cd hash-cracker
```

## 💻 Usage

### Generate test hash
```bash
python3 hash_cracker.py --test "password123" -a md5
```

### Create sample wordlist
```bash
python3 hash_cracker.py --create-wordlist
```

### Dictionary attack
```bash
# Basic dictionary attack
python3 hash_cracker.py 5d41402abc4b2a76b9719d911017c592 -m dictionary

# SHA256 with custom wordlist
python3 hash_cracker.py ef92b778bafe771e89245b89ecbc08a44a4e166c06659911881f383d4473e94f -a sha256 -w custom.txt

# Adjust thread count for faster cracking
python3 hash_cracker.py 482c811da5d5b4bc6d497ffa98491e38 -t 100
```

### Brute force attack
```bash
# Brute force with lowercase letters (4 chars max)
python3 hash_cracker.py 098f6bcd4621d373cade4e832627b4f6 -m brute -l 4 -c lower

# Brute force with digits only
python3 hash_cracker.py 5d41402abc4b2a76b9719d911017c592 -m brute -c digits -l 6

# Alphanumeric brute force
python3 hash_cracker.py 900150983cd24fb0d6963f7d28e17f72 -m brute -c alphanum -l 3
```

## ⚠️ Disclaimer
**Educational Use Only**
- Only crack hashes you created or have explicit permission to test
- Unauthorized password cracking may violate laws and policies
- Always ensure proper authorization before testing
- Use responsibly and ethically

## 📄 License
MIT License - Educational use only
