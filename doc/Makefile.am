EXTRA_DIST=libambix.doxy \
	libambix.incl

html_DATA=
if HAVE_DOXYGEN
html_DATA+=apiref/*
endif

apiref/*: all-local

all-local:
	$(DOXYGEN) $(srcdir)/libambix.doxy

clean-local:
	-rm -rf apiref

uninstall-local:
	-rm -rf "$(DESTDIR)$(docdir)/apiref"
