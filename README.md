Flow Connect: High-Performance Logic Engine 🧩
A sophisticated path-finding puzzle game built with Vanilla JavaScript. This project demonstrates the implementation of complex game state management, coordinate-based collision detection, and optimized win-condition algorithms.

🚀 [Live Demo Link Here]
🎯 Technical Objectives
The goal was to build a robust grid-based engine that handles real-time user interactions while maintaining a strict set of logical rules:

Adjacency Validation: Ensuring paths only progress to neighboring cells.

Path Overwrite Protection: Dynamically clearing intersecting paths of different colors.

Automated Win-Validation: A dual-check system for connection completion and 100% board coverage.

🛠️ Key Engineering Features
Dynamic Grid Synchronization: The UI is mapped to a centralized gridData object, ensuring the "Source of Truth" is always consistent with the DOM.

Manhattan Distance Implementation: Custom logic to validate movement, preventing diagonal jumps or non-linear pathing.

State-Based Event Handling: Managed drawing states using isDrawing and isTargetReached flags to provide a professional "Manual Lock" feel.

Memory Efficient: Zero external dependencies (No jQuery, No React), showcasing strong proficiency in core JavaScript (ES6+).

🏗️ Core Logic Breakdown
Path Persistence: Each cell tracks its current color and whether it's a fixed "Dot" or a drawable "Path."

Collision Handling: When a new path intersects an old one, the engine identifies the specific color of the old path and resets all its non-dot cell states across the grid.

Win Algorithm: ```javascript // Connection Check: startDot.color === endDot.color // Coverage Check: totalFilledCells === gridCapacity (25)


💻 Tech Stack
Frontend: HTML5, CSS3 (CSS Grid & Flexbox)

Logic: Vanilla JavaScript (ES6+)

Deployment: GitHub Pages

📖 How to Run Locally
Clone the repository:

Bash

git clone https://github.com/svg-shubham/flow-connect-puzzle-engine.git
Open main.html in any modern browser.

Author: Shubham (svg-shubham)

Role: Frontend Developer / Logic Engineer

Open for opportunities in high-performance web development.
