```
** THIS IS ALPHA-QUALITY CODE **
** USE AT YOUR OWN RISK!      **

usage: sortdir [-s xxx] [-rwv] path

  Options: -s xxx  Directory sort options
           -w      Enable writing to disk
           -v      Verbose output
           -h      This help

Directory sort options xxx, is a list of fields on which to
sort. The sort options are processed left-to-right.
  n  sort by filename ascending
  N  sort by filename descending
  t  sort by type ascending
  T  sort by type descending
  d  sort directories to top
  D  sort directories to bottom

e.g.: sortdir -w -s nd .
Will sort the current directory first by name (ascending),
then sort directories to the top, and will write the sorted
directory to disk.
```

