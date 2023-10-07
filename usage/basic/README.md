# Basic

usage:  `g [options] [path]`

:smile: option started with one <mark style="color:blue;">-dash</mark> or two <mark style="color:blue;">--dashes</mark> are both OK:

```bash
g --checksum --checksum-algorithm sha256 
# or g -checksum -checksum-algorithm=sha256
```

Simply running `g` without any additional option will list files in current working directory, with color

<figure><img src="../../.gitbook/assets/截屏2023-06-18 15.02.21.png" alt=""><figcaption></figcaption></figure>

### show hidden files/directories&#x20;

`g -a` : show all, including `.` and `..`

`g -A` : show all, excluding `.` and `..`

### with icons

```bash
g --icon
```

<figure><img src="../../.gitbook/assets/截屏2023-06-18 15.08.24.png" alt=""><figcaption></figcaption></figure>

this option will be overridden by `--no-icon`

###
