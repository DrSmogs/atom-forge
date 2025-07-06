# Atom Forge - Game Development Plan

**Genre**: Roguelike Reactor Management Shooter
**Engine**: Godot 4.x
**Theme**: 1980s Soviet CRT retro tech meets particle physics
**Status**: First-time game project; learning-focused build

---

## 🎯 Game Premise

Control a nuclear reactor by firing subatomic particles from a gun, creating and managing atoms to achieve goals and survive. Stability, heat, radiation, and charge all matter. Each level ends in a shop where you stack powerful, weird upgrades to bend the reactor’s rules and survive increasing chaos.

---

## 📌 Project Goals

* Learn Godot step-by-step, applying real features in meaningful order.
* Avoid complete rewrites by building a flexible, modular system.
* Reach a fun, playable proof-of-concept quickly.
* Introduce mechanics and complexity progressively.

---

## ✅ Stage Breakdown

### **STAGE 0 – Setup & Repo**

* [x] GitHub repository: `atom-forge`
* [x] Godot 4 project initialized
* [x] Folder structure:

  ```
  /scenes
  /scripts
  /assets
  /ui
  /particles
  /atoms
  /upgrades
  ```

---

### **STAGE 1 – Playable Core (Proof of Concept)**

**Goal**: Test base mechanic — shoot → collide → create atom → collect.

**Features**:

* [ ] Particle gun that fires protons, neutrons, electrons
* [ ] Basic reactor chamber with physics
* [ ] Particle collision logic to create atoms (simplified)
* [ ] Charge system determines probe attraction (positive/negative)
* [ ] Atoms collected give score/currency

**Learning Goals**:

* Scenes, physics, signals, and timers
* Basic UI (score, collected atoms)

---

### **STAGE 2 – Reactor Systems**

**Goal**: Introduce basic reactor simulation and threats.

**Features**:

* [ ] Atom decay mechanic (based on neutron imbalance)
* [ ] Radiation particle emission increases exposure
* [ ] Bouncing atoms generate heat
* [ ] Reactor status UI: heat and radiation bars
* [ ] Game over if thresholds exceeded

**Learning Goals**:

* State-driven actors (atoms)
* Random timers, effect handling

---

### **STAGE 3 – Shop + Upgrades**

**Goal**: Create meaningful upgrade decisions.

**Features**:

* [ ] End of level = enter shop
* [ ] 3 random upgrades shown
* [ ] Upgrades apply modifiers (cooling boost, new gun, etc.)
* [ ] Upgrade tracker in UI
* [ ] Currency = atom value collected

**Learning Goals**:

* Scriptable upgrades
* UI layout and events
* Random generation

---

### **STAGE 4 – Gameplay Loop & Progression**

**Goal**: Full loop: play → shop → scale → repeat.

**Features**:

* [ ] Levels increase difficulty (more decay, heat, rare atoms)
* [ ] Unlock new atoms gradually
* [ ] Add new hazards (unstable atoms, field effects)

**Learning Goals**:

* Level manager
* Dynamic difficulty
* Reusable spawning patterns

---

### **STAGE 5 – Visuals & Polish**

**Goal**: Create the Cold War CRT aesthetic.

**Features**:

* [ ] Retro green/amber visuals, scanline shader
* [ ] Custom pixel font
* [ ] CRT-style UI (radar lines, knobs)
* [ ] Particle effects: sparks, fusions, radiation
* [ ] Sound FX and synth music

**Resources**:

* [https://kenney.nl/](https://kenney.nl/)
* [https://opengameart.org/](https://opengameart.org/)
* CRT Shader: [https://github.com/miloyip/godot-crt-shader](https://github.com/miloyip/godot-crt-shader)

---

## 🧩 Expanded Features & Ideas

### 🔥 Reactor Events

* Coolant Leak
* Radiation Surge
* Core Breach
* Magnet Failure

### 🧪 Fusion & Chemistry

* Hydrogen + Hydrogen → Helium
* Rare atom chains
* Special "reactive" pairings for bonuses

### 🧠 Loadouts / Player Classes

* **The Engineer** – More cooling, precision gun
* **The Alchemist** – Bonus value from rare atoms
* **The Janitor** – Extra radiation meds, faster decay cleanup

### 🛠️ Combo System

* Chain collections for score multipliers
* Stability streaks reduce heat buildup

### 🏗️ Reactor Architect Mode (Future)

* Drag/drop reactor pieces
* Configure custom reactors

### 🧬 Meta-Progression

* Unlock new atom types
* New particle gun types
* Reactor part unlocks

### 🌌 Environment Modifiers

* Magnetic Storm – drift
* Gravity Shift – downward pull
* Vacuum Chamber – decay accelerates

### 🦠 Rogue Particles

* Infect other atoms
* Clone themselves
* Must be removed quickly

### ⚡ Charge Field System

* Use electric fields to move atoms
* Probes can repel/attract using polarity

---

## 🧰 Sample Upgrade Names

| Name                 | Effect                   |
| -------------------- | ------------------------ |
| **Stabilizer Core**  | Slows atom decay         |
| **Mag Coil Mk.III**  | Stronger probe range     |
| **Gluon Burst**      | Create fusion fields     |
| **Red Mercury Shot** | Fires 3 particles        |
| **Iodine Drip**      | Reduces radiation slowly |
| **Quantum Sponge**   | Converts heat to energy  |

---

## 🛣️ Roadmap Summary

| Stage | Focus                 | Status |
| ----- | --------------------- | ------ |
| 0     | Setup & Project Init  | ✅      |
| 1     | Core Gameplay         | ☐      |
| 2     | Reactor Simulation    | ☐      |
| 3     | Shop & Upgrades       | ☐      |
| 4     | Progression Loop      | ☐      |
| 5     | Visual Style & Polish | ☐      |

---

## ✨ Final Notes

Atom Forge is designed to be expandable without needing rewrites. Prioritize clean modular code in Godot (Nodes + Signals), use Export variables for tuning, and avoid over-optimizing early. Build small and iterate.

Happy forging! ⚛️
