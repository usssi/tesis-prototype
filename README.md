# Kalimba Ranch Keeper

![](https://img.shields.io/badge/Unreal%20Engine-5-313131?logo=unrealengine)
![](https://img.shields.io/badge/Blueprints-%E2%9C%93-blue)
[![itch.io](https://img.shields.io/badge/View%20on-itch.io-red?logo=itchdotio)](https://ussi.itch.io/kalimba-ranch-keeper)

> A rhythm mobile game using a virtual kalimba to teach music theory through interactive farm care.

## Game Captures

<p align="center">
  <img src="https://img.itch.zone/aW1hZ2UvMzQyNzQxMi8yMDc2NDUyNi5wbmc=/original/5s7LCz.png" alt="Kalimba Ranch Keeper Screenshot 2" width="322"/>
  <img src="https://img.itch.zone/aW1hZ2UvMzQyNzQxMi8yMDc2NDUwMS5wbmc=/original/wmv2T3.png" alt="Kalimba Ranch Keeper Screenshot 1" width="232"/>
  <img src="https://img.itch.zone/aW1hZ2UvMzQyNzQxMi8yMDc2NDU0MC5wbmc=/original/C5ws3l.png" alt="Kalimba Ranch Keeper Screenshot 3" width="334"/>
</p>


---

**Table of Contents**
- [About the Game](#about-the-game)
  - [Gameplay Features](#gameplay-features)
- [Technical Overview & My Role (Lead Developer)](#technical-overview--my-role-lead-developer)
- [Core Mechanic Development & Evolution](#core-mechanic-development--evolution)
- [Contributors](#contributors)
- [License](#license)

---

## About the Game

**Kalimba Ranch Keeper** is a rhythm-based mobile game developed in Unreal Engine 5, designed to teach fundamental music concepts interactively. Players engage with charming farm animals by playing real musical notes on a virtual kalimba interface, tackling rhythmic challenges to maintain and grow their ranch.

Blending colorful visuals with intuitive, responsive gameplay and an educational core, **Kalimba Ranch Keeper** aims to merge music theory (rhythm, melody) with engaging simulation mechanics. It's designed for players of all ages seeking a creative way to explore music.

The game is **currently in active development**.

* **[View on my Portfolio (More Details & Visuals)](https://www.ussi.dev/portfolio-ussi/kalimba-ranch-keeper)**
* [View on Itch.io (Play/Download Protoype)](https://ussi.itch.io/kalimba-ranch-keeper)

### Gameplay Features

-   **Rhythm-Based Interaction:** Play notes on a virtual kalimba in time with visual cues.
-   **Music Theory Integration:** Learn rhythm and melody concepts through direct gameplay.
-   **Farm Simulation:** Care for animals and improve their habitats by successfully playing songs.
-   **Progressive Unlocks:** Discover new animals, songs, and decorations as you master the mechanics.
-   **Educational Core:** Designed to potentially transfer learned rhythmic and melodic skills to real instruments.

## Technical Overview & My Role (Lead Developer)

Developed in **Unreal Engine 5**, primarily utilizing **Blueprints** for core systems and gameplay logic. As Lead Developer, I architected and implemented key technical features:

* **Core Rhythm System:** Engineered the mechanics for precise note detection, timing accuracy against music tracks, and player input validation, inspired by rhythm-action game paradigms.
* **Sequencer Integration for Note Spawning:** Implemented a core workflow using UE5's **Sequencer**. Musical tracks were composed visually in Sequencer, which then drove the timed spawning of interactive note actors via custom Blueprint logic.
* **Audio Synchronization:** Developed systems within UE5 for tightly synchronized music playback and dynamic audio feedback directly linked to gameplay events (e.g., note hits/misses) and player performance.
* **Gameplay Logic (Blueprints):** Programmed the progression systems, state changes for farm simulation elements (animal feedback, habitat upgrades), and content unlock mechanics entirely using Blueprints.
* **Mobile UI/UX Implementation:** Designed and implemented the user interface and interaction flow tailored for mobile platforms using UMG (Unreal Motion Graphics).

## Core Mechanic Development & Evolution

The project's foundation was building a robust, data-driven rhythm system within UE5.

The primary technical challenge involved integrating **UE5 Sequencer** with **Blueprint** gameplay systems. The goal was to allow musical composition directly in Sequencer, which would then reliably trigger gameplay events. This was achieved by developing Blueprint logic that could:
1.  Parse custom events or data embedded within Sequencer tracks.
2.  Use this data to spawn note actors at precise moments synchronized with the audio track.
3.  Manage the lifecycle of these note actors and validate player input against their timing windows.

Initial prototypes validated this Sequencer-driven rhythm mechanic. To enhance player engagement beyond simple visual feedback, the system was integrated with farm simulation elements. Player performance in the rhythm sections now directly drives state changes and visual updates within the simulation layer (e.g., animal happiness meters, habitat visual upgrades), all managed via Blueprint logic, creating a technically interconnected gameplay loop.

## Contributors

-   [usssi](https://github.com/usssi) (Joaquin Driussi) - Lead Developer

## License

> This project is currently in development. The latest build is available for testing on [Itch.io](https://ussi.itch.io/kalimba-ranch-keeper)
