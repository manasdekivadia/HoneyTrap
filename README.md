# HoneyTrap
HoneyTrap is a lightweight yet powerful honeypot designed to detect and log unauthorized access attempts on SSH and HTTP services. It simulates vulnerable systems to attract attackers, capturing valuable threat intelligence while misleading malicious actors.

🚀 Features

✅ SSH Honeypot – Captures brute-force attacks, logs credentials, and attacker behavior.

✅ HTTP Honeypot – Mimics web applications to detect web-based attacks (SQLi, XSS, etc.).

✅ Logging & Analysis – Records attack details for further analysis.

✅ Customizable Traps – Configure fake vulnerabilities to lure attackers.

✅ Lightweight & Easy to Deploy – Runs on minimal hardware with Python.

⚙️ How It Works
Attackers attempting to log into the SSH service are monitored and logged.

Suspicious HTTP requests (e.g., scans, injections) are captured and stored.

Logs provide insights into attack patterns, malicious IPs, and exploit techniques.

The templates folder contain the main html code for a simple login page.


## 📂 Project Structure

- `honeytrap.py` - Main script to launch SSH or web honeypots.
- `ssh_honeytrap.py` - SSH-based honeypot implementation using `paramiko`.
- `web_honeytrap.py` - Web-based honeypot using `Flask`.
- `login.html` - Fake login page for the web honeypot.

## 🛠️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/manasdekivadia/HoneyTrap.git
cd HoneyTrap
```
### 2️⃣ Run the honeypot

- **SSH Honeypot**
  ```bash
  python honeytrap.py -a 0.0.0.0 -p 2222 -u username -pw password -s
  ```
- **Web Honeypot**
  ```bash
  python honeytrap.py -a 0.0.0.0 -p 5000 -w
  ```

## 📜 Logs & Monitoring

- **SSH logs:** Stored in `ssh_audits.log`
- **Web login attempts:** Logged in `http_audits.log`

## ⚠️ Disclaimer

This tool is for security research and educational purposes only. Use it responsibly and only in environments you own or have explicit permission to monitor.

## 🏆 Contributions

Feel free to fork and improve this honeypot! Submit pull requests with enhancements or report issues.

---


