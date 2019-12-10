# merge_cr2
Merge image xmp files and their .CR2.xmp counterparts to merge the rating.

## Usage
```
usage: merge_cr2 [-h] [-r] [-n] [-v] dirname

Merge image XMP metadata.

positional arguments:
  dirname        Name of the directory to process

optional arguments:
  -h, --help     show this help message and exit
  -r, --recurse  Recursively go through directory.
  -n, --dry-run  Perform a dry-run, i.e., do not modify anything but only show
                 what would be done.
  -v, --verbose  Increases verbosity. Can be specified multiple times to
                 increase.
```

For example, to apply recursively to a directory and first try out what it
would do: 

```
$ ./merge_cr2 -r -n /home/sickterm/bilderchen
```

then, to actually do it:

```
$ ./merge_cr2 -r /home/sickterm/bilderchen
```

## License
GNU GPL-3.
