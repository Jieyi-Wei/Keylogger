# Keylogger Detection System

## Course: Ethical Hacking (CPSC_5207EL_61_2025SP)
## Team: Group 16
## Members: Jieyi Wei (0457264), Shirui Zhang (0453239), Baoqiang Chu (0460699), Haige Yu (0457924)


This project implements a **cross-platform Python-based keylogger** with behavior-based detection and Fernet encryption. It was developed for academic and ethical hacking purposes under CPSC_5207EL_61_2025SP.

> ⚠️ This project is for **educational use only**. Do not deploy on systems without explicit consent.

## ✅ Features

- ⌨️ Keystroke logging (pynput)
- 📋 Clipboard monitoring (pyperclip)
- 🎙️ Microphone recording (sounddevice)
- 📸 Screenshot capture (Pillow)
- 🔐 Fernet encryption and decryption of all logs
- ⚠️ Behavior-based detection (high-frequency input, unauthorized clipboard/screen/mic access)
- 📁 Tested on Windows 11 and macOS Monterey (ARM64)

## 📁 Output Files

| File               | Description                    |
|--------------------|--------------------------------|
| key_log.txt        | Raw keystrokes                 |
| clipboard.txt      | Clipboard content              |
| audio.wav          | Microphone audio               |
| screenshot.png     | Captured screen                |
| syseinfo.txt       | System info snapshot           |
| alerts.txt         | Behavior detection alerts      |
| *.enc              | Encrypted versions of the above|

## 🔐 Decryption Tool

A separate script (`DecryptFile.py`) decrypts `.enc` files using the key stored in `encryption_key.txt`. Use responsibly.

## 📦 Dependencies

Install all required packages using:

```bash
pip install -r requirements.txt
