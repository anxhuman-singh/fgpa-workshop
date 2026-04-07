# 📘 FPGA Workshop – Day 2

## 🧠 Overview

This project demonstrates basic digital logic operations using an FPGA board with the PYNQ framework. The program reads input from switches and controls LEDs based on logical operations such as AND, OR, NOR, and NAND.

---

## 🎯 Objectives

* Interface with FPGA hardware using Python
* Read switch inputs
* Perform logic operations
* Control LEDs based on results

---

## 🛠️ Requirements

* PYNQ-supported FPGA board (Zynq-based)
* Python with `pynq` library
* Base overlay file (`base.bit`)

---

## 📂 Code Description

### 1. Load Base Overlay

Loads the FPGA configuration and gives access to LEDs and switches.

### 2. LED Initialization

* Turns all LEDs ON briefly
* Then turns them OFF
* Acts as a startup indicator

### 3. Continuous Execution

* Reads two switches
* Performs logic operations
* Updates LEDs accordingly

---

## ⚙️ Logic Operations

| Operation | Expression                | Description                       |
| --------- | ------------------------- | --------------------------------- |
| AND       | `switch1 & switch2`       | True only if both switches are ON |
| OR        | `switch1 or switch2`      | True if at least one switch is ON |
| NOR       | `not(switch1 or switch2)` | True if both switches are OFF     |
| NAND      | `not(switch1 & switch2)`  | True if not both are ON           |

---

## 💡 LED Mapping

| LED   | Function | Behavior                          |
| ----- | -------- | --------------------------------- |
| LED 0 | AND      | ON when both switches are ON      |
| LED 1 | OR       | ON when at least one switch is ON |
| LED 2 | NOR      | ON when both switches are OFF     |
| LED 3 | NAND     | ON when NOT both switches are ON  |

---

## 🖨️ Console Output

The program prints:

* Logic results (OR, NAND)
* Status messages such as:

  * `output = and true`
  * `output = or true`
  * `output = not true`
  * `output = false (invalid)`

---

## ⚠️ Notes

* The program runs in an infinite loop (`while True`)
* Stop manually using `Ctrl + C`

---

## ▶️ How to Run

```bash
python main.py
```

---

## 📌 Future Improvements

* Add proper XOR logic
* Improve output messages
* Add GUI or display support
* Implement switch debouncing

---

## 👨‍💻 Author

Anshuman Singh