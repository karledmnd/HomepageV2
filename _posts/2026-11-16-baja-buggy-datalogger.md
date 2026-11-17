---
title: "Baja Buggy Datalogger"
date: 2026-11-16 20:00:00 +0000
categories: [Projects]
description: "A custom datalogger PCB for a Baja buggy - GPS, IMU and suspension data on one board."
image:
  path: /assets/img/posts/datalogger.png
  alt: "3D render of the datalogger PCB"
author: false
---

## 📌 Project Overview

A datalogger PCB built for a Baja buggy. It records what the car is doing on track, so the driving data can be downloaded and looked at afterwards.

- **Primary Goal:** Log wheel speeds, suspension travel, driver inputs, GPS and IMU data to onboard memory.
- **Tech Stack:** KiCad, ESP32-S3, u-blox MAX-M10S, LSM6DSL.
- **Status:** In development - component placement & routing in progress.

---

## 🛠️ Key Specifications & Hardware Architecture

| Feature | Details / Components |
| :--- | :--- |
| **Microcontroller** | ESP32-S3-MINI-1 |
| **GPS** | u-blox MAX-M10S with external SMA antenna |
| **IMU** | LSM6DSL 6-axis accelerometer & gyroscope |
| **Analog Inputs** | 2x ADS1115 - suspension travel, brake pressure, pedal & steering position |
| **Wheel Speed** | 4x pulse inputs |
| **Storage** | Onboard SPI NOR flash (no SD card) |
| **Power** | 12V input with buck converter to 3V3 |

---

## ⚙️ Design & Implementation Details

### Still a work in progress. Check back soon <3
