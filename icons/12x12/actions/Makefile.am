size = 12x12
context = actions
iconsdir = $(themedir)/$(size)/$(context)
icons_DATA = 				 		\
		info.png 		\
		list-add.png 		\
		list-remove.png
EXTRA_DIST = $(icons_DATA)

install-data-local: install-iconsDATA
	(cd $(DESTDIR)$(themedir)/$(size) && $(ICONMAP) -c $(context) -e $(iconsrcdir)/icons/my-mapping.xml)

uninstall-local:
	rm -Rf $(DESTDIR)$(themedir)/$(size)/$(context)
