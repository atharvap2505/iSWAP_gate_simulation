# Quantum Mechanics Project - XY Hamiltonian and iSWAP Gate Simulation

This project is implemented as a part of the PHY F311 - Quantum Mechanics 2 at BITS Pilani K.K. Birla Goa Campus, and intends to simulate the XY Hamiltonian time evolution and demonstrates the iSWAP gate implementation using Qiskit.

## Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

## Setup Instructions

### 1. Clone and Navigate to the Project Directory

```bash
git clone https://github.com/atharvap2505/iSWAP_gate_simulation.git
cd iSWAP_gate_simulation
```

### 2. Create a Virtual Environment

Create a virtual environment to isolate project dependencies:

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

**On Linux/Mac:**
```bash
source venv/bin/activate
```

**On Windows:**
```bash
venv\Scripts\activate
```

You should see `(venv)` prefix in your terminal prompt, indicating the virtual environment is active.

### 4. Install Dependencies

Install all required packages using the requirements file:

```bash
pip install -r requirements.txt
```

## Running in VS Code

### 1. Open the Project in VS Code

Open VS Code and navigate to the project folder:

```bash
code .
```

Or use **File → Open Folder** in VS Code.

### 2. Install Required Extensions

Install the following VS Code extensions:
- **Python** (by Microsoft)
- **Jupyter** (by Microsoft)

You can install them by:
- Opening the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
- Searching for "Python" and "Jupyter"
- Clicking Install

### 3. Open the Notebook

Open `iSWAP_simulation.ipynb` in VS Code. It should open in the notebook editor.

### 4. Select Python Interpreter

1. Click on the kernel picker in the top-right corner of the notebook (it may say "Select Kernel")
2. Choose **Python Environments**
3. Select the virtual environment you created (`venv`)
   - It should be listed as `./venv/bin/python` or similar

### 5. Run the Notebook

Execute cells by:
- Clicking the **▶ Run** button next to each cell
- Pressing `Shift + Enter` to run the current cell and move to the next
- Using **Run All** from the top toolbar to execute all cells

The first cell will automatically install required packages if they're missing.

## Running with Jupyter Notebook (Alternative)

If you prefer the classic Jupyter interface:

```bash
jupyter notebook
```

This will open a browser window. Click on `iSWAP_simulation.ipynb` to open the notebook.

Execute the cells in order by pressing `Shift + Enter` or using the "Run All" option from the Cell menu.

## Deactivating the Virtual Environment

When you're done working on the project, deactivate the virtual environment:

```bash
deactivate
```

## Project Structure

- `iSWAP_simulation.ipynb` - Main Jupyter notebook containing the simulation code
- `requirements.txt` - Python package dependencies
- `README.md` - This file
- `documentation.pdf` - Compiled PDF documentation of the code and theory
- `concurrence_plot.png` - Generated plot of entanglement dynamics
- `circuit_diagram.txt` - Text representation of the quantum circuit

## Dependencies

- **numpy**: Numerical computing library
- **matplotlib**: Plotting and visualization
- **qiskit**: Quantum computing framework
- **qiskit-aer**: High-performance simulator for Qiskit

## Troubleshooting

### Import Errors
If you encounter import errors, ensure:
1. The virtual environment is activated
2. All packages are installed: `pip list` should show qiskit, numpy, matplotlib, and qiskit-aer
3. Try reinstalling: `pip install --force-reinstall -r requirements.txt`

### VS Code Kernel Issues
If the notebook can't find the packages in VS Code:
1. Make sure you've selected the correct Python interpreter (the one in your `venv` folder)
2. Try reloading the window: `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) → "Developer: Reload Window"
3. Restart VS Code completely

### Classic Jupyter Kernel Issues
If using Jupyter Notebook and it can't find the packages:
1. Install ipykernel: `pip install ipykernel`
2. Add the virtual environment to Jupyter: `python -m ipykernel install --user --name=venv`
3. In Jupyter, select Kernel → Change Kernel → venv

## Additional Resources

- [Qiskit Documentation](https://qiskit.org/documentation/)
- [Qiskit Tutorials](https://qiskit.org/learn/)
- See `documentation.pdf` for detailed explanation of the physics and code
