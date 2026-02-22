# Urban Pulse: Transformer-based Analytics of Spatio-temporal Urban Stratification

## About the Paper
[cite_start]Traditional urban analytics have historically been constrained by cross-sectional datasets that represent urban environments as discrete temporal states, often struggling with the Modifiable Areal Unit Problem (MAUP)[cite: 25, 27]. [cite_start]"Urban Pulse" introduces a novel analytical framework to decode the spatiotemporal evolution of urban stratification across ten major US and UK cities over a decade[cite: 18]. 

### 1. Methodology
[cite_start]To ensure consistent spatial connectivity and mitigate MAUP, this research standardizes spatial units using the H3 Hexagonal discrete global grid system (Resolution 8)[cite: 28, 83]. [cite_start]We formalize the urban structure into multi-dimensional tensors representing seven socio-economic pillars (e.g., Finance, Consumption, Night Economy)[cite: 85]. 

[cite_start]We propose a hybrid **Transformer-Variational Autoencoder (Transformer-VAE)** architecture[cite: 18, 94]. [cite_start]The multi-head self-attention mechanism captures non-linear, long-term functional dependencies across different time scales [cite: 100][cite_start], while the variational bottleneck maps these discrete Point-of-Interest (POI) trajectories into a continuous latent manifold to account for the stochastic nature of urban sprawl[cite: 95, 212].

### 2. Key Discoveries
Mapping evolutionary trajectories into the continuous latent space reveals critical insights into global urban networks:

* [cite_start]**Morphology Dictates Entropy:** The representational complexity of the latent manifold is intrinsically linked to urban physical morphology[cite: 297]. [cite_start]Compact, transit-oriented cities (e.g., New York, London) feature deeply integrated socio-economic amenities that co-evolve synchronously, requiring fewer latent dimensions (Active Units) to encode[cite: 247, 249, 250]. [cite_start]In contrast, sprawling, car-dependent cities (e.g., Chicago, Houston) suffer from severe spatial fragmentation, resulting in highly stochastic functional trajectories that demand significantly larger latent capacities[cite: 174, 244, 299].
* **Intra-National Synergy vs. Transnational Divergence:** Trajectory tracking challenges the assumption of uniform globalization. [cite_start]Driven by the digital economy and tech talent agglomeration, US coastal hubs (New York, Los Angeles, San Francisco) are experiencing rapid intra-national functional convergence[cite: 218, 265, 267]. [cite_start]Simultaneously, major macroeconomic shocks (such as Brexit) have catalyzed a transnational decoupling, widening the micro-functional distance between historically synchronized financial centers like New York and London[cite: 258, 261, 263].

### 3. Proactive Governance & Social Implementation
Beyond theoretical network analysis, this methodology offers actionable tools for urban planners. [cite_start]By establishing the **Functional Drift Vector**, we quantify the velocity and nature of neighborhood transitions[cite: 154]. [cite_start]When the model detects abnormal accelerations in a grid's drift velocity, it indicates severe physical restructuring[cite: 289]. [cite_start]This trajectory deviation serves as a high-resolution early-warning system to "nowcast" acute gentrification, enabling planners to intervene proactively and mitigate the displacement of vulnerable populations[cite: 290, 303].

## Repository Structure
* `urban_app.py`: The main Streamlit application providing an interactive 3D Deck.gl atlas and static matplotlib renderings.
* `Data/`: Directory intended for the global urban evolution dataset (`Global_Urban_Evolution_2016_2025.csv`).
* `temp_maps/`: Auto-generated directory for caching Contextily enhanced basemaps.

## Installation and Usage

### Prerequisites
Ensure you have Python 3.8 or higher installed on your system.

### 1. Clone the Repository
First, clone this repository to your local machine and navigate into the project directory:
```bash
git clone [https://github.com/YourUsername/YourRepository.git](https://github.com/YourUsername/YourRepository.git)
cd YourRepository
