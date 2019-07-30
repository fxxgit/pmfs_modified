#
# Makefile for the linux pmfs-filesystem routines.
#

#obj-m += pmfs.o

#pmfs-y := bbuild.o balloc.o dir.o file.o inode.o namei.o super.o symlink.o ioctl.o pmfs_stats.o journal.o xip.o wprotect.o

#all:
#	make -C /lib/modules/$(shell uname -r)/build M=`pwd`

#clean:
#	rm -rf *.o *.mod.c modules.* Module.* *.ko




obj-$(CONFIG_PMFS) += pmfs.o
obj-$(CONFIG_PMFS_TEST_MODULE) += pmfs_test.o

pmfs-y := bbuild.o balloc.o dir.o file.o inode.o namei.o super.o symlink.o ioctl.o pmfs_stats.o journal.o xip.o wprotect.o

pmfs-$(CONFIG_PMFS_WRITE_PROTECT) += wprotect.o
pmfs-$(CONFIG_PMFS_XIP) += xip.o
