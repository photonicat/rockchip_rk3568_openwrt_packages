#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pam
PKG_VERSION:=2.0.2
PKG_RELEASE:=1

PYPI_NAME:=python-pam
PYPI_SOURCE_NAME:=python-pam
PKG_HASH:=97235235ba9b82dbae8068d1099508455949b275f77273ca22fdbd8b1fb5d950

PKG_LICENSE:=MIT
PKG_MAINTAINER:=Miguel Grinberg <miguel.grinberg@gmail.com>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-pam
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-pam
  URL:=https://pypi.org/project/pam
  DEPENDS:=+python3 +python3-six
endef

define Package/python3-pam/description
Python PAM module using ctypes, py3.
endef

$(eval $(call Py3Package,python3-pam))
$(eval $(call BuildPackage,python3-pam))
$(eval $(call BuildPackage,python3-pam-src))
