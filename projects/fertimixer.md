---
layout: project
type: project
image: img/fertimixer/FertigationPrototype.jpg
title: "Interactive Qualifying Project: Automated Fertilizer Mixing System"
# date: Jan 2024 – Mar 2024
start: 2024-01-01
end:   2024-03-31
published: true
labels:
  - Control Systems
  - IoT
  - Environmental Analysis
  - Prototyping
summary: "Designed a dual-tank fertigation prototype with a control system for NESS Fertigation, and analyzed its environmental impact using RIAM."
---

<figure class="text-center">
  <img class="img-fluid d-block mx-auto" src="{{ site.baseurl }}/img/fertimixer/FertigationProduct.png" alt="Dual tank fertigation prototype designed for NESS Fertigation.">
  <figcaption>
    Final prototype of the dual-tank solar-powered fertigation system, created for NESS Fertigation in Neot Semadar, Israel.
  </figcaption>
</figure>

## Project Overview
As part of our **Interactive Qualifying Project (IQP)** at WPI, our team collaborated with **NESS Fertigation** to improve their existing fertilizer mixing system. We designed and built a **solar-powered, fully automated dual-tank fertigation prototype** that increases scalability, reduces environmental impact, and minimizes operator input.  

The project was carried out remotely at **Venice, Italy**, in partnership with NESS Fertigation. Our final deliverables included a **working prototype**, a **design/user’s manual** for reproducibility, and a **Rapid Impact Assessment Matrix (RIAM)** to evaluate environmental benefits.

---

## Technical Contributions
- **Microcontroller System:** Developed using an **Arduino Nano ESP32-S3** and programmed in **C++**, with fault detection, deep sleep modes, and communication with SolTag controllers.
- **Valve Control:** Designed a dual-tank switching mechanism with **six solenoid valves** managed via **L298N motor drivers**, ensuring continuous operation by alternating filling and emptying cycles.
- **Sensors & Monitoring:** Integrated float sensors for tank level detection and implemented error reporting over analog signals for system reliability.
- **Power System:** Sized and tested a **solar panel system** to meet daily energy demand (~44 Wh/day), confirming that a single 30W panel could power the prototype.
- **Housing:** Designed and prototyped a weather-resistant, ventilated enclosure in **SolidWorks**, balancing passive cooling with protection against desert heat and rainfall.

---

## Environmental Impact
We conducted a **Rapid Impact Assessment Matrix (RIAM)** comparing our design against conventional fertilizer systems. Results showed:  
- Reduced fertilizer runoff and eutrophication risk.  
- Lower CO₂ emissions by using **solar energy** instead of diesel generators.  
- Improved scalability and ease of adoption in remote, resource-limited communities.  

---

## Deliverables
- 🌎 [Digital WPI Published Paper](https://digital.wpi.edu/concern/student_works/df65vc99v?locale=en)
- 📄 [Final IQP Report (PDF)]({{ site.baseurl }}https://digital.wpi.edu/downloads/sx61dr69z?locale=en)  
- 📄 [Design/User’s Manual (PDF)]({{ site.baseurl }}https://digital.wpi.edu/downloads/d791sm28b?locale=en)  
- 💻 [GitHub Repository](https://github.com/maximus-lazer/Fertigation-Mixing-Controller)  

---