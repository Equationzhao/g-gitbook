# fuzzy match path

Q: I'm currently in path A, but I wanna list the files in path B which I don't know the exact path.

A: use `g -f` to do a fuzzy search. `g` will remember the paths you've passed to g before\*, and once you pass your path args to g with `-f` option, `g` will calculate the score for each paths in index, using the algorithm in [`fzf`](https://github.com/junegunn/fzf) project, and it will return the path with highest score as the result, listing entries there.

> \*: which is store at 'UserConfigDir/g/index'
>
> On Unix systems, UserConfigDir is $XDG\_CONFIG\_HOME as specified by https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html if non-empty, else $HOME/.config.&#x20;
>
> On Darwin, UserConfigDir is $HOME/Library/Application Support.&#x20;
>
> On Windows, UserConfigDir is %AppData%.

### list

`--li` list index

### disable index update

by default, g will store every absolute path it receives.&#x20;

use `--disable-index` or in short `-di` to disable index update.

### remove index

`--rm` `--remove-index` paths

`--rebuild-index` remove all

`--remove-current-path` remove the working directory from index.

`--remove-invalid-path` will try to access all the path stored, and remove those can't be accessed.
