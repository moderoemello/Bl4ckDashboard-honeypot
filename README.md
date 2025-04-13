![ChatGPT_Image_Apr_13__2025__03_15_47_PM-removebg-preview](https://github.com/user-attachments/assets/0a162e5d-146a-4c58-8c22-31dc52c61125)

**bl4ckDashboard** is a real-time Node.js-powered honeypot monitoring system designed to help security teams and researchers visualize malicious activity collected from the [Cowrie](https://github.com/cowrie/cowrie) SSH/Telnet honeypot. It connects to a MariaDB/MySQL database storing Cowrie logs and displays intuitive graphs, session metadata, and attack trends through a clean browser-based dashboard.

---

## 🔍 Features

- 📈 **Top Usernames & Passwords** attempted during brute-force attacks
- 🌐 **Top Countries** by attacker IP geo-location
- 🕵️ **Command Log** of what attackers do post-login
- 📥 **Download Tracker** of attempted malware or payload retrievals
- ⏱️ **Recent Sessions** with duration and country
- 📊 **Attacks Over Time** (hourly trend)
- 🔁 **Most Retried IPs** and failed attempts
- 🔑 **Most Seen SSH Key Fingerprints**
- 🧠 **Backend API** returns JSON for easy integrations

---
![image](https://github.com/user-attachments/assets/211f9bc7-12d0-42c3-a52f-fe284fa29235)



## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/bl4ckDashboard.git
cd bl4ckDashboard

# Install dependencies
npm install

# Configure your database connection inside `app.js`
# Make sure Cowrie is logging into MySQL/MariaDB and Apache is reverse proxying correctly

# Start the app
node app.js
