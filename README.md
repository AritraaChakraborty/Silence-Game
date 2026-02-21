# 🌑 Silence: Demon Realm

**Silence: Demon Realm** is a high-stakes survival game built with vanilla JavaScript and CSS3. It explores the tension between movement and visibility, forcing players to balance their survival instincts with the risk of "Chaos."

Created by **Team Recurrex : Aritraa,Mainak,Abir** for the 2026 Code 2 Console Game Development Competition.

---

## 🕹️ Gameplay Mechanics

In the Demon Realm, movement is noise. Your goal is to survive for **90 seconds** while being hunted by shadows.

- **Movement (The Chaos Bar)**: Every time you move using the arrow keys, your "Chaos" increases. If the bar fills completely, you lose.
- **The Hunters**: Demons spawn periodically and track your location. As they get closer, your reality (the screen) begins to shake.
- **Safe Zones**: Cyan circles appear randomly. While inside these zones, you are invisible to the demons, allowing you to catch your breath.
- **The Ambient Fear**: The background color shifts to deep red as your Chaos levels rise, indicating your proximity to failure.

## 🛠️ Technical Implementation

### Faux-3D Perspective
The game utilizes CSS `perspective` and `transform: rotateX(60deg)` to create a 3D arena feel while maintaining the lightweight performance of 2D DOM elements.

### Vector-Based AI
The demon entities utilize basic vector math to calculate the distance and direction to the player:
- **Direction calculation**: `(heroX - demonX) / distance`
- **Dynamic Proximity Trigger**: Triggers a screen-shake function when the distance vector falls below 120 pixels.

### Procedural Systems
- **Collision Detection**: Uses Euclidean distance checks to determine if the player is within a `safeZone` radius.
- **Resource Management**: Implements a decay function for the "Chaos" variable to reward players for periods of stillness.

## 🚀 Built With
- **HTML5**
- **CSS3** (Keyframe animations, Radial gradients)
- **Vanilla JavaScript** (No external frameworks or libraries)

---
*Developed as a B.Tech First-Year Project | IEM Kolkata*
