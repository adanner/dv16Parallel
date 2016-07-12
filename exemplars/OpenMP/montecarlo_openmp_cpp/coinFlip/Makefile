TGTS = coinFlip_seq coinFlip_omp coinFlip_omp_seeds

all:  $(TGTS)


CXX = g++
CXXFLAGS = -Wall -ansi -pedantic -std=c++11
LFLAGS = -fopenmp

%: %.cpp
	$(CXX) $(CXXFLAGS) $(LFLAGS) $< -o $@

clean:
	rm -f a.out $(TGTS)

.PHONY: all clean
