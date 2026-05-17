# AI Powered Banking Authentication System

## Overview

The AI Powered Banking Authentication System is a secure banking verification platform developed using Artificial Intelligence Facial Recognition OTP Verification and Spoof Detection techniques. The project uses Raspberry Pi live streaming Flask backend InsightFace machine learning models and Twilio SMS services to provide secure customer authentication.

The system identifies customers using real time facial recognition and grants dashboard access only after successful OTP verification. The project also includes spoof detection and session banning features to prevent fake authentication attempts.

---

# Features

* Real time facial recognition
* OTP based customer authentication
* Spoof detection and session banning
* Live video streaming using Raspberry Pi
* Customer dashboard with banking details
* SQLite and CSV based logging
* Twilio SMS integration
* Secure multi layer authentication

---

# Technologies Used

## Programming Languages

* Python
* Java
* HTML
* CSS
* JavaScript

## Frameworks and Libraries

* Flask
* OpenCV
* InsightFace
* Ultralytics YOLO
* SQLite
* Twilio API

## Hardware

* Raspberry Pi
* USB Camera
* Ethernet Communication

---

# System Architecture

Customer Login
↓
Start Recognition
↓
Raspberry Pi Camera Stream
↓
Face Detection using InsightFace
↓
Customer Recognition
↓
Spoof Detection using YOLO
↓
OTP Generation
↓
SMS Delivery using Twilio
↓
OTP Verification
↓
Customer Dashboard Access
↓
Database and CSV Logging

---

# Project Structure

```bash
banking-ai/
│
├── app.py
├── banking_ml.py
├── customer_db.py
├── otp_store.py
├── SendSms.java
│
├── templates/
│   ├── login.html
│   ├── otp.html
│   └── dashboard.html
│
├── logs/
│   ├── banking.db
│   ├── customer_logs.csv
│   └── recognized_customer.txt
│
└── models/
```

# Working Principle

1. The customer opens the banking web application.

2. The Flask backend launches the banking ML recognition system.

3. Raspberry Pi streams live video frames to the server.

4. InsightFace detects and recognizes customer faces.

5. The system checks for spoof attempts using YOLO object detection.

6. If the customer is verified successfully an OTP is generated.

7. Twilio SMS service sends the OTP to the registered mobile number.

8. The customer enters the OTP on the verification page.

9. If the OTP matches the customer dashboard is displayed.

10. Login details are stored in SQLite database and CSV log files.

---

# Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/banking-ai.git
cd banking-ai
```

## Create Virtual Environment

```bash
python -m venv bank
```

## Activate Environment

### Windows

```bash
bank\Scripts\activate
```

### Linux

```bash
source bank/bin/activate
```

## Install Dependencies

```bash
pip install flask
pip install opencv-python
pip install insightface
pip install ultralytics
pip install numpy
pip install onnxruntime-gpu
pip install pytz
```

---

# Run Flask Server

```bash
python app.py
```

---

# Run Java OTP Module

```bash
javac SendSms.java
```

---

# Database Logging

The system stores:

* Customer login details
* Login time and date
* Session verification records

Storage formats:

* SQLite Database
* CSV Log Files

---

# Spoof Detection

The project includes spoof detection using YOLO object detection.

The system detects:

* Mobile phone spoofing
* Fake authentication attempts
* Suspicious objects

If spoofing is detected:

* Session is banned
* OTP generation is stopped
* Customer access is denied

---

# Results

* Successful real time facial recognition
* Accurate OTP verification
* Secure dashboard access
* Real time spoof detection
* Session banning implementation
* Stable customer authentication workflow

---

# Future Enhancements

* Cloud database integration
* Advanced anti spoofing
* Mobile banking support
* Voice authentication
* Blockchain based banking security

---

# Conclusion

The AI Powered Banking Authentication System provides secure intelligent and real time customer verification using Artificial Intelligence and OTP based authentication. The project successfully combines machine learning spoof detection and banking security into a single authentication platform.

---

# Author

Prasannaa K

Electronics and Communication Engineering
