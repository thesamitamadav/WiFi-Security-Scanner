# WiFi Security Scanner 🔒

A simple tool to analyze WiFi network security — scan available WiFi networks, detect insecure configurations, and highlight potential vulnerabilities.

## 🔍 Overview  
WiFi Security Scanner scans nearby WiFi networks (SSIDs), checks security settings (WEP/WPA/WPA2/WPA3), and helps you identify networks with weak or outdated security. Ideal for network audits, penetration-test practice, or personal security checks.

## ✅ Features  
- Detect available WiFi networks and list their SSID, signal strength, and security protocol.  
- Flag networks with weak security protocols (e.g. WEP or open networks).  
- Easy-to-read reports of network security status.  
- Cross-platform compatibility (Windows / Linux / macOS) — provided underlying scanning tools are supported.  
- Simple, minimal codebase — easy to understand, extend, or integrate.  

## 🧰 Requirements  
- Python 3.x (or language/environment the script uses)  
- Platform-appropriate dependencies or permissions to scan WiFi networks (may require administrative/root privileges)  
- (Optionally) additional utilities/libraries if required by OS for wireless scanning  

## 🚀 Usage / Installation  

```bash
# Clone the repository
git clone https://github.com/thesamitamadav/WiFi-Security-Scanner.git
cd WiFi-Security-Scanner

# Run the scanner script
python wifi_scanner.py   # or appropriate command depending on the main file name
```
⚠️ On many OSes, scanning WiFi network info requires elevated permissions. Run accordingly (e.g. sudo python wifi_scanner.py on Linux / macOS).

## 🧩 How it Works

The script scans available WiFi networks using system wireless interfaces / native WiFi scanning tools.

Parses security protocol reported by the WiFi driver.

Determines risk level:

Open / WEP → Insecure

WPA / WPA2 → Acceptable (depending on signal strength & passphrase)

WPA3 → Secure (if supported)

Displays summary list / report with SSID, security, signal and risk status.

## 📚 Disclaimer & Ethical Use

This tool is intended only for auditing networks you own or have explicit permission to test.
Use on public / unknown / third-party networks without permission may be illegal or unethical.
You use it at your own risk. The author is not responsible for misuse.

## 📝 Contributing

Feel free to open issues or submit pull requests.
Possible contributions:

Support for more operating systems / wireless drivers

Enhanced reporting (CSV/JSON output)

GUI / CLI improvements

Additional security checks (e.g. password strength, MAC filtering analysis)

## 👤 Author

Samita Madav — Cybersecurity & IT Specialist

## 📄 License 

This project is licensed under the MIT License — you are free to use, modify, and distribute it, provided proper credit is given.

