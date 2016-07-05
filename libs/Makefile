SHELL = /bin/sh

CC = gcc-5 -std=c99 -fPIC
CFLAGS = -shared -fopenmp -Wall
INCLUDES = -I.
LIBS =  -lm -lfftw3f

all: shotwem.so

shotwem.so:
	${CC} ${INCLUDES} shotwem.c seismic.c wem.c -o shotwem.so ${CFLAGS} ${LIBS}

clean:
		-rm -f *.o *.so
