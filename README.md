# FSociety Tool

**Portable Multi-Function ESP8266 Tool**

---

# 🚀 Features

## 📶 WiFi

| **Feature** | **Description** |
|------------|----------------|
| **Scan** | Discover nearby WiFi networks |
| **Select AP** | Choose a target from the scanned list |
| **Attack (Deauth)** | Send deauthentication packets |
| **Beacon Spam** | Broadcast fake WiFi networks |
| **Graph** | Real-time signal strength graph |

## 📡 RF 433 MHz

| **Feature** | **Description** |
|------------|----------------|
| **Jammer** | RF noise generator |
| **Read** | Capture and save RF codes |
| **Send** | Replay saved RF codes |
| **Delete** | Remove saved RF codes |
| **Analyzer** | Live pulse analyzer |

## 📺 Infrared (IR)

| **Feature** | **Description** |
|------------|----------------|
| **TV-B-Gone** | Control TV power functions |
| **Jammer** | Multi-protocol IR transmission |
| **Read** | Capture and decode IR signals |
| **Send** | Replay saved IR codes |
| **Delete** | Remove saved IR codes |

## 🎮 Other

| **Feature** | **Description** |
|------------|----------------|
| **Evil Portal** | Captive portal testing tool |
| **Pong** | Classic arcade game |
| **Breakout** | Brick breaker game |
| **About** | Creator information |
| **Splash Screen** | Custom boot logo |
| **EEPROM Storage** | Save RF and IR codes |

---

# 🛠 Hardware Requirements

| **Component** | **Description** |
|-------------|---------------|
| **ESP8266** | NodeMCU / Wemos D1 Mini |
| **OLED 0.96" I2C** | 128×64 Display |
| **433 MHz TX Module** | RF Transmission |
| **433 MHz RX Module** | RF Reception |
| **IR Receiver** | VS1838B / TSOP38238 |
| **IR LED + 2N2222** | IR Transmission |
| **3 Push Buttons** | Menu Navigation |

---

# 🔌 Wiring

| **Component** | **ESP8266 Pin** | **GPIO** |
|--------------|----------------|----------|
| **OLED SDA** | D2 | GPIO4 |
| **OLED SCL** | D1 | GPIO5 |
| **Button UP** | D5 | GPIO14 |
| **Button DOWN** | D6 | GPIO12 |
| **Button SELECT** | D7 | GPIO13 |
| **433 MHz TX DATA** | D0 | GPIO16 |
| **433 MHz RX DATA** | D4 | GPIO2 |
| **IR LED** | D8 | GPIO15 |
| **IR Receiver OUT** | D3 | GPIO0 |

> **Note:** All buttons use the internal pull-up resistors. Connect one side of each button to **GND** and the other side to the corresponding GPIO.

---

# 📦 Required Libraries

- **Adafruit SSD1306**
- **Adafruit GFX Library**
- **ESP8266WiFi**
- **rc-switch**
- **IRremoteESP8266**

---

# ⚡ Installation

1. Open **web.esphome.io**
2. Connect your **ESP8266** via USB
3. Click **Connect**
4. Select **FSociety_Tool.bin**
5. Set Flash Address to **0x0**
6. Click **Program**
7. Wait until flashing is complete

---

# 🎮 Controls

| **Button** | **Action** |
|-----------|-----------|
| **UP** | Navigate Up |
| **DOWN** | Navigate Down |
| **SELECT** | Confirm / Enter |
| **HOLD SELECT** | Exit Current Mode |

---

---

---

# ℹ️ About

**FSociety Tool** was created and developed by **Ahmadreza**.

---

# ⚠️ Disclaimer

This project is intended for educational and research purposes only.

The author is not responsible for any misuse, damage, or illegal activities resulting from the use of this software. Use it only on devices, systems, and networks that you own or have explicit permission to test.
