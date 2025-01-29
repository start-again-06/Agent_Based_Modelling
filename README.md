# Agent_Based_Modelling

🦠 Bacterial Chemotaxis Simulation 🧫
📌 Overview
This project simulates the movement of bacteria in a nutrient field using randomized velocity updates and density-based decision making. The bacteria move in response to the concentration of nutrients, adjusting their direction probabilistically.

✨ Features
✅ Bacteria Movement Simulation – Models random movement and chemotaxis behavior
✅ Density Field Calculation – Defines nutrient concentration in a 2D environment
✅ Randomized Velocity Updates – Simulates bacterial tumbling and running
✅ Visualization – Generates heatmaps of bacteria movement

📂 Workflow
1️⃣ Define the Nutrient Field

Density decreases with distance from the center
Alternative function: Sharp nutrient boundary at 15μm
2️⃣ Bacterial Motion Model

Run-and-tumble behavior:
Move forward if nutrient density increases (probability P1)
Change direction if density decreases (probability 1 - P2)
Velocity vector updates randomly
3️⃣ Simulation & Visualization

Iterates over 200 time steps
Bacteria positions are updated based on chemotaxis rules
Snapshots saved every 40 steps for visualization
📊 Results & Insights
Bacteria prefer high-nutrient areas, clustering in regions of higher density.
Randomized tumbling helps them explore but favors nutrient-rich zones.
Periodic boundary conditions prevent bacteria from leaving the domain.
🐞 Bug Fixes & Improvements
🚨 Fix Indentation Error in update() method
✅ Add correct indentation for self.randomize_velocity() inside update().

🚨 Fix Duplicate get_density() Definition
✅ Ensure only one get_density() function is used.

🚨 Fix numpy Import
✅ Replace numpy with np to match the correct alias in draw() function.

🔚 Conclusion
This project demonstrates bacterial chemotaxis using a simple agent-based model. It can be extended to more complex simulations, such as:
🔬 Multi-bacteria interactions
🦠 Biological pattern formation
📉 Real-world chemotaxis studies

📜 License
🔓 This project is licensed under the MIT License – feel free to use and modify it!
