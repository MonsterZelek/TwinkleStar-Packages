#
# Copyright (C) 2013-2014 twstars.com
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=TSblockly-multiplewheel
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)
PKG_INSTALL_DIR:=$(PKG_BUILD_DIR)/ipkg-install

include $(INCLUDE_DIR)/kernel.mk
include $(INCLUDE_DIR)/package.mk

define Package/TSblockly-multiplewheel
	SECTION:=TSblockly-multiplewheel
	CATEGORY:=TwinkleStar
	TITLE:=TwinkleStar setwifi by web
endef

define Package/TSblockly-multiplewheel/description
	This package is a bridge connected to the communication blockly and TwinkleStar 
endef

define Build/Prepare
        echo
endef

define Build/Compile
        echo
endef

define Package/TSblockly-multiplewheel/install
	$(INSTALL_DIR) $(1)/www/
	$(INSTALL_DIR) $(1)/www/cgi-bin
	$(CP) ./files/www/blockly $(1)/www/ -rf
	$(CP) ./files/www/cgi-bin/* $(1)/www/cgi-bin -rf
endef

$(eval $(call BuildPackage,TSblockly-multiplewheel))
