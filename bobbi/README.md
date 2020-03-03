** Random GNO Utilities by Bobbi **

The stuff in this directory was developed by Bobbi from scratch, rather than being ported from another operating system.

* Sortdir *

This all purpose disk utility can perform a number of useful functions on ProDOS volumes:

- Operates at whole volume, sub-tree or individual directory level
- Directory and free-list integrity checking and repair
- Multi level directory sort by name, size, ctime, mtime, type, folders to top etc.
- Filename case conversion to upper, lower, initial capital or camel case
- ctime / mtime datestamp conversion from ProDOS 1.0-2.4.2 to ProDOS 2.5+ format and vice versa

See the manpage *sortdir.1* for more info.

* Extend *

Simple GNO utility which can modify the volume directory of a ProDOS volume to make it extensible under ProDOS 2.5 and later operating systems.  A little bit of explanation is in order here.  ProDOS 2.5 (under development at the time of writing this in March 2020) removes an age-old restriction of Apple's ProDOS.  From v1.0 to v2.4.2 ProDOS has only supported a fixed size volume (or root) directory of four blocks (which works out to be 51 entries.)  ProDOS 2.5 removes this restriction and allows the volume directory to be extensible just like a subdirectory.  In order to enable this extension, a couple of magic bytes must be written to the volume directory.  This utility can do precisely this.  It can also reverse the change, provided the volume directory has not actually been extended beyond 4 blocks by writing more than 51 entries to it.

* nl *

A very simple implementation of the classic UNIX *nl* utility, which I was missing in GNO.  It is not part of v7 so I whipped up my own.  This program is actually too simple minded and doesn't work properly in some corner cases.  I will return to it when the urge strikes me (or the bugs bite me.)
