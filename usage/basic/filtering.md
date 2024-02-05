# Filtering

### hidden file

`-a` : show all, including `.` and `..`

`-A` `--almost-all`: show all, excluding `.` and `..`

`--hidden`: show hidden files/dirs only

### no directories, files only

`--no-dir` or `--file`

### no files, directories only

`--only-dir` or `-D`,`--dir`

### ignore backups

do not list implied entries ending with \~

`--ignore-backups` or `-B`

### git-ignore

`--git-ignore`&#x20;

### ignore entries matching the given Glob

`--ignore` , `-I`&#x20;

### entries matching Glob

`match` , `-M`

### filename ending with target extension

`--ext=ext1,ext2,...` : show matched results

`--no-ext=ext1,ext2,...` : ignore matched results

### files matching given mime types

`--only-mime=target1,target2,...`

{% hint style="info" %}
`--only-mime` will not match or remove any directory

use `--nodir` to remove all the directories&#x20;
{% endhint %}

### top N

`limitN=num` or `limit=num`

> num < 0 means infinity

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### before/after

`before=01-02`

`before='01-02 15:04'`&#x20;

`before=15:04`

`before=2006-01-02`

`before=2006-01-02 15:04`

