FC = gfortran
executables := $(patsubst %.f,%.out,$(wildcard *.f))
requirements = surface.dat

all:
	make $(executables)

%.out: %.f $(requirements)
	$(FC) $*.f -o $*.out

clean:
	-rm *.out
