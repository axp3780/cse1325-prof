CXXFLAGS += -std=c++17
GTKFLAGS = `/usr/bin/pkg-config gtkmm-3.0 --cflags --libs`

all: hello hello_button hello_world

hello: 00_hello.cpp 
	$(CXX) $(CXXFLAGS) 00_hello.cpp  $(GTKFLAGS) -o hello
hello_button: 01_main.cpp 01_mainwin.cpp *.h
	$(CXX) $(CXXFLAGS) 01_main.cpp 01_mainwin.cpp $(GTKFLAGS) -o hello_button
hello_world: 02_main.cpp 02_mainwin.cpp *.h
	$(CXX) $(CXXFLAGS) 02_main.cpp 02_mainwin.cpp $(GTKFLAGS) -o hello_world
clean:
	rm -f *.o *.gch a.out hello hello_button hello_world

