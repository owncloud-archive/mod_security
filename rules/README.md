Regex collection
==========

| Type | Expression | Special |
|---------|------------|------------|
| Filesystem (PHP): Directory name | !(\\.\\./&#124;\\.\\.\\\\\\\\&#124;'&#124;\") | Filter against path traversals and potential SQL injections
| Filesystem (PHP): Filename | !(\\.\\./&#124;\\.\\.\\\\\\\\&#124;'&#124;\") | Filter against path traversals
| Filesystem (SWF): Filename | !("&#124;') | Filter against cross-site flashing
| Username | ^([a-zA-Z0-9_\\.@]+)$ | Same regular expression as ownCloud uses
| Requesttoken | ^[a-z0-9]+$ |
| Password | | Passwords are allowed to contain any characters
| App ID | [a-zA-Z_\-0-9]+$ |