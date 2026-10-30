# let

yet another pacman wrapper

## usage

```bash
let package in       # install a package
let package update   # update a package
let package out      # remove a package
let package denied   # remove a package and its unused dependencies
let updatesys        # update the entire system
```

- `in` → `pacman -S --needed package`
- `update` → `pacman -S package`
- `out` → `pacman -R package`
- `denied` → `pacman -Rns package`
- `updatesys` → `pacman -Syu`

## installation

```bash
git clone https://github.com/thatguynully/let
cd let
mkdir -p "$HOME/.local/bin"
mv ./let "$HOME/.local/bin/"
```

make sure `$HOME/.local/bin` is in your `PATH`!
