
CFLAGS=-Wall -Wextra --pedantic -Wno-incompatible-pointer-types

all: a.out example.o lina.o

a.out: example.o lina.o
	gcc example.o lina.o
example.o: tests/example.c src/lina.h
	gcc ${CFLAGS} -c tests/example.c src/lina.h
lina.o: src/lina.c src/lina.h
	gcc ${CFLAGS} -c src/lina.c src/lina.h

clean:
	rm a.out lina.o example.o src/lina.h.gch
