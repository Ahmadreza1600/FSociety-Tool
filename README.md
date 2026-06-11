FSociety Tool

A portable multi-function tool for ESP8266 with an OLED display, inspired by Flipper Zero.
Includes WiFi Deauther, RF 433 MHz jammer & code reader, IR TV‑B‑Gone & jammer, Evil Portal, and built‑in games.

---

🚀 Features

WiFi

· Scan – discover nearby WiFi networks.
· Select AP – choose a target from the scanned list.
· Attack (Deauth) – send deauthentication packets with a robust packet structure (web‑based format) to disconnect clients.
· Beacon Spam – broadcast thousands of fake WiFi networks with a custom SSID.
· Graph – real‑time signal strength bar chart (64 bars) across all 2.4 GHz channels.

RF 433 MHz

· Jammer – strong RF noise generator on the 433 MHz band.
· Read – capture and save remote control codes (rc‑switch library).
· Send – replay saved codes.
· Delete – remove individual saved codes.
· Analyzer – live pulse analyzer with 64 moving bars.

IR (Infrared)

· TV‑B‑Gone – turn off/on over 100 TV models using stored power codes.
· Jammer – aggressive multi‑protocol IR jammer (NEC, Sony, RC5, RC6, Panasonic, JVC + raw pulses).
· Read – capture IR signals and decode common protocols.
· Send / Delete – manage saved IR codes.

Other

· Evil Portal – create a fake WiFi access point with a Google‑style phishing page; captured credentials are shown on the OLED.
· Games – Pong and Breakout (Snake removed for performance).
· About – displays creator information.
· Splash Screen – custom bitmap displayed at boot.
· Persistent Storage – RF and IR codes are saved in EEPROM.

---

🛠️ Hardware Requirements

Component Description
ESP8266 (NodeMCU, Wemos D1 Mini, etc.) main board
OLED 0.96" I2C (128×64) display
433 MHz transmitter module RF code transmission
433 MHz receiver module RF code reception
IR receiver (VS1838B / TSOP38238) IR signal capture
IR LED + NPN transistor (2N2222) + 100 Ω resistor IR signal transmission
3 push buttons menu navigation

---

🔌 Wiring

Component ESP8266 Pin GPIO
OLED SDA D2 4
OLED SCL D1 5
Button UP D5 14
Button DOWN D6 12
Button SELECT D7 13
433 TX DATA D0 16
433 RX DATA D4 2
IR LED (via transistor) D8 15
IR receiver OUT D3 0

All buttons use the internal pull‑up resistors; connect one side of each button to GND and the other to the corresponding GPIO.

---

📦 Required Libraries

If you compile the code yourself, install these libraries via Arduino Library Manager:

· Adafruit SSD1306
· Adafruit GFX Library
· ESP8266WiFi (built‑in)
· rc‑switch
· IRremoteESP8266

---

⚡ Installation (Flashing the Binary)

A pre‑compiled firmware file (FSociety_Tool.bin) is provided – no Arduino IDE needed!

1. Visit web.esphome.io (ESP Web Tools flasher).
2. Connect your ESP8266 board to the computer via USB.
3. Click “Connect” and select the correct serial port.
4. In the firmware upload section, click “Choose File” and select the FSociety_Tool.bin file.
5. Set the flash address to 0x0 (the default for ESP8266 binaries).
6. Click “Program” and wait until the process finishes.
7. After a successful flash, the device will reboot and display the splash screen for 2 seconds, then enter the main menu.

(If you prefer to compile the source code yourself, use Arduino IDE with the required libraries and upload as usual.)

---

🎮 Usage

Navigate the menu using the three buttons:

· UP / DOWN – move through menu items.
· SELECT – enter a submenu / start an action / go back (hold to exit active modes like Attack or Jammer).

Menu Overview

· WiFi → Scan → Select AP → Attack / Beacon Spam / Graph
· RF → Jammer / Read / Send / Delete / Analyzer
· IR → TV‑B‑Gone / Jammer / Read / Send / Delete
· Evil Portal – starts a fake WiFi network; credentials appear on the OLED when submitted.
· Games → Pong / Breakout
· About – creator info.

---

⚠️ Disclaimer

This tool is intended for educational purposes and authorized security testing only.
You may only use it on devices and networks that you own or for which you have explicit written permission.
Unauthorized use against third‑party networks or devices is illegal and the author assumes no responsibility for any misuse.

---

👤 Author

Ahmadreza
Project: FSociety Tool v1.0

“With great power comes great responsibility.”

---

📄 License

This project is released for personal and educational use. Redistribution or commercial use without permission is prohibited.
