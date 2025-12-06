🌐 WiFi-Security-Scanner
A Modern WiFi Threat Analysis, Security Scoring & Monitoring Tool Built with Python + PyQt5

📌 Project Overview

WiFi-Security-Scanner is a professional-grade wireless security auditing tool designed to scan nearby WiFi networks, evaluate their security posture, detect threats, and generate detailed reports.
It is built with Python, PyQt5, and includes a clean, modern GUI suitable for cybersecurity portfolios, research projects, and real-world demonstrations.
The application extracts WiFi metadata (SSID, BSSID, encryption, channel, frequency, vendor, etc.), performs security scoring using a custom algorithm, classifies risks, and highlights suspicious networks through a threat-detection engine.# WiFi-Security-Scanner
A modern WiFi Security Scanner built with Python &amp; PyQt5. Features real-time wireless scanning, encryption analysis, risk scoring, vendor identification, rogue AP detection, auto-scan engine, and export options (PDF, CSV, JSON). Designed for cybersecurity learning and wireless auditing.

🚀 Key Features: 

WiFi Network Scanning,
Automatic detection of all nearby wireless networks,
SSID, BSSID, Channel, Frequency (2.4 / 5 GHz),
Signal strength evaluation,
Router vendor identification (MAC prefix → manufacturer)

🛡 Security Scoring Engine: 

Detects encryption type (WPA3 / WPA2 / WPA / WEP / Open),
Custom scoring model (0–100)

Evaluates:
Strength of encryption,
Signal reliability,
Default SSIDs (JioFiber, TP-Link, Netgear, etc.),
SSID complexity

⚠ Threat Detection Engine:

Automatically identifies:
Open networks,
WEP or weakly protected networks,
Duplicate SSIDs (possible evil-twin attacks),
Default router names,
Suspicious low-signal but secure networks,
Inconsistent BSSID patterns

Displays:

Threat summary,
Color-coded risk classification,
Real-time alerts

🖥 Modern PyQt5 Interface: 

Dark mode UI,
Smart color-coded rows based on security level,
Smooth table rendering,
Status bar notifications,
Auto-scan mode (re-scans every 5 seconds),
Tabs for Security View and Raw Logs

📄 Export Options: 

Export results as JSON,
Export structured CSV,
Generate professional PDF security reports

🧰 Windows Executable Ready:

Builds into a standalone .exe using PyInstaller.

🧩 Requirements

Python:	3.9+ recommended,
OS:	Windows 10/11 (full support) / Linux (limited),
Dependencies:	PyQt5, ReportLab

▶ How to Run the Application

python wifi_gui.py

🛠 Build a Standalone Windows EXE

Run:
pyinstaller --onefile --windowed --icon=icon.ico wifi_gui.py

Executable output will be located in:
/dist/WiFiScanner.exe

🔍 Threat Engine – How It Works

The Threat Detection Engine uses real-world wireless security rules:

🔹 Open Network (Very High Risk)

No encryption

Vulnerable to sniffing & MITM

🔹 Weak Encryption (WEP)

Easily crackable

Automatically marked CRITICAL

🔹 Default Router SSIDs

Example: TP-LINK_1234, JioFiber, NETGEARxx

Often indicates unchanged factory configurations

Penalty added in scoring

🔹 Duplicate SSIDs (Evil Twin)

If two networks share:

Same SSID

Different BSSID

Different signal patterns

→ The engine flags it as possible rogue AP.

🔹 Suspicious Low-Signal but Secure Networks

Secure but very weak networks can suggest:

Remote spoofed AP

Extended-range attacks

📄 License

This project is licensed under the MIT License.

You are free to use, modify, and distribute it as long as attribution is given.

MIT License © 2025 Samita Madav

👩‍💻 Author / Contact

Samita Madav,
Cybersecurity & Ethical Hacking Enthusiast
