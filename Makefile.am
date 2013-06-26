DIST_SUBDIRS = m4 t

# EXTRA_DIST = jd_path.h jd_utf8.h

SUBDIRS = . t

ACLOCAL_AMFLAGS = -I m4

lib_LTLIBRARIES = libhlsm3u8.la

include_HEADERS = hlsrelay.h

bin_PROGRAMS = hlsrelay

libhlsm3u8_la_SOURCES = hlsm3u8.c hlsm3u8.h

hlsrelay_SOURCES = hlsrelay.c utils.c utils.h
hlsrelay_LDADD = libhlsm3u8.la

test: all
	cd t && $(MAKE) test

