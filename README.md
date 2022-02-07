# KmCaster

[![Download On Flathub](https://flathub.org/assets/badges/flathub-badge-en.svg)](https://flathub.org/apps/details/com.whitemagicsoftware.kmcaster)

This is the [Flatpak](https://flatpak.org/) build for
[KmCaster](https://github.com/DaveJarvis/kmcaster), a simple tool to display keyboard
and mouse events on your screen.

It looks like this:

![KmCaster](https://user-images.githubusercontent.com/973709/112867135-74051280-90b2-11eb-813e-07828882003e.png)

Since this repository only contains the Flatpak build instructions, please **open only
flatpak-specific issues**.

## Development

```sh
# Enable repo
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
# Install dependencies
flatpak-builder build-dir com.whitemagicsoftware.kmcaster.yaml --force-clean --install-deps-only --install-deps-from flathub
# Build and install
flatpak-builder build-dir com.whitemagicsoftware.kmcaster.yaml --install --user --force-clean
# Run it
flatpak run com.whitemagicsoftware.kmcaster
```
