# KatzPlotkin
This is an archive of the Fortran programs provided by Joseph Katz and Allen Plotkin in their book titled [Low-Speed Aerodynamics](https://doi.org/10.1017/CBO9780511810329).  The authors reserve all rights to the code and these programs are transcribed verbatim for ease of use solely for educational purposes.
This project is currently a work in progress.

## Directory structure
Each `pXX` directory contains a program.  
Inside each directory, the source code is named `pXX.f` and an example output is provided with the name `pXX.log`.  
A Makefile (tested on Linux) is also provided.

## Usage
Compile the code using either the provided `Makefile` or using the command:
```Bash
gfortran p14.f -o p14.out
```
You can then run it using 
```Bash
./p14.out
```

## List of programs
| Code | Program details | Availability  |
| ---- | -------------   | ------------- |
|  01  | Grid generator for van de Vooren airfoil shapes. Programs 3-11 use this as input. | :heavy_check_mark: |
|  02  | 2D Neumann boundary condition: Discrete vortex, thin wing method | :heavy_check_mark: |
|  03  | 2D Neumann boundary condition: Constant strength source method   | :heavy_check_mark: |
|  04  | 2D Neumann boundary condition: Constant strength doublet method  | |
|  05  | 2D Neumann boundary condition: Constant strength vortex method   | |
|  06  | 2D Neumann boundary condition: Linear strength source method     | |
|  07  | 2D Neumann boundary condition: Linear strength vortex method     | |
|  08  | 2D Dirichlet boundary condition: Constant strength doublet method        | |
|  09  | 2D Dirichlet boundary condition: Constant strength source/doublet method | |
|  10  | 2D Dirichlet boundary condition: Linear strength doublet method          | |
|  11  | 2D Dirichlet boundary condition: Quadratic strength doublet method       | |
|  12  | 3D: Constant strength source/doublet element | |
|  13  | 3D: Vortex lattice method for rectilinear lifting surfaces (with ground effect) | |
|  14  | 3D: Constant strength sources and doublets with the Dirichlet boundary condition | :heavy_check_mark: |
|  15  | 2D: Sudden acceleration of a flat plate at angle of attack (using a single lumped vortex element)| :heavy_check_mark: |
|  16  | 3D: Unsteady motion of a thin rectangular lifting surface (Upgrade of program 13) | |
