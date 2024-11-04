AIO SCAN - Web Security Scanner
A comprehensive tool for assessing web domain security by checking TLS, headers, cookies, and more.

<!-- Add an illustrative banner image -->

Overview
AIO SCAN is a Python-based tool designed to analyze a web domain's security headers, TLS version, and cookie attributes. It provides a concise report and an option to export results to a CSV file.

📋 Features
TLS Version Detection: Identify the TLS version for a given domain.
Security Headers Check: Verify the presence of critical security headers.
Cookie Security: Analyze cookies for HTTPOnly and Secure attributes.
DNS Resolution and Redirect Handling: Ensures the domain resolves correctly and follows any redirections.
CSV Export: Optionally export results for documentation.
🖥️ Installation
Install the necessary libraries (you may also choose to let the script handle dependencies automatically):

bash
Copy code
pip install requests prettytable termcolor
🚀 How to Use
Clone the repository:

bash
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
Follow the prompts for the analysis report and CSV export.

📝 Sample Output
After running the scan, you’ll see results in a structured table:

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
📊 CSV Export
Choose to export results for documentation and further analysis. The CSV file will be saved as <domain>_<timestamp>.csv.

🧑‍💻 Contributing
Contributions are welcome! Please check out the contribution guidelines in the CONTRIBUTING.md.

🛠️ Future Enhancements
Adding support for batch domain analysis.
Expanding security checks to include additional headers and HTTP methods.
🤝 License
Distributed under the MIT License. See LICENSE for more information.
