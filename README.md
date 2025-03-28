# Composite Laminate Analyzer

## Overview
This Jupyter Notebook provides an interactive tool for analyzing composite laminate materials. The calculator computes the ABD matrix (stiffness matrix) for a user-defined stacking sequence of composite plies and visualizes the results.

## Features
- **Material Library**: Includes three common composite materials with their mechanical properties
- **Interactive Interface**: 
  - Dropdown menu for material selection
  - Slider for ply angle adjustment
  - Input field for layer thickness
- **Stacking Sequence Builder**: Add multiple layers with different orientations
- **ABD Matrix Calculation**: Computes the full stiffness matrix (A, B, D components)
- **Visualization**:
  - Stacking sequence diagram
  - Stiffness distribution through thickness

## Available Materials
1. Carbon/Epoxy (AS4/3501-6)
2. Glass/Epoxy (S2/3501-6)
3. Kevlar/Epoxy

## How to Use
1. Select a material from the dropdown menu
2. Set the ply angle using the slider (-90° to +90°)
3. Enter the layer thickness in millimeters
4. Click "Add Layer" to add to the stacking sequence
5. Repeat steps 1-4 for each layer
6. Click "Calculate ABD Matrix" to perform the analysis
7. View results in the "Results" tab and visualizations in the "Visualization" tab
8. Use "Clear Layers" to reset the stacking sequence

## Technical Details
The calculator uses classical laminate theory to compute:
- **A matrix**: Extensional stiffness matrix (units: N/m)
- **B matrix**: Coupling stiffness matrix (units: N)
- **D matrix**: Bending stiffness matrix (units: N·m)

## Dependencies
- Python 3.x
- Jupyter Notebook
- Required packages:
  - numpy
  - pandas
  - matplotlib
  - ipywidgets

