# nudoku #

nudoku is a ncurses based sudoku game.

## Install ##

### Using package manager ###

#### Arch Linux ####
I heard rumors of nudoku being in the [AUR](https://aur.archlinux.org/packages/nudoku-git/).

#### Funtoo/Gentoo ####
Add [strangeland-overlay](https://github.com/jubalh/strangeland-overlay).

Then run:

```
emerge --sync
emerge nudoku -a
```

### openSUSE ###

For Leap 42.1 and Tumbleweed nudoku is in the official repositories.
On 13.2 you need to add the the games repository and install nudoku via zypper.

```
zypper ar http://download.opensuse.org/repositories/games/openSUSE_13.2/ games
zypper in nudoku
```

### From Source ###

#### Dependency ####
- ncurses

#### Compilation ####

Get the lastest .tar.xz [release](https://github.com/jubalh/nudoku/releases) and extract it.
Then run:

```
./configure
make
./src/nudoku
```

For the git version you will have to do:

```
git clone https://github.com/jubalh/nudoku
cd nudoku
autoreconf -i
./configure
make
./src/nudoku
```

Add `-DDEBUG` to `make` to have some debug output.

## Bugtracker ##

https://github.com/jubalh/nudoku/issues

