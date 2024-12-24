**Gaming dependency**
* wine
* dbus
* steam
* goverlay
* gnutls
* lib32-gnutls
* base-devel
* gtk2
* gtk3
* lib32-gtk2
* lib32-gtk3
* libpulse
* lib32-libpulse
* alsa-lib
* lib32-alsa-lib
* alsa-utils
* alsa-plugins
* lib32-alsa-plugins
* giflib
* lib32-giflib
* libpng
* lib32-libpng
* libldap
* lib32-libldap
* openal
* lib32-openal
* libxcomposite
* lib32-libxcomposite
* libxinerama
* lib32-libxinerama
* ncurses
* lib32-ncurses
* vulkan-icd-loader
* lib32-vulkan-icd-loader
* ocl-icd
* lib32-ocl-icd
* libva
* lib32-libva
* gst-plugins-base-libs
* lib32-gst-plugins-base-libs
* sdl2
* lib32-sdl2
* v4l-utils
* lib32-v4l-utils
* sqlite
* lib32-sqlite


For arch linux 
* Dependency
```
sudo pacman -S dbus gnutls lib32-gnutls base-devel gtk2 gtk3 lib32-gtk2 lib32-gtk3 libpulse lib32-libpulse alsa-lib lib32-alsa-lib alsa-utils alsa-plugins lib32-alsa-plugins giflib lib32-giflib libpng lib32-libpng libldap lib32-libldap openal lib32-openal libxcomposite lib32-libxcomposite libxinerama lib32-libxinerama ncurses lib32-ncurses vulkan-icd-loader lib32-vulkan-icd-loader ocl-icd lib32-ocl-icd libva lib32-libva gst-plugins-base-libs lib32-gst-plugins-base-libs sdl2 lib32-sdl2 v4l-utils lib32-v4l-utils sqlite lib32-sqlite
```
* Steam and lutris
```
sudo pacman -S steam lutris
```
  
Specially check if lib32 graphics drivers are installed in you pc. In arch linux steam package includes that lib32 driver you can select it and install with steam.
