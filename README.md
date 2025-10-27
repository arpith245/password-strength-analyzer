# 🔐 Password Strength Analyzer & Custom Wordlist Generator

A Python-based tool that helps you analyze password strength and generate custom wordlists from user-provided hints.
Useful for ethical hacking labs, cybersecurity education, and password policy testing.

## 🧩 Features

🔍 Analyze password strength using zxcvbn or entropy calculation

🧠 Generate smart wordlists from hints (name, pet, date, etc.)

💡 Add leetspeak variations (e.g., a→@, o→0, s→$)

📄 Export results as .txt for cracking tools

🖥 Simple CLI, ready for automation or GUI extension

## ⚙ Installation

Clone the repository:

git clone https://github.com/yourusername/password-strength-analyzer.git
cd password-strength-analyzer


Install required dependencies:

pip install -r requirements.txt

## 🚀 Usage
### 🔒 Analyze Password

Check how strong your password is:

python password_strength_tool/analyzer.py analyze --password "P@ssw0rd123"


Example output:

{'score': 3, 'entropy': 56.4, 'feedback': {'suggestions': ['Add more symbols or numbers']}}

### 🧾 Generate Wordlist

Create a custom wordlist from your hints:

python password_strength_tool/analyzer.py generate --hints abhay dog 2001 --out abhay_wordlist.txt


## 📁 Folder Structure
password-strength-analyzer/
│
├── password_strength_tool/
│   └── analyzer.py
├── tests/
│   └── test_analyzer.py
├── requirements.txt
├── README.md
└── .gitignore

## 🧪 Testing

Run basic tests using:

pytest tests/

## ⚠ Disclaimer

This tool is for educational and ethical use only.
Do not use it for unauthorized password cracking or testing.
