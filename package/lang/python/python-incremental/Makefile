#
# Copyright (C) 2018 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-incremental
PKG_VERSION:=17.5.0
PKG_RELEASE:=2

PYPI_NAME:=incremental
PKG_HASH:=7b751696aaf36eebfab537e458929e194460051ccad279c72b755a167eebd4b3

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Jeffery To <jeffery.to@gmail.com>

include ../pypi.mk
include $(BUILD_DIR)/package.mk
include ../python3-package.mk

define Package/python3-incremental
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Versions your Python projects
  URL:=https://github.com/twisted/incremental
  DEPENDS:=+python3-light
endef

define Package/python3-incremental/description
Incremental is a small library that versions your Python projects.
endef

$(eval $(call Py3Package,python3-incremental))
$(eval $(call BuildPackage,python3-incremental))
$(eval $(call BuildPackage,python3-incremental-src))
