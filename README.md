# 🚉 Dynamic–AI Rail Signalling

![Status](https://img.shields.io/badge/Status-Ongoing-blue)
![Python](https://img.shields.io/badge/Python-3.10%2B-yellow)
![Frontend](https://img.shields.io/badge/Frontend-HTML%2C%20CSS%2C%20JS-orange)
![AI](https://img.shields.io/badge/AI%20Module-Enabled-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

### **AI-Powered Railway Signalling and Platform Management System**  
_Reimagining train operations with adaptive signalling, real-time intelligence, and automated station assistance._

---

## 🧭 Overview

**Dynamic–AI Rail Signalling** is an ongoing research-driven project that integrates **Artificial Intelligence (AI)** with **Dynamic Moving Block Signalling** to revolutionize railway operations and enhance safety, speed, and efficiency.

Traditional **Fixed Block Systems** divide railway tracks into rigid, predefined sections, which often leads to underutilization and delays. This project overcomes that limitation by implementing **Dynamic Moving Blocks**, where block lengths vary continuously in real time based on:
- Train **speed**
- **Braking distance**
- **Track occupancy**
- **Congestion level**

The system also introduces an **AI Decision Support Engine** that assists **Station Masters** by offering intelligent recommendations for:
- 🚉 Platform allotment  
- 🚦 Signal control decisions  
- 🕒 Train sequencing and prioritization  
- ⚡ Conflict resolution during high traffic  

---

## 🚀 Key Features

- 🧠 **AI-Assisted Decision Engine**  
  Provides intelligent, data-driven suggestions for train routing, platform management, and real-time conflict resolution.  

- 🚦 **Dynamic Moving Block Signalling**  
  Adaptive block creation and management based on live train parameters such as speed and proximity, replacing outdated fixed-block methods.  

- 🕹️ **Static vs Dynamic Simulation**  
  Includes both modes to compare performance, safety margins, and efficiency improvements visually.  

- 📊 **Interactive Web Interface**  
  Enables real-time visualization of train movements, signals, and platform decisions via an intuitive dashboard.  

- ⚙️ **Modular Architecture**  
  Cleanly separated modules for signalling logic, AI decision-making, and frontend interface for easy scalability and debugging.  

---

## 🧑‍💻 Tech Stack

| Layer | Technologies Used |
|:------|:------------------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend & Logic** | Python |
| **AI Engine** | Custom rule-based and learning-driven models |
| **Simulation Modes** | Static & Dynamic signalling |
| **Version Control** | Git & GitHub |

---

## 🧩 Project Structure

flowchart TD
%% Input Layer
A[Train Data Input] -->|Speed, Position, Braking Distance| B[Dynamic Block Computation]

%% Dynamic Block Computation
B -->|Check Track Occupancy| C{Is Block Safe?}
C -->|Yes| D[Update Signals]
C -->|No| E[Delay Train / Alert Operator]

%% AI Decision Engine
D --> F[AI Decision Engine]
E --> F
F -->|Evaluate Station Congestion| G[Platform Allotment & Train Sequencing]

%% Visualization
G --> H[Web Visualization Interface]
H --> I[Operator / Station Master]

%% Feedback Loop for Multiple Trains
I -->|Train Updates| A
