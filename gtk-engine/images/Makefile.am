
IMAGES = \
	button-corner-active-bottom-left.png		\
	button-corner-active-bottom-right.png		\
	button-corner-active-top-left.png		\
	button-corner-active-top-right.png		\
	button-corner-disabled-bottom-left.png		\
	button-corner-disabled-bottom-right.png		\
	button-corner-disabled-top-left.png		\
	button-corner-disabled-top-right.png		\
	button-corner-normal-bottom-left.png		\
	button-corner-normal-bottom-right.png		\
	button-corner-normal-top-left.png		\
	button-corner-normal-top-right.png		\
	button-corner-prelight-bottom-left.png		\
	button-corner-prelight-bottom-right.png		\
	button-corner-prelight-top-left.png		\
	button-corner-prelight-top-right.png		\
	button-default-corner-active-bottom-left.png	\
	button-default-corner-active-bottom-right.png	\
	button-default-corner-active-top-left.png	\
	button-default-corner-active-top-right.png	\
	button-default-corner-normal-bottom-left.png	\
	button-default-corner-normal-bottom-right.png	\
	button-default-corner-normal-top-left.png	\
	button-default-corner-normal-top-right.png	\
	button-default-corner-prelight-bottom-left.png	\
	button-default-corner-prelight-bottom-right.png	\
	button-default-corner-prelight-top-left.png	\
	button-default-corner-prelight-top-right.png	\
	combo-caret-active.png				\
	combo-caret-disable.png				\
	combo-caret-normal.png				\
	combo-caret-prelight.png			\
	arrow-bottom-active.png				\
	arrow-bottom-disable.png			\
	arrow-bottom-normal.png				\
	arrow-top-active.png				\
	arrow-top-disable.png				\
	arrow-top-normal.png				\
	check-active-not-set.png			\
	check-active-set.png				\
	check-active-inconsistent.png			\
	check-disable-not-set.png			\
	check-disable-set.png				\
	check-disable-inconsistent.png			\
	check-normal-not-set.png			\
	check-normal-set.png				\
	check-normal-inconsistent.png			\
	check-prelight-not-set.png			\
	check-prelight-set.png				\
	check-prelight-inconsistent.png			\
	radio-active-not-set.png			\
	radio-active-set.png				\
	radio-active-inconsistent.png			\
	radio-disable-not-set.png			\
	radio-disable-set.png				\
	radio-disable-inconsistent.png			\
	radio-normal-not-set.png			\
	radio-normal-set.png				\
	radio-normal-inconsistent.png			\
	radio-prelight-not-set.png			\
	radio-prelight-set.png				\
	radio-prelight-inconsistent.png			\
	scroll-bar-h-bkg-disable.png			\
	scroll-bar-h-bkg-normal.png			\
	scroll-bar-h-left-active.png			\
	scroll-bar-h-left-normal.png			\
	scroll-bar-h-left-prelight.png			\
	scroll-bar-h-mid-active.png			\
	scroll-bar-h-mid-normal.png			\
	scroll-bar-h-mid-prelight.png			\
	scroll-bar-h-right-active.png			\
	scroll-bar-h-right-normal.png			\
	scroll-bar-h-right-prelight.png			\
	scroll-button-h-left-active.png			\
	scroll-button-h-left-normal.png			\
	scroll-button-h-left-prelight.png		\
	scroll-button-h-right-active.png		\
	scroll-button-h-right-normal.png		\
	scroll-button-h-right-prelight.png		\
	pane-h.png					\
	pane-v.png					\
	scale-button-active.png				\
	scale-button-disable.png			\
	scale-button-normal.png				\
	scale-button-prelight.png			\
	scale-corner-left-disable.png			\
	scale-corner-left-normal.png			\
	scale-corner-mid-disable.png			\
	scale-corner-mid-normal.png			\
	scale-corner-right-disable.png			\
	scale-corner-right-normal.png			\
	progress-shadow-bottom.png			\
	progress-shadow-corner-bottom-left.png		\
	progress-shadow-corner-bottom-right.png		\
	progress-shadow-corner-top-left.png		\
	progress-shadow-corner-top-right.png		\
	progress-shadow-left.png			\
	progress-shadow-right.png			\
	progress-shadow-top.png				\
	handlebar-top.png				\
	handlebar-mid.png				\
	handlebar-bottom.png				\
	check-menu-disable-set.png			\
	check-menu-normal-set.png			\
	check-menu-prelight-set.png			\
	radio-menu-disable-set.png			\
	radio-menu-normal-set.png			\
	radio-menu-prelight-set.png			\
	dark-button-corner-active-bottom-left.png	\
	dark-button-corner-active-bottom-right.png	\
	dark-button-corner-active-top-left.png		\
	dark-button-corner-active-top-right.png		\
	dark-button-corner-disabled-bottom-left.png	\
	dark-button-corner-disabled-bottom-right.png	\
	dark-button-corner-disabled-top-left.png	\
	dark-button-corner-disabled-top-right.png	\
	dark-button-corner-normal-bottom-left.png	\
	dark-button-corner-normal-bottom-right.png	\
	dark-button-corner-normal-top-left.png		\
	dark-button-corner-normal-top-right.png		\
	dark-button-corner-prelight-bottom-left.png	\
	dark-button-corner-prelight-bottom-right.png	\
	dark-button-corner-prelight-top-left.png	\
	dark-button-corner-prelight-top-right.png
	

noinst_DATA = images.h
CLEANFILES = $(noinst_DATA)

BUILT_SOURCES =	images.h
    
images.h: $(IMAGES) Makefile
	rm -f images.h ;\
	for tmp in $(IMAGES) ;\
	do \
	pix_name=`echo  $$tmp | sed -e "s/\.png//g" | sed -e "s/-/_/g"` ;\
	$(GDK_PIXBUF_CSOURCE) --rle --name=$$pix_name $$tmp >> images.h ;\
	done

EXTRA_DIST = $(IMAGES) images.h
