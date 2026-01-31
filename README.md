# Agent Based Modelling  
## Bacterial Chemotaxis Simulation

---

## System Overview
This project simulates **bacterial chemotaxis** using an **agent-based modeling framework**. Individual bacteria act as autonomous agents that move within a two-dimensional nutrient field, adjusting their velocity probabilistically based on local nutrient density gradients.

The model captures essential run-and-tumble behavior observed in biological chemotaxis systems.

---

## High-Level Architecture

### Environment Layer
- Two-dimensional spatial domain  
- Nutrient density field defined analytically  
- Density decreases with distance from the center  
- Optional sharp nutrient boundary to study gradient effects  

---

### Agent Layer
- Each bacterium is modeled as an independent agent  
- State variables include position, velocity, and local density  
- Agents operate under periodic boundary conditions  

---

### Motion and Decision Layer
**Chemotaxis Model:**
- Run-and-tumble dynamics  
- Movement decision based on nutrient density comparison  

**Behavior Rules:**
- Continue moving forward if nutrient density increases (probability $$\( P_1 \)$$ )  
- Change direction if nutrient density decreases (probability $$\( 1 - P_2 \)$$ )  
- Velocity vectors randomized to simulate tumbling  

---

### Simulation Layer
- Discrete-time simulation over fixed time steps  
- Agent positions updated iteratively based on decision rules  
- Simulation executed for 200 time steps  

---

### Visualization Layer
- Heatmaps generated to represent bacterial concentration  
- Position snapshots saved every 40 time steps  
- Visual inspection of clustering and migration patterns  

---

## Execution Flow
1. Define the nutrient density field  
2. Initialize bacterial agents with random positions and velocities  
3. Compute local nutrient density for each agent  
4. Apply run-and-tumble decision rules  
5. Update agent velocities and positions  
6. Enforce periodic boundary conditions  
7. Visualize bacterial distribution at regular intervals  

---

## Results & Insights
- Bacteria preferentially accumulate in high-nutrient regions  
- Randomized tumbling enables exploration of the domain  
- Chemotactic bias leads to emergent clustering behavior  
- Periodic boundaries maintain spatial continuity  

---

## Bug Fixes & Improvements
- Fixed indentation error in the velocity randomization routine  
- Removed duplicate nutrient density function definition  
- Corrected NumPy alias usage for consistency across modules  

---

## Scalability & Extensibility
- Supports extension to multi-agent interactions  
- Can incorporate cell-cell communication mechanisms  
- Extendable to time-varying or heterogeneous nutrient fields  
- Suitable as a foundation for biological pattern formation studies  

---

## Applications
- Agent-based modeling of biological systems  
- Chemotaxis and microbial behavior studies  
- Educational demonstrations of emergent dynamics  
- Prototype simulations for biological transport phenomena  

---

## License
MIT License. Free to use, modify, and distribute for academic and research purposes.
