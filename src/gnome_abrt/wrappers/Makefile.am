wrappersexecdir = $(pyexecdir)/gnome_abrt/wrappers

wrappersexec_PYTHON =  __init__.py

wrappersexec_LTLIBRARIES = _wrappers.la

_wrappers_la_SOURCES = \
    module.c \
    configure.c \
    common.h

_wrappers_la_CPPFLAGS = \
    $(GLIB_CFLAGS) \
    $(PYTHON_CFLAGS) \
    $(PYGOBJECT3_CFLAGS) \
    $(GTK_CFLAGS) \
    $(LIBREPORT_GTK_CFLAGS)

_wrappers_la_LDFLAGS = \
    $(LIBREPORT_GTK_LIBS) \
    $(GTK_LIBS) \
    $(PYGOBJECT3_LIBS) \
    -module \
    -avoid-version \
    -export-symbols-regex init_wrappers