# KatzPlotkin
An archive of the Fortran programs provided by Joseph Katz and Allen Plotkin in their book Low-Speed Aerodynamics

## Directory structure
Each `PXX` directory contains a program code.  
Inside each directory, the source code is named `pXX.F` and an example output is provided with the name `pXX.log`.  
A Makefile for use on Linux systems is also provided.

## Usage
Compile the code using either the provided `Makefile` or using the command:
```Bash
gfortran p14.F -o p14.out
```
You can then run it using 
```Bash
./p14.out
```
