# Makefile for job_submit/partition plugin

AUTOMAKE_OPTIONS = foreign

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -DSLURM_PLUGIN_DEBUG -I$(top_srcdir)

pkglib_LTLIBRARIES = job_submit_partition.la

# Job submit partition plugin.
job_submit_partition_la_SOURCES = job_submit_partition.c
job_submit_partition_la_LDFLAGS = $(PLUGIN_FLAGS)
