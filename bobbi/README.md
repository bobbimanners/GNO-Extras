```
** THIS IS ALPHA-QUALITY CODE **
** USE AT YOUR OWN RISK!      **

usage: sortdir [-s xxx] [-n x] [-rDwcvVh] path

  Options: -s xxx  Directory sort options
           -n x    Filename upper/lower case options
           -r      Recursive descent
           -D      Whole-disk mode (implies -r)
           -w      Enable writing to disk
           -c      Use creation time rather than modification
           -v      Verbose output
           -V      Verbose debugging output
           -h      This help

Upper/lower case option x:
  l  convert filenames to lower case             eg: read.me
  u  convert filenames to upper case             eg: READ.ME
  i  convert filenames to initial upper case     eg: Read.me
  c  convert filenames to camel case             eg: Read.Me

Directory sort options xxx, is a list of fields on which to
sort. The sort options are processed left-to-right.
  n  sort by filename ascending
  N  sort by filename descending
  d  sort by modification (or creation [-c]) date ascending
  D  sort by modification (or creation [-c]) date descending
  t  sort by type ascending
  T  sort by type descending
  f  sort folders (directories) to top
  F  sort folders (directories) to bottom
  b  sort by blocks used ascending
  B  sort by blocks used descending
  e  sort by EOF position ascending
  E  sort by EOF position descending

e.g.: sortdir -w -s nf .
Will sort the current directory first by name (ascending),
then sort directories to the top, and will write the sorted
directory to disk.
