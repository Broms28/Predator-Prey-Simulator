# Predator/Prey Empire Simulation

[cite_start]**Authors:** Yaal Luka Edrey Gatignol (k24045451) & Rom Steinberg (k24067133) [cite: 124, 125]

---

## ⚔️ Simulation Overview

[cite_start]This project is a dynamic predator/prey simulation that models the interactions between five historical empires within a shared environment[cite: 130]. [cite_start]The empires battle for dominance through movement, recruitment, and combat until only one remains standing[cite: 132, 133]. [cite_start]The simulation is enhanced by a weather system that directly influences the behavior and abilities of each empire, adding a layer of strategic complexity[cite: 134].


[cite_start]*Figure 1: A diagram illustrating the object-oriented architecture of the simulation[cite: 155].*

---

## ✨ Features

### Empires
[cite_start]The simulation features five unique empires, each inheriting from an abstract `Empire` class and possessing distinct traits, enemies, and periods of activity[cite: 157, 133]:

* **🇬🇧 The British Empire (Predator):** Hunts Persians and Romans. [cite_start]Inactive during night time and "tea time" (3-5 PM)[cite: 161, 163]. [cite_start]Gains a speed boost in rainy weather[cite: 162, 190].
* **🇪🇸 The Spanish Empire (Predator):** Hunts Amazonians and Romans. [cite_start]Inactive during night time and "siesta time" (2-4 PM)[cite: 164, 166]. [cite_start]Gains an attack range boost in sunny weather[cite: 165, 188].
* [cite_start]**🏛️ The Roman Empire (Predator & Prey):** Hunts Persians and Amazonians but is hunted by the Spanish and British[cite: 167]. [cite_start]Composed of only male soldiers who can only recruit male civilians[cite: 168, 169].
* **🏹 The Amazonian Empire (Prey):** Hunted by the Spanish and Romans. [cite_start]Composed of only female warriors who can only recruit female civilians[cite: 173, 174, 175]. [cite_start]They become "invisible" during foggy weather[cite: 175, 193].
* [cite_start]**🏺 The Persian Empire (Prey):** Hunted by the British and Romans[cite: 177].

### Civilian System
* [cite_start]Civilians are neutral entities that can be recruited by any empire to join their ranks[cite: 181].
* [cite_start]They can move and reproduce independently[cite: 185].
* [cite_start]If all civilians are eliminated, they will eventually respawn to maintain the simulation's balance[cite: 184].

### 🌦️ Dynamic Weather System
[cite_start]The weather changes dynamically, affecting all empires on the field[cite: 187]:
* [cite_start]**Sunny:** Spanish soldiers can attack from twice as far[cite: 188].
* [cite_start]**Rainy:** British soldiers can move twice in a single step[cite: 190].
* [cite_start]**Foggy:** Amazonian soldiers "disappear" from the map, becoming difficult to target[cite: 193].
* [cite_start]**Snowy:** All soldiers have a 50% chance of skipping their turn[cite: 194].
* [cite_start]**Moderate:** Default weather with no special effects[cite: 195].

### 🎵 Dynamic Music
* [cite_start]The simulation features a dynamic music system where each empire has a unique theme[cite: 197, 198].
* [cite_start]The background music changes to match the theme of the empire that is currently "winning" (has the most soldiers)[cite: 198].
* [cite_start]A final victory anthem is played when one empire has conquered all others[cite: 202].

---

## 🐞 Known Bugs and Issues

* [cite_start]Due to the random nature of the initial setup, a single empire may occasionally dominate the entire simulation from the start[cite: 207, 208].
* [cite_start]The simulation's end-game can be lengthy if the final two empires do not interact or enter a repopulation cycle[cite: 209, 210].
* [cite_start]When the weather is foggy, Amazonians are still vulnerable to attacks even though they appear invisible[cite: 211].

---

## 🚀 Getting Started

To run this project:

1.  Clone the repository.
2.  Open the project in your preferred Java IDE.
3.  Ensure you have the required libraries for handling graphics and sound.
4.  Run the main `Simulator` class.
