AUTOMAKE_OPTIONS = foreign

SUBDIRS = math

BUILT_SOURCES = libbenchmark.la

noinst_LTLIBRARIES = libbenchmark.la
libbenchmark_la_SOURCES = \
    benchmark.c
libbenchmark_la_CPPFLAGS = $(AM_CPPFLAGS) -DNDEBUG
libbenchmark_la_LIBADD = $(BENCHMARK_LIBS)

noinst_HEADERS = benchmark.h bench_tmpl.h
noinst_PROGRAMS = example

example_SOURCES = example.c
example_CPPFLAGS = $(AM_CPPFLAGS) -DNDEBUG
example_LDADD = libbenchmark.la $(top_builddir)/src/libpal.la
