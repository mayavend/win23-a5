SOURCES = $(wildcard *.c)
OBJECTS = $(SOURCES:.c=.o)
EXECUTABLE = calculator

# Target
all: $(EXECUTABLE)


%.o: %.c operations.h
	gcc -c $< -o $@

# Link .o files to executable calculator
$(EXECUTABLE): $(OBJECTS)
	gcc $^ -o $@

# Delete all .o files
clean:
	rm -f $(OBJECTS)

.PHONY: all clean