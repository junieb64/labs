CFLAGS = -Wall -Werror

.PHONY: all clean format

all: reverse_test

reverse_test: test_reverse.c reverse.c reverse.h
	gcc $(CFLAGS) $^ -o $@

clean:
	rm -f reverse_test

format:
	clang-format -style=Google -i <reverse>.h <test_reverse>.c <reverse>.c

