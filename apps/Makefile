all:
	$(MAKE) -C bundle2pset
	$(MAKE) -C dmrecon
	$(MAKE) -C makescene
	$(MAKE) -C meshconvert
	$(MAKE) -C scene2pset
	$(MAKE) -C fssrecon
	$(MAKE) -C mesh2pset
	$(MAKE) -C meshalign
	$(MAKE) -C meshclean

clean:
	$(MAKE) -C bundle2pset $@
	$(MAKE) -C dmrecon $@
	$(MAKE) -C makescene $@
	$(MAKE) -C meshconvert $@
	$(MAKE) -C scene2pset $@
	$(MAKE) -C fssrecon $@
	$(MAKE) -C mesh2pset $@
	$(MAKE) -C meshalign $@
	$(MAKE) -C meshclean $@

BINDIR ?= $(HOME)/bin/
APPDIR := $(shell pwd)

links:
	ln -si $(APPDIR)/bundle2pset/bundle2pset $(BINDIR)
	ln -si $(APPDIR)/dmrecon/dmrecon $(BINDIR)
	ln -si $(APPDIR)/makescene/makescene $(BINDIR)
	ln -si $(APPDIR)/meshconvert/meshconvert $(BINDIR)
	ln -si $(APPDIR)/scene2pset/scene2pset $(BINDIR)
	ln -si $(APPDIR)/fssrecon/fssrecon $(BINDIR)
	ln -si $(APPDIR)/mesh2pset/mesh2pset $(BINDIR)
	ln -si $(APPDIR)/meshalign/meshalign $(BINDIR)
	ln -si $(APPDIR)/meshclean/meshclean $(BINDIR)
	ln -si $(APPDIR)/umve/umve $(BINDIR)

.PHONY: all clean links
