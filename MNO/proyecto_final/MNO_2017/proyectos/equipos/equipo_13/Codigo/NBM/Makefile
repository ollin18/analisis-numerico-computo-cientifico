CFLAGS = -O
CC = gcc
LIBS = -lm -lgsl -lgslcblas

NBM:NBM.o leergml.o
	$(CC) $(CFLAGS) -o NBM NBM.o leergml.o $(LIBS)

NBM.o:NBM.c red.h leergml.h Makefile
	$(CC) $(CFLAGS) -c NBM.c

leergml.o:leergml.c leergml.h red.h
	$(CC) $(CFLAGS) -c leergml.c
