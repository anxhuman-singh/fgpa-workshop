# 📘 Mini Hackathon

## 🧠 Overview

This mini hackathon project is a simple **signed calculator** built on the **PYNQ-Z2** board.

It uses:

* 2 switches to choose input values
* 4 push buttons to control the calculator
* 4 LEDs to display the result

---

## ⚙️ Working

The project stores two values:

* `A`
* `B`

The switches are used to select a signed input value, and the buttons are used to save values, change operation, and compute the result.

Supported operations:

* Addition
* Subtraction
* Multiplication
* Division

---

## 🔹 Button Functions

* `BTN0` -> Change input mode between `A` and `B`
* `BTN1` -> Capture the value from switches
* `BTN2` -> Change operation
* `BTN3` -> Compute and display result

---

## 🔹 Input Values

The 2 switches are used to generate signed values.

Possible values:

* `00` -> `0`
* `01` -> `1`
* `10` -> `-2`
* `11` -> `-1`

---

## 💡 Output Display

The result is shown on 4 LEDs:

* LED 0 to LED 2 show the magnitude
* LED 3 shows the sign

If the result is negative, the sign LED turns ON.

---

## ⚠️ Notes

* The program runs continuously
* Button press detection is event-based
* Division by zero is handled by showing `0`
* Output range is limited before displaying on LEDs

---
