# wesh
Script to process directories into static webpages relying on directories for navigation with easy configuration for end user.

# Requirements
POSIX shell and pandoc unless `$MARKUPPROCESSINGPROGRAM` in script file is specified to use other program to process markup files into pages.

# Synopsis
```
wesh [-t DIR] [-e DIR] [-p DIR] [-f]
```

# Description
Unlike `werc`, `wesh` processes a directory and makes exported directory with static pages ready to be hosted with http servers using shell script, while `werc` uses CGI to process pages for HTTP server software.

And also with extensions author made after being unsatisfied with what `werc` offers and requires and taking out other things `werc` offers that author does not feel it's necessary for his work. 

# Options
Arguments to options are mantadory.
```
[-t DIR] Directory to process. $TARGETDIR in script
[-e DIR] Where to export processed directory. $EXPORTDIR in script
[-p DIR] Directory containing exported page styling such as stylesheets. $PUBDIR in script
[-f]     If export directory already exists, overwrite it. $OVERWRITEEXPORT in script
```

# Directories
* `export` - Exported webpages. Not required to be specified in script, however stop if already exists unless script is forced to remove said directory.
* `pub` - Styling and graphics for exported webpages. Required as default stylesheet correctly set visual structure of web pages.
* `site` - Unprocessed web pages. Required as script converts contents of directories into with webpages along converting markup files into webpages if found such as markdown files. Contains example directory.

# Preview
<img width="700" alt="preview1" src="https://github.com/user-attachments/assets/45192422-dbbd-467d-bf79-8f8952837499" />
<img width="700"  alt="preview2" src="https://github.com/user-attachments/assets/8f61e2a5-8431-4751-8781-6b4e61252d64" />
<img width="700"  alt="preview3" src="https://github.com/user-attachments/assets/d4c37002-1408-47f8-af11-1a83d1b6784d" />

# See also
* [werc](http://werc.cat-v.org/) - software which `wesh` is inspired from.
