#
# Copyright (C) 2020-2022 HandsomeMod Project
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=qcom-firmware
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/LeeHe-gif/qcom-firmware.git
PKG_SOURCE_VERSION:=14cc4b0f5ccde6276b603968e9e5acbf682a5717

PKG_MAINTAINER:=Handsomeyingyan <handsomeyingyan@gmail.com>
STRIP:=:

include $(INCLUDE_DIR)/package.mk

define Package/qcom-firmware-default
  SECTION:=firmware
  CATEGORY:=Firmware
endef

define Build/Compile
	mkdir $(PKG_BUILD_DIR)/dragonboard
	mcopy -i $(PKG_BUILD_DIR)/dragonboard-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/dragonboard
	mkdir $(PKG_BUILD_DIR)/openstick-ufi001b
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001b-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001b
	mkdir $(PKG_BUILD_DIR)/openstick-ufi001c
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001c-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001c
	mkdir $(PKG_BUILD_DIR)/openstick-ufi003
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi003-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi003
	mkdir $(PKG_BUILD_DIR)/openstick-ufi103s
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi103s-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi103s
	mkdir $(PKG_BUILD_DIR)/openstick-sp970
	mcopy -i $(PKG_BUILD_DIR)/openstick-sp970-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-sp970
	mkdir $(PKG_BUILD_DIR)/openstick-uz801
	mcopy -i $(PKG_BUILD_DIR)/openstick-uz801-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-uz801
	mkdir $(PKG_BUILD_DIR)/openstick-uz801v3
	mcopy -i $(PKG_BUILD_DIR)/openstick-uz801v3-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-uz801v3
	mkdir $(PKG_BUILD_DIR)/wt88047
	mcopy -i $(PKG_BUILD_DIR)/wt88047-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt88047
	mkdir $(PKG_BUILD_DIR)/wt86047
	mcopy -i $(PKG_BUILD_DIR)/wt86047-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt86047	
endef

define Package/qcom-apq8016-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI001B WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI001C WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI003 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi103s-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI103S WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-sp970-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick SP970 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-uz801-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UZ801 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-uz801v3-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UZ801V3 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-wt8x047-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Redmi 2 WIFI & Bluetooth firmware
endef

define Package/qcom-apq8016-wcnss-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI nv data
endef

define Package/qcom-msm8916-wcnss-wt88047-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Wingtech Wt88047
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001b-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI001B
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001c-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI001C
endef

define Package/qcom-msm8916-wcnss-openstick-ufi003-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI003
endef

define Package/qcom-msm8916-wcnss-openstick-ufi103s-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI103S
endef

define Package/qcom-msm8916-wcnss-openstick-sp970-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick SP970
endef

define Package/qcom-msm8916-wcnss-openstick-uz801-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UZ801
endef

define Package/qcom-msm8916-wcnss-openstick-uz801v3-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UZ801V3
endef

define Package/qcom-apq8016-modem-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 modem firmware
endef

define Package/qcom-msm8916-modem-wt88047-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt88047
endef

define Package/qcom-msm8916-modem-wt86047-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt86047
endef

define Package/qcom-msm8916-modem-openstick-ufi001b-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI001B
endef

define Package/qcom-msm8916-modem-openstick-ufi001c-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI001C
endef

define Package/qcom-msm8916-modem-openstick-ufi003-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI003
endef

define Package/qcom-msm8916-modem-openstick-ufi103s-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI103S
endef

define Package/qcom-msm8916-modem-openstick-sp970-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick SP970
endef

define Package/qcom-msm8916-modem-openstick-uz801-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UZ801
endef

define Package/qcom-msm8916-modem-openstick-uz801v3-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UZ801V3
endef

