# 📘 FPGA Workshop – Day 3

## 🧠 Overview

Day 3 covers basic combinational circuits using switches as inputs and LEDs as outputs in PYNQ.

Topics covered:

* Half Adder
* Half Subtractor
* 4:1 Multiplexer

---

## 📂 Code Explanation

### 🔹 1. Setup

* `BaseOverlay('base.bit')` is used to access switches and LEDs
* LEDs are blinked at the beginning to check board working

---

### 🔹 2. Half Adder

* Takes two switch inputs
* Shows:

  * Sum on LED 0
  * Carry on LED 1

---

### 🔹 3. Half Subtractor

* Takes two switch inputs
* Shows:

  * Difference on LED 0
  * Borrow on LED 1

---

### 🔹 4. 4:1 Multiplexer

* Uses four switches as input lines
* Uses two switches as select lines
* Selected output is shown on LED 0

---

## ⚠️ Notes

* Programs run continuously in `while True`
* Stop execution using `Ctrl + C`

---
