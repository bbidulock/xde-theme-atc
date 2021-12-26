---
layout: default
---
[xde-theme-atc -- read me first file.  2021-12-08]: #

xde-theme-atc
===============

Package `xde-theme-atc-1.2.4` was released under CCPL:cc-by-nc-nd-3.0
license 2021-12-08.

This is a theme and a set of backgrounds for the _XDE (X Desktop
Environment)_ that provides a set of backgrounds on
a Air Traffic Control theme.
This theme uses the Squared-grey style from the [`xde-styles`][11]
package.

The source for `xde-theme-atc` is hosted on [GitHub][1].


Release
-------

This is the `xde-theme-atc-1.2.4` package, released 2021-12-08.
This release, and the latest version, can be obtained from [GitHub][1],
using a command such as:

    $> git clone https://github.com/bbidulock/xde-theme-atc.git

Please see the [RELEASE][3] and [NEWS][4] files for release notes and
history of user visible changes for the current version, and the
[ChangeLog][5] file for a more detailed history of implementation
changes.  The [TODO][6] file lists features not yet implemented and
other outstanding items.

Please see the [INSTALL][8] file for installation instructions.

When working from `git(1)`, please use this file.  An abbreviated
installation procedure that works for most applications appears below.

This release is published under CCPL:cc-by-nc-nd-3.0 (primarily because
the base styles used to develop these styles were licensed under this
license).
Please see the license in the file [COPYING][10].

Please note that xde-theme-atc is no longer released as
a tarball and is only released as git commits; use:

    $> ./autogen.sh
    $> ./configure --version

to determine the version associated with a given commit in the
checked out working directory.  Note that this is the same version
as executing:

    $> git describe|sed 's,[-_],.,g;s,\.g*,,'

in the checked out working directory.

Note that only HEAD commits are stable: do not attempt to use any
other commit as only HEAD is synchronized with other packages in
the suite.


Quick Start
-----------

The quickest and easiest way to get `xde-theme-atc` up and
running is to run the following commands:

    $> git clone https://github.com/bbidulock/xde-theme-atc.git
    $> cd xde-theme-atc
    $> ./autogen.sh
    $> ./configure
    $> make
    $> make DESTDIR="$pkgdir" install

This will configure, compile and install `xde-theme-atc` the
quickest.  For those who like to spend the extra 15 seconds reading
`./configure --help`, some compile time options can be turned on and off
before the build.

For general information on GNU's `./configure`, see the file
[INSTALL][8].


Prerequisites
-------------

This package needs the [`xde-styles`][11] package to be useful and also
requires the `xde-setbg(1)` program from the [`xde-ctools`][12] package.


Issues
------

Report issues on GitHub [here][2].


Samples
-------

Following is a sample screenshot of the theme taken under the [ADWM][13]
window manager:

![adwm.jpg](scrot/adwm.jpg "Wallpaper #2")

Following are the eight wallpapers included in the theme:

![atc.jpg](images/atc.jpg "Wallpaper #1")
![atc2.jpg](images/atc2.jpg "Wallpaper #2")
![changi.jpg](images/changi.jpg "Wallpaper #3")
![gatwick.jpg](images/gatwick.jpg "Wallpaper #4")
![jersey.jpg](images/jersey.jpg "Wallpaper #5")
![takeoff.jpg](images/takeoff.jpg "Wallpaper #6")
![routes.jpg](images/routes.jpg "Wallpaper #7")
![sillouette.jpg](images/sillouette.jpg "Wallpaper #8")

Following are an additional twelve wallpapers that may be used to
customize the theme:

![control.jpg](images/control.jpg "Additional Image #1")
![cyeg.jpg](images/cyeg.jpg "Additional Image #2")
![darktower.jpg](images/darktower.jpg "Additional Image #3")
![dulles.jpg](images/dulles.jpg "Additional Image #4")
![floor.jpg](images/floor.jpg "Additional Image #5")
![jersey_atc.jpg](images/jersey_atc.jpg "Additional Image #6")
![lax.jpg](images/lax.jpg "Additional Image #7")
![main.jpg](images/main.jpg "Additional Image #8")
![reagan.jpg](images/reagan.jpg "Additional Image #9")
![sunrise_control_tower.jpg](images/sunrise_control_tower.jpg "Additional Image #10")
![united.jpg](images/united.jpg "Additional Image #11")
![virtual.jpg](images/virtual.jpg "Additional Image #12")



[1]: https://github.com/bbidulock/xde-theme-atc
[2]: https://github.com/bbidulock/xde-theme-atc/issues
[3]: https://github.com/bbidulock/xde-theme-atc/blob/master/RELEASE
[4]: https://github.com/bbidulock/xde-theme-atc/blob/master/NEWS
[5]: https://github.com/bbidulock/xde-theme-atc/blob/master/ChangeLog
[6]: https://github.com/bbidulock/xde-theme-atc/blob/master/TODO
[7]: https://github.com/bbidulock/xde-theme-atc/blob/master/COMPLIANCE
[8]: https://github.com/bbidulock/xde-theme-atc/blob/master/INSTALL
[9]: https://github.com/bbidulock/xde-theme-atc/blob/master/LICENSE
[10]: https://github.com/bbidulock/xde-theme-atc/blob/master/COPYING
[11]: https://github.com/bbidulock/xde-styles
[12]: https://github.com/bbidulock/xde-ctools
[13]: https://bbidulock.github.io/adwm

[ vim: set ft=markdown sw=4 tw=72 nocin nosi fo+=tcqlorn spell: ]: #
