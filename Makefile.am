
AUTOMAKE_OPTIONS = nostdinc

dist_xdetheme_DATA = \
	theme/theme.ini \
	theme/themerc

dist_wmakertheme_DATA = \
	theme/style

dist_xdeimage_DATA = \
	images/atc.jpg \
	images/atc2.jpg \
	images/changi.jpg \
	images/gatwick.jpg \
	images/jersey.jpg \
	images/takeoff.jpg \
	images/sillouette.jpg \
	images/routes.jpg

EXTRA_DIST = \
	images/atc2.jpg \
	images/atc.jpg \
	images/changi.jpg \
	images/control.jpg \
	images/cyeg.jpg \
	images/darktower.jpg \
	images/dulles.jpg \
	images/floor.jpg \
	images/gatwick.jpg \
	images/jersey_atc.jpg \
	images/jersey.jpg \
	images/lax.jpg \
	images/main.jpg \
	images/reagan.jpg \
	images/routes.jpg \
	images/sillouette.jpg \
	images/sunrise_control_tower.jpg \
	images/takeoff.jpg \
	images/united.jpg \
	images/virtual.jpg

install-data-hook:
	mkdir -p $(DESTDIR)$(waimeastylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(waimeastylesdir)/$(style)
	mkdir -p $(DESTDIR)$(fluxboxstylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(fluxboxstylesdir)/$(style)
	mkdir -p $(DESTDIR)$(blackboxstylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(blackboxstylesdir)/$(style)
	mkdir -p $(DESTDIR)$(icewmthemesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(icewmthemesdir)/$(style)
	mkdir -p $(DESTDIR)$(jwmthemesdir)
	$(LN_S) ../styles/$(basestyle) $(DESTDIR)$(jwmthemesdir)/$(style)
	mkdir -p $(DESTDIR)$(ctwmstylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(ctwmstylesdir)/$(style)
	mkdir -p $(DESTDIR)$(vtwmstylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(vtwmstylesdir)/$(style)
	mkdir -p $(DESTDIR)$(twmstylesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(twmstylesdir)/$(style)
	mkdir -p $(DESTDIR)$(pekwmthemesdir)
	$(LN_S) $(basestyle) $(DESTDIR)$(pekwmthemesdir)/$(style)
	mkdir -p $(DESTDIR)$(themedir)
	$(LN_S) ../$(basestyle)/openbox-3 $(DESTDIR)$(themedir)/openbox-3
	mkdir -p $(DESTDIR)$(themedir)
	$(LN_S) ../$(basestyle)/gtk-2.0 $(DESTDIR)$(themedir)/gtk-2.0
	mkdir -p $(DESTDIR)$(wmakerthemedir)
	mkdir -p $(DESTDIR)$(fluxboxbgdir)
	mkdir -p $(DESTDIR)$(blackboxbgdir)
	mkdir -p $(DESTDIR)$(wmakerbgdir)
	mkdir -p $(DESTDIR)$(xdeimagedir)
	for p in $(dist_xdeimage_DATA) ; do \
		f=$$(basename $$p .jpg) ; \
		install -m644 $(top_srcdir)/images/$$f.jpg $(DESTDIR)$(xdeimagedir)/$$f.jpg ; \
		$(LN_S) ../../../images/$(stylesubdir)/$$f.jpg $(DESTDIR)$(wmakerthemedir)/$$f.jpg ; \
		$(LN_S) ../../images/$(stylesubdir)/$$f.jpg $(DESTDIR)$(fluxboxbgdir)/$$f.jpg ; \
		$(LN_S) ../../images/$(stylesubdir)/$$f.jpg $(DESTDIR)$(blackboxbgdir)/$$f.jpg ; \
		$(LN_S) ../../images/$(stylesubdir)/$$f.jpg $(DESTDIR)$(wmakerbgdir)/$$f.jpg ; \
	done
	for f in $(baseprefix)back $(baseprefix)icon $(baseprefix)tbar $(baseprefix)tile ; do \
		$(LN_S) ../../../WindowMaker/Pixmaps/$$f.xpm $(DESTDIR)$(wmakerthemedir)/$$f.xpm ; \
	done

