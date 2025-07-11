# Talha Smartwatch – ESP32 PCB Project

This is a custom smartwatch project built using the ESP32 module. I designed a custom PCB for it using KiCad, with the goal of creating a compact, wearable board that supports a display, power management, and wireless features. The board is meant to serve as the core of a basic smartwatch.

## Blinky Test

As a first test, I ran a basic blink sketch to make sure the board powered on correctly and the ESP32 was working. The onboard LED blinked successfully.

![Blinky](images/blinky.gif)

## Schematic

This is the full schematic I created in KiCad. It includes the ESP32-WROOM module, power regulation, crystal, buttons, and headers for display and battery.

[![Schematic](images/esp32-smartwatch.png)](images/esp32-smartwatch.pdf)

## PCB Layer Views

The board is a 4-layer PCB. These are the individual layers exported from KiCad.

### All Layers (combined)

![All layers](images/all_layers.PNG)

### Top Layer - Signal

![Top layer](images/top_layer.PNG)

### Inner Layer 1 - Ground

![Inner layer 1](images/in1_GND.PNG)

### Inner Layer 2 - VCC and Signal

![Inner layer 2](images/in2_VCC.PNG)

### Bottom Layer - Signal

![Bottom layer](images/bott_layer.PNG)

## Files in this Repository

- `esp32-smartwatch.kicad_sch` – KiCad schematic file  
- `esp32-smartwatch.kicad_pcb` – KiCad PCB layout  
- `bom.md` – Bill of Materials  
- `JOURNAL.md` – Build journal with progress logs  
- `README.md` – Project description (this file)  
- `images/` – All PCB and schematic images  

---

Designed and built for Hack Club Highway  
Project by Mohammed Talha
