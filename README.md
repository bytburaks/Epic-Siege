# 3D Lane-Based Tactical Siege & Strategy Game

This repository contains a 3D lane-based real-time tactical strategy game developed using **Unity** and **C#**. Heavily inspired by siege and tug-of-war strategy games, the project focuses on automated unit navigation, modular state-driven combat AI, and dynamic evolution/progression systems across distinct battlefield lanes.

---

## 🛠️ Tech Stack & Key Features

*   **Game Engine:** Unity 3D
*   **Language:** C# (Object-Oriented Programming, SOLID Principles)
*   **Navigation:** Unity NavMesh Components for dynamic, multi-lane pathfinding.
*   **AI Architecture:** Finite State Machine (FSM) for automated unit decision-making.
*   **Systems:** Real-time unit spawning, modular health/damage structures, and currency/evolution management.

---

## ⚙️ Technical Highlights (What I Implemented)

### 1. Finite State Machine (FSM) for Unit AI
*   Developed a robust **Finite State Machine** to govern automated unit behaviors. 
*   Units smoothly transition between states like `Marching`, `ChasingEnemy`, `Attacking`, and `Dead` based on real-time distance calculations and aggro-radius scanning using overlap spheres.

### 2. Multi-Lane NavMesh Navigation
*   Utilized Unity's **NavMesh** system to guide units along specific, dedicated lanes without clipping into obstacles or cross-routing unintentionally.
*   Coded dynamic path-recalculation logic, ensuring units navigate around active combat blocks or structures while prioritizing the enemy base at the end of their designated lane.

### 3. Modular Combat & Health Architecture
*   Designed a decoupled, reusable `Health` and `Damageable` component system that applies to all unit types (melee, ranged, bosses).
*   Implemented hit registration and attack timing sync using Unity animations and event-driven damage application to ensure precise combat feel.

### 4. Unit Evolution & Spawning Systems
*   Coded a progression manager that tracks player resources (gold/mana) and unlocks advanced unit tiers or "evolutions" mid-game.
*   Implemented a lane-specific spawning queue that handles unit initialization, team assignment, and target destination setting dynamically at runtime.

---

## 🎮 Game Loop & Controls

1.  **Generate Income:** Accumulate resources over time by holding ground or defeating enemy waves.
2.  **Select Lane & Unit:** Choose which type of unit to deploy (e.g., Warrior, Archer) and pick the target lane (Left, Center, Right).
3.  **Push and Evolve:** Upgrade your units to higher evolutionary forms to counter enemy high-tier spawns.
4.  **Destroy the Gate:** Push your army through the lanes to breach the enemy base and win the siege.

---

## 🎮 Game Photos
<img width="942" height="542" alt="1" src="https://github.com/user-attachments/assets/9b0ee814-485a-4fbe-92cf-6b006faf199c" />
<img width="940" height="527" alt="2" src="https://github.com/user-attachments/assets/c6d1c167-67b2-4056-b0cc-3126008d98c2" />
<img width="938" height="523" alt="3" src="https://github.com/user-attachments/assets/d8a9cad6-7e50-4567-9de7-8dd78db283ce" />

