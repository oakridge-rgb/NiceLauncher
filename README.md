# Nice Launcher

A fork of [Olauncher](https://github.com/tanujnotes/Olauncher) (Minimal AF Launcher)
with a **Graphite & Ice** restyle — cool, quiet, and electric.

![Nice Launcher](fastlane/metadata/android/en-US/images/icon.png)

## What's different from Olauncher

| | Olauncher | Nice Launcher |
| --- | --- | --- |
| Identity | Olauncher branding, yellow accent | **Nice Launcher**, ice-cyan accent (`#22D3EE`) |
| Palette | pure black / pure white text | **graphite** (`#15181E`) day text, **ice-white** (`#F4F8FB`) night text — everything downstream (shadows, dialogs, popups, drawer) retints automatically via the theme attrs |
| Clock | 50–66sp, plain date | bigger clock (54–72sp) with tight tracking, **small-caps letterspaced date** |
| Icon | Olauncher logo | geometric **N** glyph, ice gradient on graphite, adaptive + all densities |
| Install | `app.olauncher` | `app.nicelauncher` (installs side-by-side with Olauncher) |
| Version | 6.11.5 (117) | 6.11.5-nice.1 (118) |

Everything else is untouched Olauncher: gestures, hidden apps, daily wallpapers,
work-profile support, double-tap-to-lock. **Zero Kotlin code changed** — the whole
restyle rides on Olauncher's resource-driven theme system (`primaryColor` attrs),
which is exactly why this fork will stay easy to rebase onto upstream releases.

## Build

Standard Android project: open in Android Studio / Code on the Go, or:

```
./gradlew assembleDebug      # APK at app/build/outputs/apk/debug/
```

AGP 8.9.1, Kotlin 2.1.20, Gradle 8.11.1, minSdk 24, targetSdk 36. No extra
repositories, no snapshot dependencies.

## Credits & license

All credit for the launcher itself goes to [Tanuj](https://github.com/tanujnotes)
and the Olauncher contributors — this fork only re-dresses it. GPLv3, same as
upstream. The "Olauncher Pro" listing referenced in-app still belongs to the
original developer.
