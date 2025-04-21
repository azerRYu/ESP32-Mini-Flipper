# Mini Flipper Zero (ESP32)

**An educational, ethical hacking project using an ESP32 board to simulate a Flipper Zero-style device.**

## Project Overview

This project aims to recreate some fun and educational features of the Flipper Zero using an ESP32 and basic electronic components. It is intended **for learning purposes only** (white-hat / ethical hacking).

## Hardware Components

- ESP32 board  
- 3.7V 1500mAh LiPo battery (external power on Wokwi)
- 0.96" OLED screen (SSD1306 I2C)  
- IR LED (transmitter)  
- IR receiver diode  
- Resistors (220Ω for LEDs, etc.)
- 4 push buttons:
  - Scroll  
  - OK  
  - Back  
  - Menu (shortcut to main menu)  
- Power ON/OFF switch  
- Status LED (to indicate power or activity)

## Menu Options

When powered on, the user is shown a simple menu using buttons and OLED display:

1. **IR Remote**  
   - Submenu:  
     - Power On  
     - Power Off  
     - Volume +  
     - Volume -  
     - Receive IR Code  
   - Sends common IR codes for TV brands (like LG, Samsung, Sony, etc.) using brute-force logic.  
   - Can also receive and store IR codes in a local history.

2. **Fake WiFi**  
   - Two modes:  
     - Predefined SSID list (e.g., "FreeWifi", "iPhone_14", "Police_Surveillance")  
     - Random fake SSID spammer (e.g., FakeWiFi_0000, FakeWiFi_1234...)  
   - These SSIDs will appear on nearby devices as if they are real Wi-Fi networks.

3. **WiFi Scan + Deauther**  
   - Scan all nearby Wi-Fi networks and display them on OLED  
   - Select one network and choose whether to launch a deauthentication attack.

4. **Deauther**  
   - Deauthenticates all Wi-Fi devices connected to nearby access points.  
   - Useful for testing and educational purposes (white-hat only).

5. **Fake Bluetooth**  
   - Displays fake Bluetooth pairing requests (AirPods, speakers, etc.) on nearby smartphones.

## Goals

- Learn about IR communication  
- Understand how WiFi scanning and packet injection work  
- Experiment with device spoofing and signal simulation  
- Build a physical interface (buttons + screen) similar to real tools like Flipper Zero

## Warning

This project is for **educational purposes only**. Do **not** use these tools to interfere with other people’s devices or networks without permission. All use must be ethical and legal according to your country’s laws.


