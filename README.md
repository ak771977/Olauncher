![Olauncher](https://repository-images.githubusercontent.com/278638069/db0acb80-661b-11eb-803e-926cae5dccb4)


# Olauncher | Minimal AF Launcher
AF stands for Ad-Free :D

## Custom Features (This Fork)

This fork includes additional customization options:

### Dual Timezone Clock
- Display two timezones side-by-side (Local | NY time)
- Perfect for tracking multiple time zones
- Toggle on/off in Settings → "Dual timezone (Local | NY)"
- Minimal design that fits the launcher aesthetic

### Default App Drawer Option
- Choose between text-based app list or Android's default app drawer
- Great for users who prefer the classic grid-style drawer
- Toggle in Settings → "Use default app drawer"
- Swipe up to open (works with either option)

### Zero Home Apps Support
- Remove all home screen apps (0-8 apps supported)
- Swipe gestures remain fully functional
- Perfect for an ultra-minimal home screen

## Install

#### Install from [F-Droid](https://f-droid.org/packages/app.olauncher) or [Play Store](https://play.google.com/store/apps/details?id=app.olauncher) or download the APK from the [latest release](https://github.com/tanujnotes/Olauncher/releases/).

[<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
    alt="Get it on F-Droid"
    height="80">](https://f-droid.org/packages/app.olauncher)
[<img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
    alt="Get it on Play Store"
    height="80">](https://play.google.com/store/apps/details?id=app.olauncher)

To maintain the simplicity of the launcher, a few niche features are available but hidden.

Please check out the [About](https://tanujnotes.substack.com/p/olauncher-minimal-af-launcher?utm_source=github) page in the Olauncher settings for a complete list of features and FAQs.

## Build from Source

Want to compile and use this custom version? Here's how:

### Prerequisites
- Android Studio (latest version recommended)
- JDK 11 or higher
- Android device or emulator

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/ak771977/Olauncher.git
   cd Olauncher
   git checkout claude/customize-launcher-clock-011CUq3qvWcNYgiV3XQofcAd
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - File → Open → Select the Olauncher folder
   - Wait for Gradle sync to complete

3. **Build the APK**
   - Build → Build Bundle(s) / APK(s) → Build APK(s)
   - Or run from terminal:
     ```bash
     ./gradlew assembleDebug
     ```
   - APK will be in: `app/build/outputs/apk/debug/app-debug.apk`

4. **Install on your device**
   - **Via Android Studio:** Connect device → Run → Select device
   - **Via ADB:**
     ```bash
     adb install app/build/outputs/apk/debug/app-debug.apk
     ```
   - **Manual:** Copy APK to phone → Open file → Install

5. **Set as default launcher**
   - Press Home button → Select Olauncher → Set as default
   - Or: Settings → Apps → Default apps → Home app → Olauncher

### Using the New Features

After installation:
1. Long press anywhere on the home screen to open Settings
2. Find "Dual timezone (Local | NY)" to enable dual clock display
3. Find "Use default app drawer" to switch between drawer styles
4. Set "Apps on home screen" to 0-8 (including 0 for completely empty home)

##

License: [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)

@tanujnotes | [X/Twitter](https://twitter.com/tanujnotes) | [Bluesky](https://bsky.app/profile/tanujnotes.bsky.social)

**[See my other apps](https://play.google.com/store/apps/dev?id=7198807840081074933)**

##

*New: We're working on an open source notes app called Note Safe (previously Note to Self). What's cool about it - it has a chat like interface and end-to-end encryption. [Take a look!](https://github.com/jeerovan/ntsapp)*
