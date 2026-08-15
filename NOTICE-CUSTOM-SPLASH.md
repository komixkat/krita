# Modifications to this fork

This is a fork of KDE/krita (https://github.com/KDE/krita, upstream:
https://invent.kde.org/graphics/krita), distributed under the same license
as the original — GNU GPLv3, see COPYING. Individual files retain their
original SPDX license headers.

Per GPLv3 section 5(a), modified files must carry a notice stating they
were changed and when:

## 2026-08-15 — Configurable splash screen

**File changed:** `libs/ui/kis_splash_screen.cpp`
**Changed by:** komixkat
**What changed:** `KisSplashScreen::getImageSource()` now checks for a
user-supplied image at `$KRITA_CUSTOM_SPLASH` or
`<config dir>/custom_splash.png` before falling back to the compiled-in
splash resource. No other behavior was changed. Full diff in
`custom-splash.patch` at the repo root and in the corresponding git commit.

No other files in this tree have been modified from upstream.
