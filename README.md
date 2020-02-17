# LotusOS #

<img src="https://raw.githubusercontent.com/LotusOS/android_manifest/pie/IMG_20191122_201827_999.jpg"> 

Getting Started:
==============

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Packages Install Ubuntu :
```bash
   sudo dpkg --add-architecture i386 && sudo apt-get update && sudo apt-get upgrade -y && sudo apt-get install -y git-core gnupg flex bison gperf build-essential zip curl zlib1g-dev gcc-multilib g++-multilib libc6-dev-i386 lib32ncurses5-dev x11proto-core-dev libx11-dev lib32z-dev libgl1-mesa-dev libxml2-utils xsltproc unzip bc repo nano && sudo apt-get install -y git gnupg flex bison gperf build-essential zip curl zlib1g-dev gcc-multilib g++-multilib libc6-dev-i386 x11proto-core-dev libx11-dev libgl1-mesa-dev libxml2-utils xsltproc unzip bc repo nano libssl-dev && sudo apt-get install -y openjdk-8-jdk android-tools-adb bc bison build-essential curl flex g++-multilib gcc-multilib gnupg gperf imagemagick lib32readline-dev lib32z1-dev liblz4-tool libncurses5-dev libsdl1.2-dev libssl-dev libwxgtk3.0-dev libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc yasm zip zlib1g-dev && sudo apt-get install -y build-essential kernel-package libncurses5-dev bzip2 android-liblog android-libbacktrace libtinyxml2-6 android-libutils android-sdk-build-tools git-lfs libncurses5:i386 libncurses5 ccache build-essential p7zip-full git libgtk2.0-dev chrpath libncurses5-dev libdbus-1-dev ruby libgl1-mesa-dev "^libxcb.*" libx11-xcb-dev libxrender-dev libxi-dev flex bison gperf patchelf build-essential kernel-package libncurses5-dev bzip2 android-liblog android-libbacktrace libtinyxml2-6 android-libutils android-sdk-build-tools git-lfs libncurses5:i386 libncurses5 ccache
```

To initialize your local repository, use a command like this:

```bash
    repo init -u https://github.com/LotusOS/android_manifest.git -b pie
```

Then to sync up:
================

```bash
    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

Additionally, you can define the number of parallel download repo should do:

```bash
    repo sync -f -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

Compilation of Lotus OS:
====================

From root directory of Project, perform following commands in terminal


```bash
source build/envsetup.sh
lunch lotus_<devicecodename>-userdebug
make bacon -j$(nproc --all)
```
-----------------------------------------------------------------------------

 Credits:
=======
 * [**CyanogenMod**](https://github.com/Cyanogenmod)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**AOSP**](https://android.googlesource.com)
 * [**CherishOS**](https://github.com/CherishOS)
 * [**Evolution-X**](https://github.com/Evolution-X)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**DirtyUnicorns**](https://github.com/dirtyunicorns)
 * [**AospExtended**](https://github.com/AospExtended)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**Havoc-OS**](https://github.com/Havoc-OS)
 * [**AOSCP**](https://github.com/AOSCP)
 * [**NitogenOS**](https://github.com/NitogenOS)
 * [**MSM-Xtended**](https://github.com/MSM-Xtended)
 * [**DescendantOS**](https://github.com/Descendant)
 * [**BootleggersROM**](https://github.com/BootleggersROM)
 * [**AICP**](https://github.com/AICP)
 
-----------------------------------------------------------------------------
