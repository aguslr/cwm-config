# cwm configuration

## About

This repository stores my configuration of [cwm][], *a window manager for X11
which contains many features that concentrate on the efficiency and transparency
of window management*.

## Getting the files

### Using Git

If we have Git installed on the system, we can get the files directly from the
repository:

```sh
git clone https://github.com/aguslr/cwm-config
```

After this, every time we want to update the files we do:

```sh
cd cwm-config && git pull
```

### Without Git

If Git is not installed, we can still get the files as long as we have a basic
Unix environment available:

```sh
wget https://github.com/aguslr/cwm-config/tarball/main -O - | tar -xzv --strip-components 1 --exclude={README.md}
```

### Installing with Stow

To easily create and manage links to the files we can use GNU [Stow][] as
follows:

```sh
stow -vt ~ -S .
```

[cwm]: https://github.com/chneukirchen/cwm
[stow]: https://www.gnu.org/software/stow/
