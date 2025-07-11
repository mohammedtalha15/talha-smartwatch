---
title: "ESP32 Smartwatch"
author: "Mohammed Talha (mohammedtalha15)"
description: "A custom-built ESP32-based smartwatch PCB with display, power management, and sensors."
created_at: "2025-06-20"
total_time_hours: 28
---

# Journal – ESP32 Smartwatch PCB

## Week 1 – Planning & Research (5 hours)

I wanted to build something wearable and practical — that’s how I got the idea for making my own smartwatch. I explored some community projects and references like the open-smartwatch repo and checked what chips and displays were commonly used. I decided I would base mine around the ESP32 for its versatility and WiFi/Bluetooth features.

I finalized that this project would include a display (for showing time, sensor values, etc.), a Li-ion battery with charger circuit, and minimal buttons. I also made a rough list of required components and functionalities I’d need.

---

## Week 2 – KiCad Setup & Schematic Design (6 hours)

This week I set up KiCad and began building the schematic. I created the full block diagram for how the ESP32 would connect to the rest of the components: display (via SPI), push buttons, charging circuit (TP4056), and a voltage regulator.

I added custom symbols and footprints to the KiCad library and started routing the schematic using proper decoupling capacitors and GPIO mapping. I kept everything neat so the PCB process would be smoother later.

---

## Week 3 – PCB Layout & Routing (7 hours)

With the schematic done, I moved on to laying out the board in KiCad. I spent quite a bit of time getting the placement right since I was aiming for a compact layout that could fit inside a small smartwatch enclosure.

I did a 4-layer board (Signal, GND, VCC, and Signal bottom) to keep things clean. I added mounting holes, adjusted track widths, added ground fills, and made sure impedance-critical traces were fine. Also had to fix a few DRC warnings.

By the end of the week, I had the PCB design ready.

---

## Week 4 – BOM Finalization & Gerber Generation (5 hours)

I finalized the Bill of Materials this week — listing all the components with part numbers and sourcing options. I optimized the BOM to make sure the components I picked were available either on LCSC, Mouser, or Amazon India.

Then I generated all the required Gerber files, added assembly files (positions.csv, designators.csv), and exported a 3D render of the board using KiCad.

I reviewed the board again before uploading everything to GitHub and ensured all schematic + layout files were properly organized.

---

## Week 5 – Documentation & Final Touches (5 hours)

I wrote the README.md clearly explaining each layer of the board with screenshots. I included:

- Blinky test GIF
- Schematic preview
- PCB layer screenshots

I also added a LICENSE file, detailed BOM with INR/USD prices and links, and this journal file. After confirming all repo files were in place, I pushed everything and prepared for submission to Hack Club’s Highway program.

---

**Total Time Spent: 28 hours**


This was one of the most challenging but rewarding PCB projects I’ve done so far. I learned a lot about KiCad, PCB design, and power management circuits. Looking forward to actually assembling and testing this soon.
<img width="744" height="740" alt="image" src="https://github.com/user-attachments/assets/a9156b50-22ed-4ea7-8833-5c0ff35d946e" />

