###Kernel-3.10 Source for HM2014011(MT6582) 

		sudo apt-get install ccache
		sudo gedit ~/.bashrc
Add:

		export USE_CCACHE=1
		export CCACHE_DIR=~/android/.ccache

Build:

		sudo chmod -R 777 * ~/android_kernel_Xiaomi_HM2014011/arm-eabi-4.8
		cd ~/android_kernel_Xiaomi_HM2014011/kernel-3.10
		export ARCH=arm && export ARCH_MTK_PLATFORM=mt6582 && export CROSS_COMPILE=~/android_kernel_Xiaomi_HM2014011/arm-eabi-4.8/bin/arm-eabi-
		make clean
		make 2014011_debug_defconfig
		./build.sh

* Working
  * LCM: r69431_hd720_dsi_vdo
  * Other stuff

* Not Working
  * LCM: r61308_dsi_vdo and nt35521_hd720_dsi_vdo
  * Other unknown stuff


