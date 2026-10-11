.PHONY: all clean

all: calculator

calculator: src/main.o src/calculator.o src/logger.o
	gcc src/main.o src/calculator.o src/logger.o -o calculator

src/main.o: src/main.c
	gcc -c src/main.c -o src/main.o -Iinclude

src/calculator.o: src/calculator.c
	gcc -c src/calculator.c -o src/calculator.o -Iinclude

src/logger.o: src/logger.c
	gcc -c src/logger.c -o src/logger.o -Iinclude

clean:
	rm -f src/*.o calculator
