#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-legacy-cgi
PKG_VERSION:=2.6.4
PKG_RELEASE:=1

PYPI_NAME:=legacy-cgi
PYPI_SOURCE_NAME:=legacy_cgi
PKG_HASH:=abb9dfc7835772f7c9317977c63253fd22a7484b5c9bbcdca60a29dcce97c577

PKG_LICENSE:=PSF-2.0 
PKG_MAINTAINER:=Jack Rosenthal <jack@rosenth.al>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-legacy-cgi
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-legacy-cgi
  URL:=https://pypi.org/project/legacy-cgi
  DEPENDS:=+python3
endef

define Package/python3-legacy-cgi/description
Fork of the standard library cgi and cgitb modules removed in Python 3.13.
endef

$(eval $(call Py3Package,python3-legacy-cgi))
$(eval $(call BuildPackage,python3-legacy-cgi))
$(eval $(call BuildPackage,python3-legacy-cgi-src))
