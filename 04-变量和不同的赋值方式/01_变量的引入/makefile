
CC := gcc
TARGET := hello.out

$(TARGET) : func.o main.o
	$(CC) -o $(TARGET) func.o main.o

func.o : func.c
	$(CC) -o func.o -c func.c

main.o : main.c
	$(CC) -o main.o -c main.c

all : $(TARGET)

clean : FORCE
	rm *.o $(TARGET)

FORCE :