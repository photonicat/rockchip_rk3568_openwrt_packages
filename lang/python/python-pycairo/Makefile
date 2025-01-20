#
# Copyright (C) 2019 CZ.NIC, z. s. p. o. (https://www.nic.cz/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=pycairo
PKG_VERSION:=1.27.0
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=5cb21e7a00a2afcafea7f14390235be33497a2cce53a98a19389492a60628430

PKG_MAINTAINER:=Christoph Reiter <reiter.christoph@gmail.com>
PKG_LICENSE:=LGPL-2.1
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-pycairo
  SUBMENU:=Python
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Python interface for cairo
  URL:=https://pypi.org/project/pycairo
  DEPENDS:=+python3-light +libcairo
endef

define Package/python3-pycairo/description
  The Pycairo bindings are designed to match the cairo C API as closely as possible,
  and to deviate only in cases which are clearly better implemented in a more ‘Pythonic’ way.
endef

$(eval $(call Py3Package,python3-pycairo))
$(eval $(call BuildPackage,python3-pycairo))
$(eval $(call BuildPackage,python3-pycairo-src))
