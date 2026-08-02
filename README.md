# TPS54332-Step-Down-Buck-Converter-Board
KiCad PCB design, schematic, and design files for a TPS54332-based step-down buck converter circuit.
# ⚡ TPS54332 Step-Down Buck Converter Board

This repository contains the complete KiCad design files, Gerber output files, datasheets, interactive BOM, 3D STEP models, and schematic for a compact, high-efficiency Step-Down (Buck) DC-DC Converter module based on the **Texas Instruments TPS54332** IC.

---

## 📌 Project Overview
* **IC Model:** Texas Instruments TPS54332DDAR
* **Input Voltage Range:** 3.5V to 28V
* **Output Voltage:** Adjustable (Configured via feedback resistors)
* **Continuous Output Current:** Up to 3.5A
* **Switching Frequency:** 3.5MHz
* **Design Tool:** KiCad 10.0

---

## 🛠️ Key Features
* **High Efficiency:** Integrated 80mΩ high-side MOSFET for efficient power conversion.
* **Adjustable Output:** Voltage divider network with precision resistors and potentiometer options.
* **Protection Features:** Internal eco-mode, pulse-by-pulse current limiting, thermal shutdown, and overvoltage protection.
* **Optimized Layout:** Low-ESR ceramic capacitor placement and solid ground plane routing for minimal output ripple and noise.

---

## 📐 Design Calculations & Output Voltage Setup

The output voltage ($V_{out}$) of the TPS54332 is configured using the feedback resistor divider ($R_1$ and $R_2$) connected to the **VSENSE** pin.

### Formula:
$$V_{out} = V_{ref} \times \left(1 + \frac{R_1}{R_2}\right)$$

Where:
* $V_{ref} = 0.8 \text{ V}$ (Internal Reference Voltage of TPS54332)
* $R_1$: Top feedback resistor
* $R_2$: Bottom feedback resistor / potentiometer

---

## 📁 Repository Structure
```text
├── 2026-07-27_B-TPS54332-BRK_R0.1.zip   # Complete project package containing all design & output files
