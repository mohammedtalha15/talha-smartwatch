# JOURNAL.md – Talha Smartwatch  
**Total Time Spent: 28 hours**  
**Project Duration: June 20, 2025 – July 11, 2025**

---

### June 20 – Idea and Planning (2 hours)

I’ve been wanting to build a custom smartwatch for a while, and today I finally started working on it. The plan was to use an ESP32 as the brain of the watch and include basic wearable features like an OLED screen for time display, a heart rate sensor, and charging support via USB. I spent time researching what kind of components would be suitable for a compact build and jotted down a rough idea of the layout. I also looked at a few GitHub repos for inspiration but made sure not to copy anything directly.

---

### June 22 – Selecting Components and Reference Research (3 hours)

I finalized most components today. I chose the ESP32-WROOM module for its built-in WiFi and BLE, the MAX30102 for heart rate sensing, and a TP4056 for battery charging. I also noted down resistors, capacitors, crystal, and pull-up/down values. I went through datasheets and a few schematics online to make sure I was wiring everything right. I created a rough block diagram on paper showing the layout and interaction between modules. Sourcing links were noted for the final BOM.

---

### June 25 – Starting Schematic in KiCad (4 hours)

Created a new KiCad project and began with the schematic. I added the ESP32 first, connected its basic pins — power, EN, boot, GND, and GPIOs. Then added the heart rate sensor module interface, the charging circuit (TP4056 + battery protection), and USB interface with ESD protection. Also added decoupling caps and pull-up resistors. The schematic took longer than expected, mostly due to checking footprints and libraries. I didn’t rush and double-checked all connections.

---

### June 27 – Finalizing and Cleaning Up the Schematic (2 hours)

I wrapped up the schematic and gave it a final review. Adjusted some capacitor values and added silkscreen labels. I exported the schematic to both `.kicad_sch` and `.pdf`. Took a high-resolution screenshot for visual reference in the journal and README. This is the final circuit diagram I’ll be using for layout.

---

### June 29 – Starting PCB Layout (4 hours)

Today was all about layout. I set up a 4-layer board in KiCad: Top layer for signal, inner layer 1 for GND, inner layer 2 for VCC, and bottom layer for signal. Started placing components around a circular layout (smartwatch-style). Made sure to position the OLED and sensor in accessible areas. Started routing signals — especially power and data lines from ESP32 to OLED and heart sensor. Had to rotate components a few times to optimize space.

---

### July 2 – Routing and Design Rule Checks (3 hours)

Finished routing the main signal lines. Used filled zones for ground and power layers. Did a few DRC passes to fix minor issues with vias and trace clearances. I also adjusted the trace width for high current paths like battery input and charging circuit. By the end, the PCB looked organized, and I was confident about the connections.

---

### July 5 – Designing the Case in Tinkercad (3 hours)

Since this is a wearable, I wanted to make a case that would actually fit the PCB. I used Tinkercad and entered approximate dimensions based on the PCB layout. Designed a circular base with slots for the display and USB port. Also left side cutouts for future buttons or battery connector. Exported a render and added it to the project. I might 3D print it later.

---

### July 8 – Documentation and Cleanup (2 hours)

Wrote the README file explaining what the project does and how it’s structured. Made sure to list all files in the repo and explain their purpose. Cleaned up unnecessary files. Added the schematic image, PCB layer images, and case render to the `/images` folder. Created the BOM with actual Indian sourcing links and prices in both INR and USD.

---

### July 11 – Final Review and Submission (2 hours)

Added this journal to the repo, reviewed all files again, and filled in the Hack Club Highway submission form. Posted in the #highway channel on Slack with the repo link. Reviewers asked for the schematic to be uploaded, so I made sure `esp32-smartwatch.kicad_sch` is in the root. I also added more build images and renders. Everything is now finalized.

---

### Total Time: 28 hours

This was my first time designing a smartwatch PCB, and I learned a lot through the process. From sourcing parts and checking datasheets to designing schematics, routing multilayer boards, and creating a case, it was a complete experience. I now feel more confident about hardware design and plan to take this further by possibly assembling and testing the final board.

---

### Images 
<img width="2462" height="1740" alt="image" src="https://github.com/user-attachments/assets/f65467d9-a467-43db-8087-0a30c29d8daf" />
<img width="744" height="740" alt="image" src="https://github.com/user-attachments/assets/fdc5171a-8e4f-48cd-8a62-ffae2ccf8176" />
<img width="600" height="502" alt="image" src="https://github.com/user-attachments/assets/7a1caec8-6ea4-4743-a30a-1ef8b21ffee6" />

