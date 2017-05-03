# ogre3d_test

## Linux Install

### Prerequisite

Run this command :
```sudo zypper ar http://download.opensuse.org/repositories/games/openSUSE_Tumbleweed/ games```
Then run :
```zypper in gcc-c++ libXaw-devel freetype2-devel freeimage-devel libXrandr-devel zziplib-devel cmake```

### Ogre Install

1. [Ogre 1.10 download](https://bitbucket.org/sinbad/ogre/get/v1-10-4.zip)
2. Decompress :
```unzip sinbad-ogre-1fc934daba1e.zip```
3. Move to sources directory :
```cd ogre_src_v1-8-0```
4. Create build directory :
```mkdir build```
5. Move into build directory :
```cd build```
6. Trigger cmake, passing path to Ogre sources directory :
```cmake ..```
7. If the CMake results look good, build Ogre (The -j2 specifies how many parallel compilation jobs to run. Substitute the number of processor cores on your system, e.g. -j2 for a dual-core, -j4 for a quad core... ) :
```make -j4```

## Window Install 

### Get CMake

Download the release depend to your platform from this [link](https://cmake.org/download/).

### Get MinGW

Get it from [here](http://www.mingw.org/).

### get DirectX 9 SDK

Get it from [here](https://www.microsoft.com/en-us/download/details.aspx?id=6812).

### Get sources of Ogre dependencies

Get it from [here](https://bitbucket.org/cabalistic/ogredeps).

### Get Ogre3D SDK

Get it from [here](http://www.ogre3d.org/download/sdk). Run the installer then unpack it to a suitable location. Go to the directory of the newly installed sdk and copy the full path to set the environment variable. Enter the following in any Command Prompt window (Windows Vista/7/8/newer): `setx OGRE_HOME "<path-to-OgreSDK-here>"`
