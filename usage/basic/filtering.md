# Filtering

### hidden file

`-a` : show all, including `.` and `..`

`-A` `--almost-all`: show all, excluding `.` and `..`

`--hidden`: show hidden files/dirs only

### no directories, files only

`-no-dir` or --`file`

### no files, directories only

`--only-dir` or `-D`,`--dir`

### ignore backups

do not list implied entries ending with \~

`--ignore-backups` or `-B`

### git-ignore

`--git-ignore`&#x20;

### ignore entries matching the given Glob

`--ignore-glob` or `--ignore` , `-I`&#x20;

### entries matching Glob

`--glob` or `match` , `-M`

### files ending with target extension

`--ext=ext1,ext2,...` : show matched results

<figure><img src="../../.gitbook/assets/截屏2023-06-19 01.17.36.png" alt="" width="315"><figcaption></figcaption></figure>

`--noext=ext1,ext2,...` : ignore matched results

<figure><img src="../../.gitbook/assets/截屏2023-06-19 01.21.02.png" alt=""><figcaption></figcaption></figure>

### files matching given mime types

`--mime-only=target1,target2,...`

<figure><img src="../../.gitbook/assets/截屏2023-06-19 01.56.35.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
`--mime-only` will not match or remove any directory

use `--nodir` to remove all the directories&#x20;
{% endhint %}

### top N

`limitN=num` or `limit=num`

> num < 0 means infinity

<figure><img src="../../.gitbook/assets/截屏2023-06-18 22.23.29.png" alt=""><figcaption></figcaption></figure>

### before/after

`before=01-02`

`before='01-02 15:04'`&#x20;

`before=15:04`

`before=2006-01-02`

`before=2006-01-02 15:04`

