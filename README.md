# Meshtastic-alt-il 📡
Community guide for configuring Meshtastic devices with our shared frequency, encryption, and network settings.


# Meshtastic Community Setup Guide 🌐

Welcome to our shared Meshtastic configuration project!  
This guide explains how to set up your device to join our community mesh network

# Disclaimer ⚠️
This guide is provided for community use only, for community educational purposes only.  
The authors and maintainers are not responsible for any device damage, interference, or legal issues arising from the use of these settings.
Always follow local regulations and use devices responsibl.
Participation in any shared network (like Telegram groups) is voluntary, and users should exercise caution and avoid sharing personal information.

## 🔍 What Is Meshtastic?

[**Meshtastic**](https://meshtastic.org/) is an open-source project that lets people communicate over long distances **without cellular or internet service** using **LoRa (Long Range) radios**.  

Each device acts as a **node** in a mesh network — messages hop automatically from one device to another, extending coverage across cities, trails, or remote areas.  

You can use Meshtastic for:
- Off-grid messaging between phones  
- Community emergency networks  
- Outdoor adventures and events  
- IoT and telemetry applications  

Meshtastic supports encrypted channels, but this community profile uses public channel settings and should not be treated as private. It remains **low-power** and **free to use** — no SIM card or subscription required.

---

## 📡 Overview

This document helps users configure their Meshtastic devices with:
- The correct frequency and modem settings
- Shared channel name and encryption
- Recommended hardware and power setups

---

## 🛠 Getting Started
Join out community
[💬 Telegram Group (requires admin approval)](https://t.me/+C4y1eP6NxwlhM2Y0)
### 1. Flash Your Device
Use the [Meshtastic Flasher](https://flasher.meshtastic.org/) to install the latest firmware.

### 2. Load Our Configuration
The Key for the OpenComm chanel will is pinned in the General topic in the telegram channel.

## ⚙️ Configuration Summary


| Parameter | Setting | Notes |
|------------|----------|-------|
| **Region** | United States | Set this in device settings |
| **Preset** | Medium Range - Fast (MediumFast) | Good balance of range and latency |
| **Frequency Slot** |  70 | Important: Use Frequency Slot 70 (919.375 MHz) for this network. |
| **Center Frequency** |  919.375 MHz |Important: Use Frequency Slot 70 (919.375 MHz) for this network. |
| **MQTT** | Disabled | Use only if you are a radio "island" and wish to be a mqtt "relay". |
| **MQTT** | MQTT Root Topic | msh/US/IL972 |
| **Transmission** |  Enabled | |
| **Max Hops** | 7 | Recommended for stable mesh performance |

## 🔗📊 Channels

Meshtastic channels can use encryption, but shared public keys do not provide private communication. Our community uses this channel configuration:

| Channel            | Description                  | Encrypted?                |
|--------------------|------------------------------|---------------------------|
| ***OpenComm***     | Used for general chatting | Yes |
| ***MediumFast***   | MediumFast channel | Public default key (not private) |





**Tips for Channels:**
- Adjust the number of hops depending on your network density.
- Do not modify frequency slots unless you are certain about local regulations.


## 📦 Recommended Mesh Devices for Starters

If you're new to Meshtastic, here are some popular and beginner-friendly devices that work well with our shared network settings:

| Device | Notes |
|--------|-------|
| **Seeed Wio Tracker L1** | Includes OLED display, GPS and a 5-way joystick. Based on NRF chip, much more power efficient. Very easy to flash, popular in the Meshtastic community. Great for outdoor use. Small and portable.|
| **Seeed SenseCAP Card Tracker T1000-E** | VERY small, VERY portable. Has a surprisingly good antenna for its size.|
| **Heltec WiFi LoRa 32 V3/V4** | Compact, includes OLED display, V3 has 0.96" OLED, V4 has updated board layout. No GPS, high battery comsumtion. |
| **Generic ESP32 + LoRa modules** | Requires a bit more DIY effort but very flexible for experimenting with mesh networks. |

**Tips for beginners:**
- Start with a **Heltec** — easiest to flash and widely supported.  
- Make sure to flash the **latest Meshtastic firmware** before joining the network.  
- Pair your device with the **Meshtastic mobile app** for easier configuration and monitoring.  
- **Important:** Always select the proper frequency for your region. Using the wrong frequency may be illegal or could interfere with other radio services.

##
