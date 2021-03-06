#
# Copyright (C) 2015 Alon Bar-Lev <alon.barlev@gmail.com>
# SPDX-License-Identifier: GPL-3.0-or-later
#
MAINTAINERCLEANFILES= $(srcdir)/Makefile.in

dist_noinst_DATA = \
	README.md \
	$(NULL)

dist_web_DATA = \
	demo.html \
	demo2.html \
	demosites.html \
	demosites2.html \
	dashboard.html \
	dashboard.js \
	dashboard_info.js \
	dashboard_info_custom_example.js \
	dashboard.css \
	dashboard.slate.css \
	favicon.ico \
	goto-host-from-alarm.html \
	index.html \
	infographic.html \
	robots.txt \
	refresh-badges.js \
	registry.html \
	sitemap.xml \
	tv.html \
	version.txt \
	$(NULL)

weblibdir=$(webdir)/lib
dist_weblib_DATA = \
	lib/bootstrap-3.3.7.min.js \
	lib/bootstrap-slider-10.0.0.min.js \
	lib/bootstrap-table-1.11.0.min.js \
	lib/bootstrap-table-export-1.11.0.min.js \
	lib/bootstrap-toggle-2.2.2.min.js \
	lib/clipboard-polyfill-be05dad.js \
	lib/c3-0.4.18.min.js \
	lib/d3-4.12.2.min.js \
	lib/d3pie-0.2.1-netdata-3.js \
	lib/dygraph-c91c859.min.js \
	lib/dygraph-smooth-plotter-c91c859.js \
	lib/fontawesome-all-5.0.1.min.js \
	lib/gauge-1.3.2.min.js \
	lib/jquery-2.2.4.min.js \
	lib/jquery.easypiechart-97b5824.min.js \
	lib/jquery.peity-3.2.0.min.js \
	lib/jquery.sparkline-2.1.2.min.js \
	lib/lz-string-1.4.4.min.js \
	lib/morris-0.5.1.min.js \
	lib/pako-1.0.6.min.js \
	lib/perfect-scrollbar-0.6.15.min.js \
	lib/raphael-2.2.4-min.js \
	lib/tableExport-1.6.0.min.js \
	$(NULL)

webcssdir=$(webdir)/css
dist_webcss_DATA = \
	css/morris-0.5.1.css \
	css/bootstrap-3.3.7.css \
	css/bootstrap-theme-3.3.7.min.css \
	css/bootstrap-slate-flat-3.3.7.css \
	css/bootstrap-slider-10.0.0.min.css \
	css/bootstrap-toggle-2.2.2.min.css \
	css/c3-0.4.18.min.css \
	$(NULL)

webfontsdir=$(webdir)/fonts
dist_webfonts_DATA = \
	fonts/glyphicons-halflings-regular.eot \
	fonts/glyphicons-halflings-regular.svg \
	fonts/glyphicons-halflings-regular.ttf \
	fonts/glyphicons-halflings-regular.woff \
	fonts/glyphicons-halflings-regular.woff2 \
	$(NULL)

webimagesdir=$(webdir)/images
dist_webimages_DATA = \
	images/alert-128-orange.png \
	images/alert-128-red.png \
	images/alert-multi-size-orange.ico \
	images/alert-multi-size-red.ico \
	images/animated.gif \
	images/check-mark-2-128-green.png \
	images/check-mark-2-multi-size-green.ico \
	images/netdata.svg \
	images/post.png \
	images/seo-performance-16.png \
	images/seo-performance-24.png \
	images/seo-performance-32.png \
	images/seo-performance-48.png \
	images/seo-performance-64.png \
	images/seo-performance-72.png \
	images/seo-performance-114.png \
	images/seo-performance-128.png \
	images/seo-performance-256.png \
	images/seo-performance-512.png \
	images/seo-performance-multi-size.ico \
	images/seo-performance-multi-size.icns \
	$(NULL)


webwellknowndir=$(webdir)/.well-known
dist_webwellknown_DATA = \
	$(NULL)

webdntdir=$(webdir)/.well-known/dnt
dist_webdnt_DATA = \
	.well-known/dnt/cookies \
	$(NULL)

version.txt:
	if test -d "$(top_srcdir)/.git"; then \
		git --git-dir="$(top_srcdir)/.git" log -n 1 --format=%H; \
	fi > $@.tmp
	test -s $@.tmp || echo 0 > $@.tmp
	mv $@.tmp $@

.PHONY: version.txt
