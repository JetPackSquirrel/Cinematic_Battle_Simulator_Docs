# Cinematic Battle Simulator Documentation
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/46645a6b-6b9b-41af-9a61-d3679b82df01" />

[View on Fab →](https://www.fab.com/listings/5e6fe2d3-9460-4f86-9220-af701514baeb)

---

## Overview

**Cinematic Battle Simulator** is a bueprint-based battle simulation system for **Unreal Engine 5**, designed specifically for **cinematic creators, virtual production teams, and game developers** who need convincing large-scale melee battles—fast.

The system allows you to stage **thousands of AI-driven agents** with minimal setup, while still offering extensive control over behavior, scale, and presentation. Whether you're blocking a cinematic shot or orchestrating a full battlefield, Cinematic Battle Simulator gives you believable chaos without complexity.

A ready-to-use demo scene is included, and the system is built to integrate seamlessly with your existing assets, animations, and characters.

---

## Key Features

- **18 configurable army parameters** for fine-grained control  
- **21 modular Blueprints** (no C++ required)  
- **AI-driven melee combat system**  
- **Adaptable grid & random spawners**  
- **Wave-based battle orchestration**  
- **Demo level included** for immediate use  
- Designed for **performance, flexibility, and cinematic scale**

---

## Installation & Quick Start

1. Purchase **Cinematic Battle Simulator** on Fab and add it to your Unreal Engine 5 project.
2. Open **Project Settings** and configure the following:

### Required Engine Settings

**Engine → Crowd Manager**
- Max Agents: `100,000`
- Max Agent Radius: `100,000`

**Engine → General Settings**
- Maximum Loop Iteration Count: `100,000`

3. Open the included **Demo Scene** to see the system in action.

---

## Creating a Battle in Your Own Level

1. Add **at least two Spawner Blueprints** to your level (one per army).
2. Enclose the battle area in a **Nav Mesh Bounds Volume**.
3. Adjust the army parameters as desired.
4. Press Play.

That’s it—your battle is live.

---

## Army Parameters

Each spawner exposes a comprehensive set of parameters to control scale, behavior, and presentation:

- **Army** – Assigns agents to one of two armies (default: Alpha / Omega)
- **Mesh** – Skeletal mesh used by the agent
- **Number per Wave** – Agents spawned per wave
- **Waves** – Total number of spawn waves
- **Wave Delay** – Delay (seconds) between waves

### Combat & Movement

- **Speed** – Relative movement speed
- **Size** – Relative agent size
- **Range** – Relative combat range
- **Strength** – Number of hits an agent can take before dying
- **Strength Variation** – Randomized variation per agent
- **Sophisticated Fighting** – Enables advanced combat logic

### Spawning & Formation

- **Random Spawn** – Enables randomized spawn positions
- **Formation Randomness** – Deviation from grid formation when Random Spawn is disabled

### Animation & Death

- **Attack Montages** – Array of attack animations
- **Defend Montages** – Array of defense animations
- **Death Montages** – Array of death animations
- **Blend Space** – 1D Blend Space controlling walk/run cycles
- **Ragdoll** – Enables physics-based death

---

## Advanced Customization

All Blueprints are cleanly structured and fully editable.  
While no customization is required out of the box, advanced users can extend combat logic, AI behavior, or spawning rules to suit specific production needs.

---

## Limitations

- Melee combat only  
- Maximum of **two opposing armies**  
- Spawner Blueprints **must not be rotated** (rotate the environment instead)

These constraints are intentional to maintain performance and deterministic behavior at scale.

---

## Troubleshooting

### Agents Are Not Moving
- Reduce agent count or agent size
- Increase spawner size
- Ensure the Nav Mesh fully covers the battle area
- Verify Crowd Manager settings

### Fewer Agents Than Expected
- Increase **Maximum Loop Iteration Count** in Project Settings

### Jittering or Collisions
- Reduce total agent count
- Increase spawner size

### Animation Issues
- Ensure Skeletal Mesh, Montages, and Blend Space all match

---

## Support

For support, questions, or feedback:

**[jetpacksquirrel@jetpacksquirrel.uk](mailto:jetpacksquirrel@jetpacksquirrel.uk)**
