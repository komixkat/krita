<p align="center">
  <img src="https://krita.org/images/hero-image-50.webp" alt="Krita" width="100%">
</p>

# krita, with a custom splash screen

This is a fork of [Krita](https://krita.org), the free and open source digital painting app. The only difference from upstream: the splash screen (the Kiki artwork you see on launch) can be swapped for any image you want, without recompiling.

Built for Arch Linux via GitHub Actions. See [`NOTICE-CUSTOM-SPLASH.md`](./NOTICE-CUSTOM-SPLASH.md) for what changed and [`custom-splash.patch`](./custom-splash.patch) for the exact diff.

## Install

Add this repo to `/etc/pacman.conf`:

```
[komixkat]
SigLevel = Optional TrustAll
Server = https://github.com/komixkat/krita/releases/download/rolling
```

Then:

```
sudo pacman -Sy
sudo pacman -S krita-git
```

New builds land here weekly and show up in a normal `sudo pacman -Syu`, no manual downloads needed.

## Usage

```
mkdir -p ~/.config/krita
cp your_image.png ~/.config/krita/custom_splash.png
```

Restart Krita. Delete that file to go back to the default splash.

## License

GPLv3, same as upstream. See [`COPYING`](./COPYING).
