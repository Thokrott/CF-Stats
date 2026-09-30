<p align="center">
  <img src="app-icon.png" width="112" alt="CF Stats fire-cat icon">
</p>

<h1 align="center">CF Stats</h1>

<p align="center">
  A playful Codeforces dashboard and home-screen streak widget for Android.
</p>

<p align="center">
  <a href="https://github.com/Thokrott/CF-Stats/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/Thokrott/CF-Stats?display_name=tag&style=for-the-badge&color=2DD37A"></a>
  <img alt="Android 8+" src="https://img.shields.io/badge/Android-8%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white">
  <img alt="Kotlin" src="https://img.shields.io/badge/Kotlin-native-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white">
</p>

![CF Stats hero](hero.png)

## Your Codeforces momentum, at a glance

CF Stats turns public Codeforces activity into a focused mobile dashboard. The widget keeps the current streak visible on the home screen, while the app reveals the history behind it: contribution activity, solved-problem ratings, strongest topics, submissions, acceptance rate, and upcoming contests.

The fire cat changes pose during the day—calm after you submit, increasingly worried as midnight approaches.

## Highlights

- **3 × 1 streak widget** with expressive fire-cat poses
- **365-day activity heatmap** with tap-to-expand and horizontal scrolling
- **All-time solved count** with an optional manual correction for problems missing from the public API
- **Problem-rating distribution**, average rating, and hardest solved problem
- **Strongest topic tags** based on unique accepted problems
- **Upcoming Codeforces contests** with Div. 1–4, Educational, and Other filters
- **Custom reminder time** when no submission has been made that day
- **Local-first settings**—no Codeforces password or API key required
- **Adaptive launcher icon** and Android 15 edge-to-edge support

![Widget and activity showcase](widget-showcase.png)

## Install

1. Open the [latest release](https://github.com/Thokrott/CF-Stats/releases/latest).
2. Download `CF-Stats.apk`.
3. Allow installation from your browser or file manager when Android asks.
4. Open **CF Stats**, enter your Codeforces handle, and refresh.
5. Long-press the home screen, open **Widgets**, and add **CF Stats**.

Android may warn that the app is from outside Google Play. The downloadable APK is built directly from this repository.

## How the numbers work

- A streak day is a calendar day with at least one Codeforces submission.
- Solved totals and rating statistics count unique accepted problems returned by `user.status`.
- Codeforces sometimes omits older problems from that public response. Use **Settings → Solved-problem correction** to add the small difference shown on your profile.
- Dates use the phone's local timezone.

## Compatibility

CF Stats supports **Android 8.0 (API 26) and newer**. It uses native Android views and a resizable widget, with no device-specific dependency. The interface has been tuned for modern Pixel phones and remains responsive across common phone widths.

## Build from source

Requirements: JDK 17 and Android SDK 35.

```bash
./gradlew assembleDebug
```

The APK is created at `app/build/outputs/apk/debug/app-debug.apk`.

## Data and privacy

CF Stats reads public data from the official Codeforces API. Your handle, cached statistics, filters, solved-count correction, and reminder preferences stay on the device. See [PRIVACY.md](PRIVACY.md) for details.

## Disclaimer

CF Stats is an independent project and is not affiliated with or endorsed by Codeforces.
