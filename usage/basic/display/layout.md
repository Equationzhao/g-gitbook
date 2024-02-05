---
description: output layout
---

# Layout

### Format

`--format=layout`

across -x, commas -m, horizontal -x, long -l, single-column -1, verbose -l, vertical -C, table -tb, HTML -html, Markdown -md, CSV -csv, TSV -tsv, json -j, tree -T

| layout        | aliases       |                                                               |
| ------------- | ------------- | ------------------------------------------------------------- |
| across        | x, horizontal |                                                               |
| vertical      | C             | Default                                                       |
| commas        | m             |                                                               |
| long          | l, verbose    | also add perm,total-size,size,owner,group,time, icons to view |
| single-column | 1             |                                                               |
| markdown      | md            | no color and icons                                            |
| csv           |               | no color and icons                                            |
| tsv           |               | no color and icons                                            |
| json          | j             | no color and icons                                            |
| tree          | T             |                                                               |

### Zero

end each output line with NUL, not newline

`--zero` or `-0`

### Tree 🌳&#x20;

list in trees&#x20;

`--tree` or `-T`

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
some feature doesn't work in the tree view.

like --limit=N doesn't support tree view
{% endhint %}

### Recurse&#x20;

recurse into directory&#x20;

`--recurse` or `-R`&#x20;

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

### Limit tree/recurse depth

`--depth=num` or `--level=num`

> num < 0 means no limit&#x20;

### Others

Please refer to the [man page](https://github.com/Equationzhao/g/blob/master/g.md) or program output with  `--help`&#x20;
