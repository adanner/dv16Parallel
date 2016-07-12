TGTS = trap-omp trap-omp-notworking trap-omp-timed trap-omp-unfinished trap-omp-working
all:  $(TGTS)


CXX = g++
CXXFLAGS = -Wall -ansi -pedantic -std=c++11
LFLAGS = -fopenmp

%: %.cpp
	$(CXX) $(CXXFLAGS) $(LFLAGS) $< -o $@

clean:
	rm -f a.out $(TGTS)

.PHONY: all clean