define Package/qcom-apq8016-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b00 \
		$(1)/lib/firmware/wcnss-ufi001b.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b01 \
		$(1)/lib/firmware/wcnss-ufi001b.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b02 \
		$(1)/lib/firmware/wcnss-ufi001b.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b04 \
		$(1)/lib/firmware/wcnss-ufi001b.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b06 \
		$(1)/lib/firmware/wcnss-ufi001b.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b09 \
		$(1)/lib/firmware/wcnss-ufi001b.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b10 \
		$(1)/lib/firmware/wcnss-ufi001b.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b11 \
		$(1)/lib/firmware/wcnss-ufi001b.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.mdt \
		$(1)/lib/firmware/wcnss-ufi001b.mdt
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b00 \
		$(1)/lib/firmware/wcnss-ufi001c.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b01 \
		$(1)/lib/firmware/wcnss-ufi001c.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b02 \
		$(1)/lib/firmware/wcnss-ufi001c.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b04 \
		$(1)/lib/firmware/wcnss-ufi001b.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b06 \
		$(1)/lib/firmware/wcnss-ufi001b.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b09 \
		$(1)/lib/firmware/wcnss-ufi001b.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b10 \
		$(1)/lib/firmware/wcnss-ufi001b.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.b11 \
		$(1)/lib/firmware/wcnss-ufi001b.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.mdt \
		$(1)/lib/firmware/wcnss-ufi001b.mdt
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b00 \
		$(1)/lib/firmware/wcnss-ufi003.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b01 \
		$(1)/lib/firmware/wcnss-ufi003.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b02 \
		$(1)/lib/firmware/wcnss-ufi003.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b04 \
		$(1)/lib/firmware/wcnss-ufi003.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b06 \
		$(1)/lib/firmware/wcnss-ufi003.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b09 \
		$(1)/lib/firmware/wcnss-ufi003.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b10 \
		$(1)/lib/firmware/wcnss-ufi003.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.b11 \
		$(1)/lib/firmware/wcnss-ufi003.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.mdt \
		$(1)/lib/firmware/wcnss-ufi003.mdt
endef

define Package/qcom-msm8916-openstick-ufi103s-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b00 \
		$(1)/lib/firmware/wcnss-ufi103s.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b01 \
		$(1)/lib/firmware/wcnss-ufi103s.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b02 \
		$(1)/lib/firmware/wcnss-ufi103s.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b04 \
		$(1)/lib/firmware/wcnss-ufi103s.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b06 \
		$(1)/lib/firmware/wcnss-ufi103s.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b09 \
		$(1)/lib/firmware/wcnss-ufi103s.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b10 \
		$(1)/lib/firmware/wcnss-ufi103s.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.b11 \
		$(1)/lib/firmware/wcnss-ufi103s.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.mdt \
		$(1)/lib/firmware/wcnss-ufi103s.mdt
endef

define Package/qcom-msm8916-openstick-sp970-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b00 \
		$(1)/lib/firmware/wcnss-sp970.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b01 \
		$(1)/lib/firmware/wcnss-sp970.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b02 \
		$(1)/lib/firmware/wcnss-sp970.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b04 \
		$(1)/lib/firmware/wcnss-sp970.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b06 \
		$(1)/lib/firmware/wcnss-sp970.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b09 \
		$(1)/lib/firmware/wcnss-sp970.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b10 \
		$(1)/lib/firmware/wcnss-sp970.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.b11 \
		$(1)/lib/firmware/wcnss-sp970.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.mdt \
		$(1)/lib/firmware/wcnss-sp970.mdt
endef

define Package/qcom-msm8916-openstick-uz801-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b00 \
		$(1)/lib/firmware/wcnss-uz801.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b01 \
		$(1)/lib/firmware/wcnss-uz801.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b02 \
		$(1)/lib/firmware/wcnss-uz801.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b04 \
		$(1)/lib/firmware/wcnss-uz801.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b06 \
		$(1)/lib/firmware/wcnss-uz801.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b09 \
		$(1)/lib/firmware/wcnss-uz801.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b10 \
		$(1)/lib/firmware/wcnss-uz801.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.b11 \
		$(1)/lib/firmware/wcnss-uz801.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.mdt \
		$(1)/lib/firmware/wcnss-uz801.mdt
endef

