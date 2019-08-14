# libgui
[![Build Status](https://travis-ci.org/Maschell/libgui.svg?branch=wut)](https://travis-ci.org/Maschell/libgui/tree/wut)  

## Usage
Following steps are required for initialization:
```C
memoryInitialize();			// Initialize memory management

//DO GUI STUFF HERE!

memoryRelease();
```

Link the application with:
```Makefile
-lgui -lfreetype -lgd -lpng -ljpeg -lz -lmad -lvorbisidec -logg -lbz2

```

You also need to add the freetype2  nclude path to your Makefile. Example:

```Makefile
-I$(PORTLIBS_PATH)/ppc/include/freetype2
```

TODO: provide more information

## Dependencies
To be able to use libgui, you need to install the following dependencies:

- [wut](https://github.com/devkitPro/wut/)
- Install the required portlibs via `(dkp-)pacman -Syu ppc-zlib ppc-libmad ppc-libogg ppc-libgd ppc-freetype ppc-libjpeg-turbo ppc-libpng ppc-libvorbisidec ppc-glm ppc-bzip2`

# Credits
- Orignally based on https://github.com/dborth/libwiigui
- Wii U port / modification / new functions / sound / much more by dimok.
- Minor changes by Maschell
