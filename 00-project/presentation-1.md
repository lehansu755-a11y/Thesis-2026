# Custom 2D Physics Engine for Games

| **name** | Sulehan |
|---|---|
| **neptun** | CRX1CQ |
| **id** | 2026-OL-05 |

## Introduction

A **2D physics engine** simulates how objects move and interact in a two-dimensional game world.

It is responsible for basic physical behaviours such as:

- Movement and velocity
- Gravity and acceleration
- Collision detection
- Collision response

### Basic Physics Process

**Force / Gravity → Velocity → Position → Collision → Response**

The goal of this project is to build a basic 2D physics engine from scratch and understand how its core systems work.

---

# Problem

The project focuses on two main technical problems.

## 1. Performance

When the number of objects increases:

**More Objects → More Object Pairs → More Collision Checks → Higher Computational Cost**

A simple collision detection method can have approximately:

### **O(n²) time complexity**

This may become a performance problem when many objects are simulated at the same time.

## 2. Simulation Stability

Even if collisions are detected correctly, the simulation may still become unstable.

- **Penetration** — objects overlap each other
- **Jittering** — resting or stacked objects shake
- **Unstable Stacking** — stacked objects cannot remain stable
- **Tunneling** — fast-moving objects may pass through colliders

### Main Challenge

**Stable + Efficient Real-Time Simulation**

---

# Target Users

## 2D Game Developers

The engine can provide basic physics functionality for small 2D games.

Possible functions include:

- Object movement
- Gravity
- Collision detection
- Collision response
- Basic physical interactions

The physics system can work independently without requiring a complete large game engine.

## Students

The project can also help students understand:

- Rigid Body representation
- Collision detection
- Collision response
- Basic physics simulation
- Performance and stability problems

---

# Planned Scope

## Basic Mathematics & Movement

- Vector2
- Position
- Velocity
- Acceleration
- Force
- Mass
- Gravity

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

### Not Included in the First Version

- Complex polygon collisions
- Advanced joint systems
- Soft-body physics
- Fluid simulation
- A complete game engine

**First priority: build a small, understandable and stable physics core.**

---

# Initial User Journey

## 1. Create a Physics World

Create the environment for the physics simulation.

↓

## 2. Create Physical Objects

Add objects such as:

**Boxes / Circles**

↓

## 3. Define Object Properties

- Position
- Mass
- Velocity
- Collider Shape

↓

## 4. Start the Simulation

The physics engine automatically updates the objects.

↓

## 5. Observe the Result

**Move → Fall → Collide → Slide / Bounce → Stop**

The user can observe and test the physical behaviour of different objects.

---

# Next Step

## Stage 1 — Basic Mathematics & Movement

Implement:

**Vector2 → Position → Velocity → Acceleration → Gravity**

Goal: make objects move and fall correctly.

## Stage 2 — Rigid Body System

Create physical objects with:

- Position
- Mass
- Velocity

## Stage 3 — Collision Detection

Implement:

- Circle vs Circle
- Box vs Box
- Circle vs Box

## Stage 4 — Collision Response & Stability

Investigate:

- Penetration
- Jittering
- Stacking Stability
- Tunneling

## Stage 5 — Performance Testing

Test with increasing numbers of objects and measure:

- Number of collision checks
- Physics update time
- Simulation performance

### Final Goal

**Stable and Efficient Real-Time 2D Physics Simulation**
