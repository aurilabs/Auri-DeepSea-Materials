# 🌊 Auri Labs: Deep-Sea HEA Explorer (v1.0)

(Screenshot of the Auri Labs Materials Explorer GUI in action, mining stable thermodynamic phases).

## 🔬 Overview

Auri-DeepSea-HEA-Explorer is a custom computational materials science tool developed to accelerate the discovery of High-Entropy Alloys (HEAs) specifically designed for extreme marine environments (Deep-Sea Mining, ROVs, and Submarine components).

Instead of relying on costly and time-consuming trial-and-error metallurgy, this Python-based application leverages the Materials Project REST API (mp-api) to mine thousands of elemental combinations, filtering for thermodynamic stability, low melting points, and theoretical corrosion resistance.

## ⚙️ The Engineering Challenge & Strategy

Standard HEA designs for extreme environments often rely on refractory metals like Molybdenum (Mo), Tungsten (W), or Tantalum (Ta), which have melting points exceeding $2600^\circ\text{C}$.

The Hardware Constraint: My current home-laboratory setup utilizes a 2500W Zero Voltage Switching (ZVS) induction heater with a practical crucible limit of approximately $1300^\circ\text{C}$.

The Auri Labs Solution: To bypass this limitation while maintaining deep-sea integrity, this explorer focuses on liquid-phase dissolution and eutectic principles. We prioritize elements like:

Aluminum (Al) & Copper (Cu): Low melting points ($660^\circ\text{C}$ and $1085^\circ\text{C}$) to form the liquid matrix, providing immense biofouling and chloride-pitting resistance via passivation layers.

Nickel (Ni), Iron (Fe), Zinc (Zn): Dissolved into the matrix to induce severe lattice distortion (the core mechanism of HEAs), turning the alloy into a high-strength solid solution capable of withstanding $5000$ meters of hydrostatic pressure (~$50$ MPa).

## 🚀 Features

CustomTkinter GUI: A sleek, dark-mode user interface for easy parameter input.

Automated Combinatorics: Automatically generates 3, 4, and 5-element chemical systems (chemsys) based on user input.

Thermodynamic Filtering: Queries the Materials Project database to return only stable or highly-viable metastable structures (energy_above_hull < 0.05 eV/atom).

Formation Energy Sorting: Ranks candidates by how aggressively the atoms "want" to bond.

## 🛠️ Installation & Usage

Clone the repository:
git clone https://github.com/YourUsername/Auri-DeepSea-HEA-Explorer.git
cd Auri-DeepSea-HEA-Explorer

Install the required dependencies:
pip install mp-api customtkinter python-dotenv

Set up your API Key:
Create a free account on Materials Project.
Get your API key and create a .env file in the root directory.
Add the following line to the .env file: MP_API_KEY="your_api_key_here"

Run the application:
python auri_materials_explorer.py

🧪 Next Steps (The Auri Labs Roadmap)

- Phase 1 (Current): Data mining and computational discovery (API + GUI).

- Phase 2: Visualizing the champion alloys (e.g., $Al_2FeNi$) using VESTA to analyze lattice distortion and quantum bonding.

- Phase 3: Importing mechanical parameters into COMSOL Multiphysics to simulate macroscopic hydrostatic stress on ROV components.

- Phase 4: Physical synthesis using the 2500W ZVS induction heater and the Auri-Aging Station v1 for precipitation hardening.

Built with passion for Deep-Tech, Materials Informatics, and Ocean Engineering.


## Türkçe Özet
Bu proje, yüksek erime noktalı metallere ihtiyaç duymadan, yerel atölye imkanlarıyla (ZVS indüksiyon fırını) üretilebilecek derin deniz alaşımları geliştirmek amacıyla başlatılmıştır. Materials Project API'sini kullanarak 1300°C altında stabil faz sergileyen Al-Cu-Ni-Fe sistemli Yüksek Entropili Alaşımlar (HEA) tespit edilmiştir. Proje, TEG (Termoelektrik Jeneratör) çalışmalarımın yanında paralel bir AR-GE faaliyeti olarak yürütülmektedir.
