# Makefile

CC = g++
CFLAGS = -I./inc
SRC_DIR = src
OBJ = $(patsubst $(SRC_DIR)/%.cpp, $(SRC_DIR)/%.o, $(wildcard $(SRC_DIR)/*.cpp))
EXEC = test

all: $(EXEC)

$(EXEC): $(OBJ)
	$(CC) -o $@ $^

$(SRC_DIR)/%.o: $(SRC_DIR)/%.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(SRC_DIR)/*.o $(EXEC)
	rm -f *.o

.PHONY: all clean