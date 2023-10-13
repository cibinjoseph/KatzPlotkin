# KatzPlotkin
This is an archive of the fixed-format Fortran programs provided by Joseph Katz and Allen Plotkin in their book titled [Low-Speed Aerodynamics](https://doi.org/10.1017/CBO9780511810329).  The authors of the book reserve all rights to the code and these programs are transcribed verbatim for ease of use solely for educational purposes.

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

| Code | Program details                                                                   | Boundary Condit.n | 2D/3D | Availability       |
| ---- | ----------------------------------------------------------------------------------| ----------------- | ----- | ------------------ |
| 01   | Grid generator for van de Vooren airfoil shapes. Programs 3-11 use this as input. | --                |   --  | :heavy_check_mark: |
| 02   | Discrete vortex, thin wing method                                                 | Neumann           |   2D  | :heavy_check_mark: |
| 03   | Constant strength source method                                                   | Neumann           |   2D  | :heavy_check_mark: |
| 04   | Constant strength doublet method                                                  | Neumann           |   2D  | :heavy_check_mark: |
| 05   | Constant strength vortex method                                                   | Neumann           |   2D  | :heavy_check_mark: |
| 06   | Linear strength source method                                                     | Neumann           |   2D  | :heavy_check_mark: |
| 07   | Linear strength vortex method                                                     | Neumann           |   2D  | :heavy_check_mark: |
| 08   | Constant strength doublet method                                                  | Dirichlet         |   2D  | :heavy_check_mark: |
| 09   | Constant strength source/doublet method                                           | Dirichlet         |   2D  | :heavy_check_mark: |
| 10   | Linear strength doublet method                                                    | Dirichlet         |   2D  | :heavy_check_mark: |
| 11   | Quadratic strength doublet method                                                 | Dirichlet         |   2D  | :heavy_check_mark: |
| 12   | Constant strength source/doublet element                                          | --                |   3D  | :heavy_check_mark: |
| 13   | Vortex lattice method for rectilinear lifting surfaces (with ground effect)       | --                |   3D  | :heavy_check_mark: |
| 14   | Constant strength sources and doublets                                            | Dirichlet         |   3D  | :heavy_check_mark: |
| 15   | Sudden acceleration of a flat plate at angle of attack (using a single lumped vortex element) | --    |   2D  | :heavy_check_mark: |
| 16   | Unsteady motion of a thin rectangular lifting surface (Upgrade of program 13)     |                   |   3D  | :heavy_check_mark: |
