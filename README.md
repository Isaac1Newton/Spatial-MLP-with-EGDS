# Spatial-MLP-with-EGDS
High-Precision Airfoil Flow-Field Prediction based on Spatial Multilayer Perceptron with Error-Gradient-Guided Data Sampling (EGDS), implemented with PyTorch.

## Core Components

### Spatial MLP Model
Coordinate-based grid-free backbone with a spatial decoder and channel-wise multi-head attention.

### EGDS Sampling Strategy
Prioritizes high-information spatial points via prediction error and physical quantity gradient magnitude, boosting learning efficiency in high-gradient flow regions.

### Data Preprocessing Pipeline
Airfoil parameterization (CST-DE method), flow field processing and Signed Distance Function (SDF) feature integration for geometric representation.

