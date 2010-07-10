libdir=$(prefix)/lib/openvanilla/

lib_LTLIBRARIES = OVIMGeneric.la
OVIMGeneric_la_SOURCES = CIN-Defaults.cpp CIN-Defaults.h OVIMGeneric.cpp OVIMGeneric.h
OVIMGeneric_la_CPPFLAGS = -I$(top_srcdir)/Frameworks/OpenVanilla -I$(top_srcdir)/Modules/SharedLibrary/
OVIMGeneric_la_LIBADD = ../SharedLibrary/libSharedLibrary.la
OVIMGeneric_la_LDFLAGS = -module -avoid-version -no-undefined -Wl,-E -Bsymbolic

EXTRA_DIST= OVIMGeneric-Info.plist
