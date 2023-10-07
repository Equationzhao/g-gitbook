---
description: how to install g
---

# Install

### Pre-built executable&#x20;

[release](https://github.com/Equationzhao/g/releases)

### Build from source

g is written in Golang, so if you want to build g your self, you should have go1.20 (or later) installed.

```bash
go install -ldflags="-s -w -v"  github.com/Equationzhao/g@latest
```

make sure `$GOPATH/bin` is in your `PATH`

### Via package manager

#### Archlinux

aur ![](https://img.shields.io/aur/version/g-ls?color=1793d1\&label=g-ls\&logo=arch-linux\&style=for-the-badge)

```bash
yay -S g-ls
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

