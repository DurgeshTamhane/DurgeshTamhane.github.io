---
layout: single
title: "Detection of Defects in Steel Sheets Under Coatings by Magnetic Flux Leakage (MFL)"
collection: projects
permalink: /projects/mfl-steel-under-coatings/
author_profile: true
header:
  teaser: /images/projects/mfl-steel-under-coatings.jpg   # optional: replace with your image
status: completed
tags: [NDE, MFL, steel, coatings, sensors, low-cost]
---

A low-cost Magnetic Flux Leakage (MFL) scanner detects hidden discontinuities in steel sheets even when they’re covered by millimeter-scale coatings—useful for tanks, pipelines, and white-goods panels where corrosion/defects hide under paint or cladding. :contentReference[oaicite:0]{index=0}

## Overview
The device couples two small neodymium magnets to a microcontroller board with an in-built LIS2MDL magnetometer, streaming three-axis magnetic data to a phone over Bluetooth for live scan visualization and logging. The magnetometer’s ±50 G range and compact form factor keep the system inexpensive and portable. :contentReference[oaicite:1]{index=1}

## Why MFL?
Defects (gaps, wall loss) disturb the otherwise uniform magnetic flux in a magnetized ferromagnetic sheet; the leaked field above the defect is picked up by a magnetic sensor—no powders or consumables required, unlike classic magnetic particle testing. :contentReference[oaicite:2]{index=2}

## Method & Hardware
- **Magnetization:** Two permanent magnets mounted on the scanner induce flux into the steel. A COMSOL model confirms adequate flux paths in the sheet stack-up. :contentReference[oaicite:3]{index=3}  
- **Sensing:** Onboard LIS2MDL magnetometer (three axes, ±50 G). Data rate set to ~2 samples/s; scan speed must be slow enough not to outrun sampling. :contentReference[oaicite:4]{index=4}  
- **Interface:** Bluetooth link to a phone for live display and storage. :contentReference[oaicite:5]{index=5}

## Experiments
Two 1 mm carbon-steel sheets were placed on a flat surface; the electrical/mechanical gap between them was varied to emulate a defect. Scans were repeated with different coatings atop the sheets: paper (~1.4 mm), plywood (~4 mm, then stacked to 8 mm and 12 mm), rubber (~2 mm; stacked to ~4 mm), dense cardboard (~3 mm), and mixed stacks (10.4 mm and 30.4 mm total). :contentReference[oaicite:6]{index=6}

## Results
- **Defect sensitivity:** Measured leakage increased with defect size; while not strictly linear, the trend was directly proportional. :contentReference[oaicite:7]{index=7}  
- **Through-coating detection:** Discontinuities were detected beneath single coatings and mixed stacks up to **30.4 mm** total thickness. :contentReference[oaicite:8]{index=8}  
- **Baselines vary by coating:** Background levels shift across materials; detection should rely on the absolute change within each coating condition rather than comparing to a no-coating baseline. :contentReference[oaicite:9]{index=9}

## Key Takeaways
- Portable, inexpensive MFL tool for concealed defects in steel sheet applications. :contentReference[oaicite:10]{index=10}  
- Works under a range of common coatings (paper, wood, rubber, cardboard) and mixed stacks to several centimeters. :contentReference[oaicite:11]{index=11}  
- Practical guidance: keep scanning speed within the sensor’s sampling limit (~2 Hz in tests) to avoid missing features. :contentReference[oaicite:12]{index=12}

## Project Notes
Term project report for **CE 720: Non-Destructive Testing of Materials**. For figures (apparatus, scans, and COMSOL field plots), extract images from the report and save them under `/images/projects/mfl-steel-under-coatings/`—then add them to this page as needed. :contentReference[oaicite:13]{index=13}
