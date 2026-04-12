# 📘 FPGA Workshop – Day 4

## 🧠 Overview

Day 4 focuses on implementing counters on the PYNQ-Z2 board and displaying the count on LEDs.

---

## 📂 Code Explanation

### 🔹 1. Setup & Initialization

* `BaseOverlay('base.bit')` loads the FPGA design
* LEDs are blinked at the start to verify board operation

---

### 🔹 2. Basic Counter (0–15)

* A counter runs from `0` to `15`
* Each bit of the counter is mapped to LEDs 0–3
* LEDs show the binary value of the counter

---

### 🔹 3. Switch-Controlled Counter

* The counter runs only when `switches[0]` is ON
* LEDs update every second to show the count
* When the switch is OFF, the counter stops

---

## ⚠️ Notes

* The second program runs in an infinite loop (`while True`)
* Stop execution using `Ctrl + C`

---
