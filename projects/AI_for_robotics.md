---
layout: project
type: project
image: img/RBE/Bomberman.png
title: "Artificial Intelligence for Robotics"
# date: Jan 2025 – Mar 2025
start: 2025-01-01
end:   2025-03-31
published: true
labels:
  - Python
  - A*
  - Q-Learning
  - State Machine
  - Heuristic Search
  - Reinforcement Learning
  - Artificial Intelligence
summary: "Designed Bomberman-playing AI agents in two projects: first using A* with a state machine, then expanding to Approximate Q-Learning with adaptive behaviors, achieving at least 50% survival across all scenarios."
---

<figure>
  <img class="img-fluid" src="{{ site.baseurl }}/img/RBE/Bomberman.png" alt="Bomberman AI agents navigating a gridworld with monsters.">
  <figcaption class="text-center">
    AI agents developed in RBE4701 navigating Bomberman environments with monsters, walls, and hazards.
  </figcaption>
</figure>

## Project Overview
As part of **RBE4701: Artificial Intelligence for Robotics**, our team developed autonomous Bomberman agents for two sequential projects. Each project built upon the previous, exploring different AI techniques for decision-making, path planning, and survival against increasingly difficult monster behaviors. In both projects, the benchmark was to achieve at least **50% survival across five scenarios**.

---

## Project 1: Heuristic A* with State Machine
- Implemented a **state machine** with two modes:  
  - **Normal:** A* search guided the agent to the exit.  
  - **Avoidance:** Triggered when monsters were nearby, rerouting around hazards.  
- Explored multiple **heuristics** (Manhattan, Chebyshev, Pythagorean) for path planning.  
- Added supporting methods for monster detection and avoidance (`monster_near`, `avoid_monster`, `monster_heuristic`).  
- **Results:**  
  - ✅ 100% survival in simple/no-monster maps.  
  - ✅ 92–82% survival with random or self-preserving monsters.  
  - ⚠️ 58% survival against aggressive monsters or multi-monster maps.  
- **Key Contribution:** Showed that heuristic A* plus a simple state machine can reliably solve most cases, but struggles with aggressive pursuit.

---

## Project 2: Approximate Q-Learning with A* Fallback
- Implemented an **Approximate Q-Learning agent** with two features:  
  - Reciprocal distance to the exit (positive).  
  - Reciprocal distance to nearest monster (negative).  
- Expanded the **state machine** to three modes:  
  - **Q-Learning:** Default exploration/decision-making.  
  - **Bomb:** Placed bombs when blocked, avoided danger zones with timers.  
  - **A\*:** Deterministic fallback when a safe path was available.  
- Persisted learned weights in **JSON files** to adapt across runs.  
- **Results:**  
  - ✅ 100% survival with no or random monsters.  
  - ✅ 80% survival with self-preserving monsters.  
  - ✅ 60% with aggressive monsters.  
  - ✅ 50% in multi-monster maps.  
- **Key Contribution:** Combined learning with deterministic planning, enabling adaptability across scenarios and meeting the benchmark in all cases.

---

## Key Takeaways
- Progressed from **heuristic A*** pathfinding to **reinforcement learning**, showing clear improvement in adaptability.  
- State machine design allowed structured switching between exploration, evasion, and bomb-usage behaviors.  
- Both approaches achieved the required survival benchmark, with Q-Learning providing better robustness in difficult scenarios.  

---

## Media & Links
- 📄 [Project 1 Report (PDF)]({{ site.baseurl }}/img/RBE/RBE4701_Group1_Project1.pdf)  
- 📄 [Project 2 Report (PDF)]({{ site.baseurl }}img/RBE/RBE4701_Group1_Project2.pdf) 
- 💻 [GitHub Repository](https://github.com/Robert-Gunduz/RBE470x-Project-Team01)  