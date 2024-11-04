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
