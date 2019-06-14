CXXFLAGS = -g -Wall
LDLIBS = -lGL -lglfw -lGLEW -lXrandr -lXinerama -lXcursor -lXi \
-lXxf86vm -lX11 -lpthread -lrt -lm -ldl -lglut -lGLU -lGL

OBJECTS = $(patsubst %.c,%.o,$(wildcard *.c))
TARGET = c0117035


${TARGET} : ${OBJECTS}
	${LINK.cc} $^ ${LOADLIBES} ${LDLIBS} -o $@
	./c0117035

.PHONY : clean
clean :
	-${RM} ${TARGET} ${OBJECTS} *~ .*~ core
