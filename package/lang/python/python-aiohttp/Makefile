#
# Copyright (C) 2019-2020 CZ.NIC, z. s. p. o. (https://www.nic.cz/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=aiohttp
PKG_VERSION:=3.6.1
PKG_RELEASE:=2

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=fc55b1fec0e4cc1134ffb09ea3970783ee2906dc5dfd7cd16917913f2cfed65b

PKG_MAINTAINER:=Josef Schlehofer <pepe.schlehofer@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:aio-libs_project:aiohttp

include ../pypi.mk
include $(BUILD_DIR)/package.mk
include ../python3-package.mk

define Package/python3-aiohttp
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Async http client/server framework (asyncio)
  URL:=https://github.com/aio-libs/aiohttp
  DEPENDS:= \
	+python3-light \
	+python3-attrs \
	+python3-chardet \
	+python3-multidict \
	+python3-async-timeout \
	+python3-yarl \
	+python3-logging \
	+python3-codecs \
	+python3-cgi \
	+python3-openssl
endef

define Package/python3-aiohttp/description
  Asynchronous HTTP client/server framework for asyncio and Python3.
endef

$(eval $(call Py3Package,python3-aiohttp))
$(eval $(call BuildPackage,python3-aiohttp))
$(eval $(call BuildPackage,python3-aiohttp-src))
