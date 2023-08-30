testetsetstetsetstets

# shwer
Script to process directories into static webpages relying on directories for navigation.

# Requirements
POSIX shell and pandoc unless `$MARKUPPROCESSINGPROGRAM` in script file is specified to use other program to process markup files into pages.

# Synopsis
```
shwer [-t DIR] [-e DIR] [-p DIR] [-f]
```

# Description
Unlike werc, `shwer` processes a directory and makes exported directory with static pages ready to be hosted with http servers using shell script, while werc uses CGI to process pages for HTTP server software.
And also with extensions author made after being unsatisfied with what `werc` offers and requires. 

# Options
Arguments to options are mantadory.
```
[-t DIR] Directory to process. $TARGETDIR in script
[-e DIR] Where to export processed directory. $EXPORTDIR in script
[-p DIR] Directory containing exported page styling such as stylesheets. $PUBDIR in script
[-f]     If export directory already exists, overwrite it. $OVERWRITEEXPORT in script
```

# See also
* [werc](http://werc.cat-v.org/) - software which `shwer` was inspired from.
* This killer drawing i made just to test this markdown thing ![cool photo](killerwhale.png)
