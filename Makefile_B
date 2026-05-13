# Makefile (część B) — uzupełnij reguły wieloplikowe
# Cel: zbudować program "program" z plików main.c i utils.c
# Wymagania:
# - osobna kompilacja do plików .o
# - linkowanie do programu "program"
# - poprawne zależności z utils.h
# - target clean usuwa *.o i program

CC = gcc
CFLAGS = -Wall -Wextra -O2

program: main.o utils.o 
	$(CC) main.o utils.o -o program

main.o: main.c utils.h
	$(CC) -c main.c -o main.o $(CFLAGS)
utils.o: utils.c utils.h
	$(CC) -c utils.c -o utils.o $(FLAGS)

clean:
	rm -f *.o program
