PROGRAM = ssd1306
CXX = gcc
OBJECTS = \
	ssd1306.o \

.SUFFIXES: .o .c

all: $(PROGRAM)

$(OBJECTS): %.o:%.c
	$(CXX) -fPIC -c $<

$(PROGRAM): $(OBJECTS)
	$(CXX) $(INC) -o $(PROGRAM) $(OBJECTS) -lwiringPi

clean:
	rm -f *.o $(PROGRAM)

