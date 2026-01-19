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
│
├── main.py                       # CLI entry point for the tool
├── README.md                      # Project overview, installation, usage
├── requirements.txt               # Python dependencies
├── .gitignore                     # Files/folders to ignore in Git
│
├── data/
│   └── raw_logs/                  # Raw log files for testing / analysis
│
├── logs/
│   ├── __init__.py
│   ├── log_analyzer.py            # Functions to check passwords, export CSV, stats
│   └── logs.py                    # Logging helper functions (admin/user/master logs)
│
├── password_policies_manager/
│   ├── __init__.py
│   └── password_policies_manager.py  # Password generation, validation, policy checking
│
└── __pycache__/                   # (ignored by Git) compiled Python files


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