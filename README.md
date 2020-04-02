Description
===========
movie thumbnailer (mtn)  
fork from http://moviethumbnail.sourceforge.net/  

Movie Thumbnailer (mtn) saves thumbnails (screenshots) of movie or video files to image files (jpg, png).
It uses FFmpeg's libavcodec as its engine, so it supports all popular codecs, e.g. h.265/hevc, h.264, mpeg1, mpeg2, mp4, vc1, wmv, xvid, divx...     
mtn was originaly developed by tuit (tuitfun); though most of its magic is actually done
by FFmpeg libraries. For documents, please see in the doc directory and at
https://gitlab.com/movie_thumbnailer/mtn/wikis/home .


Dependency
==========
 - ffmpeg   (>=3.1)
 - gd       (>=2.0.33)

Getting source
==============
```
$ git clone https://gitlab.com/movie_thumbnailer/mtn.git
```

Installation
============

From source
-----------
```sh
$ cd src
$ make
$ make install

```

From community repository
-----------

See [wiki](https://gitlab.com/movie_thumbnailer/mtn/wikis/home#install-from-community-repository) page

Getting build dependencies
==========================

**[Fedora](https://getfedora.org/)** 26
```sh
$ dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
$ dnf install ffmpeg-devel gd-devel make gcc-c++  
```

**[Debian](https://www.debian.org/)** 9, **[Ubuntu](https://www.ubuntu.com/)** 17.10, **[LinuxMint](https://linuxmint.com)** 19, **[MX Linux](https://mxlinux.org/)** 18, ...  
```sh
$ sudo apt-get install libgd-dev libavutil-dev libavcodec-dev libavformat-dev libswscale-dev make  
```

**[Archlinux](https://www.archlinux.org/), [Manjaro](https://manjaro.org/)**  
```sh
$ sudo pacman -S ffmpeg gd
```

**[OpenSUSE](http://opensuse.org/)** 15  
(FFmpeg in repository is unfortunately compiled with only a few video codecs)
```sh
$ zypper install ffmpeg-4-libavcodec-devel ffmpeg-4-libavdevice-devel ffmpeg-4-libavformat-devel ffmpeg-4-libswscale-devel gd-devel freetype2-devel libjpeg62-devel make gcc 
```

**[CentOS](https://centos.org/)** 7  
```sh
$ yum localinstall https://download1.rpmfusion.org/free/el/rpmfusion-free-release-7.noarch.rpm    
$ yum install ffmpeg-devel gd-devel make gcc-c++    
```

**[FreeBSD](https://www.freebsd.org/)** 10  
```sh
$ pkg install gmake ffmpeg libgd
$ gmake
```

Windows
=======
Read the info in Make.MinGW.bat and run:

```
C:\..\mtn\src> Make.MinGW.bat
```

macOS [(brew)](https://brew.sh/)
=====


If you don't want to contribute please refer to the installation guide
[here](https://gitlab.com/movie_thumbnailer/mtn/wikis/home#macos-homebrew)
instead.

```sh
$ brew install ffmpeg libgd
$ make
$ sudo make install
```

Links
=====
 * [FFmpeg project](http://www.ffmpeg.org)
 * [libgd project](https://libgd.github.io)
 * [libgd library and dependecies](http://gnuwin32.sourceforge.net/packages/gd.htm)
 * [MinGW](http://www.mingw.org/)
 * [RPM Fusion repository](https://rpmfusion.org/)
 * [RPM Macros](https://docs.fedoraproject.org/en-US/packaging-guidelines/RPMMacros/)
 * [GitLab yaml](https://docs.gitlab.com/ee/ci/yaml/README.html)
