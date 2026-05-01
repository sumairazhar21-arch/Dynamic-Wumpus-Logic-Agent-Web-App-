Dynamic Wumpus World Logic Agent (Web-Based AI System)

A Knowledge-Based Agent that explores a dynamically generated Wumpus World environment using **Propositional Logic, Knowledge Base (KB), and Resolution Refutation**. The system visually demonstrates AI reasoning in real-time through a web interface.

---

 Live Demo
> Add your deployed link here (e.g., Vercel / Netlify)
http://127.0.0.1:5000/
>
> 
---
 Project Overview

This project implements a **dynamic inference-driven AI agent** that navigates a grid-based Wumpus World environment. The agent does not initially know hazard locations and must deduce safe paths using logical reasoning.

Key idea:  
> The agent learns and reasons instead of brute-force exploration.

---

 Key Features

Dynamic Environment
- User-defined grid size (Rows × Columns)
- Random placement of:
  - 🕳️ Pits
  - 👹 Wumpus
- Each run generates a new environment

 Knowledge-Based Reasoning
- Propositional Logic Knowledge Base (KB)
- Percepts:
  - 💨 Breeze → nearby pit
  - 👃 Stench → nearby Wumpus
- Logical rule generation (TELL operation)

 Inference Engine
- Resolution Refutation algorithm
- CNF (Conjunctive Normal Form) conversion
- Safety checking via contradiction detection (ASK operation)

 Intelligent Agent Behavior
- Only moves to **proven safe cells**
- Avoids uncertain or dangerous paths
- Updates knowledge dynamically after every move

 Web Visualization
- Interactive grid UI (Canvas / DOM-based)
- Cell states:
  - 🟩 Safe
  - ⬜ Unvisited / Unknown
  - 🟥 Pit / Wumpus (detected)
- Real-time percept display

Metrics Dashboard
- Total inference steps count
- Current percepts at agent location
- Agent movement tracking

---

 Tech Stack

### Frontend
- HTML5 / CSS3 / JavaScript
- Canvas / DOM-based rendering (as implemented)
- Optional: React / Vue (if used)

### Backend (if applicable)
- Python / Flask / Node.js

### AI Logic
- Propositional Logic Engine
- CNF Converter
- Resolution Refutation Algorithm

---
