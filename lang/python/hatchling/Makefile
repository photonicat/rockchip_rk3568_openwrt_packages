#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=hatchling
PKG_VERSION:=1.29.0
PKG_RELEASE:=1

PYPI_NAME:=hatchling
PKG_HASH:=793c31816d952cee405b83488ce001c719f325d9cda69f1fc4cd750527640ea6

PKG_LICENSE:=BSD-3-Clause
PKG_MAINTAINER:=Ofek Lev <oss@ofek.dev>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-hatchling
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-hatchling
  URL:=https://pypi.org/project/hatchling
  DEPENDS:=+python3
endef

define Package/python3-hatchling/description
Modern, extensible Python build backend.
endef

$(eval $(call Py3Package,python3-hatchling))
$(eval $(call BuildPackage,python3-hatchling))
$(eval $(call BuildPackage,python3-hatchling-src))
