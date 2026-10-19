---
marp: true
theme: default
size: 16:9
paginate: true
title: Real-Time 2D Physics Simulation — Presentation 1
---

# Introduction

## Real-Time 2D Physics Simulation

A 2D physics simulation focused on stability and computational efficiency.

```text
Force / Gravity
      ↓
Velocity
      ↓
Position
      ↓
Collision
      ↓
Response
```

---

# Problem

## Performance

More Objects → More Collision Checks → Higher Computational Cost

**O(n²)** for naïve pairwise collision checking.

## Simulation Stability

- Penetration
- Jittering
- Unstable Stacking
- Tunneling

---

# Target Users

## 2D Game Developers

Simulate movement and collisions in 2D games.

## Students

Understand the relationship between forces, motion, collision, and response.

---

# Planned Scope

## Basic Mathematics & Movement

- Force / Gravity
- Velocity & Position

## Physics System

- Rigid Body System
- Collision Detection
- Collision Response & Stability

## Basic Collision Shapes

- Basic shapes for 2D collision detection

## Not Included

- 3D physics simulation

---

# Initial User Journey

Create Physics World → Create Objects → Set Properties → Start Simulation → Observe Behaviour

---

# Next Step

1. **Stage 1:** Basic Mathematics & Movement
2. **Stage 2:** Rigid Body System
3. **Stage 3:** Collision Detection
4. **Stage 4:** Collision Response & Stability
5. **Stage 5:** Performance Testing

**Final Goal:** Stable and Efficient Real-Time 2D Physics Simulation
