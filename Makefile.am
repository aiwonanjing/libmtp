SUBDIRS=src util doc
ACLOCAL_AMFLAGS=-I m4

pkgconfigdir=$(libdir)/pkgconfig
pkgconfig_DATA=libmtp.pc

EXTRA_DIST=libmtp.pc libmtp.sh COPYING README.windows.txt

# This stuff only makes sense on Linux so only
# build and ship it on Linux.
#if USE_LINUX
#udevrulesdir=@UDEV@/rules.d
#hwdbdir=@UDEV@/hwdb.d
#udevrules_DATA=@UDEV_RULES@
#hwdb_DATA=69-libmtp.hwdb
#noinst_DATA=libmtp.usermap libmtp.fdi
#
#libmtp.usermap: util/mtp-hotplug
#	util/mtp-hotplug > libmtp.usermap
#
#@UDEV_RULES@: util/mtp-hotplug
#	util/mtp-hotplug -u -p"@UDEV@" @UDEV_GROUP@ @UDEV_MODE@ > @UDEV_RULES@
#
#libmtp.fdi: util/mtp-hotplug
#	util/mtp-hotplug -H > libmtp.fdi
#
#$(hwdb_DATA): util/mtp-hotplug
#	util/mtp-hotplug -w > $(hwdb_DATA)
#
#CLEANFILES = libmtp.usermap @UDEV_RULES@ libmtp.fdi libmtp.hwdb
#endif
