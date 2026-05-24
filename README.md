<img width="1000" height="500" alt="Screenshot 2026-05-24 171107" src="https://github.com/user-attachments/assets/ecdbf534-40c8-442b-9af3-48a8a65935e6" />
<h1 align="center"><b><u>Git Pre-Commit Hook for Python Linting and Secret Detection</u></b></h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue.svg" />
  <img src="https://img.shields.io/badge/Git-Hooks-red.svg" />
  <img src="https://img.shields.io/badge/Security-Checks-green.svg" />
  <img src="https://img.shields.io/badge/Flake8-Linting-yellow.svg" />
</p>

---

<h2><b><u>Description</u></b></h2>

This project automates code quality and security checks before Git commits using Git hooks and shell scripting.  
It ensures that no bad code or sensitive information gets committed into the repository.

---

<h2><b><u>Features</u></b></h2>

- Python linting using `flake8`
- Detects possible passwords/API keys
- Blocks unsafe commits automatically
- Git hooks integration
- Shell scripting automation

---

<h2><b><u>Project Structure</u></b></h2>

git-hooks-security-check/
│
├── githooks/
│ └── pre-commit
│
├── work.py
├── README.md
├── screenshots/
│ └── demo.png


---

<h2><b><u>Requirements</u></b></h2>

- Python 3.x  
- Git  
- `flake8`

---

<h2><b><u>Setup</u></b></h2>

Install dependencies:

```bash
pip install flake8


cp githooks/pre-commit .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
<h2><b><u>How It Works</u></b></h2>
flake8 checks Python code quality
Script scans for possible secrets/API keys
Commit is blocked if issues are detected
<h2><b><u>Example Output</u></b></h2>

flake8 errors found. Commit blocked.


---

## 🚀 Working

The pre-commit hook runs automatically whenever a developer attempts to create a Git commit.  
It first performs Python code quality checks using **flake8** to detect syntax errors and coding standard violations.  
After linting, the script scans project files for potentially sensitive information such as passwords, API keys, and secret tokens.  

If any issue or security risk is detected, the commit process is immediately blocked to prevent unsafe code from being pushed into the repository. Otherwise, the commit is completed successfully.

---


