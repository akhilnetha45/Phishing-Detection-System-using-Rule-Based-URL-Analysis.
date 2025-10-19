## 🛡️ Phishing Detection System using Rule-Based URL Analysis
📖 Overview

This project is a Python-based phishing detection system that identifies potentially malicious websites using rule-based heuristics instead of AI or machine learning.
It analyzes various aspects of a URL—such as domain age, HTTPS usage, and URL patterns—to determine if it may be part of a phishing attempt.
This tool is simple, fast, and effective for educational or security awareness purposes.

## ⚙️ Features

🔍 Domain Age Check: Uses WHOIS lookup to find if the domain is newly created.

🔐 HTTPS Verification: Flags insecure websites that lack HTTPS connections.

🧩 Pattern Detection: Scans for IP addresses, suspicious characters, or misleading keywords in URLs.

⚙️ Customizable Threshold: You can adjust the risk level based on desired sensitivity.

💡 Simple & Lightweight: Requires no complex setup or datasets.

## 🧰 Modules and Libraries Used:

This project uses the following Python libraries:

requests – For making HTTP requests and checking URL connectivity

whois – To fetch domain registration details

datetime – To calculate domain age

urllib.parse – To parse and extract URL components

re – For detecting suspicious text patterns using regular expressions

## 🚀 Workflow

The user inputs a website URL.

The script performs several heuristic checks (HTTPS, domain age, URL structure).

Each failed check adds to the risk score.

If the total score exceeds a defined threshold, the site is flagged as “Phishing”, else marked “Legitimate.”

## 🧑‍💻 How to Run

Install the required libraries:

pip install requests python-whois


Run the script or Jupyter Notebook:

python phishing_project.ipynb


Enter a URL when prompted and check the result.

## 📊 Example Output
[INFO] Domain Age: 45 days old.
[WARNING] HTTPS Status: Insecure (HTTP).
[WARNING] Suspicious pattern detected in URL.
⚠️ Risk Score: 4 — Classified as PHISHING

## 🔮 Future Improvements

Add machine learning models for automated detection.

Integrate with a browser extension for real-time scanning.

Build a simple UI dashboard for better usability.

## 👨‍💻 Author

Akhil Sid
B.Tech Student — Project on Cybersecurity Awareness
