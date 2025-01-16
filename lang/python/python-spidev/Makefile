#
# Copyright (C) 2019 CZ.NIC, z. s. p. o. (https://www.nic.cz/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=spidev
PKG_VERSION:=3.6
PKG_RELEASE:=1

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=14dbc37594a4aaef85403ab617985d3c3ef464d62bc9b769ef552db53701115b

PKG_MAINTAINER:=Stephen Caudle <scaudle@doceme.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-spidev
  SUBMENU:=Python
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Python bindings for Linux SPI access through spidev
  URL:=https://pypi.org/project/spidev
  DEPENDS:=+python3-light
endef

define Package/python3-spidev/description
  Python bindings for Linux SPI access through spidev.
endef

$(eval $(call Py3Package,python3-spidev))
$(eval $(call BuildPackage,python3-spidev))
$(eval $(call BuildPackage,python3-spidev-src))
