# 🧭 Opriroute (In Progress)

**Opriroute** is a Python project that predicts and optimizes vehicle routing based on real road networks and machine learning models.  
It combines geospatial data processing, routing algorithms, and neural networks to create smarter route planning.

⚠️ **Project Status:** 🚧 *In Progress*

---

## 📌 Project Goals
- Load lat/lon node data and map them to a real road network
- Calculate realistic road-based distances (instead of straight-line / Euclidean)
- Train a neural network to predict delivery times or route scores
- Optimize delivery routes using OR-Tools and ML-predicted scores
- Visualize optimized routes on a map

---

## 🛠️ Tech Stack
- Python 3
- [osmnx](https://github.com/gboeing/osmnx) & [networkx](https://networkx.org/) for road-based graph & routing
- TensorFlow / PyTorch for machine learning
- pandas & numpy for data processing
- folium / matplotlib for visualization
- Google OR-Tools (optional) for advanced routing optimization

---

## 📂 Project Structure
```plaintext
geo_route_optimizer/
├── data/
│   ├── raw/                # Raw lat/lon data
│   ├── processed/          # Cleaned data with road-based distances
│   └── external/          # External datasets if any
├── notebooks/              # Exploration and visualization notebooks
├── src/                    # Core source code
│   ├── config.py
│   ├── data_loader.py
│   ├── feature_engineering.py
│   ├── model.py
│   ├── train.py
│   ├── evaluate.py
│   └── optimizer.py
├── tests/                  # Unit tests
├── visualizations/         # Output plots & route maps
├── requirements.txt        # Python dependencies
├── README.md
└── .gitignore
```

## 🚀 Quick Start
###⚠️ Work in progress: the following steps will be updated as development continues.
```bash
git clone https://github.com/yourusername/geo_route_optimizer.git
cd geo_route_optimizer
python -m venv venv
source venv/bin/activate  # on Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## 📝 Current Focus

### ✅ Data Preparation
- [x] Collect and prepare raw lat/lon node data
- [ ] Map each node to the nearest road network node using **osmnx**
- [ ] Calculate realistic road-based distances between all node pairs

### 🧠 Machine Learning
- [ ] Design initial neural network architecture to predict delivery times or route scores
- [ ] Prepare training dataset (features & labels)
- [ ] Train and evaluate baseline model

### 📦 Routing Optimization
- [ ] Build routing optimizer using **networkx** or **OR-Tools**
- [ ] Integrate ML-predicted scores into optimization step
- [ ] Validate and test route outputs

### 🗺️ Visualization & Reporting
- [ ] Plot routes on interactive maps using **folium**
- [ ] Create notebooks to explain and showcase results
- [ ] Document findings and decisions

### ⚙️ Project & Code Setup
- [x] Set up Python project structure
- [x] Create initial `requirements.txt` and `.gitignore`
- [ ] Add unit tests in `tests/` folder
- [ ] Write clean docstrings and comments in source code

---

> This section will be updated regularly as progress continues!
