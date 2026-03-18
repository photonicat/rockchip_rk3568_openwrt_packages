#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=scikit-build-core
PKG_VERSION:=0.12.2
PKG_RELEASE:=1

PYPI_NAME:=scikit-build-core
PKG_HASH:=562e0bbc9de1a354c87825ccf732080268d6582a0200f648e8c4a2dcb1e3736d

PKG_LICENSE:=Apache-2.0
PKG_MAINTAINER:=Henry Schreiner <henryfs@princeton.edu>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-scikit-build-core
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-scikit-build-core
  URL:=https://pypi.org/project/scikit-build-core
  DEPENDS:=+python3
endef

define Package/python3-scikit-build-core/description
Build backend for CMake based projects.
endef

$(eval $(call Py3Package,python3-scikit-build-core))
$(eval $(call BuildPackage,python3-scikit-build-core))
$(eval $(call BuildPackage,python3-scikit-build-core-src))
