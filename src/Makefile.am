moduledir = $(libdir)/gtk-3.0/modules

libgtkparasite_la_SOURCES = \
	action-list.c \
	action-list.h \
	inspect-button.c \
	module.c \
	parasite.h \
	prop-list.h \
	prop-list.c \
	property-cell-renderer.c \
	property-cell-renderer.h \
	widget-tree.h \
	widget-tree.c \
	window.c

libgtkparasite_la_LDFLAGS = \
	-rpath $(moduledir) -module -avoid-version \
	$(GTK_LIBS) \
	$(PYGTK_LIBS) \
	@LDFLAGS@

libgtkparasite_la_LIBADD =


module_LTLIBRARIES = libgtkparasite.la

INCLUDES = $(GTK_CFLAGS)

if HAVE_X11
INCLUDES += -DHAVE_X11
endif
