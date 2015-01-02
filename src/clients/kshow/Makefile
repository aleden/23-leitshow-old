CC=gcc
LIBS=/home/honig/squidlights2/src/lights.o -L/usr/local/lib -ljack -lfftw3 -lm 
CFLAGS=-O3 -I /home/honig/squidlights2/include -std=gnu99
TARGETS=fft.o

all: kleitshow

kleitshow: $(TARGETS)
	$(CC) $(TARGETS) $(LIBS) -o $@

.o: $*.c
	$(CC) $(CFLAGS) $(LIBS) $< -o $%

clean:
	rm -f kleitshow
	rm -f *.o
