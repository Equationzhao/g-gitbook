---
description: entries' meta data to show
---

# View

### Name

#### show full path

`--full-path`&#x20;

#### Relative path

`--relative-to=base`&#x20;

<figure><img src="../../.gitbook/assets/截屏2023-06-18 21.45.50.png" alt=""><figcaption></figcaption></figure>

#### Quote name

enclose entry names in double quotes(overridden by `--literal`)

`-Q` or `--quote-name`

#### print entry names without quoting

`--literal` or `-N`

#### Git status

show git status

`--git`&#x20;

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### with time

```bash
--time
```

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

</div>

the default time is modified time, which can be changed by option `--time-type`

or use option `--create`  `--mod`  `--access`  `--birth(macOS)`

<table><thead><tr><th>type</th><th>option</th><th data-hidden></th></tr></thead><tbody><tr><td>access</td><td>time-type=access</td><td></td></tr><tr><td>modified</td><td>time-type=mod</td><td></td></tr><tr><td>create</td><td>time-type=create</td><td></td></tr></tbody></table>

if you want to show them all, use the option `--time-type=access,mod,create,birth` to combine them

<figure><img src="../../.gitbook/assets/截屏2023-06-18 15.25.14.png" alt="" width="375"><figcaption></figcaption></figure>

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

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/截屏2023-06-18 16.00.03.png" alt=""><figcaption></figcaption></figure>

</div>

### with size

`--size`

#### recursive size

the size of the directory is itself, use `g --size --recursive-size` to show the size of the whole directory&#x20;

<div>

<figure><img src="../../.gitbook/assets/截屏2023-06-18 16.22.13.png" alt="" width="229"><figcaption><p>size</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/截屏2023-06-18 16.47.23.png" alt="" width="209"><figcaption><p>recursive size</p></figcaption></figure>

</div>

#### change unit

&#x20;`--size-unit=bit/b/k/.../auto`

or `--block-size=...`

#### total size

`--total-size --size` show the total size of all listing files/directories (overridden by --`no-total-size`)

<figure><img src="../../.gitbook/assets/截屏2023-06-18 16.50.02.png" alt="" width="325"><figcaption></figcaption></figure>

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

### with permission bits

`g --perm`&#x20;

### with mime type

`g --mime`

#### mime parent type

`g --mime-parent`

#### charset

`g --charset`

#### detect size

when enabling mime-type option, `g` will read the file to detect mime type

use `--exact-detect-size=512kb/1M/.../nolimit/infinity` to change the size of bytes g will read from the file&#x20;

> &#x20;0 means nolimit&#x20;

### with checksum

`g --checksum`

default: sha1

use `--checksum-algorithm=algo1,algo2...` to change algorithm

> algo: md5,sha1, sha224, sha256, sha384, sha512, crc32

<figure><img src="../../.gitbook/assets/截屏2023-06-18 19.35.18.png" alt=""><figcaption></figcaption></figure>
