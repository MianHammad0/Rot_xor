# Rot_X0r - Advanced XSS & SSTI Scanner

## 🚀 About Rot_X0r
Rot_X0r is an advanced automated security testing tool for finding **XSS (Cross-Site Scripting)** and **SSTI (Server-Side Template Injection)** vulnerabilities in web applications. It automates endpoint discovery, parameter detection, and payload injection, making it a powerful tool for security researchers and bug bounty hunters.


## 🛠 Installation
### **1. Clone the Repository**
```bash
git clone https://github.com/MianHammad0/Rot_xor.git
cd Rot_X0r
```

### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3. Install FFUF & Arjun (Required)**
- **FFUF** (Fast web fuzzer):
  ```bash
  sudo apt install ffuf
  ```
- **Arjun** (Parameter discovery tool):
  ```bash
  pip install arjun
  ```

## 🚀 Usage
### **Basic XSS & SSTI Testing**
```bash
python3 rot_x0r.py -u https://example.com
```

### **Run With Custom Parameters**
```bash
python3 rot_x0r.py -u https://example.com --params "search,query,id"
```

### **Run Blind XSS Payloads**
```bash
python3 rot_x0r.py -u https://example.com --blind-xss "https://your-xss-hunter.com"
```

### **Save Output Results**
```bash
python3 rot_x0r.py -u https://example.com --output results.txt
```

## 🛡️ How It Works
1. **Finds Endpoints** using FFUF (fuzzing URLs)
2. **Detects Parameters** using Arjun
3. **Injects XSS & SSTI Payloads** into parameters
4. **Detects & Saves Vulnerabilities**
5. **Includes WAF Bypass & DOM-based Scanning**

## 📜 License
Rot_X0r is an open-source project created by **Mian Hammad**. Use it responsibly.

## 🤝 Contributing
Feel free to submit issues or pull requests to improve Rot_X0r. 🚀

---

Would you like to add GitHub Actions for CI/CD automation? 🔥

