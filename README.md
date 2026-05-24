# slowrx Flatpak

Flatpak packaging for [slowrx](https://windytan.github.io/slowrx/), an SSTV decoder for amateur radio.

## Requirements

- [flatpak](https://flatpak.org/setup/)
- [flatpak-builder](https://docs.flatpak.org/en/latest/flatpak-builder.html)
- GNOME SDK:

```sh
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak install flathub org.gnome.Sdk//50
```

## Building and installing

```sh
flatpak-builder --user --install --force-clean build-dir io.github.windytan.slowrx.yaml
```

## Running

```sh
flatpak run io.github.windytan.slowrx
```

## Uninstalling

```sh
flatpak uninstall io.github.windytan.slowrx
```
