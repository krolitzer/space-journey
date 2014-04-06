CC=g++
CFLAGS=-c -Wall
LDFLAGS=-lsfml-graphics -lsfml-window
SOURCES=Game.cpp 
#State.cpp GameModel.cpp MainMenu.cpp
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=space_adventure

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@

.cpp.o: 
	$(CC) $(CFLAGS) $< -o $@

clean:
	rm -f space_adventure
	rm -f *.o
