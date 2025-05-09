#  File:	 Makefile
#  Author:	 Johan Bevemyr
#  Created:	 Fri Oct 18 09:59:34 1996

WARNING_OPTIONS =
LANGUAGE_OPTIONS = 
COMPILER_OPTIONS = -g 

CFLAGS   = $(WARNING_OPTIONS) $(LANGUAGE_OPTIONS) $(COMPILER_OPTIONS)

######################################################################

HEADER_FILES = serial.h
SOURCE_FILES = serial.c

OBJECT_FILES = $(SOURCE_FILES:.c=.o)

######################################################################

all: ../priv/serial

../priv/serial: $(OBJECT_FILES)
	$(CC) -o $@ $(LDFLAGS) $(OBJECT_FILES) $(LDLIBS)

clean:
	rm -f priv/serial $(OBJECT_FILES)

serial.o: serial.c serial.h

