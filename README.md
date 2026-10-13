# Subway Surfers Classic

Based on the original classic Subway Surfers, which no longer ran on some newer phones. This build brings it back to modern ARM64 Android devices, with a focus on pure gameplay.

## Download and install

Download [the APK](Subway-Surfers-Classic-Pure-ARM64.apk).

- **Version:** 1.4-pure
- **Requires:** Android 7.0 or newer with ARM64 app support
- **Tested on:** Samsung Galaxy A55 5G running Android 16

Portrait and landscape are supported. The game follows your phone's rotation lock and rotates when auto-rotate is enabled.

Android 7.0 or newer alone isn't enough. Your phone must support ARM64 apps. There is no 32-bit ARM or x86 build, and compatibility with other phones hasn't been tested.

This is a custom classic build, not the current official release.

## Changes from the original game

- **Pure gameplay:** Missions, daily letters, mystery boxes, their buttons, and related gameplay popups are removed. Mission progression and rewards are disabled.
- **No head starts:** Run-start bonus buttons are removed. Regular powerups can still be collected during a run.
- **Faster runs:** The game accelerates twice as quickly. Starting speed stays the same, and maximum speed is 50% higher, reached after the same three minutes.
- **Maxed upgrades:** Jetpack, super sneakers, coin magnet, and 2x multiplier use their maximum upgrade tier.
- **Unlimited hoverboards:** Hoverboards have no inventory limit or cooldown, with their normal duration during a run.
- **Double scoring:** The permanent score bonus is enabled, separately from the collectible 2x powerup.
- **Cleaner pause screen:** Mission notes are removed, and Resume works immediately without showing “WAIT.” The notebook remains on the death/score screen.
- **Rotation support:** Both portrait and landscape follow the phone's rotation settings.
- **Rendering fixes:** Updated mesh geometry and adjusted the 2x pickup and worn jump shoes to reduce invisible objects and overlapping textures.

## Known issues

Fixes for texture glitches and invisible trains worked during testing, but these issues might still return. The project isn't perfect, so other bugs and glitches may occur too.

## ADB installation

To install through ADB into the main profile:

```sh
adb install --user 0 -r Subway-Surfers-Classic-Pure-ARM64.apk
```

On the tested Samsung phone, an ADB installation that included multiple profiles also installed the app into the clone profile, creating a second icon. Use `--user 0` to install only into the main profile. The duplicate came from installing across profiles through ADB.

## APK checksum

SHA-256:

```text
7dcf4530773d4dd3022df9c5efa7228ea84de2c7677b5a492e5152f6461b2e94
```
