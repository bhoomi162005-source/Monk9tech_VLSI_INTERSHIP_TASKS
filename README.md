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
# 🟢 Day 2 – GitHub & Linux Overview

## 🔹 Why Linux?
- Most **VLSI tools run on Linux**
- GitHub is used for:
  - Version control
  - Team collaboration
  - Project tracking

---

## 🐧 Linux Overview

### 🔸 What is Linux?
- Open-source operating system
- Stable, secure, and fast
- Widely used in:
  - VLSI tools
  - Servers
  - Embedded systems

---
# 📘 GitHub Overview  
**Internship Topic:** GitHub Fundamentals  
**Company:** Monk9 Tech  

---

## 🔹 What is GitHub?
GitHub is a **cloud-based platform** used to store, manage, and share code.  
It works with **Git**, a version control system that tracks changes in files over time.

GitHub allows engineers to:
- Save their projects online
- Work on code safely without losing previous versions
- Collaborate with teams efficiently

---

## 🔹 Why GitHub is Used?
GitHub is used to:
- Maintain **project versions**
- Collaborate with multiple developers
- Track progress and changes in code
- Store project documentation and notes
- Share work with mentors, teams, and companies

---

## 🔹 Importance of GitHub in Engineering

### 👩‍💻 For Engineering Students
- Showcases projects in one place
- Builds a strong technical profile
- Helps in internships and placements
- Encourages clean and organized coding habits

---

### 🏭 For Industry & Companies
- Enables team collaboration
- Maintains code history and backups
- Reduces errors and code conflicts
- Improves development workflow

---

### 🔬 For VLSI & Semiconductor Domain
- Used to manage:
  - RTL designs
  - Scripts
  - Documentation
- Helps track design changes across versions
- Supports open-source EDA tools and flows

---

## ⭐ Key Takeaways
- GitHub is an essential tool for modern engineers
- It promotes collaboration and version control
- Strong GitHub usage improves career opportunities
- Learning GitHub is a long-term professional skill

---

# 📘 Day 3  Basics of Floor planning + Github and Linux & Labs

---

## 🟢 Part 1: Basics of Floor Planning (VLSI)

### 🔹 What is Floor Planning?
Floor planning is the **first physical design step** in the RTL to GDSII flow.  
It defines **how different blocks are arranged inside the chip**.

📌 It is similar to **city zoning before construction**.

---

### 🔹 Why Floor Planning is Important?
- Controls chip **area and shape**
- Reduces **routing congestion**
- Improves **performance and timing**
- Helps in efficient **power distribution**

Poor floor planning can lead to:
- Timing failures
- Power issues
- Routing congestion

---

### 🔹 What is Decided During Floor Planning?
- Core size and shape
- Placement of:
  - Macros (CPU, SRAM, IPs)
  - Standard cell area
  - IO pads
- Power and ground planning strategy

---

### 🔹 Key Floor Planning Terms

#### 🧠 Die
- Outer boundary of the chip

#### 🧩 Core
- Area where standard cells are placed

#### 🧱 Macros
- Large pre-designed blocks
- Examples: SRAM, PLL, CPU

#### 🔌 IO Pads
- Interface between chip and external world

---

### 🔹 Goals of Good Floor Planning
- Minimum wire length
- Less congestion
- Balanced power distribution
- Better timing closure
-
