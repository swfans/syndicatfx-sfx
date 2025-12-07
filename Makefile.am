ACLOCAL_AMFLAGS = --install -I m4

instrumconf_DATA = sound/midipats.cfg
instrumconfdir = $(prefix)/$(PARENT_PACKAGE)/sound

sound/%.cfg: $(top_srcdir)/instruments/%.cfg
	$(MKDIR_P) "$(@D)"
	cp -p "$<" "$@"

instrumpats_DATA = \
  sound/Tone_000/008_Celesta.pat \
  sound/Tone_000/012_Marimba.pat \
  sound/Tone_000/013_Xylophone.pat \
  sound/Tone_000/024_Acoustic_guitar.pat \
  sound/Tone_000/026_Electric_Jazz_Guitar.pat \
  sound/Tone_000/032_BassLead.pat \
  sound/Tone_000/041_Viola.pat \
  sound/Tone_000/093_Metal_Pad.pat \
  sound/Tone_000/096_Tubular_Bells.pat \
  sound/Tone_000/100_Brightness.pat \
  sound/Tone_000/100_FX5.pat \
  sound/Tone_000/103_Star_Theme.pat \
  sound/Tone_000/115_Woodblock.pat \
  sound/Tone_000/125_5th_Saw_Wave.pat
instrumpatsdir = $(prefix)/$(PARENT_PACKAGE)/sound/Tone_000

sound/Tone_000/%.pat: $(top_srcdir)/instruments/Tone_000/%.pat
	$(MKDIR_P) "$(@D)"
	cp -p "$<" "$@"

docs_DATA = README.md sfx_config.h
docsdir = $(prefix)/$(PARENT_PACKAGE)

EXTRA_DIST = instrumpats instrumconf docs

install-data-hook:
	cd "$(DESTDIR)${prefix}/$(PARENT_PACKAGE)"; \
	mv README.md sfx_readme.md
