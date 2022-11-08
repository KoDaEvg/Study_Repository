Target = hello
CC=g++
SOURCES=$(wildcard *.cpp)
OBJECTS=$(SOURCES:.cpp=.o)


all: $(SOURCES) $(Target)

$(Target): $(OBJ) 

  $(CC) $(OBJ) -o $@
.cpp.o:
  $(CC) $< -o $@

hello: hello.cpp
	g++ -O2 hello.cpp -o hello -DNDEBUG -Wall

clean:
	rm -rf *.o