define Package/qcom-msm8916-openstick-uz801v3-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b00 \
		$(1)/lib/firmware/wcnss-uz801v3.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b01 \
		$(1)/lib/firmware/wcnss-uz801v3.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b02 \
		$(1)/lib/firmware/wcnss-uz801v3.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b04 \
		$(1)/lib/firmware/wcnss-uz801v3.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b06 \
		$(1)/lib/firmware/wcnss-uz801v3.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b09 \
		$(1)/lib/firmware/wcnss-uz801v3.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b10 \
		$(1)/lib/firmware/wcnss-uz801v3.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.b11 \
		$(1)/lib/firmware/wcnss-uz801v3.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3/wcnss.mdt \
		$(1)/lib/firmware/wcnss-uz801v3.mdtre
endef

define Package/qcom-msm8916-wt8x047-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b00 \
		$(1)/lib/firmware/wcnss-wt8x047.b00
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b01 \
		$(1)/lib/firmware/wcnss-wt8x047.b01
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b02 \
		$(1)/lib/firmware/wcnss-wt8x047.b02
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b04 \
		$(1)/lib/firmware/wcnss-wt8x047.b04
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b06 \
		$(1)/lib/firmware/wcnss-wt8x047.b06
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b09 \
		$(1)/lib/firmware/wcnss-wt8x047.b09
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b10 \
		$(1)/lib/firmware/wcnss-wt8x047.b10
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.b11 \
		$(1)/lib/firmware/wcnss-wt8x047.b11
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.mdt \
		$(1)/lib/firmware/wcnss-wt8x047.mdt
endef

define Package/qcom-apq8016-wcnss-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-wt88047-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt8x047-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-wt8x047.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001b-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-ufi001b.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001c-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-ufi001c.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi003-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-ufi003.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi103s-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-ufi103s.bin
endef

define Package/qcom-msm8916-wcnss-openstick-sp970-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-sp970.bin
endef

define Package/qcom-msm8916-wcnss-openstick-uz801-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-uz801.bin
endef

define Package/qcom-msm8916-wcnss-openstick-uz801v3-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801v3-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv-uz801v3.bin
endef

define Package/qcom-apq8016-modem-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-wt88047-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-wt86047-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-ufi001b-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/mba.mbn $(1)/lib/firmware/mba-ufi001b.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b00 $(1)/lib/firmware/modem-ufi001b.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b01 $(1)/lib/firmware/modem-ufi001b.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b02 $(1)/lib/firmware/modem-ufi001b.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b03 $(1)/lib/firmware/modem-ufi001b.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b04 $(1)/lib/firmware/modem-ufi001b.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b05 $(1)/lib/firmware/modem-ufi001b.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b08 $(1)/lib/firmware/modem-ufi001b.b08
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b13 $(1)/lib/firmware/modem-ufi001b.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b14 $(1)/lib/firmware/modem-ufi001b.b14
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b15 $(1)/lib/firmware/modem-ufi001b.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b16 $(1)/lib/firmware/modem-ufi001b.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b17 $(1)/lib/firmware/modem-ufi001b.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b18 $(1)/lib/firmware/modem-ufi001b.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b22 $(1)/lib/firmware/modem-ufi001b.b22
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b23 $(1)/lib/firmware/modem-ufi001b.b23
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.b25 $(1)/lib/firmware/modem-ufi001b.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001b/modem.mdt $(1)/lib/firmware/modem-ufi001b.mdt
endef

