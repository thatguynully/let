# let
yet another pacman wrapper

## usage

```bash
let package in   # install a package
let package out  # remove a package
```

- `in` → `pacman -S package`
- `out` → `pacman -Rns package`

## installation

```bash
git clone https://github.com/thatguynully/let
cd let
mkdir -p "$HOME/.local/bin"
mv ./let "$HOME/.local/bin/"
```

make sure `$HOME/.local/bin` is in your `PATH`!