# Spatial-MLP-with-EGDS
High-Precision Airfoil Flow-Field Prediction based on Spatial Multilayer Perceptron with Error-Gradient-Guided Data Sampling (EGDS), implemented with PyTorch.
## Core Components

### Spatial MLP Model: 
Coordinate-based grid-free backbone with a spatial decoder (enforces global flow consistency) and channel-wise multi-head attention (enhances cross-variable coupling of pressure and velocity fields).
### EGDS Sampling Strategy: 
Prioritizes high-information spatial points via prediction error and physical quantity gradient magnitude (plus random sampling for diversity), boosting learning efficiency in high-gradient flow regions.
### Data Preprocessing Pipeline: 
Airfoil parameterization (CST-DE method), flow field normalization (mean shift elimination, nondimensionalization, range scaling) and Signed Distance Function (SDF) feature integration for geometric representation.
### Training & Inference Module: 
