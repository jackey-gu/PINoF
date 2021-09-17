SUBDIRS := $(shell pwd)
VERSION := $(shell uname -r)

KSRC := /lib/modules/$(VERSION)/build
MPRE := /lib/modules/$(VERSION)/extra
INCS := $(SUBDIRS)/include 

all: kernel

kernel:
	make -C $(KSRC) M=$(SUBDIRS)/host KCFLAGS="-DDEBUG" INCDIR="-I$(INCS) -I$(SUBDIRS)/host" modules
	make -C $(KSRC) M=$(SUBDIRS)/target KCFLAGS="-DDEBUG" INCDIR="-I$(INCS) -I$(SUBDIRS)/target " modules

clean:
	make -C $(KSRC) M=$(SUBDIRS)/host clean
	make -C $(KSRC) M=$(SUBDIRS)/target clean

