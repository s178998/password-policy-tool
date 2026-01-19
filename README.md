# Password Policy Tool

**Standalone Password Policy Toolkit** for generating, validating, and analyzing passwords.  

This tool is designed to be lightweight and self-contained, providing the following functionality:

## Features

- ✅ Generate strong passwords that meet policy requirements  
- ✅ Validate passwords against defined policies  
- ✅ Check passwords from files (all, valid, or invalid)  
- ✅ Export logs to CSV for auditing purposes  
- ✅ Generate password statistics (length, valid, invalid counts)  
- ✅ Command-line interface (CLI) for easy interaction  

## Installation

1. Clone or download this repository:

```bash
git clone https://github.com/s178998/CyberOpsToolkit.git
cd cyber_tools/password_policy_tool
```
2. Create and activate a Python virtual environment:
``` bash
python3 -m venv venv
source venv/bin/activate
```
3. Install dependencies:
``` bash
pip install -r requirements.txt
```
Usage

Run the main CLI:
``` bash
python3 main.py
```

## Follow the on-screen menu to:

1. Check single passwords

2. Generate passwords

3. Export logs
4. Generate statistics

Project Structure
password_policy_tool/
├── main.py                       # CLI entry point
├── logs/
│   ├── log_analyzer.py           # Password log checking and reporting
│   └── logs.py                   # Log management
├── password_policies_manager/
│   └── password_policies_manager.py  # Password generation and policy checks
├── data/
│   └── raw_logs/                 # Optional folder for raw password logs
└── __init__.py

Contributing

Fork the repository and submit pull requests for new features or bug fixes.

Ensure password policies remain secure and up-to-date.

License

This project is open-source and free to use for educational or professional purposes.


---

### **requirements.txt**
bcrypt==4.0.1

## Notes:
bcrypt is used for hashing and verifying passwords.