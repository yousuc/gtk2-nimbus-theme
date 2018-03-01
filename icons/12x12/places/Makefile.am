size = 12x12
context = places
iconsdir = $(themedir)/$(size)/$(context)
icons_DATA = 				 		\
		file.png 		\
        folder-documents.png        \
        folder-download.png     \
		folder-drag-accept.png 		\
        folder-music.png        \
        folder-pictures.png     \
        folder-publicshare.png      \
        folder-saved-search.png     \
        folder-templates.png        \
        folder-videos.png       \
		folder.png
EXTRA_DIST = $(icons_DATA)

install-data-local: install-iconsDATA
	(cd $(DESTDIR)$(themedir)/$(size) && $(ICONMAP) -c $(context) -e $(iconsrcdir)/icons/my-mapping.xml)

uninstall-local:
	rm -Rf $(DESTDIR)$(themedir)/$(size)/$(context)
