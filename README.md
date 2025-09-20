# Predator/Prey Empire Simulation

**Authors:** Yaal Luka Edrey Gatignol & Rom Steinberg 

---

## ⚔️ Simulation Overview

This project is a dynamic predator/prey simulation that models the interactions between five historical empires within a shared environment. The empires battle for dominance through movement, recruitment, and combat until only one remains standing. The simulation is enhanced by a weather system that directly influences the behavior and abilities of each empire, adding a layer of strategic complexity.

---

## ✨ Features

### Empires
The simulation features five unique empires, each inheriting from an abstract `Empire` class and possessing distinct traits, enemies, and periods of activity:

**🇬🇧 The British Empire (Predator):** Hunts Persians and Romans. Inactive during night time and "tea time" (3-5 PM). Gains a speed boost in rainy weather.
**🇪🇸 The Spanish Empire (Predator):** Hunts Amazonians and Romans. Inactive during night time and "siesta time" (2-4 PM). Gains an attack range boost in sunny weather.
**🏛️ The Roman Empire (Predator & Prey):** Hunts Persians and Amazonians but is hunted by the Spanish and British. Composed of only male soldiers who can only recruit male civilians.
**🏹 The Amazonian Empire (Prey):** Hunted by the Spanish and Romans. Composed of only female warriors who can only recruit female civilians. They become "invisible" during foggy weather.
**🏺 The Persian Empire (Prey):** Hunted by the British and Romans.

### Civilian System
* Civilians are neutral entities that can be recruited by any empire to join their ranks.
* They can move and reproduce independently.
* If all civilians are eliminated, they will eventually respawn to maintain the simulation's balance.

### 🌦️ Dynamic Weather System
The weather changes dynamically, affecting all empires on the field:
**Sunny:** Spanish soldiers can attack from twice as far.
**Rainy:** British soldiers can move twice in a single step.
**Foggy:** Amazonian soldiers "disappear" from the map, becoming difficult to target.
**Snowy:** All soldiers have a 50% chance of skipping their turn.
**Moderate:** Default weather with no special effects.

### 🎵 Dynamic Music
* The simulation features a dynamic music system where each empire has a unique theme.
* The background music changes to match the theme of the empire that is currently "winning" (has the most soldiers).
* A final victory anthem is played when one empire has conquered all others.

---

## 🐞 Known Bugs and Issues

* Due to the random nature of the initial setup, a single empire may occasionally dominate the entire simulation from the start.
* The simulation's end-game can be lengthy if the final two empires do not interact or enter a repopulation cycle.
* When the weather is foggy, Amazonians are still vulnerable to attacks even though they appear invisible.

---

## 🚀 Getting Started

To run this project:

1.  Clone the repository.
2.  Open the project in your preferred Java IDE.
3.  Ensure you have the required libraries for handling graphics and sound.
4.  Run the main `Simulator` class.
