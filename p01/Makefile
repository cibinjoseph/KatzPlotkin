FC = gfortran
executables := $(patsubst %.f,%.out,$(wildcard *.f))
requirements = 

all:
	make $(executables)

%.out: %.f $(requirements)
	$(FC) $*.f -o $*.out

clean:
	-rm *.out
