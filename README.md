# Agent_Based_Modelling

# 🦠 Bacterial Chemotaxis Simulation 🧫

## 📌 Overview
This project simulates the movement of bacteria in a nutrient field using randomized velocity updates and density-based decision making. The bacteria move in response to the concentration of nutrients, adjusting their direction probabilistically.

---

## ✨ Features
✅ **Bacteria Movement Simulation** – Models random movement and chemotaxis behavior  
✅ **Density Field Calculation** – Defines nutrient concentration in a 2D environment  
✅ **Randomized Velocity Updates** – Simulates bacterial tumbling and running  
✅ **Visualization** – Generates heatmaps of bacteria movement  

---

## 📂 Workflow

### 1️⃣ Define the Nutrient Field
- Nutrient density decreases with distance from the center  
- Optional variation: sharp nutrient boundary at 15 μm  

### 2️⃣ Bacterial Motion Model
- **Run-and-tumble behavior**:
  - Move forward if nutrient density increases (probability `P1`)  
  - Change direction if density decreases (probability `1 - P2`)  
- Velocity vector updates randomly to simulate tumbling  

### 3️⃣ Simulation & Visualization
- Simulates bacterial movement for **200 time steps**  
- Bacteria positions are updated based on chemotaxis rules  
- **Snapshots saved every 40 steps** for visual inspection  

---

## 📊 Results & Insights

- Bacteria cluster in **high-nutrient regions**, showing effective chemotaxis  
- Randomized tumbling enables **exploration**, yet favors nutrient-rich zones  
- **Periodic boundary conditions** ensure continuity in the simulation domain  

---

## 🐞 Bug Fixes & Improvements

- 🚨 **Fix Indentation Error in `update()` method**  
  - ✅ Corrected `self.randomize_velocity()` indentation  

- 🚨 **Fix Duplicate `get_density()` Definition**  
  - ✅ Removed redundant function definition  

- 🚨 **Fix numpy Import**  
  - ✅ Replaced `numpy` with `np` to match existing alias in `draw()` function  

---

## 🔚 Conclusion
This project demonstrates **bacterial chemotaxis** using a simple agent-based model. It provides a solid base to extend toward more complex biological simulations, such as:

🔬 Multi-bacteria interactions  
🦠 Biological pattern formation  
📉 Real-world chemotaxis studies  

---

## 📜 License

🔓 **MIT License** – Free to use and modify!

