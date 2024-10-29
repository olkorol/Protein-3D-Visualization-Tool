# Protein 3D Visualization Tool

## Overview
The **Protein 3D Visualization Tool** is a Python script that automates the process of downloading and visualizing three-dimensional structures of proteins from the RCSB PDB database. This tool provides customizable visualization options, allowing you to color different structural elements (e.g., alpha helices, beta sheets, loops) and specific chains within a protein structure, making it a useful tool for structural biology and bioinformatics.

## Key Features
- **Automatic PDB File Download**: Simply input a PDB ID to download the corresponding structure file from the RCSB PDB.
- **Custom Visualization**: Color various secondary structural elements and chains in distinct colors.
- **Image Output**: Save the visualized structure as a high-quality PNG image.

## Installation
### Requirements
- Python 3.x
- [Requests](https://pypi.org/project/requests/) for downloading files from the web
- [PyMOL](https://pymol.org/2/) with its API (requires PyMOL to be installed on your system)

### Setting Up
Install the required dependencies by running:
```bash
pip install requests
```
Ensure that PyMOL is installed and accessible from your Python environment. You may refer to PyMOL's [installation guide](https://pymolwiki.org/index.php/Windows_Install) for assistance.

## Usage
1. **Clone this repository** and navigate to the project directory:
```bash
git clone https://github.com/your-username/protein-3d-visualization.git
cd protein-3d-visualization
```

2. **Run the Script**:
```bash
python visualize_protein.py
```
3. **Input the PDB ID** of the protein you want to visualize (e.g., `1A6M` for hemoglobin). The script will:
- Download the PDB file.
- Visualize the structure with custom color settings.
- Save the visualization as a PNG image in the current directory.

### Example Output
Running the script with PDB ID `1A6M` generates an image file named `1A6M_colored_visualization.png`, which displays the hemoglobin protein structure with distinct colors for helices, sheets, and loops, along with unique colors for each chain (if available).

## Code Customization
This script includes customizable options:
- **Color Schemes**: Modify colors for secondary structures (`alpha helices`, `beta sheets`, `loops`) and specific chains.
- **Output Directory and Image Settings**: Adjust the `output_image` variable and `cmd.png` parameters for customized image output.

## License
This project is licensed under the MIT License. See `LICENSE` for more information.

## Acknowledgements
- The [RCSB PDB](https://www.rcsb.org/) for providing protein structure data.
- [Schrödinger, Inc.](https://www.schrodinger.com/) for PyMOL.