---
title: "Custom 2D Physics Engine for Games"
text-scale: 80%
h1-scale: 85%
h2-scale: 70%
h3-scale: 85%
table-scale: 85%
---

<!-- @slide Introduction -->
<!-- @layout AA/BC/BC/BC/BC/BC/BC/BC collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Custom 2D Physics Engine for Games

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

| **name** | Sulehan |
|---|---|
| **neptun** | CRX1CQ |
| **id** | 2026-OL-05 |

The goal of this project is to build a basic 2D physics engine from scratch and understand how its core systems work.

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

## Introduction

A **2D physics engine** simulates how objects move and interact in a two-dimensional game world.

It is responsible for basic physical behaviours such as:

- Movement and velocity
- Gravity and acceleration
- Collision detection
- Collision response

### Basic Physics Process

**Force / Gravity → Velocity → Position → Collision → Response**

---

<!-- @slide Problem -->
<!-- @layout AA/BC/BC/BC/BC/BC/BC/BC collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Problem

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 90% -->

The project focuses on two main technical problems.

## 1. Performance

When the number of objects increases:

**More Objects → More Object Pairs → More Collision Checks → Higher Computational Cost**

A simple collision detection method can have approximately:

### **O(n²) time complexity**

This may become a performance problem when many objects are simulated at the same time.

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

## 2. Simulation Stability

Even if collisions are detected correctly, the simulation may still become unstable.

- **Penetration** — objects overlap each other
- **Jittering** — resting or stacked objects shake
- **Unstable Stacking** — stacked objects cannot remain stable
- **Tunneling** — fast-moving objects may pass through colliders

### Main Challenge

**Stable + Efficient Real-Time Simulation**

---

<!-- @slide Target Users -->
<!-- @layout AA/BC/BC/BC/BC/BC/BC/BC collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Target Users

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

## 2D Game Developers

The engine can provide basic physics functionality for small 2D games.

Possible functions include:

- Object movement
- Gravity
- Collision detection
- Collision response
- Basic physical interactions

The physics system can work independently without requiring a complete large game engine.

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

## Students

The project can also help students understand:

- Rigid Body representation
- Collision detection
- Collision response
- Basic physics simulation
- Performance and stability problems

---

<!-- @slide Planned Scope -->
<!-- @layout AAA/BCD/BCD/BCD/BCD/BCD/BCD/BCD collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Planned Scope

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

## Basic Mathematics & Movement

- Vector2
- Position
- Velocity
- Acceleration
- Force
- Mass
- Gravity

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

## Physics System

- Physics World
- Rigid Body System
- Collider System
- Basic Collision Detection
- Basic Collision Response
- Simulation Stability

## Basic Collision Shapes

- Circle Collider
- Box / AABB Collider

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

### Not Included in the First Version

- Complex polygon collisions
- Advanced joint systems
- Soft-body physics
- Fluid simulation
- A complete game engine

**First priority: build a small, understandable and stable physics core.**

---

<!-- @slide Initial User Journey -->
<!-- @layout AAAAA/BCDEF/BCDEF/BCDEF/BCDEF/BCDEF/BCDEF/BCDEF collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Initial User Journey

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

### 1. Create a Physics World

Create the environment for the physics simulation.

**→**

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

### 2. Create Physical Objects

Add objects such as:

**Boxes / Circles**

**→**

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

### 3. Define Object Properties

- Position
- Mass
- Velocity
- Collider Shape

**→**

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

### 4. Start the Simulation

The physics engine automatically updates the objects.

**→**

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 95% -->

### 5. Observe the Result

**Move → Fall → Collide → Slide / Bounce → Stop**

The user can observe and test the physical behaviour of different objects.

---

<!-- @slide Next Step -->
<!-- @layout AAA/BCD/BCD/BCD/BCD/BCD/BCD/BCD collapse -->
<!-- @slide-theme slate sky gray -->

<!-- @set-align left -->
<!-- @set-gap 0.65 -->

# Next Step

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 85% -->

### Stage 1 — Basic Mathematics & Movement

Implement:

**Vector2 → Position → Velocity → Acceleration → Gravity**

Goal: make objects move and fall correctly.

### Stage 2 — Rigid Body System

Create physical objects with:

- Position
- Mass
- Velocity

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 85% -->

### Stage 3 — Collision Detection

Implement:

- Circle vs Circle
- Box vs Box
- Circle vs Box

### Stage 4 — Collision Response & Stability

Investigate:

- Penetration
- Jittering
- Stacking Stability
- Tunneling

***

<!-- @set-align left -->
<!-- @set-gap 0.65 -->
<!-- @set-scale 85% -->

### Stage 5 — Performance Testing

Test with increasing numbers of objects and measure:

- Number of collision checks
- Physics update time
- Simulation performance

### Final Goal

**Stable and Efficient Real-Time 2D Physics Simulation**
