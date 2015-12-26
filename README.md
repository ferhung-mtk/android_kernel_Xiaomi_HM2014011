###Kernel-3.10 Source for HM2014011(MT6582) 

		sudo apt-get install ccache
		sudo gedit ~/.bashrc
Add:

		export USE_CCACHE=1
		export CCACHE_DIR=~/android/.ccache

Build:

		sudo chmod -R 777 * ~/MT6582-LP-KERNEL/arm-eabi-4.8
		cd ~/MT6582-LP-KERNEL/kernel-3.10
		export ARCH=arm && export ARCH_MTK_PLATFORM=mt6582 && export CROSS_COMPILE=~/MT6582-LP-KERNEL/arm-eabi-4.8/bin/arm-eabi-
		make clean
		make 2014011_debug_defconfig
		./build.sh

* Not Working
  * LCM
  * Other unknown stuff


