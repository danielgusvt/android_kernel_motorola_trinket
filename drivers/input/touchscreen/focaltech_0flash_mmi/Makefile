# Makefile for the focaltech touchscreen drivers.

obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_core.o
obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_ex_fun.o
obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_ex_mode.o
obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_gesture.o
obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_esdcheck.o
obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_point_report_check.o
#obj-$(CONFIG_TOUCHSCREEN_FTS)	+=  focaltech_test/

obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI)	+=  focaltech_flash.o

obj-$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8756) += focaltech_flash_ft8756.o
obj-$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8756) += focaltech_spi_v1_1_1.o

ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_ENABLE_DOUBLE_TAP)),)
	ccflags-y += -DFOCALTECH_SENSOR_EN
endif
