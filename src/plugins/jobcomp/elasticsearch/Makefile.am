# Makefile for jobcomp/elasticsearch plugin

AUTOMAKE_OPTIONS = foreign

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -DSLURM_PLUGIN_DEBUG -I$(top_srcdir) $(LIBCURL_CPPFLAGS)

AS_ELASTICSEARCH_SOURCES = jobcomp_elasticsearch.c

if WITH_CURL
pkglib_LTLIBRARIES = jobcomp_elasticsearch.la

jobcomp_elasticsearch_la_SOURCES = $(AS_ELASTICSEARCH_SOURCES)
jobcomp_elasticsearch_la_LDFLAGS = $(PLUGIN_FLAGS)
jobcomp_elasticsearch_la_LIBADD = $(LIBCURL) ../common/libjobcomp_common.la

else
EXTRA_jobcomp_elasticsearch_la_SOURCES = $(AS_ELASTICSEARCH_SOURCES)
endif
