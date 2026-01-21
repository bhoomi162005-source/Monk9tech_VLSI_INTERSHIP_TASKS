# Monk9tech_VLSI_INTERSHIP_TASKS
# Day 1 Overview of physical design
# 📘 VLSI Internship Notes – Day 1  
**Company:** Monk9 Tech  
**Topic:** RTL to GDSII Flow  
**Concept:** *Building a Chip is Like Building a City* 🏙️➡️💻

---

## 🧠 Core Idea
Building a semiconductor chip is similar to building a city:
- Planning before construction is critical
- Poor planning causes congestion, power issues, and failures
- Each design stage has a specific role

---

## 🏙️ Chip vs City Analogy

| City Element | Chip Element |
|-------------|-------------|
| City boundary | Die |
| City zones | Floorplan |
| Buildings | Standard Cells / Macros |
| Roads | Routing |
| Power grid | Power Planning |
| Final inspection | Sign-off |

---

## 🔹 IC Design Components & Terminologies

### 🧩 Die
- The outer boundary of the chip
- Contains the **core + IO pads**
- Printed multiple times on a wafer

### 🧠 Core
- Main functional area of the chip
- Contains logic cells, IPs, and nets

### 🧱 IPs (Intellectual Property)
- Pre-designed functional blocks
- Examples: **SRAM, ADC, DAC, PLL**
- Can be **hard IP** or **soft IP**

### 🔌 IO Pads
- Interface between chip and external world
- Carry **input, output, and power signals**

### 🧪 PDK (Process Design Kit)
- Bridge between **foundry & design**
- Contains:
  - Design rules (DRC)
  - Device models
  - LVS rules

---

## 🔄 ASIC Design Overview (RTL → GDSII)

**Simplified Flow:**
---

## 🧾 RTL (Register Transfer Level)
- High-level design description
- Defines **what the chip does**
- No physical information
- Like a **city master plan**

---

## 🏗️ Synthesis
- Converts RTL into logic gates
- Uses **Standard Cell Library (SCL)**
- Output: **Gate-level netlist**

📌 *City Analogy:*  
Master plan → Actual building blueprint

---

## 📐 Floor Planning
- Decides:
  - Core size
  - Placement of macros (CPU, SRAM)
  - IO pad locations

🎯 Goals:
- Minimize wire length
- Reduce congestion
- Improve performance

---

## ⚡ Power Planning
- Designs **VDD & GND network**
- Uses:
  - Power rings
  - Power straps
  - Power pads

📌 *Like building electricity infrastructure for a city*

---

## 📦 Placement
- Places standard cells inside core
- Two stages:
  - **Global Placement** (rough)
  - **Detailed Placement** (optimized)

Rules followed:
- No overlap
- Proper orientation
- Fixed boundaries

---

## 🛣️ Routing
- Connects all components using metal layers
- Uses **vias and tracks**
- Must satisfy:
  - Timing
  - DRC rules
  - Signal integrity

📌 *City roads & highways*

---

## ✅ Sign-Off
Final verification before manufacturing:

### ✔ Physical Checks
- **DRC:** Design Rule Check
- **LVS:** Layout vs Schematic

### ✔ Timing Check
- **STA:** Static Timing Analysis

✔ Ensures chip is **manufacturable & reliable**

---

## 🏁 Final Output
- **GDSII file**
- Sent to foundry for fabrication

---

## 🛠️ Tools & Flow Reference
- OpenLane Flow
- RTL → GDSII automation
- Uses PDK + EDA tools

---

## ⭐ Key Takeaways
- Planning is the most critical step
- Each VLSI stage depends on the previous one
- Poor floorplanning leads to routing & power issues
- RTL to GDSII is a structured, rule-driven flow

---

📌 *Day 1 focused on understanding the big picture of VLSI physical design.*
