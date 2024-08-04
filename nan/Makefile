# Variables
CC = gcc
CFLAGS = -Wall -g

# Les cibles
all: main

main: main.o func1.o func2.o
	$(CC) $(CFLAGS) -o main main.o func1.o func2.o

main.o: main.c func1.h func2.h
	$(CC) $(CFLAGS) -c main.c

func1.o: func1.c func1.h
	$(CC) $(CFLAGS) -c func1.c

func2.o: func2.c func2.h
	$(CC) $(CFLAGS) -c func2.c

clean:
	rm -f *.o main

