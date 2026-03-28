GETPRJ
======

## Help

getprj

    Usage: getprj NAMES...
    
    Search a project named "NAME" in a directory listed in one of
    the following places:
    
      - PROJECT_PATH        Space separated directory list.
      - /etc/projectdirs    Newline separated directory list.
      - ~/.projectdirs      Newline separated directory list.
    
    Supported flags:
    
      -l      List project directories.
      -c      Clear cache (~/.getprj.cache).
      -m MSG  Print message when not found.
    
    The cache is updated each time a project is not found.

point

    Usage: point NAME [PATHNAME]
    
    Point from the current directory to PATHNAME. Links are saved
    in ".point" file. Scripts can require you to specify a path the
    following way:
    
    Example script:
    
        #!/bin/sh -e
        te="$(point -g te 'The testing environment.')"
        test -n "${te}"
        "${te}/test.sh" ./program
    
    Files: .point

## Collaborating

Feel free to open bug reports and feature/pull requests.

More software like this here:

1. [https://harkadev.com/prj/](https://harkadev.com/prj/)
2. [https://devreal.org](https://devreal.org)
