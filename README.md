# Partial differential equation (PDE)

This repository is a school project in my course of PDE at SDU - Odense.
The subject is: Review Chorin’s method and simulate incompressible Navier-Stokes flow simulations around obstacles.
This repository will show you some example of simulation using FEniCS.


## Installation

To install FEniCS, you can follow this guide: https://fenicsproject.org/download/

However, I recommend you to use FEniCS on Anaconda:

- If you don't have Anaconda, check here:
    https://docs.continuum.io/anaconda/install/


- Create the FEniCS environment: 
    ```bash
	conda create -n fenicsproject -c conda-forge fenics
	```

- Activate FEniCS: 
    ```bash
	conda activate fenicsproject
    ```
	
- Install mathplotlib inside FEniCS environment:
    ```bash
	pip install matplotlib
    ```    

## Usage

- Activate FEniCS: 
    ```bash
	conda activate fenicsproject
    ```
- Run scripts: 
    ```bash
	ns_cylinder.py
    ```
As we are creating an animation using matplotlib, the program will save it in your folder.
So visualize the animations, I recommend you to use ParaView.
You can download it here: https://www.paraview.org/download/

Once in Paraview, to reproduce the image you saw earlier, you have to follow these options:

- In Paraview, open the two files pressureCylinder.xdmf and velocityCylinder.xdmf

- Apply

- Hide to velocity, so we can see the color from the pressure

- Add 'Glyph' to the velocity, and apply.

- Change the scale array to f_31, and reduce the scale factor (like 0.05) and apply. Reduce also the opacity to 0.6.

- You can start the simulation. If the color in uniformly blue, you have to activate the coloring option of the pressure: "Use separate color map".



## Theory

You can find the explanation of Chorin's method and the IPCS on the Report.pdf.
