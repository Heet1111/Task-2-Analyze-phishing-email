🚀 Overview

This repository contains the submission for Task 2 of my Cyber Security Internship.
The objective of this task is to analyze a phishing email, identify red flags, understand email spoofing techniques, and perform a full header analysis to determine whether the email is legitimate or malicious.

📨 1. Sample Phishing Email

The phishing email used for analysis attempts to impersonate Microsoft Support and tricks the user into clicking a malicious verification link.

The full email is available in:
📄 phishing_email.txt

🕵️ 2. Phishing Indicators Identified

Key red flags found during the examination:

❌ Fake sender domain: microsoft-verificationcenter.com

❌ Display name spoofing: “Microsoft Support”

❌ Suspicious link: Contains misspelling verfiy instead of verify

❌ Generic greeting: “Hello User” instead of real username

❌ Malicious attachment: SecurityLog_Report.rar

❌ Urgent, threatening language to scare the user

❌ Poor email formatting and missing official branding

❌ Sender IP not belonging to Microsoft

Full analysis is included in:
📄 analysis_report.pdf (or .txt if you uploaded text)

📡 3. Email Header Analysis

A detailed header analysis was conducted using an online email header analyzer.

Key Findings:

SPF: fail

DKIM: none

DMARC: fail

Sender IP 207.182.142.88 not owned by Microsoft

Message-ID contains fake domain

Routing path does not match Microsoft mail servers

Spam score: 5.6 / 5 – flagged as possible spam

These results confirm that the email is spoofed and malicious.


🛡 4. Conclusion

After examining both the email content and header metadata, it is confirmed that the email is a phishing attempt designed to steal user credentials by impersonating Microsoft.

The combination of:

Fake domain

Authentication failures

Malicious link

Suspicious attachment

Non-Microsoft IP

proves that this email is not legitimate.
