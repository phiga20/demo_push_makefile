.PHONY: rule1
CC := gcc
CFLAGS := -I.

INC_FILES := hello.h

rule1: main.o hello.o
	$(cc) -o $@ $^ $(CFLAGS)
clean:
	rm hello *.o
