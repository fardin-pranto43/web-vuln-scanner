# 🔍 Web Vulnerability Scanner

**Interactive tool for detecting and learning about web vulnerabilities** — XSS, CSRF, SQL Injection, insecure headers, and more.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Click%20Here-blue?style=for-the-badge)](https://fardin-pranto43.github.io/web-vuln-scanner/)

## ✨ Features

- **18 Vulnerability Types Detected**
  - Critical: XSS, eval(), SQL Injection, hardcoded credentials, HTTP vs HTTPS
  - High: CSRF, missing headers, weak passwords, debug mode
  - Medium/Low: Input validation, stack traces, CORS misconfiguration
  
- **Real-Time Scanning** — Paste code, get instant vulnerability detection
- **Educational** — Each vulnerability includes:
  - Plain English explanation of the risk
  - ❌ Bad code example (vulnerable)
  - ✅ Good code example (secure)
  - 🔧 Step-by-step fix instructions
  
- **Risk Scoring** — Automatic vulnerability severity calculation (0-100)
- **Zero Dependencies** — Pure HTML/CSS/JavaScript, runs entirely in browser
- **Privacy First** — No server communication, no data collection

## 🚀 Quick Start

### Online (Fastest)
**Just click:** [https://fardin-pranto43.github.io/web-vuln-scanner/](https://fardin-pranto43.github.io/web-vuln-scanner/)

### Local
1. Download `index.html` from this repo
2. Double-click to open in browser
3. Start scanning code

## 📝 How to Use

1. **Paste Code** — Copy any HTML, CSS, or JavaScript into the left panel
2. **Scan** — Click "Scan for Vulnerabilities" (or it auto-scans)
3. **Review** — See detected vulnerabilities with severity levels
4. **Learn** — Read explanations and examples for each issue
5. **Fix** — Implement the recommended security improvements

### Try These Examples

Paste any of these to see the scanner in action:
let userInput = getUserInput();
document.getElementById('output').innerHTML = userInput; // ❌ DANGEROUS

**SQL Injection:**
let userId = getUserInput();
let query = "SELECT * FROM users WHERE id = " + userId; // ❌ DANGEROUS
**Missing CSRF Token:**
<form method="POST" action="/transfer"> <input name="amount" type="text"> <!-- Missing CSRF token --> </form> ```
Hardcoded Credentials:

**XSS Vulnerability:**
const API_KEY = "sk-1234567890abcdef";  // ❌ EXPOSED IN CODE


🎓 Educational Value
This tool teaches:

✅ OWASP Top 10 vulnerabilities

✅ How attacks work and why they're dangerous

✅ Secure coding best practices

✅ Risk assessment methodology

✅ How to fix vulnerabilities correctly

Perfect for:

Developers — Learn to spot security issues before deployment

Students — Master's/Bachelor's cybersecurity programs

Teams — Security awareness training

Interviews — Demonstrate practical security knowledge

💻 Technical Details
Aspect	Details
Tech Stack	HTML5, CSS3, JavaScript ES6+
File Size	~15 KB (single file)
Dependencies	Zero (pure browser)
Deployment	GitHub Pages
Performance	Instant scanning (no server latency)
Privacy	100% local — no external requests
🔧 Vulnerability Patterns Detected
CRITICAL (40 pts each)

Unescaped innerHTML (XSS)

eval() function usage

SQL Injection (string concatenation)

Hardcoded credentials

HTTP instead of HTTPS

HIGH (25 pts each)

Missing CSRF tokens

No SameSite cookies

Missing security headers

Weak password requirements

Logging sensitive data

MEDIUM/LOW (15/5 pts)

Missing input validation

Exposed stack traces

Debug mode enabled

CORS allowing all origins

🎯 Use Cases
For Job Interviews:

Demonstrates practical understanding of real vulnerabilities

Shows you can explain complex security concepts clearly

Proves ability to build functional tools

For Master's Applications:

Shows initiative in learning cybersecurity

Demonstrates self-directed learning

Portfolio piece that differentiates you

For Security Teams:

Quick security assessment tool

Developer training resource

Code review assistant

📚 OWASP Reference
Vulnerabilities covered align with OWASP Top 10 and CWE Top 25:

CWE-79: Improper Neutralization of Input During Web Page Generation (XSS)

CWE-89: Improper Neutralization of Special Elements used in SQL Command (SQL Injection)

CWE-352: Cross-Site Request Forgery (CSRF)

CWE-798: Use of Hard-Coded Credentials

CWE-287: Improper Authentication

🚀 Future Enhancements
 More vulnerability patterns (XXE, SSRF, RCE, etc.)

 CVSS score calculation

 Downloadable security reports

 Multi-language code detection

 Dark mode

 Vulnerability database integration

📄 License
MIT License — Free for educational and personal use

👨‍💻 Author
Fardin Pranto
Cybersecurity Master's Applicant | Bangladesh
Focus: Web Security, Vulnerability Assessment, Secure Development

