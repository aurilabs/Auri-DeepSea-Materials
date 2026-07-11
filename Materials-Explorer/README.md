🌊 Auri Labs: Deep-Sea HEA Explorer (v1.0)


(Screenshot of the Auri Labs Materials Explorer GUI in action, mining stable thermodynamic phases).

🔬 Overview

Auri-DeepSea-HEA-Explorer is a custom computational materials science tool developed to accelerate the discovery of High-Entropy Alloys (HEAs) specifically designed for extreme marine environments (Deep-Sea Mining, ROVs, and Submarine components).

Instead of relying on costly and time-consuming trial-and-error metallurgy, this Python-based application leverages the Materials Project REST API (mp-api) to mine thousands of elemental combinations, filtering for thermodynamic stability, low melting points, and theoretical corrosion resistance.

⚙️ The Engineering Challenge & Strategy

Standard HEA designs for extreme environments often rely on refractory metals like Molybdenum (Mo), Tungsten (W), or Tantalum (Ta), which have melting points exceeding $2600^\circ\text{C}$.

The Hardware Constraint: My current home-laboratory setup utilizes a 2500W Zero Voltage Switching (ZVS) induction heater with a practical crucible limit of approximately $1300^\circ\text{C}$.

The Auri Labs Solution: To bypass this limitation while maintaining deep-sea integrity, this explorer focuses on liquid-phase dissolution and eutectic principles. We prioritize elements like:

Aluminum (Al) & Copper (Cu): Low melting points ($660^\circ\text{C}$ and $1085^\circ\text{C}$) to form the liquid matrix, providing immense biofouling and chloride-pitting resistance via passivation layers.

Nickel (Ni), Iron (Fe), Zinc (Zn): Dissolved into the matrix to induce severe lattice distortion (the core mechanism of HEAs), turning the alloy into a high-strength solid solution capable of withstanding $5000$ meters of hydrostatic pressure (~$50$ MPa).

🚀 Features
