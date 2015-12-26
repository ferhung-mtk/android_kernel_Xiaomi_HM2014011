
include $(srctree)/drivers/misc/mediatek/Makefile.custom

# Module project related part

ifeq ($(CONFIG_MTK_SENSOR_SUPPORT),y)
ifeq ($(CONFIG_MTK_LTR553),y)
obj-y	+=  alsps/ltr553/
endif

ifeq ($(CONFIG_MTK_LTR558),y)
obj-y	+=  alsps/ltr558/
endif

ifeq ($(CONFIG_MTK_STK3X1X),y)
obj-y	+=  alsps/stk3x1x/
endif

ifeq ($(CONFIG_MTK_BMI058_AUTO),y)
obj-y	+=  accelerometer/bmi058_auto/
endif

ifeq ($(CONFIG_MTK_LSM330_AUTO),y)
obj-y	+=  accelerometer/lsm330_auto/
endif

ifeq ($(CONFIG_MTK_AKM8963),y)
obj-y	+=  magnetometer/akm8963/
endif

ifeq ($(CONFIG_MTK_HSCDTD006_AUTO),y)
obj-y	+=  magnetometer/hscdtd006_auto/
endif

ifeq ($(CONFIG_MTK_L3GD20),y)
obj-y   +=  gyroscope/l3gd20/
endif

ifeq ($(CCONFIG_MTK_BMI058_AUTO),y)
obj-y   +=  gyroscope/bmi058/
endif

ifeq ($(CONFIG_MTK_BMG160),y)
obj-y   +=  gyroscope/bmg160/
endif
endif

ifneq ($(CONFIG_ARCH_MTK_PROJECT),)
ARCH_MTK_PROJECT := $(shell echo $(CONFIG_ARCH_MTK_PROJECT))
obj-y	+= core/
obj-y	+= dct/dct/
endif

#obj-y	+=  hdmi/
obj-y	+=  flashlight/
obj-y	+=  camera/camera/
obj-y	+=  vibrator/
obj-y	+=  leds/
obj-y	+=  keypad/
obj-y	+=  sound/
obj-y	+=  accdet/
obj-y	+=  partition/
