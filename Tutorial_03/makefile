CSRCS=texturedGeometry.cpp

CFLAGS = -g -c -O2 -DLINUX -lrt

INCLUDE = -I. -I/usr/local/include/ -I/usr/include/ -I/usr/include/X11/ -I/usr/include/GL 
INCOSG = -I/usr/local/include
LDLIBS = -lm -lrt -ldl -lGL -lrt -lGLU -lpthread -lXext -lX11 -lrt

LDFLAGS=-losg -losgGA -losgDB -losgViewer -losgText -losgUtil -lOpenThreads
LDOSG = -L/usr/lib -losg -losgViewer
COBJS=$(patsubst %.cpp,%.o,$(CSRCS))

CC = g++

EXE=run

all:
	$(CC) $(CSRCS) $(LDFLAGS) $(LDLIBS)  -o $(EXE)

