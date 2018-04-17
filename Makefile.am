ACLOCAL_AMFLAGS = -I m4
MAINTAINERCLEANFILES = Makefile.in aclocal.m4 config.guess config.h.in \
		config.sub compile configure depcomp install-sh ltmain.sh \
		missing module.desktop config.rpath mkinstalldirs \
		m4/libtool.m4  m4/lt~obsolete.m4 m4/ltoptions.m4 \
		m4/ltsugar.m4 m4/ltversion.m4

SUBDIRS = src

EDJE_FLAGS = -v \
	         -id $(top_srcdir)

filesdir =  $(datadir)
files_DATA = module.desktop e-module-classicmenu.edj

EXTRA_DIST = module.desktop.in \
	         icon.png \
	         e-module-classicmenu.edc

%.edj:  %.edc
	$(EDJE_CC) $(EDJE_FLAGS) $< $@

clean-local:
	rm -rf e-module-classicmenu.edj module.desktop *~
uninstall:
	rm -rf $(DESTDIR)$(datadir)
