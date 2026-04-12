# 📘 FPGA Workshop – Day 5

## 🧠 Overview

Day 5 implements a 4-bit shift register using the PYNQ-Z2 buttons and LEDs.

---

## 📂 Code Explanation

### 🔹 1. Setup

* `BaseOverlay('base.bit')` loads the FPGA design
* A 4-bit `state` list stores the register contents

---

### 🔹 2. Displaying the State

* LEDs 0–3 show the current `state`
* The console prints the state after each update

---

### 🔹 3. Button Controls

* Button 0: shift right, insert `0` at MSB
* Button 1: shift left, insert `1` at LSB
* Button 2: shift left, insert `0` at LSB
* Button 3: shift left, insert `0` at LSB

---

## ⚠️ Notes

* The program runs continuously (`while True`)
* Button press is handled using a simple release wait
* Stop execution using `Ctrl + C`

---
