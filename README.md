## 🛡️ Phishing Detection System using Rule-Based URL Analysis
## 📖 Overview

This project is a Rule-Based Phishing URL Detection System that analyzes URLs using multiple security heuristics instead of machine learning. It calculates a risk score and risk percentage based on domain age, HTTPS status, suspicious patterns, DNS validation, blacklist matching, URL length, and domain structure to determine whether a URL is likely safe or a phishing attempt.

## ⚙️ Features

🔐 HTTPS verification

📅 Domain age detection (new domains flagged)

🌐 DNS record validation

🚫 Blacklist domain checking

📏 URL length analysis

➖ Hyphen detection in domain

⚠️ Suspicious pattern detection (IP address, '@', sensitive keywords)

📊 Risk score + risk percentage output

✅ Clear verdict: Likely Safe or Phishing Attempt

## 🧰 Modules and Libraries Used:

requests → To check HTTPS status

whois → To retrieve domain creation date

socket → To verify DNS existence

datetime → To calculate domain age

urllib.parse → To extract domain details

re → For pattern matching in URLs

## 🚀 Workflow

> User enters a URL.

> URL is normalized (adds HTTP if missing).

> System extracts domain information.

> Multiple security checks are performed:

	  Domain age check

	  HTTPS validation

	  Pattern analysis

	  URL length check

	  Hyphen detection

	  DNS verification

    Blacklist comparison

> Risk scores from all checks are added.

> Risk percentage is calculated.

> Final verdict is displayed.

## 🧑‍💻 How to Run

Install required libraries:

pip install requests python-whois

Save the Python file (e.g., phishing_detector.py).

Run the script:

python phishing_detector.py

Modify the analyze_url() input to test different URLs.

## 📊 Example Output

--------------------------------------------------
Analyzing: http://google-secure-login.com/update

[WARNING] Domain Age: 45 days
[WARNING] HTTPS: Not Secure
[WARNING] Sensitive keyword found
[WARNING] Hyphen in domain
[INFO] DNS record exists

Final Risk Score: 5
Risk Percentage: 50.00%
Verdict: 🚨 PHISHING ATTEMPT
--------------------------------------------------

## 🔮 Future Improvements

📂 Add CSV file input for bulk URL testing

📊 Generate graphical risk report

🌍 Integrate real-time phishing threat APIs

🧠 Upgrade to hybrid model (rule-based + ML)

🖥 Develop a lightweight web interface

## 👨‍💻 Author

Akhil Sid
Cybersecurity & AI Enthusiast
Rule-Based Phishing Detection Lab Project (2026)
