ACLOCAL_AMFLAGS = -I m4
MAINTAINERCLEANFILES = Makefile.in aclocal.m4 config.guess config.h.in \
		config.sub compile configure depcomp install-sh ltmain.sh \
		missing module.desktop config.rpath mkinstalldirs \
		m4/libtool.m4  m4/lt~obsolete.m4 m4/ltoptions.m4 \
		m4/ltsugar.m4 m4/ltversion.m4

SUBDIRS = src

filesdir =  $(datadir)
files_DATA = module.desktop

EXTRA_DIST = module.desktop.in \
	         icon.png
clean-local:
	rm -rf module.desktop *~

uninstall:
	rm -rf $(DESTDIR)$(datadir)
