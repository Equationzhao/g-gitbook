# Sorting

### Sort option

`--sort=order`

sort by field, default: ascending and case insensitive.

available fields:&#x20;

* nature(default)
* none(nosort)
* name
* .name(sorts by name without a leading dot)
* size
* time
* owner
* group
* extension
* width
* inode
* mimetype&#x20;

> field beginning with Uppercase is case sensitive\
> use field followed by '-descend' to sort in descending order

#### combined

eg: `--sort=ext,size-descend,Name`

it will sort entries by extension first, for those having the same extension, comparing their size, if two have the same size, comparing their name( case sensitive)

#### nature sort

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>nature sort</p></figcaption></figure>

<table><thead><tr><th>type </th><th data-type="number">Priority </th></tr></thead><tbody><tr><td>hidden directory </td><td>0</td></tr><tr><td>directory</td><td>1</td></tr><tr><td>files</td><td>2</td></tr><tr><td>link</td><td>3</td></tr><tr><td>name</td><td>4</td></tr></tbody></table>

### Dir first

List directories before other files

`--dir-first`

### Others

Please refer to [man page](https://github.com/Equationzhao/g/blob/master/g.md) or try `--help`&#x20;
