#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-blinker
PKG_VERSION:=1.9.0
PKG_RELEASE:=1

PYPI_NAME:=blinker
PKG_HASH:=b4ce2265a7abece45e7cc896e98dbebe6cead56bcf805a3d23136d145f5445bf

PKG_LICENSE:=MIT
PKG_MAINTAINER:=Pallets Ecosystem <contact@palletsprojects.com>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-blinker
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-blinker
  URL:=https://pypi.org/project/blinker
  DEPENDS:=+python3
endef

define Package/python3-blinker/description
Fast, simple object-to-object and broadcast signaling.
endef

$(eval $(call Py3Package,python3-blinker))
$(eval $(call BuildPackage,python3-blinker))
$(eval $(call BuildPackage,python3-blinker-src))
