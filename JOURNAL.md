---
title: "T-Smartwatch Journal"
author: "Mohammed Talha"
description: "Build log for a custom ESP32 smartwatch PCB designed using KiCad"
created_at: "2025-06-20"
total_time_hours: 28
---

# Journal – T-Smartwatch (ESP32 Smartwatch PCB)

## 🗓️ June 20 – Idea & Planning (2 hours)
Started thinking about building my own smartwatch PCB. I wanted to make something compact using ESP32 and include features like heart rate sensor, OLED display, and USB charging. I took notes from other open-source watch projects and decided to build one in KiCad.

## 🗓️ June 23 – Schematic Design & Part Research (3 hours)
Selected the major components – ESP32-WROOM, MAX30102 heart rate sensor, SSD1306 OLED, SI1317DL voltage regulator, and USB-C connector. Started building the schematic in KiCad and created custom symbols where needed.

## 🗓️ June 25 – Completed Schematic (2 hours)
Wired up power supply lines, decoupling caps, USB charging circuit, and I2C lines for OLED + sensor. Verified connections using datasheets.

## 🗓️ June 27 – Board Layout Started (3 hours)
Started arranging components and defining board shape. Opted for a rectangular layout. Set up 4-layer stack with separate ground and power planes. Placed USB and screen for user-accessibility.

## 🗓️ June 29 – Routing and Cleanup (3 hours)
Did most of the routing for power and signal lines. Kept traces short, used minimal vias, and ensured no DRC errors. Placed silkscreen text carefully.

<img width="760" height="756" alt="image" src="https://github.com/user-attachments/assets/7a4304ec-cf27-49a9-b235-e32f7b07df68" />
 
<img width="753" height="744" alt="image" src="https://github.com/user-attachments/assets/d47cac8a-fc1b-44aa-aeec-c0745e762aab" />


## 🗓️ July 2 – Final Touches on PCB (3 hours)
Added labels, cleaned routing paths, adjusted clearances. Verified power and ground fills. Ran design rule check and ERC.


## 🗓️ July 4 – 3D Render & Schematic Output (2 hours)
Generated 3D render using KiCad’s viewer and saved schematic as PDF. Took screenshots of all four PCB layers and final layout.


## 🗓️ July 6 – Case Design (2 hours)
Used online 3D box generator to design a basic smartwatch enclosure to match PCB size. Added cutouts for USB and screen.

## 🗓️ July 8 – Documentation and README (3 hours)
Wrote README from scratch describing what the board does and how it’s laid out. Listed all images and files. Verified schematic matches description.

## 🗓️ July 10 – Final Checks and Polish (3 hours)
Reviewed all files, checked BOM values and links. Wrote this journal, created LICENSE, and made sure everything is in the right format.

## 🗓️ July 11 – Submitted! (0 hours)
Submitted the final GitHub repo to Hack Club Highway and shared in #highway Slack channel.

---

**✅ Total Time Spent: 28 hours**
