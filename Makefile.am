ACLOCAL_AMFLAGS = --install -I m4

docs_DATA = README.md sfx_config.h
docsdir = $(prefix)/$(PARENT_PACKAGE)

EXTRA_DIST = docs

install-data-hook:
	cd "$(DESTDIR)${prefix}/$(PARENT_PACKAGE)"; \
	mv README.md sfx_readme.md
