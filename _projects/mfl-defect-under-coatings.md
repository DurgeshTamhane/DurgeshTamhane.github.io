---
title: "Detection of Defects in Steel Sheets Under Coatings using Magnetic Flux Leakage"
status: completed
date: 2025-08-21
description: "Term project report for the course CE 720: Non-Destructive Testing of Materials at IIT Bombay"
layout: single
collection: projects
author_profile: true
permalink: /projects/mfl-steel-under-coatings/
---

Steel structures are often protected with coatings to prevent corrosion. However, defects such as pits, cracks, or localized corrosion can develop **beneath these coatings**, compromising long-term durability. Traditional inspection methods often require **removing the coating**, which is labor-intensive, time-consuming, and may damage the surface.  

This project explores the use of **Magnetic Flux Leakage (MFL)** for *non-destructive detection of hidden defects* under coatings. MFL works by magnetizing a steel specimen and measuring flux "leakage" caused by discontinuities. This allows defect detection **without removing the coating**.

---

## Objectives
- Develop a methodology for detecting defects beneath coatings using MFL.  
- Study the influence of coating thickness and defect geometry on detection sensitivity.  
- Validate MFL signals against controlled artificial defects.  

---

## Experimental Setup
- **Specimens**: Mild steel sheets with artificial defects (notches and corrosion pits) introduced.  
- **Coatings**: Applied polymer-based coatings of varying thickness to simulate protective layers.  
- **Excitation**: A DC magnetizing yoke was used to induce flux into the specimen.  
- **Sensors**: A Hall effect sensor array scanned across the surface to measure flux leakage.  
- **Data Acquisition**: Signals were digitized and analyzed to extract leakage patterns.  

👉 *[Insert Figure of MFL setup here]*  

---

## Methodology
1. **Magnetization**: Steel plate was magnetized using a yoke, ensuring near-saturation magnetization.  
2. **Defect Simulation**: Artificial slots and pits were created on the steel surface before coating.  
3. **Coating Application**: Coatings of thickness ranging from ~100 μm to ~500 μm were applied.  
4. **Scanning**: The Hall sensor scanned over coated regions containing defects.  
5. **Signal Analysis**:  
   - Raw leakage signals were collected.  
   - Signal-to-noise ratios (SNR) were computed to evaluate detection limits.  
   - Signal shape (peaks, asymmetry) was compared with defect type.  

---

## Results
- **Clear Leakage Peaks**: Defects beneath coatings produced distinguishable peaks in the MFL signal.  
- **Effect of Coating Thickness**:  
  - Thinner coatings (≤200 μm) showed sharp, high SNR signals.  
  - Thicker coatings attenuated signals but defects remained identifiable.  
- **Defect Geometry Influence**:  
  - Wider notches produced broader leakage signals.  
  - Deeper pits gave stronger amplitudes, confirming MFL sensitivity to depth.  
- **Repeatability**: Multiple scans confirmed stability of measurements.  

👉 *[Insert Figures of sample signal graphs]*  

---

## Key Findings
- MFL can **reliably detect sub-surface defects** in steel sheets without removing protective coatings.  
- Coating thickness does reduce sensitivity but does not eliminate defect visibility up to ~500 μm.  
- The method is especially suitable for **in-field inspection of pipelines, tanks, and coated steel sheets**.  
- Compared to destructive methods, MFL offers a **fast, low-cost, and scalable** inspection solution.  

---

## Outcome
This study validated the feasibility of **non-destructive defect detection in coated steel** using Magnetic Flux Leakage. With optimization of sensor sensitivity and magnetization strength, the approach can be extended to **industrial-scale corrosion monitoring**.  

👉 *[Insert Figure: Summary schematic of defect detection workflow]*  

---


## Components

In this work, a sensitive Hall sensor (LIS2MDL) is used, which comes inbuilt with the microcontroller in **STMicroelectronics’s SensorTile.box**.

### About the LIS2MDL
The **LIS2MDL** is an ultra-low-power, high-performance 3-axis digital magnetic sensor with a dynamic range of ±50 gauss. It offers a 16-bit digital output, supports both SPI and I²C interfaces, includes a programmable interrupt generator, embedded self-test, and operates across −40 °C to +85 °C. ([LIS2MDL, STMicroelectronics, 2018](https://www.st.com/resource/en/datasheet/lis2mdl.pdf))

### About SensorTile.box
The **SensorTile.box (STEVAL-MKSBOX1V1)** is a ready-to-use wireless IoT and wearable sensor platform. It features multiple high-precision sensors—including the LIS2MDL magnetometer—integrated with Bluetooth connectivity, a rechargeable battery, and support for entry/expert application modes via the ST BLE Sensor app. ([SensorTile.box, STMicroelectronics, 2021](https://www.st.com/resource/en/data_brief/steval-mksbox1v1.pdf))


## Recommended Citation
<p style="font-size:0.85em; color:gray;">
Tamhane, D., <i>Detection of Defect in Steel Sheets Under Coatings by Magnetic Flux Leakage</i>.  
Term project report for CE 720: Non-Destructive Testing of Materials, IIT Bombay.  
Available at: <a href="https://durgeshtamhane.github.io/projects/mfl-steel-under-coatings/">https://durgeshtamhane.github.io/projects/mfl-steel-under-coatings/</a>
</p>

---

## BibTeX
```bibtex
@techreport{tamhane2025mfl,
  author       = {Tamhane, Durgesh},
  title        = {Detection of Defect in Steel Sheets Under Coatings by Magnetic Flux Leakage},
  institution  = {Indian Institute of Technology Bombay},
  year         = {2025},
  type         = {Term Project Report},
  note         = {Submitted as part of CE 720: Non-Destructive Testing of Materials},
  howpublished = {\url{https://durgeshtamhane.github.io/projects/mfl-steel-under-coatings/}}
}
