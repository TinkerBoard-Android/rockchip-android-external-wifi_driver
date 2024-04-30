# SPDX-License-Identifier: GPL-2.0
SKW_SRC_ROOT := $(src)
SKW_EXTRA_INC := $(SKW_SRC_ROOT)/include/linux/platform_data
SKW_EXTRA_FLAGS = -I$(SKW_EXTRA_INC) -include $(SKW_EXTRA_INC)/skw6160_config.h
SKW_EXTRA_SYMBOLS := $(SKW_EXTRA_INC)/drivers/seekwaveplatform/Modules.symvers

SKW_EXTRA_FLAGS += -DCONFIG_SEEKWAVE_PLD_RELEASE

export skw_extra_flags=$(SKW_EXTRA_FLAGS)
export skw_extra_symbols=$(SKW_EXTRA_SYMBOLS)

export CONFIG_WLAN_VENDOR_SEEKWAVE := m
export CONFIG_SKW_VENDOR := y

#export CONFIG_SKW_USB=m
# export CONFIG_SKW_PCIE=m
export CONFIG_SKW_BSP_BOOT=m
export CONFIG_SKW_BSP_UCOM=m
export CONFIG_SKW_SDIOHAL=m
export CONFIG_SEEKWAVE_BSP_DRIVERS=m

obj-m += drivers/
