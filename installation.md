# Installation

### Installation Guide

#### Via package manager

**Arch Linux (AUR)**

```bash
yay -S g-ls
```

**Homebrew 🍺**

```bash
brew install g-ls
```

or use the homebrew tap:

```bash
brew tap equationzhao/core git@github.com:Equationzhao/homebrew-g.git
```

```bash
brew install g-ls
```

**Windows Scoop**

```powershell
scoop install https://raw.githubusercontent.com/Equationzhao/g/master/scoop/g.json
```

```powershell
# upgrade
scoop uninstall g # uninstall first
scoop install https://raw.githubusercontent.com/Equationzhao/g/master/scoop/g.json
```

**Winget**

TODO, see [issue](https://github.com/Equationzhao/g/issues/119)

#### Pre-built executable

**install script**

**install**

```sh
bash -c "$(curl -fsSLk https://raw.githubusercontent.com/Equationzhao/g/master/script/install.sh)"
```

**uninstall**

```sh
curl -fsSLk https://raw.githubusercontent.com/Equationzhao/g/master/script/install.sh | bash /dev/stdin -r     
```

**deb**

download from [release](https://github.com/Equationzhao/g/releases) page

```bash
sudo dpkg -i g_$version_$arch.deb
```

**tar.gz/zip**

just download from [release page](https://github.com/Equationzhao/g/releases), extract the gzip and add the executable file to your `PATH`

#### From source

Requires Go version >= 1.21

```bash
go install -ldflags="-s -w"  github.com/Equationzhao/g@latest
```

Alternatively, clone the repo for a dev version:

```bash
git clone github.com/Equationzhao/g
cd g
go build -ldflags="-s -w" 
# then add the executable file to your `PATH`
```

### Validate Installation&#x20;

use `g -v` to check version

```bash
g -v # check version
```

you should see output like this:

```
💡 g - a powerful ls
 | Version                0.11.1
 | Go Version             1.20.5
 | Compiler               gc
 | Platform               linux/amd64

 | Copyright (C) 2023 Equationzhao. MIT License
 | This is free software: you are free to change and redistribute it.
 | There is NO WARRANTY, to the extent permitted by law.
```

## check new version

`g --check-new-version`
