FC = gfortran
executables := $(patsubst %.f,%.out,$(wildcard *.f))
requirements = AFOIL2.DAT

all:
	make $(executables)

%.out: %.f $(requirements)
	$(FC) $*.f -o $*.out

clean:
	-rm *.out
