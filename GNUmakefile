.POSIX:
.SUFFIXES:
.PHONY: all clean install check

PROJECT   =getprj
VERSION   =1.0.0
PREFIX    =/usr/local
BUILDDIR ?=.build

all:
clean:
install:
check:
## -- BLOCK:license --
install: install-license
install-license: README.md COPYING
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp README.md COPYING $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/getprj $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
