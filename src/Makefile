# THANKS CHATGPT

CC := gcc
CFLAGS := -Wall -Wextra -g

# Source files
SRCS := $(wildcard *.c)

# Object files
OBJS := $(SRCS:.c=.o)

# Target executable
TARGET := main

# Default target
all: $(TARGET)

# Compile source files into object files
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Link object files into the target executable
$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) $^ -o $@

# Clean up object files and the target executable
clean:
	rm -f $(OBJS) $(TARGET)