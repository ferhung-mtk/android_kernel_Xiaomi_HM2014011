include $(srctree)/drivers/misc/mediatek/Makefile.custom

# In case the platform does NOT support this type of sensors

obj-y   +=  accel.o accel_factory.o

ifeq ($(CONFIG_MTK_K2DH),y)
obj-y   +=  k2dh/
endif

ifeq ($(CONFIG_MTK_BMA050),y)
obj-y   +=  bma050/
endif
ifeq ($(CONFIG_MTK_BMA050_NEW),y)
obj-y   +=  bma050-new/
endif
ifeq ($(CONFIG_MTK_BMA222E),y)
obj-y   +=  bma222E/
endif
ifeq ($(CONFIG_MTK_BMA222E_NEW),y)
obj-y   +=  bma222E-new/
endif
ifeq ($(CONFIG_MTK_MPU6050G),y)
obj-y   +=  mpu6050g/
endif
ifeq ($(CONFIG_MTK_MPU6050G_NEW),y)
obj-y   +=  mpu6050g-new/
endif
ifeq ($(CONFIG_MTK_BMA250),y)
obj-y   +=  bma250/
endif
ifeq ($(CONFIG_MTK_KXTIK1004),y)
obj-y   +=  kxtik1004/
endif

ifeq ($(CONFIG_MTK_MPU6515A),y)
obj-y   +=  mpu6515/
endif

ifeq ($(CONFIG_MTK_BMA222E_AUTO),y)
obj-y   +=  bma222E_auto/
endif

ifeq ($(CONFIG_MTK_KXTJ2_1009_AUTO),y)
obj-y   +=  KXTJ2_1009_auto/
endif

ifeq ($(CONFIG_MTK_KXTJ2_1009_NEW),y)
obj-y   +=  KXTJ2_1009-new/
endif

ifeq ($(CONFIG_MTK_BMA250E),y)
obj-y   +=  bma250e/
endif

# For HM2014011
ifeq ($(CONFIG_MTK_BMI058_AUTO),y)
obj-y   +=  bmi058_auto/
endif

ifeq ($(CONFIG_MTK_LSM330_AUTO),y)
obj-y   +=  lsm330_auto/
endif
