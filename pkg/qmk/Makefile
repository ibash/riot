PKG_NAME=qmk
# PKG_URL=https://github.com/qmk/qmk_firmware
# PKG_VERSION=bdf86c4cbdb22fe800ea0beb4c680b8be5dcb5a4
# PKG_URL=https://github.com/ibash/qmk_firmware
PKG_URL=file:///Users/islam/Projects/qmk_firmware
PKG_VERSION=riot
PKG_LICENSE  = GPL-2

include $(RIOTBASE)/pkg/pkg.mk

all:
	git -C $(PKG_SOURCE_DIR) submodule update --init --recursive
	git -C $(PKG_SOURCE_DIR) submodule update --recursive
	$(QQ)"$(MAKE)" -C $(PKG_SOURCE_DIR) -f $(CURDIR)/Makefile.$(PKG_NAME)
