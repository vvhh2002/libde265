
bin_PROGRAMS = dec265

AM_CPPFLAGS = -I../libde265

dec265_DEPENDENCIES = ../libde265/libde265.la
dec265_CXXFLAGS = $(VIDEOGFX_CFLAGS)
dec265_LDFLAGS = $(VIDEOGFX_LIBS)
dec265_LDADD = ../libde265/libde265.la -lstdc++
dec265_SOURCES = dec265.cc

if MINGW
  dec265_LDFLAGS += -static-libgcc -static-libstdc++
endif

EXTRA_DIST = Makefile.vc7 \
  CMakeLists.txt \
  ../extra/getopt.c \
  ../extra/getopt.h \
  ../extra/getopt_long.c
