if ADDON_FILMON
          ADDON_FILMON_SUBDIRS = pvr.filmon
endif
if ADDON_IPTVSIMPLE
          ADDON_IPTVSIMPLE_SUBDIRS = pvr.iptvsimple
endif

### Keep this in alphabetical order
SUBDIRS = pvr.argustv \
          pvr.demo \
          pvr.dvblink \
          pvr.dvbviewer \
          pvr.hts \
          pvr.mediaportal.tvserver \
          pvr.mythtv \
          pvr.nextpvr \
          pvr.njoy \
		  pvr.pctv \
          pvr.vdr.vnsi \
          pvr.vuplus \
          pvr.wmc \
          $(ADDON_FILMON_SUBDIRS) \
          $(ADDON_IPTVSIMPLE_SUBDIRS) \
          $(ADDON_MYTHTV_SUBDIRS)

clean:
	-rm -f *.zip
	for d in $(SUBDIRS); do if test -f $$d/Makefile; then $(MAKE) -C $$d clean; fi; done

zip:
	for d in $(SUBDIRS); do if test -f $$d/Makefile; then $(MAKE) -C $$d zip; fi; done

install:
	for d in $(SUBDIRS); do if test -f $$d/Makefile; then $(MAKE) -C $$d install; fi; done

