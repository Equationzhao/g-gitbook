# Basic

usage:  `g [options] [path]`

:smile: option started with one _<mark style="color:blue;">**-dash**</mark>_ or two _<mark style="color:blue;">**--dashes**</mark>_ are both _**OK**_:

```bash
g --checksum --checksum-algorithm sha256 
# or g -checksum -checksum-algorithm=sha256
```

Simply running `g` without any additional option will list files in current working directory

### show hidden files/directories&#x20;

`g -a` : show all, including `.` and `..`

`g -A` : show all, excluding `.` and `..`

### with icons

```bash
g --icons
```

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

this option will be overridden by `--no-icon`