define Package/qcom-msm8916-modem-openstick-ufi001c-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/mba.mbn $(1)/lib/firmware/mba-ufi001c.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b00 $(1)/lib/firmware/modem-ufi001c.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b01 $(1)/lib/firmware/modem-ufi001c.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b02 $(1)/lib/firmware/modem-ufi001c.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b03 $(1)/lib/firmware/modem-ufi001c.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b04 $(1)/lib/firmware/modem-ufi001c.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b05 $(1)/lib/firmware/modem-ufi001c.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b08 $(1)/lib/firmware/modem-ufi001c.b08
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b13 $(1)/lib/firmware/modem-ufi001c.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b14 $(1)/lib/firmware/modem-ufi001c.b14
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b15 $(1)/lib/firmware/modem-ufi001c.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b16 $(1)/lib/firmware/modem-ufi001c.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b17 $(1)/lib/firmware/modem-ufi001c.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b18 $(1)/lib/firmware/modem-ufi001c.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b22 $(1)/lib/firmware/modem-ufi001c.b22
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b23 $(1)/lib/firmware/modem-ufi001c.b23
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.b25 $(1)/lib/firmware/modem-ufi001c.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi001c/modem.mdt $(1)/lib/firmware/modem-ufi001c.mdt
endef

define Package/qcom-msm8916-modem-openstick-ufi103s-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/mba.mbn $(1)/lib/firmware/mba-ufi103s.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b00 $(1)/lib/firmware/modem-ufi103s.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b01 $(1)/lib/firmware/modem-ufi103s.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b02 $(1)/lib/firmware/modem-ufi103s.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b03 $(1)/lib/firmware/modem-ufi103s.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b04 $(1)/lib/firmware/modem-ufi103s.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b05 $(1)/lib/firmware/modem-ufi103s.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b08 $(1)/lib/firmware/modem-ufi103s.b08
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b10 $(1)/lib/firmware/modem-ufi103s.b10
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b11 $(1)/lib/firmware/modem-ufi103s.b11
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b13 $(1)/lib/firmware/modem-ufi103s.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b14 $(1)/lib/firmware/modem-ufi103s.b14
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b15 $(1)/lib/firmware/modem-ufi103s.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b16 $(1)/lib/firmware/modem-ufi103s.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b17 $(1)/lib/firmware/modem-ufi103s.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b18 $(1)/lib/firmware/modem-ufi103s.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b19 $(1)/lib/firmware/modem-ufi103s.b19
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b22 $(1)/lib/firmware/modem-ufi103s.b22
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b23 $(1)/lib/firmware/modem-ufi103s.b23
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b24 $(1)/lib/firmware/modem-ufi103s.b24
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.b25 $(1)/lib/firmware/modem-ufi103s.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-ufi103s/modem.mdt $(1)/lib/firmware/modem-ufi103s.mdt
endef

define Package/qcom-msm8916-modem-openstick-ufi003-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-sp970-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/mba.mbn $(1)/lib/firmware/mba-sp970.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b00 $(1)/lib/firmware/modem-sp970.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b01 $(1)/lib/firmware/modem-sp970.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b02 $(1)/lib/firmware/modem-sp970.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b03 $(1)/lib/firmware/modem-sp970.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b04 $(1)/lib/firmware/modem-sp970.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b05 $(1)/lib/firmware/modem-sp970.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b10 $(1)/lib/firmware/modem-sp970.b10
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b13 $(1)/lib/firmware/modem-sp970.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b15 $(1)/lib/firmware/modem-sp970.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b16 $(1)/lib/firmware/modem-sp970.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b17 $(1)/lib/firmware/modem-sp970.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b18 $(1)/lib/firmware/modem-sp970.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b19 $(1)/lib/firmware/modem-sp970.b19
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b24 $(1)/lib/firmware/modem-sp970.b24
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.b25 $(1)/lib/firmware/modem-sp970.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-sp970/modem.mdt $(1)/lib/firmware/modem-sp970.mdt
endef

