
CXX = g++
CXXFLAGS = -std=c++14 -Wall -MMD
LIB = -O2 -larmadillo
EXEC = Test
OBJECTS = test.o LinearRegression.o LogisticRegression.o
DEPENDS = ${OBJECTS:.o=.d}

${EXEC}: ${OBJECTS}
	${CXX} ${CXXFLAGS} ${OBJECTS} -o ${EXEC} ${LIB}

-include ${DEPENDS}

.PHONY: clean

clean:
	rm ${OBJECTS} ${EXEC} ${DEPENDS}
