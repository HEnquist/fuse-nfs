SUBDIRS = doc fuse
ACLOCAL_AMFLAGS = -I m4

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = fuse-nfs.pc

EXTRA_DIST = \
	README \
	COPYING \
	LICENCE-GPL-3.txt \
	fuse \
	fuse-nfs.pc.in

install-exec-hook:
	$(LN_S) ${bindir}/fuse-nfs /usr/bin/mount.fuse-nfs

uninstall-hook:
	rm -f /usr/bin/mount.fuse-nfs