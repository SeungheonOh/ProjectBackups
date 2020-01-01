CFLAGS+= -Wall -Wextra -pedantic
LDADD+= -lX11 -lXext
LDFLAGS=
PREFIX?= /usr
BINDIR?= $(PREFIX)/bin

CC ?= gcc

all: main

main: main.o
	$(CC) $(LDFLAGS) -O3 -o $@ $+ $(LDADD)

clean:
	rm -f main *.o
