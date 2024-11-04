# AIO SCAN - Web Security Scanner
> A comprehensive tool for assessing web domain security by checking TLS, headers, cookies, and more.

![Banner Image](path/to/banner-image.png) <!-- Replace with your image path or URL -->

## Overview

AIO SCAN is a Python-based tool designed to analyze a web domain's security headers, TLS version, and cookie attributes. It provides a concise report and an option to export results to a CSV file.

---

### 📋 Features
- **TLS Version Detection**: Identify the TLS version for a given domain.
- **Security Headers Check**: Verify the presence of critical security headers.
- **Cookie Security**: Analyze cookies for `HTTPOnly` and `Secure` attributes.
- **DNS Resolution and Redirect Handling**: Ensures the domain resolves correctly and follows any redirections.
- **CSV Export**: Optionally export results for documentation.

---

### 🖥️ Installation

Install the necessary libraries (you may also choose to let the script handle dependencies automatically):
```bash
pip install requests prettytable termcolor
