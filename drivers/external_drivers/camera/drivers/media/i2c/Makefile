#
# Makefile for sensor drivers
#

obj-$(CONFIG_VIDEO_IMX)        += imx/
obj-$(CONFIG_VIDEO_IMX111)     += imx111/
obj-$(CONFIG_VIDEO_IMX219)     += imx219/
obj-$(CONFIG_VIDEO_IMXVB)      += imx135VB/
ifdef CONFIG_GMIN_INTEL_MID
obj-$(CONFIG_VIDEO_OV5693)     += ov5693-ecs/
else
obj-$(CONFIG_VIDEO_OV5693)     += ov5693/
endif
obj-$(CONFIG_VIDEO_T4K35)      += t4k35/
obj-$(CONFIG_VIDEO_T4K35_180)  += t4k35_180/
obj-$(CONFIG_VIDEO_T4K37)      += t4k37/

obj-$(CONFIG_VIDEO_MN34130)    += mn34130.o
mn34130-objs := mn34130/mn34130.o mn34130/dw9714.o

obj-$(CONFIG_VIDEO_MT9M114)    += mt9m114.o
obj-$(CONFIG_VIDEO_MT9E013)    += mt9e013/

obj-$(CONFIG_VIDEO_MT9D113)    += mt9d113.o

obj-$(CONFIG_VIDEO_MT9V113)    += mt9v113.o

obj-$(CONFIG_VIDEO_OV5640)     += ov5640.o

obj-$(CONFIG_VIDEO_GC2235)     += gc2235.o
obj-$(CONFIG_VIDEO_OV9724)     += ov9724.o
obj-$(CONFIG_VIDEO_OV2722)     += ov2722.o
obj-$(CONFIG_VIDEO_OV8830)     += ov8830.o

obj-$(CONFIG_VIDEO_HM2056)     += hm2056.o
obj-$(CONFIG_VIDEO_GC2155)     += gc2155.o

obj-$(CONFIG_VIDEO_S5K8AAY)    += s5k8aay.o
obj-$(CONFIG_VIDEO_S5K6B2YX)    += s5k6b2yx.o

m10mo_isp-objs := m10mo.o m10mo_fw.o m10mo_tables.o m10mo_fw_type2.o m10mo_fw_type1_5.o
obj-$(CONFIG_VIDEO_M10MO)    += m10mo_isp.o
obj-$(CONFIG_VIDEO_M10MO)    += m10mo_spi.o

obj-$(CONFIG_VIDEO_AR0543_RAW)     += ar0543_raw.o
CFFLAGS_ar0543_raw.o = -Werror
obj-$(CONFIG_VIDEO_HM2056_RAW) += hm2056_raw.o
CFFLAGS_hm2056_raw.o = -Werror

obj-$(CONFIG_VIDEO_MSRLIST_HELPER) += libmsrlisthelper.o

obj-$(CONFIG_VIDEO_AP1302)     += ap1302.o

obj-$(CONFIG_VIDEO_RT8515)     += rt8515.o
obj-$(CONFIG_VIDEO_OV680)     += ov680.o

obj-$(CONFIG_VIDEO_CSI_XACTOR) += xactor_x.o
obj-$(CONFIG_VIDEO_PIXTER) += pixter.o

#
# Makefile for flash drivers
#

obj-$(CONFIG_VIDEO_LM3554) += lm3554.o
obj-$(CONFIG_VIDEO_LM3559) += lm3559.o
obj-$(CONFIG_VIDEO_LM3642) += lm3642.o

ccflags-y += -Werror

# Add cflags to build camera sensor driver for CTP board
#ccflags-$(CONFIG_SND_CTP_MACHINE) += -DCSS15

ccflags-$(CONFIG_VIDEO_ATOMISP_CTP) += -DCSS15
