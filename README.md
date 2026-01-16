# Level Rush – Unreal Engine 5 Blueprint Systems Project

**Level Rush** is a solo-developed Unreal Engine 5 project focused on systems design, blueprint architecture, modular gameplay features, and level scripting.  
This project demonstrates my ability to build a complete gameplay loop using Unreal Blueprints—including AI behavior, combat systems, UI, level progression, and gameplay mechanics.

---

## Download (Windows Build)
**Playable Build (Windows x64):**  
[Latest Release](https://github.com/Kentaro309/LevelRush/releases/latest)

**Gameplay Video:**  
[(https://img.youtube.com/watch?v=-dRomRy_nTQ/0.jpg)](https://www.youtube.com/watch?v=-dRomRy_nTQ)

---

## Technical Overview

### Core Contributions
- **Designed and implemented all gameplay systems** using Unreal Engine Blueprints  
- **Constructed 6 progressively complex rooms** with unique hazards, enemy patterns, and triggers  
- **Created modular, data-driven turret AI** (4 behavior types + boss variant)  
- **Implemented event-driven level sequencing** (doors, wipe-wall, checkpoints, hazards)  
- **Developed reusable Blueprint components** for player movement, shooting, health, and interactions  
- **Built UI/HUD systems** (health bar, death screen, menus)  
- **Authored all gameplay scripting, logic, and functionality**  

This project is built entirely with **Blueprints**, organized with clear state-based flows, event dispatchers, and componentized logic.

---

## System Architecture

### Player Systems
- **Third-person movement**: sprint, jump, crouch  
- **Modular gun system** using Blueprint functions + collision handling  
- **Damage system** using overlap/trace events  
- **Character animation blueprint** linked to movement states  
- **Player health component** with UI binding and death handling  

### Enemy AI (Turrets)
- Fully implemented in Blueprints  
- **Line-of-sight check** (stop firing behind walls)  
- **Rotational tracking** using timelines & interpolation  
- **Bullet firing patterns** varying by turret type  
- **Hit detection & health** for destroyable turrets  
- **Four distinct AI profiles**:
  - Level 1 – slow fire rate  
  - Level 2 – dual-shot bursts  
  - Level 3 – wide bullet-wall pattern  
  - Boss – high fire rate, 8 HP, arena pressure design  

### Level Scripting & Mechanics
- **Six-room progression system**:
  - Each room unlocks on completion trigger  
  - Increasing mechanical + combat complexity  
- **Wipe-wall system**:
  - Constant forward push force  
  - Kills player if they fall behind  
  - Driven by timelines + trigger volumes  
- **Traps & obstacles**:
  - Spike traps (instant kill)  
  - Moving pillars & obstacles  
  - Death pits  
  - Hidden trap triggers (Room 5)  
- **Room logic** implemented with event dispatchers, triggers, and timelines

### Menus & UI
- **Main menu** with:
  - Play  
  - Infinite Health mode (testing)  
  - Options (window/fullscreen settings)  
  - Quit  
- **Pause menu** (pause/resume/quit)  
- **HUD**:
  - Dynamic health bar  
  - Death screen  
  - Hit feedback  

---

## Level Progression Summary (Technical Breakdown)

### Room 1  
Platforming sequence → fall triggers death event.

### Room 2  
Intro to combat + pits → integrates turret line-of-sight + trigger deaths.

### Room 3  
Environmental hazard (death pool) + Level 2 turret cluster.

### Room 4  
Moving obstacles (timeline-driven) + turret integration.

### Room 5  
Two-phase room:
- Moving spike trap system  
- Vertical moving turrets + hidden trap triggers  

### Boss Room  
- 2 boss turrets  
- 4 supporting turrets  
- Synchronized spike trap patterns  
- Arena built around LOS, cover logic, and high-pressure firing patterns  

---

## Validation & Testing Checklist
- All turrets track the player using rotational interpolation  
- Bullets collide with player & apply damage events  
- Player bullets destroy turrets  
- Spike traps + pits trigger death  
- Wipe-wall timeline activates on room entry  
- Room transitions unlock on end trigger  
- HUD health updates correctly  
- Infinite Health mode bypasses player damage  
- Menus function correctly in standalone packaged build  

---

## Repo Contents
This repository contains:
- `README.md`  
- System documentation  
- Level/feature breakdown  
- (Optional) Blueprint graph screenshots in `/Docs`  

> Due to Unreal Engine project size and Marketplace assets, the full source project is available upon request.

---

## Technologies Used
- **Unreal Engine 5 (Blueprints)**  
- Level Sequencing  
- UI Widget Blueprints  
- Behavior scripting via Timelines, Event Dispatchers, Function Libraries  
- AI firing patterns & LOS checks  
- Component-based architecture principles  

---

## Contact
**Kentaro Matsuo**  
📧 kentaromats@gmail.com  
🔗 LinkedIn: https://linkedin.com/in/kentaro-matsuo  
🔗 GitHub: https://github.com/Kentaro309
