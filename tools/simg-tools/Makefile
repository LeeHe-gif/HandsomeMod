#
# Copyright (C) 2020-2021 HandsomeMod project
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

PKG_NAME:=simg-tools
PKG_SOURCE_URL=https://github.com/HandsomeMod/simg-tools.git
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2022.11.09
PKG_SOURCE_VERSION:=8.1.0-1
PKG_MIRROR_HASH:=72ee2688c1e5941a775a324e22f57cf5be8b2e4abe5a19fb9915365cb97902f1
PKG_SOURCE:=$(PKG_NAME)-$(PKG_SOURCE_VERSION).tar.gz

include $(INCLUDE_DIR)/host-build.mk
include $(INCLUDE_DIR)/cmake.mk

define Host/Install
	$(call Host/Install/Default)
	$(INSTALL_DIR) $(STAGING_DIR_HOST)/bin
	$(INSTALL_BIN) $(HOST_BUILD_DIR)/bin/img2simg $(STAGING_DIR_HOST)/bin
	$(INSTALL_BIN) $(HOST_BUILD_DIR)/bin/simg2img $(STAGING_DIR_HOST)/bin
endef

$(eval $(call HostBuild))
