NetBSD was the first of the modern variants that is still actively developed.
It started out life as a fork of 386BSD. The focus of NetBSD is portability
which not only makes porting to new hardware easier (currently supporting over
60 different ports across may CPU architectures).  Everything from a VAX, ARM &
MIPS Windows CE based PDAs to a Sega Dreamcast and many other systems are
supported and able to run the latest version of NetBSD. There is even a
toaster which run NetBSD
The focus on portability also makes reusing components on other operating
systems easy. For example the packaging system (forked from FreeBSD (which
we will talk about next)) supports over 20 operating systems.  This enables a
consistent toolset to be used regardless of operating system.

Some of the highlights of NetBSD include ATF, unprivileged builds and portable
build infrastructure using build.sh.

ATF, as the name suggests is used for automated tests of the source code to
discover regression in the code base in an automated manner. Results can be
found on the NetBSD release engineering page.

Unprivileged builds allow a user to not only build a copy of the operating
systems without elevated privileged, but they can also build and install
software from pkgsrc in a location they have write access to (by default, in a
prefix under their home directory).

build.sh, the build framework, allows NetBSD to be built on any modern POSIX compliant operating system. Freeing the person to use a operating system of their choice to build releases.