# Makefile for job_submit/cray_aries plugin

AUTOMAKE_OPTIONS = foreign

AM_CPPFLAGS = -DSLURM_PLUGIN_DEBUG -I$(top_srcdir)

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

pkglib_LTLIBRARIES = job_submit_cray_aries.la
job_submit_cray_aries_la_SOURCES = job_submit_cray_aries.c
job_submit_cray_aries_la_LDFLAGS = $(PLUGIN_FLAGS)

