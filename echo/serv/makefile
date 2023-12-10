CC=g++
CCLAGS=-c -Wall
#LIBFLAGS=-lboost_program_options -lcryptopp
SOURCES=$(wildcard *.cpp)
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=server

all: $(SOURCES) $(EXECUTABLE)
	
$(EXECUTABLE): $(OBJECTS) 
	$(CC) $(OBJECTS) -o $@

.cpp.o:
	$(CC) $(CCLAGS) $< -o $@
	
clean:
	rm -rf *.o $(Target)
	rm -rf *.app $(Target)
