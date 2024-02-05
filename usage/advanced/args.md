# args

`g` will transform args in the following table

<table><thead><tr><th width="344">before</th><th>after</th></tr></thead><tbody><tr><td>~</td><td>$HOME</td></tr><tr><td>...</td><td>../..</td></tr><tr><td>....</td><td>../../..</td></tr><tr><td>more dots</td><td>../.......</td></tr></tbody></table>



{% hint style="info" %}
But if you have an entry named '.....', `g` will not work. You should use **`--no-path-transform`** to disable this feature.
{% endhint %}

<figure><img src="../../.gitbook/assets/截屏2023-06-19 17.39.50.png" alt=""><figcaption></figcaption></figure>
