# Electronics Portfolio — Physics Guide Series

**Author:** Xaqani Ceferli · Baku, Azerbaijan · 2026  
**Verified by:** Telman Askeraliyev — Physics Teacher, Azerbaijan (Fizika Müəllimi)  
[![Academia](https://img.shields.io/badge/Academia.edu-Profile-blue)](https://www.academia.edu)
[![SlideShare](https://img.shields.io/badge/SlideShare-Presentations-orange)](https://www.slideshare.net)
[![YouTube](https://img.shields.io/badge/YouTube-Videos-red)](https://www.youtube.com)

---

## Index

| # | Title | Links | Type |
|---|-------|-------|------|
| 01 | [Field Effect Transistors](#01--field-effect-transistors) | Academia · SlideShare | Physics Guide |
| 02 | [Amplifiers & Applications](#02--amplifiers--applications) | Academia · SlideShare | Physics Guide |
| 03 | [BJT Transistor](#03--bjt-transistor) | SlideShare | Lab Report |
| 04 | [Capacitor — Visual Guide](#04--capacitor--visual-guide) | SlideShare | Visual Guide |
| 05 | [Voltage Divider](#05--voltage-divider) | SlideShare | Physics Guide |
| 06 | [Azerbaijan Electronics Market](#06--azerbaijan-electronics-market) | SlideShare | Market Analysis |
| 07 ⭐ | [Tilt Sensor Alarm System](#07--tilt-sensor-alarm-system) | Academia · SlideShare · YouTube | Lab Report + Video |

---

## 01 — Field Effect Transistors

**JFET & MOSFET — Structure, Biasing, and Characteristics** · 13 pages

Covers JFET and MOSFET structure, operating regions, biasing circuits, key parameters, and device comparison. Includes worked calculation problems and exam-style exercises.

### Key Equations

| Quantity | Formula |
|----------|---------|
| Shockley equation (JFET saturation) | `I_D = I_DSS × (1 − V_GS / V_P)²` |
| Transconductance | `g_m = (2 × I_DSS / \|V_P\|) × (1 − V_GS / V_P)` |
| E-MOSFET saturation current | `I_D = k × (V_GS − V_T)²` |
| Conduction parameter | `k = I_D(on) / (V_GS(on) − V_T)²` |
| On-resistance (Ohmic region) | `r_DS(on) = V_DS / I_D` |
| JFET self-bias | `V_GS = −I_D × R_S` |
| Voltage-divider gate voltage | `V_G = V_DD × R2 / (R1 + R2)` |

### JFET vs MOSFET Comparison

| Property | JFET | E-MOSFET | D-MOSFET |
|----------|------|----------|----------|
| Gate insulation | PN junction (reverse biased) | SiO₂ oxide layer | SiO₂ oxide layer |
| Input impedance | ~10⁷ Ω | ~10¹⁴ Ω | ~10¹⁴ Ω |
| Channel at V_GS = 0 | ✅ ON | ❌ OFF | ✅ ON |
| V_GS polarity (N-ch) | 0 to negative | Must be positive (> V_T) | Positive or negative |
| Zero bias possible? | No | No | Yes |
| Gate current | Very small leakage | Almost zero | Almost zero |
| Main use | Low-noise analog amplifiers | Digital circuits, power switching | Analog amplifiers |

---

## 02 — Amplifiers & Applications

**Gain, Classes, Feedback, and Op-Amp Configurations** · 16 pages

Covers amplifier theory from basic gain to Op-Amp configurations, amplifier classes, frequency response, and negative feedback. Includes real-world applications from smartphones to ECG machines. References AQA / OCR / Edexcel A-Level specifications.

### Key Equations

| Quantity | Formula |
|----------|---------|
| Voltage gain | `A_V = V_out / V_in` |
| Power gain | `A_P = P_out / P_in` |
| Voltage gain in dB | `A_dB = 20 × log₁₀(A_V)` |
| Bandwidth | `BW = f_H − f_L` |
| Closed-loop gain (neg. feedback) | `A_CL = A / (1 + A·β)` |
| Inverting Op-Amp gain | `A_V = −R_f / R_in` |
| Non-inverting Op-Amp gain | `A_V = 1 + (R_f / R_in)` |
| Gain–Bandwidth product | `GBW = A_V × BW = constant` |

### Amplifier Classes

| Class | Conduction Angle | Efficiency | Distortion | Typical Use |
|-------|-----------------|------------|------------|-------------|
| A | 360° (full cycle) | ≈ 25% | Very low | Hi-fi audio, mic preamps |
| B | 180° (half cycle) | ≈ 78% | High (crossover) | Push-pull power stages |
| AB | 180°–360° | ≈ 50–70% | Low | Most audio power amps |
| C | < 180° | > 90% | Very high | RF transmitters |
| D | Switching (PWM) | ≈ 90–98% | Low (filtered) | Phones, Bluetooth, subwoofers |

---

## 03 — BJT Transistor

**Switch, Amplifier, NPN vs PNP** · 11 pages — Technical Lab Report

Covers BJT semiconductor basics, three-terminal operation, switch mode (saturation / cut-off), amplifier mode with current gain, NPN vs PNP comparison, and real-world applications.

### Key Equations

| Quantity | Formula |
|----------|---------|
| Current gain (hFE) | `β = I_C / I_B` |
| Collector current | `I_C = β × I_B` |
| Base-emitter voltage drop | `V_BE ≈ 0.7 V` (silicon NPN) |
| Saturation condition | `I_B ≥ I_C / β` |

### NPN vs PNP

| Feature | NPN | PNP |
|---------|-----|-----|
| Semiconductor layers | N – P – N | P – N – P |
| Turns ON when | Positive voltage at Base | Negative voltage at Base |
| Current direction | Collector → Emitter | Emitter → Collector |
| How common | Very common | Less common |
| Symbol arrow | Points outward on Emitter | Points inward on Emitter |
| Typical use | Digital logic, amplifiers | Complementary push-pull |

---

## 04 — Capacitor — Visual Guide

**Fundamentals, RC Time Constant & Applications**

Covers charge storage, capacitor types, charging/discharging curves, RC time constant, energy storage, and series/parallel combinations with worked examples.

### Key Equations

| Quantity | Formula |
|----------|---------|
| Capacitance | `C = Q / V` (Farads) |
| RC time constant | `τ = R × C` (seconds) |
| Energy stored | `E = ½ × C × V²` (Joules) |
| Charging voltage at time t | `V(t) = V_max × (1 − e^(−t/τ))` |
| Discharging voltage at time t | `V(t) = V₀ × e^(−t/τ)` |
| Capacitors in series | `1/C_total = 1/C₁ + 1/C₂ + ...` |
| Capacitors in parallel | `C_total = C₁ + C₂ + ...` |

> At `t = τ`, a capacitor reaches **63.2%** of V_max during charging.

---

## 05 — Voltage Divider

**Theory, Loading Effects & Sensor Applications**

Covers the voltage divider formula derivation, loading effects, BJT biasing, LDR sensor circuits, logic level shifting, and potentiometer use.

### Key Equations

| Quantity | Formula |
|----------|---------|
| Divider output (unloaded) | `V_out = V_in × R2 / (R1 + R2)` |
| Divider ratio | `k = R2 / (R1 + R2)` |
| Series branch current | `I = V_in / (R1 + R2)` |
| Effective R2 under load | `R2_eff = R2 × R_L / (R2 + R_L)` |
| Loaded output | `V_out = V_in × R2_eff / (R1 + R2_eff)` |
| LDR sensor output | `V_out = V_S × R_fixed / (R_LDR + R_fixed)` |

### Applications

| Application | Use Case |
|-------------|----------|
| LDR threshold switch | Light level → V_out → transistor base → relay ON/OFF |
| Logic level shifting | 5V microcontroller → 3.3V ESP32 / STM32 input |
| ADC sensor scaling | 0–12V sensor output → 0–5V Arduino analog input |
| BJT base biasing | Set Q-point: `V_G = V_DD × R2 / (R1 + R2)` |
| Potentiometer | Volume control, brightness adjustment, variable threshold |

---

## 06 — Azerbaijan Electronics Market

**Sales Analysis & Strategic Insights** — Market Research Report

Analyzes the Azerbaijani electronics sector — import costs, component sales trends, local vs international pricing dynamics, and strategic opportunities for students and engineers.

| Section | Content |
|---------|---------|
| Market Overview | Sector size, growth trends, key domestic players |
| Sales Analysis | Component categories (passive, active, MCU modules), demand patterns |
| Pricing Dynamics | Import costs, local vs. international pricing comparison, markup analysis |
| Opportunities | Growth areas for students, engineers, and local entrepreneurs |
| Conclusions | Key takeaways, strategic recommendations, future outlook |

---

## 07 ⭐ — Tilt Sensor Alarm System

**Tilt Sensor Activated Alarm with Relay, Buzzer, and LED** · Version 1.0 · May 2026

[![Tinkercad](https://img.shields.io/badge/Tinkercad-Simulation-green)](https://www.tinkercad.com/things/3qlm6AXiMIa)
[![YouTube](https://img.shields.io/badge/YouTube-Video-red)](https://youtu.be/kDqtHsMD2rM)
[![Academia](https://img.shields.io/badge/Academia.edu-Report-blue)](https://www.academia.edu)

A tilt-activated alarm circuit built and tested in both TinkerCAD simulation and on a real breadboard.

### How It Works

```
SW-520 Tilt Sensor ──[1kΩ R_B]──► 2N2222 NPN Base
                                        │
                  [10kΩ pull-down to GND] │ (transistor saturates when sensor closes)
                                        ▼
                                  LU-5-R Relay (9V)
                                   /         \
                               Buzzer       Red LED
```

The SW-520 tilt sensor acts as a digital trigger. When tilted, it closes and drives the 2N2222 transistor base into saturation via a 1kΩ resistor. A 10kΩ pull-down holds the base at GND when the sensor is open. When the transistor saturates, it energizes the relay, which activates both the buzzer and LED simultaneously. A 1N4148 flyback diode protects the transistor from back-EMF on relay de-energization.

### Components

| Component | Value / Part | Role |
|-----------|-------------|------|
| Tilt sensor | SW-520 | Digital trigger |
| Base resistor | 1kΩ | Current limiting to transistor base |
| Pull-down resistor | 10kΩ | Holds base LOW when sensor is open |
| Transistor | 2N2222 NPN | Switch / amplifier |
| Flyback diode | 1N4148 | Back-EMF protection |
| Relay | LU-5-R (9V) | Output switching |
| Buzzer | Piezo | Audible alarm |
| LED | Red | Visual alarm |

### Sub-project 2.6 — Dark-Activated Alarm Circuit

A companion dark-sensing alarm circuit using an LDR instead of a tilt sensor.

**Components:** Photoresistor (LDR) · 10kΩ Resistor · 2N2222 NPN · LU-5-R Relay · 1N4148 Flyback Diode · Piezo Buzzer

When ambient light decreases, the LDR resistance rises, raising the transistor base voltage above threshold, which saturates the transistor, energizes the relay, and sounds the buzzer.

🔧 [Tinkercad Circuit](https://www.tinkercad.com/things/3qlm6AXiMIa) · 🎥 [Video](https://youtu.be/kDqtHsMD2rM) · 📄 [Academic Document](https://www.academia.edu/167366385/2_6_Dark_Activated_Alarm_Circuit_Research_by_Xaqani_Ceferli_verified_by_Telman_Asgaraliyev_Fizika_Muellimi_)

---

## About

All guides verified by **Telman Askeraliyev**, Physics Teacher, Baku, Azerbaijan.  
[LinkedIn](https://linkedin.com) · [Instagram](https://instagram.com)

> Created by Xaqani Ceferli · Baku, Azerbaijan · 2026
