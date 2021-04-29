# Usage:
# make       # makes all test .prg files
# make clean # removes all .prg and .labels files

SRCS := $(wildcard *.a)
PRGS := $(SRCS:%.a=%.prg)
LIBS := $(wildcard ../libs/*.a)

all: ${PRGS}

%.prg: %.a ${LIBS}
	acme $<

clean:
	rm *.prg
	rm *.labels

