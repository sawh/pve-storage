SOURCES=Plugin.pm DirPlugin.pm LVMPlugin.pm NFSPlugin.pm ISCSIPlugin.pm RBDPlugin.pm SheepdogPlugin.pm ISCSIDirectPlugin.pm GlusterfsPlugin.pm ZFSPoolPlugin.pm ZFSPlugin.pm DRBDPlugin.pm LvmThinPlugin.pm

.PHONY: install
install:
	for i in ${SOURCES}; do install -D -m 0644 $$i ${DESTDIR}${PERLDIR}/PVE/Storage/$$i; done
	make -C LunCmd install
