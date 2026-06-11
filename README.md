:::writing{variant="document" id="74192"}

FSociety Tool

<p align="center">
  <img src="assets/logo.png" width="180" alt="FSociety Tool Logo">
</p><p align="center">
  <b>Portable Multi-Function ESP8266 Tool Inspired by Flipper Zero</b>
</p><p align="center">
  <img src="https://img.shields.io/badge/Platform-ESP8266-blue">
  <img src="https://img.shields.io/badge/Display-OLED%20128x64-black">
  <img src="https://img.shields.io/badge/Version-v1.0-green">
  <img src="https://img.shields.io/badge/Status-Stable-success">
</p>
---

🚀 Features

📶 WiFi

Feature	Description

Scan	Discover nearby WiFi networks
Select AP	Choose a target from the scanned list
Attack (Deauth)	Send deauthentication packets
Beacon Spam	Broadcast fake WiFi networks
Graph	Real-time signal strength graph


📡 RF 433 MHz

Feature	Description

Jammer	RF noise generator
Read	Capture and save RF codes
Send	Replay saved RF codes
Delete	Remove saved RF codes
Analyzer	Live pulse analyzer


📺 Infrared (IR)

Feature	Description

TV-B-Gone	Control TV power functions
Jammer	Multi-protocol IR transmission
Read	Capture and decode IR signals
Send	Replay saved IR codes
Delete	Remove saved IR codes


🎮 Other

Feature	Description

Evil Portal	Captive portal testing tool
Pong	Classic arcade game
Breakout	Brick breaker game
About	Creator information
Splash Screen	Custom boot logo
EEPROM Storage	Save RF and IR codes



---

🛠 Hardware Requirements

Component	Description

ESP8266	NodeMCU / Wemos D1 Mini
OLED 0.96" I2C	128×64 Display
433 MHz TX Module	RF Transmission
433 MHz RX Module	RF Reception
IR Receiver	VS1838B / TSOP38238
IR LED + 2N2222	IR Transmission
3 Push Buttons	Menu Navigation



---

🔌 Wiring

Component	Pin	GPIO

OLED SDA	D2	GPIO4
OLED SCL	D1	GPIO5
Button UP	D5	GPIO14
Button DOWN	D6	GPIO12
Button SELECT	D7	GPIO13
RF TX	D0	GPIO16
RF RX	D4	GPIO2
IR LED	D8	GPIO15
IR Receiver	D3	GPIO0



---

📦 Libraries

Adafruit SSD1306

Adafruit GFX Library

ESP8266WiFi

rc-switch

IRremoteESP8266



---

⚡ Flash Firmware

1. Open web.esphome.io


2. Connect ESP8266 via USB


3. Click Connect


4. Select FSociety_Tool.bin


5. Flash Address: 0x0


6. Click Program


7. Wait for completion




---

🎮 Controls

Button	Action

UP	Navigate Up
DOWN	Navigate Down
SELECT	Confirm / Enter
HOLD SELECT	Exit Current Mode



---

📂 Menu Structure

WiFi
 ├── Scan
 ├── Select AP
 ├── Attack
 ├── Beacon Spam
 └── Graph

RF
 ├── Jammer
 ├── Read
 ├── Send
 ├── Delete
 └── Analyzer

IR
 ├── TV-B-Gone
 ├── Jammer
 ├── Read
 ├── Send
 └── Delete

Evil Portal

Games
 ├── Pong
 └── Breakout

About


---

⚠ Disclaimer

This project is intended for educational purposes and authorized security testing only.

Use only on devices and networks you own or have permission to test.


---

👤 Author

Ahmadreza

FSociety Tool v1.0

> "With great power comes great responsibility."




---

📄 License

Personal and Educational Use Only.

All Rights Reserved. :::
