include $(TOPDIR)/rules.mk

PKG_NAME:=asgiref
PKG_VERSION:=3.2.10
PKG_RELEASE:=1

PYPI_NAME:=asgiref
PKG_HASH:=7e51911ee147dd685c3c8b805c0ad0cb58d360987b56953878f8c06d2d1c6f1a

PKG_MAINTAINER:=Peter Stadler <peter.stadler@student.uibk.ac.at>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(BUILD_DIR)/package.mk
include ../python3-package.mk

define Package/python3-asgiref
  SUBMENU:=Python
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Standard for Python asynchronous web apps and servers.
  URL:=https://asgi.readthedocs.io/en/latest/
  DEPENDS:=+python3-light +python3-logging +python3-asyncio
endef

define Package/python3-asgiref/description
  ASGI is a standard for Python asynchronous web apps and servers to communicate
  with each other, and positioned as an asynchronous successor to WSGI.
endef

$(eval $(call Py3Package,python3-asgiref))
$(eval $(call BuildPackage,python3-asgiref))
$(eval $(call BuildPackage,python3-asgiref-src))
