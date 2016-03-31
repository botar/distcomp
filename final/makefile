
CC       =  g++
FLAGS    = -O3 -Wall -std=gnu++0x -fopenmp #-E -g -pg
CFLAGS   = $(FLAGS)
CXXFLAGS = $(FLAGS)
LDFLAGS  = -lm 

PROGRAM_NAME=mandelbox

$(PROGRAM_NAME): main.o print.o timing.o savebmp.o getparams.o 3d.o getcolor.o distance_est.o \
	mandelboxde.o raymarching.o renderer.o init3D.o
	$(CC) -o $@ $? $(CFLAGS) $(LDFLAGS)

clean:
	rm -f *.o $(PROGRAM_NAME) $(EXEEXT) *~
