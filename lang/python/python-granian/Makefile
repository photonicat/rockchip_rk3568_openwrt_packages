include $(TOPDIR)/rules.mk

PKG_NAME:=granian
PKG_VERSION:=2.8.0
PKG_RELEASE:=1

PYPI_NAME:=granian
PKG_HASH:=0a78bbda3aea0f9f079057ee1ee8a1ecf790d4f1af88dd67493c6b8ee52506ff

PKG_MAINTAINER:=Giovanni Barillari <g@baro.dev>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DEPENDS:=python-maturin/host

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-granian
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=A Rust HTTP server for Python applications
  URL:=https://github.com/emmett-framework/granian
  DEPENDS:= \
	+python3 \
	$(RUST_ARCH_DEPENDS)
endef

define Package/python3-granian/description
Granian is a Rust HTTP server for Python applications built on top of Hyper and Tokio
endef

$(eval $(call Py3Package,python3-granian))
$(eval $(call BuildPackage,python3-granian))
$(eval $(call BuildPackage,python3-granian-src))
