# Makefile

CC = g++
CFLAGS = -I./inc
SRC_DIR = src
INC_DIR = inc
OBJ = $(SRC_DIR)/*.cpp
EXEC = test

all: $(EXEC)

$(EXEC): $(OBJ:.cpp=.o)
	$(CC) -o $@ $^

%.o: $.cpp
	$(CC) $(CFLAGS) -c $^ -o $@

clean:
	rm -f $(SRC_DIR)/*.o $(EXEC)

.PHONY: all clean