define Package/qcom-msm8916-modem-openstick-uz801-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/mba.mbn $(1)/lib/firmware/mba-uz801.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b00 $(1)/lib/firmware/modem-uz801.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b01 $(1)/lib/firmware/modem-uz801.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b02 $(1)/lib/firmware/modem-uz801.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b03 $(1)/lib/firmware/modem-uz801.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b04 $(1)/lib/firmware/modem-uz801.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b05 $(1)/lib/firmware/modem-uz801.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b08 $(1)/lib/firmware/modem-uz801.b08
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b10 $(1)/lib/firmware/modem-uz801.b10
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b11 $(1)/lib/firmware/modem-uz801.b11
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b13 $(1)/lib/firmware/modem-uz801.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b14 $(1)/lib/firmware/modem-uz801.b14
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b15 $(1)/lib/firmware/modem-uz801.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b16 $(1)/lib/firmware/modem-uz801.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b17 $(1)/lib/firmware/modem-uz801.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b18 $(1)/lib/firmware/modem-uz801.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b19 $(1)/lib/firmware/modem-uz801.b19
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b22 $(1)/lib/firmware/modem-uz801.b22
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b23 $(1)/lib/firmware/modem-uz801.b23
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b24 $(1)/lib/firmware/modem-uz801.b24
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.b25 $(1)/lib/firmware/modem-uz801.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801/modem.mdt $(1)/lib/firmware/modem-uz801.mdt
endef

define Package/qcom-msm8916-modem-openstick-uz801v3-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/mba.mbn $(1)/lib/firmware/mba-uz801v3.mbn
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b00 $(1)/lib/firmware/modem-uz801v3.b00
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b01 $(1)/lib/firmware/modem-uz801v3.b01
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b02 $(1)/lib/firmware/modem-uz801v3.b02
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b03 $(1)/lib/firmware/modem-uz801v3.b03
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b04 $(1)/lib/firmware/modem-uz801v3.b04
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b05 $(1)/lib/firmware/modem-uz801v3.b05
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b08 $(1)/lib/firmware/modem-uz801v3.b08
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b10 $(1)/lib/firmware/modem-uz801v3.b10
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b11 $(1)/lib/firmware/modem-uz801v3.b11
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b13 $(1)/lib/firmware/modem-uz801v3.b13
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b14 $(1)/lib/firmware/modem-uz801v3.b14
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b15 $(1)/lib/firmware/modem-uz801v3.b15
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b16 $(1)/lib/firmware/modem-uz801v3.b16
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b17 $(1)/lib/firmware/modem-uz801v3.b17
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b18 $(1)/lib/firmware/modem-uz801v3.b18
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b19 $(1)/lib/firmware/modem-uz801v3.b19
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b22 $(1)/lib/firmware/modem-uz801v3.b22
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b23 $(1)/lib/firmware/modem-uz801v3.b23
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b24 $(1)/lib/firmware/modem-uz801v3.b24
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.b25 $(1)/lib/firmware/modem-uz801v3.b25
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/openstick-uz801v3/modem.mdt $(1)/lib/firmware/modem-uz801v3.mdt
endef

# 创建设备检测脚本包
define Package/qcom-firmware-setup
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm firmware device detection and setup
  DEPENDS:=+qcom-msm8916-wcnss-wt88047-nv +qcom-msm8916-wt8x047-wcnss-firmware +qcom-msm8916-modem-wt88047-firmware
endef

define Package/qcom-firmware-setup/install
	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/qcom-firmware-setup $(1)/etc/init.d/qcom-firmware
	$(INSTALL_DIR) $(1)/usr/sbin
	$(INSTALL_BIN) ./files/qcom-firmware-setup $(1)/usr/sbin/qcom-firmware-setup
endef

define Package/qcom-firmware-setup/postinst
#!/bin/sh
# 启用启动脚本
[ -n "$$IPKG_INSTROOT" ] || /etc/init.d/qcom-firmware enable
exit 0
endef

$(eval $(call BuildPackage,qcom-apq8016-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001b-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001c-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi003-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi103s-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-sp970-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801v3-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-wt8x047-wcnss-firmware))
$(eval $(call BuildPackage,qcom-apq8016-wcnss-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-wt88047-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi001b-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi001c-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi003-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi103s-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-sp970-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-uz801-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-uz801v3-nv))
$(eval $(call BuildPackage,qcom-apq8016-modem-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-wt88047-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-wt86047-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi001b-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi001c-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi003-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi103s-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-sp970-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-uz801-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-uz801v3-firmware))
$(eval $(call BuildPackage,qcom-firmware-setup))
