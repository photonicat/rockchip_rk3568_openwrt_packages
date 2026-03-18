#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-wsproto
PKG_VERSION:=1.3.2
PKG_RELEASE:=1

PYPI_NAME:=wsproto
PKG_HASH:=b86885dcf294e15204919950f666e06ffc6c7c114ca900b060d6e16293528294

PKG_LICENSE:=MIT
PKG_MAINTAINER:=Thomas Kriechbaumer <thomas@kriechbaumer.name>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-wsproto
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-wsproto
  URL:=https://pypi.org/project/wsproto
  DEPENDS:=+python3 +python3-h11
endef

define Package/python3-wsproto/description
Pure-Python WebSocket protocol implementation.
endef

$(eval $(call Py3Package,python3-wsproto))
$(eval $(call BuildPackage,python3-wsproto))
$(eval $(call BuildPackage,python3-wsproto-src))
