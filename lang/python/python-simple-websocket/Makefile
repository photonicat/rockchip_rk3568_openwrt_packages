#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-simple-websocket
PKG_VERSION:=1.1.0
PKG_RELEASE:=1

PYPI_NAME:=simple-websocket
PYPI_SOURCE_NAME:=simple_websocket
PKG_HASH:=7939234e7aa067c534abdab3a9ed933ec9ce4691b0713c78acb195560aa52ae4

PKG_LICENSE:=MIT
PKG_MAINTAINER:=Miguel Grinberg <miguel.grinberg@gmail.com>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-simple-websocket
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-simple-websocket
  URL:=https://pypi.org/project/simple-websocket
  DEPENDS:=+python3
endef

define Package/python3-simple-websocket/description
Simple WebSocket server and client for Python.
endef

$(eval $(call Py3Package,python3-simple-websocket))
$(eval $(call BuildPackage,python3-simple-websocket))
$(eval $(call BuildPackage,python3-simple-websocket-src))
