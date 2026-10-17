# 💡 Arduino LED Voltage Comparison (5V vs 3.3V)

![Arduino](https://img.shields.io/badge/Hardware-Arduino%20Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Tinkercad](https://img.shields.io/badge/Simulation-Tinkercad-05568C?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## 📌 Overview
This entry-level Mechatronics / Embedded Systems project demonstrates the fundamental electrical differences when driving an LED circuit through an **Arduino Uno** using two different voltage supply rails: **5V** and **3.3V**. 

The setup uses a push-button switch, a current-limiting resistor, and a red LED to safely analyze circuit behavior, voltage drop, and LED luminance differences.

---

## 🛠️ Components & Circuit Setup

### Hardware / Simulation Components
* **1x** Arduino Uno R3
* **2x** Breadboards (Half-size)
* **2x** Red LEDs
* **2x** Push-button Switches
* **2x** Current Limiting Resistors (220Ω)
* Jumper Wires

---

## 📊 Circuit Diagram & Schematic

### Breadboard Wiring View
![Circuit Diagram](docs/circuit-diagram.png)

### Circuit Schematic (5V vs 3.3V Rails)
> Detailed schematic diagram exported from Tinkercad is available in [`docs/schematic.pdf`](docs/schematic.pdf).

---

## ⚡ Key Observations

| Parameter | 5V Rail Configuration | 3.3V Rail Configuration |
| :--- | :--- | :--- |
| **Supply Voltage ($V_{in}$)** | $5.0\text{ V}$ | $3.3\text{ V}$ |
| **LED Forward Voltage ($V_f$)** | $\approx 2.0\text{ V}$ | $\approx 2.0\text{ V}$ |
| **Resistor Voltage Drop ($V_R$)** | $\approx 3.0\text{ V}$ | $\approx 1.3\text{ V}$ |
| **Circuit Current ($I$)** | Higher ($\approx 13.6\text{ mA}$) | Lower ($\approx 5.9\text{ mA}$) |
| **Perceived Brightness** | Maximum / High | Moderate / Low |

---

## 🚀 How to Replicate

1. Open [Tinkercad Circuits](https://www.tinkercad.com/).
2. Recreate the wiring as shown in the circuit diagram:
   * Connect the **Positive (+)** rail of Board 1 to Arduino **5V**, and Board 2 to **3.3V**.
   * Connect both **Negative (-)** rails to Arduino **GND**.
   * Place a Push-button inline with the LED and Resistor in series.
3. Press the pushbuttons on each circuit to observe and compare the LED brightness.

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
