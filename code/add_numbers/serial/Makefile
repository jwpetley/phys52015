CC = icc

CFLAGS = -D_GNU_SOURCE -I. -std=c11 -O2 -qopt-report=5
LIBS = -lm

DEPS = proto.h
OBJ  = main.o add_numbers.o
EXE = addnumbers

.PHONY: all clean

all: $(EXE)

$(EXE): $(OBJ) $(DEPS)
	$(CC) $(CFLAGS) -o $@ $(OBJ) $(LIBS)

clean:
	-rm -f $(OBJ) $(EXE)
