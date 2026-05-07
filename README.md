# 📱 WhatsApp Message Automation Tool (Python)

## 🚀 Overview
This project is a Python-based WhatsApp automation system that allows users to send messages, bulk messages, scheduled messages, and template-based personalized messages using a simple CLI interface.

It simulates real-world communication automation used in marketing, education, and notification systems.

---

## ✨ Features

### 📩 1. Send Single Message
- Send WhatsApp messages instantly
- Auto country-code validation (+92 support)

### 📦 2. Bulk Messaging
- Send messages to multiple contacts
- Load contacts from CSV file
- Prevent duplicate messaging

### 🧾 3. Message Templates
- Predefined message templates (JSON)
- Dynamic placeholders:
  - {name}
  - {course}

### ⏰ 4. Scheduled Messaging
- Schedule messages at specific time (HH:MM format)
- Automated execution using Python timing logic

### 📝 5. Logging System
- Stores all message activity
- Tracks:
  - Phone number
  - Message
  - Status (Sent/Failed)
  - Timestamp

### 🛠 6. Error Handling
- Invalid number detection
- Missing country code validation
- CSV type handling fixes

---

## 🧰 Technologies Used
- Python 3
- PyWhatKit
- Pandas
- JSON (Templates)
- CSV (Contacts)

---

## 📂 Project Structure


whatsapp_automation/
│
├── main.py # Main CLI menu system
├── sender.py # Message sending logic
├── scheduler.py # Scheduling system
├── templates.py # Template handling
├── logger.py # Logging system
├── utils.py # CSV loader
│
├── contacts.csv # Contact list
├── templates.json # Message templates
├── logs.txt # Message logs
└── README.md # Documentation


---

## 📊 Sample contacts.csv

```csv
name,phone,course
Ali,+923362814132,AI
Sara,+923001234567,ML
📄 Sample templates.json
{
  "reminder": "Hello {name}, your {course} class starts tomorrow.",
  "offer": "Hi {name}, new {course} course is now available!"
}
⚙️ Installation
1. Clone the project
git clone https://github.com/yourusername/whatsapp-automation-tool.git
2. Install dependencies
pip install pywhatkit pandas
▶️ How to Run
python main.py
📌 Important Notes
Must be logged into WhatsApp Web before sending messages
Keep browser open during execution
Use correct phone format with country code (+92 for Pakistan)
Scheduling uses 24-hour format (HH:MM)
⚠️ Known Limitations
Requires internet connection
WhatsApp Web dependency
Slight delay in message scheduling
Browser automation behavior depends on system speed
🎯 Learning Outcome

This project demonstrates:

Automation using Python
File handling (CSV & JSON)
CLI application design
Real-world messaging simulation
Error handling & validation
👨‍💻 Author

Developed as a Python automation project for academic submission and real-world simulation of messaging systems.

📜 License

This project is for educational purposes only.

