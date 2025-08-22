---
title: "Detection of Wheel Misalignment Using Magnetic Sensors"
permalink: /projects/wheel-misalignment-detection/
layout: single
collection: projects
status: completed
author_profile: true
date: 2023-12-10
description: "A low-cost magnetic sensor-based system to detect camber and toe misalignment in wheels."
---

## Introduction
This project explores a **magnetic sensor-based technique for detecting wheel misalignment**, focusing on **toe** and **camber** angles. Misalignment can affect vehicle performance, safety, and tire wear. Traditional alignment machines are bulky and expensive. This work demonstrates how a compact magnetometer setup can reliably measure misalignments.

## Experimental Setup
A custom apparatus was developed to hold the wheel and allow controlled misalignment in both toe and camber orientations. A permanent magnet was mounted on the rim while a **magnetometer** was positioned strategically to capture variations in magnetic flux as the wheel rotated (Fig. 1).  
The setup allowed repeatable introduction of misalignment angles and real-time data acquisition.

![Experimental apparatus](/files/projects/images/WHEEL_APPA.png)  
*Fig. 1. Experimental setup for measuring toe and camber misalignments.*

## Magnetometer Calibration
To establish the sensor’s response, the magnetic field was recorded as a function of the distance from the magnet. As expected, the field intensity decayed exponentially with distance, and the curve fitting achieved an excellent coefficient of determination ($R^2 = 0.99973$) (Fig. 2).

![Magnetic field vs distance](/files/projects/images/b_VS_DIST.png)  
*Fig. 2. Magnetic field decay with distance from the magnet.*

## Data Acquisition and Signal Features
The magnetometer recorded the vertical field component ($B_z$) as the wheel rotated. Distinct positive and negative peaks were observed corresponding to each pass of the magnet near the sensor (Fig. 3). These signal features provided markers for alignment evaluation.

![Magnetic field vs time](/files/projects/images/b_VS_TIME.png)  
*Fig. 3. Time-series signal showing peaks in $B_z$ as the wheel rotates.*

## Misalignment Detection
By introducing known toe and camber misalignments, clear correlations were established between the misalignment angle and the magnetic field magnitude. Polynomial fits showed strong agreement with the experimental data (Fig. 4).  
- **Toe Misalignment:** Both left and right toe misalignments led to systematic changes in $B_y$.  
- **Camber Misalignment:** Increasing camber misalignment also reduced the field magnitude in a predictable fashion.

![Magnetic field vs misalignment angles](/files/projects/images/MAG_DEGRESS.png)  
*Fig. 4. Effect of toe and camber misalignments on the measured magnetic field.*

## Results and Discussion
- The sensor readings demonstrated **high repeatability** and strong correlation with the imposed misalignments.  
- The low-cost setup achieved a sensitivity suitable for detecting even small degrees of misalignment.  
- Compared to conventional alignment machines, this system is **portable, affordable, and scalable**.

## Conclusion
This project demonstrated a proof-of-concept for detecting wheel misalignment using magnetic sensors. With further refinement, such systems could enable affordable alignment checks outside specialized workshops, improving vehicle safety and reducing tire wear.

---

## Citation

**Harvard Style**  
Tamhane, D., 2023. *Detection of Wheel Misalignment Using Magnetic Sensors*. Term project report for CE 720: Non-Destructive Testing of Materials, IIT Bombay. Available at: <https://durgeshtamhane.github.io/projects/wheel-misalignment-detection/>

**BibTeX**  
```bibtex
@misc{tamhane2023wheel,
  author       = {Tamhane, Durgesh},
  title        = {Detection of Wheel Misalignment Using Magnetic Sensors},
  year         = {2023},
  note         = {Term project report for the course CE 720: Non-Destructive Testing of Materials, IIT Bombay},
  howpublished = {\url{https://durgeshtamhane.github.io/projects/wheel-misalignment-detection/}}
}
