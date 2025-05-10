# Wled-project# ESP32 WS2811 LED Strip Controller

This project demonstrates how to control a **WS2811 addressable RGB LED strip** using an **ESP32 microcontroller**. It's ideal for creating vibrant lighting effects for DIY projects, home automation, or ambient displays.

## Features

* Powered by **ESP32** (Wi-Fi + Bluetooth enabled)
* Compatible with **WS2811**, **WS2812**, **SK6812**, and similar addressable LEDs
* Supports custom lighting animations (rainbow, breathing, chasing, etc.)
* Control via:

  * Web interface (hosted on ESP32)
  * MQTT / Home Assistant (optional)
  * Button input (optional)
* Adjustable brightness and speed
* 
## Hardware Required

* ESP32 Dev Board (e.g., NodeMCU-32S or ESP32-WROOM) https://www.hnhcart.com/products/esp32?_pos=3&_sid=7510b6217&_ss=r
* WS2811 LED strip (5V or 12V depending on your model) https://www.hnhcart.com/products/ws2811-60-leds-m-rgb-addressable-led-pixel-strip-light-12v-dc-programmable-non-waterproof?_pos=2&_sid=7cbe176eb&_ss=r
* Level shifter (optional for 5V LEDs) https://www.hnhcart.com/products/4-channel-bi-directional-logic-level-converter?_pos=2&_sid=d8f4d562f&_ss=r
* Power supply (match LED voltage and total current draw)

## Included

* Basic web UI for controlling effects
* Circuit diagram and connection guide 
---

Contributions are welcome! Feel free to fork, modify, and submit a pull request.



🚀 Getting Started
1. Wiring the Circuit
Components Needed:

ESP32 dev board

WS2811 LED strip (5V or 12V)

External power supply (match strip voltage)

(Optional) Level shifter (if using 5V LEDs with 3.3V ESP32)

Connections:

WS2811 Data In → ESP32 GPIO Pin (e.g., D27/ GPI27)

WS2811 GND → ESP32 GND

WS2811 VCC → External 5V/12V supply

ESP32 GND → External power supply GND (common ground is essential)
![circuit_image](https://github.com/user-attachments/assets/43cb977e-3c3f-4417-94c0-46a01654402f)


3. Open any web browser and go to:
👉 https://install.wled.me/
Wait for the installation process to complete.


5. Once installation is complete, the setup page will prompt you to enter your Wi-Fi credentials.

⚠️ Note: Make sure you connect to a 2.4GHz Wi-Fi network, as most ESP devices do not support 5GHz.

5. After the device connects to Wi-Fi, open your web browser and go to:
👉 http://192.168.0.121/
This will open the WLED control panel.

6. Navigate to Settings > LED Preferences > LED & Hardware Setup.
![Screenshot 2025-05-11 003631](https://github.com/user-attachments/assets/486fb894-0f41-46a8-9373-e179e183e92e)

Since I’m using a WS2811 LED strip, I selected WS281x from the LED type dropdown menu.

Under GPIO, I entered GPIO 27, as that’s the pin connected to the data line of the LED strip.
![Screenshot 2025-05-11 004417](https://github.com/user-attachments/assets/4713be2b-3b5c-4ac2-af7a-baa83940c2a1)

8. Running the Project

Access the web interface via that IP in your browser.

Control the LED strip and enjoy the effects!

You can also download Wled App and control using your phone.
![wled ](https://github.com/user-attachments/assets/d1ea62c0-7b39-4e1d-a449-c5131bf37a23)

![Screenshot 2025-05-11 002824](https://github.com/user-attachments/assets/9924b1a6-3ded-48a2-8475-536cd4d3d13a)
