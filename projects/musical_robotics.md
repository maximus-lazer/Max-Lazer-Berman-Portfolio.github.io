---
layout: project
type: project
image: img/musical_robotics/EMGuitar.jpg
title: "Musical Robotics: Electromagnetic Guitar"
start: 2024-10-01
end:   2024-12-12
published: true
labels:
  - Arduino
  - Capacitive Sensing
  - Electromagnets
  - Musical Robotics
summary: "Created a self-contained electromagnetic guitar (EM Guitar) using Arduino, capacitive sensors, and electromagnets, enabling infinite sustain and new playing techniques."
---

<figure class="text-center">
  <img class="img-fluid d-block mx-auto" src="{{ site.baseurl }}/img/musical_robotics/EMGuitar.jpg" alt="Prototype of the EM Guitar with electromagnets and capacitive touch inputs.">
  <figcaption>
    Final prototype of the EM Guitar project for HU 3910: Musical Robotics.
  </figcaption>
</figure>

## Project Overview
As part of **HU3910: Musical Robotics**, our team (Curtis Soloff, Max Berman, AJ Berry) created the **Electromagnetic Guitar (EM Guitar)**. The system uses **capacitive touch fret and string sensors**, an **Arduino Uno**, and **six electromagnets driven by MOSFET boards** to generate infinite sustain and enable new styles of guitar performance. Unlike earlier projects or products (e.g., EBow, Sustainiac), our design is **self-contained**, supports **all six strings**, and allows **chords as well as single notes**.

---

<figure class="my-3 text-center">
  <iframe src="https://drive.google.com/file/d/1jW7DCQU8hoFSQ5Fff46fuOKCQ8pf-471/preview"
          width="720" height="480" allow="autoplay"></iframe>
  <figcaption class="text-muted mt-2">
    Performance piece featuring the EM Guitar and other musical robots, composed and recorded for HU3910: Musical Robotics.
  </figcaption>
</figure>

---

## Design & Implementation
- **Inputs:** Capacitive touch (MPR121 I²C boards) read copper tape frets and per-string pads, allowing flexible detection without bulky switches.  
- **Signal Generation:** The Arduino Uno computes note frequencies from string + fret inputs and outputs square waves using the internal clock. To balance volume, duty cycles varied by string (50% for high strings, 30% for A, 20% for low E).  
- **Electromagnet Drive:** Arduino outputs switch two **Mosfetti 4-channel MOSFET boards**, powering **six Adafruit P20/15 electromagnets** from a 5V USB battery bank. Adjustable 3D-printed mounts and spacers set magnet height.  
- **Audio Output:** Used **piezo pickups** instead of magnetic ones to avoid interference from the drive signals; preamp or pedal recommended for clean amplification.  
- **Power:** Powered entirely by an **Anker PowerCore MetroEssential 20000** USB battery bank, keeping the system portable and self-contained.  

---

## Results
- Achieved **infinite sustain** without string attack, producing a unique, organ-like sound.  
- Supported **simultaneous excitation of multiple strings** with mapped fret/string inputs, enabling chordal play.  
- Fully **portable design**: just plug the Arduino and MOSFET boards into the battery pack.  
- **Challenges:** occasional stuck capacitive sensors, piezo requiring high amplification, and limited dynamic control (volume tied to duty cycle, not real-time).  

---

## Modifications & Extensions
- Expanded to **12 frets of capacitive sensing** via daisy-chained MPR121 boards.  
- Integrated **electronics beneath a custom clear acrylic pickguard**, showcasing the system’s internals.  
- Code extended to **map multiple frets across multiple strings**, allowing power chords and more complex shapes.  
- Future work: per-string per-fret sensing, pressure-sensitive inputs for dynamic control, and Fourier-based auto-tuning of electromagnet signals.  

---

## Recognition
The EM Guitar was also prepared in **NIME (New Interfaces for Musical Expression) conference format**, demonstrating the project’s viability as a novel instrument design.

---

## Media & Links
- 📄 [Final Paper (PDF)]({{ site.baseurl }}/img/musical_robotics/HU 3910 Final Paper.pdf)
- 📄 [NIME-Format Submission (PDF)]({{ site.baseurl }}/img/musical_robotics/HU 3910 Final Paper NIME EM Guitar.pdf)    
- 💻 [GitHub Repository](https://github.com/DayDoubloon/HU-3910-EM-Guitar)  
