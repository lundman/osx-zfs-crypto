SUBDIRS = fm fs crypto

COMMON_H = \
	$(top_srcdir)/include/sys/arc.h \
	$(top_srcdir)/include/sys/avl.h \
	$(top_srcdir)/include/sys/avl_impl.h \
	$(top_srcdir)/include/sys/blkptr.h \
	$(top_srcdir)/include/sys/bplist.h \
	$(top_srcdir)/include/sys/bpobj.h \
	$(top_srcdir)/include/sys/bptree.h \
	$(top_srcdir)/include/sys/dbuf.h \
	$(top_srcdir)/include/sys/ddt.h \
	$(top_srcdir)/include/sys/dmu.h \
	$(top_srcdir)/include/sys/dmu_impl.h \
	$(top_srcdir)/include/sys/dmu_objset.h \
	$(top_srcdir)/include/sys/dmu_send.h \
	$(top_srcdir)/include/sys/dmu_traverse.h \
	$(top_srcdir)/include/sys/dmu_tx.h \
	$(top_srcdir)/include/sys/dmu_zfetch.h \
	$(top_srcdir)/include/sys/dnode.h \
	$(top_srcdir)/include/sys/dsl_bookmark.h \
	$(top_srcdir)/include/sys/dsl_dataset.h \
	$(top_srcdir)/include/sys/dsl_deadlist.h \
	$(top_srcdir)/include/sys/dsl_deleg.h \
	$(top_srcdir)/include/sys/dsl_destroy.h \
	$(top_srcdir)/include/sys/dsl_dir.h \
	$(top_srcdir)/include/sys/dsl_pool.h \
	$(top_srcdir)/include/sys/dsl_prop.h \
	$(top_srcdir)/include/sys/dsl_scan.h \
	$(top_srcdir)/include/sys/dsl_synctask.h \
	$(top_srcdir)/include/sys/dsl_userhold.h \
	$(top_srcdir)/include/sys/efi_partition.h \
	$(top_srcdir)/include/sys/metaslab.h \
	$(top_srcdir)/include/sys/metaslab_impl.h \
	$(top_srcdir)/include/sys/nvpair.h \
	$(top_srcdir)/include/sys/nvpair_impl.h \
	$(top_srcdir)/include/sys/range_tree.h \
	$(top_srcdir)/include/sys/refcount.h \
	$(top_srcdir)/include/sys/rrwlock.h \
	$(top_srcdir)/include/sys/sa.h \
	$(top_srcdir)/include/sys/sa_impl.h \
	$(top_srcdir)/include/sys/spa_boot.h \
	$(top_srcdir)/include/sys/space_map.h \
	$(top_srcdir)/include/sys/space_reftree.h \
	$(top_srcdir)/include/sys/spa.h \
	$(top_srcdir)/include/sys/spa_impl.h \
	$(top_srcdir)/include/sys/txg.h \
	$(top_srcdir)/include/sys/txg_impl.h \
	$(top_srcdir)/include/sys/u8_textprep_data.h \
	$(top_srcdir)/include/sys/u8_textprep.h \
	$(top_srcdir)/include/sys/uberblock.h \
	$(top_srcdir)/include/sys/uberblock_impl.h \
	$(top_srcdir)/include/sys/uio_impl.h \
	$(top_srcdir)/include/sys/unique.h \
	$(top_srcdir)/include/sys/uuid.h \
	$(top_srcdir)/include/sys/vdev_disk.h \
	$(top_srcdir)/include/sys/vdev_file.h \
	$(top_srcdir)/include/sys/vdev.h \
	$(top_srcdir)/include/sys/vdev_impl.h \
	$(top_srcdir)/include/sys/xvattr.h \
	$(top_srcdir)/include/sys/zap.h \
	$(top_srcdir)/include/sys/zap_impl.h \
	$(top_srcdir)/include/sys/zap_leaf.h \
	$(top_srcdir)/include/sys/zfeature.h \
	$(top_srcdir)/include/sys/zfs_acl.h \
	$(top_srcdir)/include/sys/zfs_context.h \
	$(top_srcdir)/include/sys/zfs_ctldir.h \
	$(top_srcdir)/include/sys/zfs_debug.h \
	$(top_srcdir)/include/sys/zfs_delay.h \
	$(top_srcdir)/include/sys/zfs_dir.h \
	$(top_srcdir)/include/sys/zfs_fuid.h \
	$(top_srcdir)/include/sys/zfs_mount.h \
	$(top_srcdir)/include/sys/zfs_rlock.h \
	$(top_srcdir)/include/sys/zfs_sa.h \
	$(top_srcdir)/include/sys/zfs_stat.h \
	$(top_srcdir)/include/sys/zfs_vfsops.h \
	$(top_srcdir)/include/sys/zfs_vnops.h \
	$(top_srcdir)/include/sys/zfs_znode.h \
	$(top_srcdir)/include/sys/zil.h \
	$(top_srcdir)/include/sys/zil_impl.h \
	$(top_srcdir)/include/sys/zio_checksum.h \
	$(top_srcdir)/include/sys/zio_compress.h \
	$(top_srcdir)/include/sys/zio.h \
	$(top_srcdir)/include/sys/zio_impl.h \
	$(top_srcdir)/include/sys/zrlock.h

KERNEL_H = \
	$(top_srcdir)/include/sys/zfs_ioctl.h \
	$(top_srcdir)/include/sys/zfs_onexit.h \
	${top_srcdir}/include/sys/zpl.h \
	$(top_srcdir)/include/sys/zvol.h \
	$(top_srcdir)/include/sys/dsl_crypto.h \
	$(top_srcdir)/include/sys/zcrypt.h \
	$(top_srcdir)/include/sys/zio_crypt.h

USER_H =

EXTRA_DIST = $(COMMON_H) $(KERNEL_H) $(USER_H)

if CONFIG_USER
libzfsdir = $(includedir)/libzfs/sys
libzfs_HEADERS = $(COMMON_H) $(USER_H)
endif

if CONFIG_KERNEL
kerneldir = /usr/src/zfs-$(VERSION)/include/sys
kernel_HEADERS = $(COMMON_H) $(KERNEL_H)
endif
