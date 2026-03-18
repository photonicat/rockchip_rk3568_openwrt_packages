#
# Copyright (C) 2015 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=pybind11
PKG_VERSION:=3.0.2
PKG_RELEASE:=1

PYPI_NAME:=pybind11
PKG_HASH:=432f01aeb68e361a3a7fc7575c2c7f497595bf640f747acd909ff238dd766e06

PKG_LICENSE:=BSD-3-Clause
PKG_MAINTAINER:=Wenzel Jakob <wenzel.jakob@epfl.ch>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-pybind11
  SECTION:=lang-python
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=python3-pybind11
  URL:=https://pypi.org/project/pybind11
  DEPENDS:=+python3
endef

define Package/python3-pybind11/description
pybind11 is a lightweight header-only library that exposes C++ types in Python
and vice versa, mainly to create Python bindings of existing C++ code. Its
goals and syntax are similar to the excellent Boost.Python library by
David Abrahams: to minimize boilerplate code in traditional extension modules
by inferring type information using compile-time introspection.
endef

$(eval $(call Py3Package,python3-pybind11))
$(eval $(call BuildPackage,python3-pybind11))
$(eval $(call BuildPackage,python3-pybind11-src))
