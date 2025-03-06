# Based on: datapath_common/third_party/hiredis-1.0.0/Makefile

export DEP_BUILD_DIR ?= build

build:
	mkdir -p $(DEP_BUILD_DIR)
	USE_SSL=1 $(MAKE) -C .. install PREFIX=$(PREFIX_DIR) INSTALL="/usr/bin/install -C"
	rm -f $(PREFIX_DIR)/lib/libhiredis*.so*

.PHONY: all build install clean distclean