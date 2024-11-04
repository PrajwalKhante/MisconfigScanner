# 🌐 AIO SCAN - Web Security Scanner
![GitHub repo size](https://img.shields.io/github/repo-size/yourusername/aio-scan)
![GitHub contributors](https://img.shields.io/github/contributors/yourusername/aio-scan)
![GitHub stars](https://img.shields.io/github/stars/yourusername/aio-scan?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/aio-scan?style=social)
![GitHub License](https://img.shields.io/github/license/yourusername/aio-scan)

A comprehensive tool for assessing web domain security by checking TLS versions, headers, cookies, and more. This Python tool is ideal for security enthusiasts, developers, and network administrators aiming to enhance web security.

---

## 📌 Table of Contents
- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Sample Output](#-sample-output)
- [CSV Export](#-csv-export)
- [Contributing](#-contributing)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## ✨ Features

- **TLS Version Detection**: Identify the TLS version for a given domain.
- **Security Headers Check**: Verify the presence of critical security headers.
- **Cookie Security**: Analyze cookies for `HTTPOnly` and `Secure` attributes.
- **DNS Resolution and Redirect Handling**: Ensures the domain resolves correctly and follows any redirections.
- **CSV Export**: Optionally export results for documentation.

---

## 💻 Installation

Ensure you have Python 3.x installed. The script will automatically handle dependencies if they’re missing.

Install the necessary libraries (or let the script handle dependencies):
```bash
pip install requests prettytable termcolor

---
## 🚀 Usage
Clone the repository:

```bash
Copy code
git clone https://github.com/yourusername/aio-scan.git
cd aio-scan

Run the script:

bash
Copy code
python aio_scan.py
Enter the target domain:

plaintext
Copy code
Enter the domain (e.g., example.com): example.com
Review results: The script will display a security report in the terminal and prompt you to save it as a CSV file if desired.

📄 Sample Output
After running the scan, you’ll see a detailed output report like the one below:

plaintext
Copy code
------------------------------------------------------
┳┳┓┳┏┓┏┓┏┓┳┓┏┓┳┏┓  ┏┓┏┓┏┓┳┓┳┓┏┓┳┓
┃┃┃┃┗┓┃ ┃┃┃┃┣ ┃┃┓  ┗┓┃ ┣┫┃┃┃┃┣ ┣┫  v0.2
┛ ┗┻┗┛┗┛┗┛┛┗┻ ┻┗┛  ┗┛┗┛┛┗┛┗┛┗┗┛┛┗  BY PRAJWAL KHANTE
------------------------------------------------------

[+] Domain is live. Status code: 200

+-------------------------+-------------+
| Header                  | Status      |
+-------------------------+-------------+
| Server                  | Apache      |
| TLS Version             | TLSv1.3     |
| Content-Security-Policy | ENABLED     |
| X-Content-Type-Options  | DISABLED    |
| ...                     | ...         |
+-------------------------+-------------+
The report includes:

Server Information: The type of web server.
TLS Version: The TLS version used by the domain.
Security Headers: Status of critical security headers like Content-Security-Policy, X-Content-Type-Options, etc.
You can also choose to export the results to a CSV file, named as <domain>_<timestamp>.csv, for easy documentation.
