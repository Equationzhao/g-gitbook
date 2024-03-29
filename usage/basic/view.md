---
description: entries' meta data to show
---

# View

Name

#### show full path (relative to /)

`--full-path`&#x20;

#### Relative path

`--relative-to=base`&#x20;

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Quote name

enclose entry names in double quotes(overridden by `--literal`)

`-Q` or `--quote-name`

#### print entry names without quoting

`--literal` or `-N`

#### Git status

show git status

`--git`&#x20;

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

#### Git branch-name/repo-status

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

### with time

`--time`

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

the default time is modified time, and can be changed by flag `--time-type`

or use flag `--create`  `--mod`  `--access`  `--birth(macOS)`

<table><thead><tr><th>type</th><th>option</th><th data-hidden></th></tr></thead><tbody><tr><td>accessed</td><td>time-type=accessed</td><td></td></tr><tr><td>modified</td><td>time-type=modified</td><td></td></tr><tr><td>created</td><td>time-type=created</td><td></td></tr></tbody></table>

if you want to show them all, use the option `--time-type=accessed,modified,created,birth` to combine them

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

#### change time-style&#x20;

the default displaying style is `Day.Month'Year Hour:Minute`  (02.Jan'06 15:04) in Golang

time-style can be changed by option `--time-style`

```bash
g --time --time-style=iso
```

Available style:

* iso
* long-iso
* full-iso
* locale
* \+FORMAT (FORMAT is interpreted like in date(1), but not fully supported)

Also, the TIME\_STYLE environment variable sets the default style to use.

#### Relative time

use `--relative-time`

### with size

`--size`

#### recursive size

the size of the directory is itself, use `g --size --recursive-size` to show the size of the whole directory&#x20;

#### change unit

&#x20;`--size-unit=bit/b/k/.../auto`

or `--block-size=...`

#### total size

`--total-size --size` show the total size of all listing files/directories (overridden by --`no-total-size`)

### with blocks

`g --block`

### with inode

`g --inode`

{% hint style="info" %}
not working on Windows&#x20;
{% endhint %}

### with link

`g --link`

### with owner/group

`g --group`

`g --owner`

#### use uid/gid (sid in Windows)

`g --owner/group --numeric`

or just `g --uid/gid`

#### smart-group

show the group name only when it's different from the owner

### with permission bits

`g --perm`&#x20;

### with mime type

`g --mime`

#### mime parent type

`g --mime-parent`

#### charset

`g --charset`

#### detect size

when enabling the mime-type option, `g` will read the file to detect mime type

use `--exact-detect-size=512kb/1M/.../nolimit/infinity` to change the size of bytes g will read from the file&#x20;

> &#x20;0 means nolimit&#x20;

### with checksum

`g --checksum`

default: sha1

use `--checksum-algorithm=algo1,algo2...` to change algorithm

> algo: md5,sha1, sha224, sha256, sha384, sha512, crc32
