# Scrollcast — Video Teleprompter

A mobile-first teleprompter + video recording web app for musicians, speakers, and creators. Works in portrait and landscape orientation on iPhone and Android. No app store required — installs directly to your home screen from your mobile browser.

## Android Support (Beta)

Android support is currently in beta and has not been fully tested across all devices. If you encounter issues, contact support at **jarnold84@protonmail.com**.

## Installing to Your Home Screen

Installing gives you a fullscreen experience with no browser chrome. Future updates deploy automatically — no need to reinstall.

**iPhone (Safari):**
1. Open Safari and navigate to your Scrollcast URL
2. Tap the Share button (box with arrow pointing up)
3. Tap **Add to Home Screen**
4. Tap **Add**

**Android (Chrome):**
1. Open Chrome and navigate to your Scrollcast URL
2. Tap the three-dot menu (⋮) in the top right
3. Tap **Add to Home screen**
4. Tap **Add**

Always open the app from the home screen icon — not the browser — for the full experience.

## Features

- **Scrolling teleprompter overlay** on top of a live camera feed
- **Portrait and landscape support** — orientation detected automatically
- **Prompter box repositions automatically** when you rotate the phone, always staying near the front-facing camera
- **9-point text positioning** — override placement at any corner, edge, or side
- **Adjustable text size, box width, box height, opacity, and scroll speed**
- **Easy script editing** — paste or type directly in the app, tap Apply to load
- **Script always rewinds to the top** when you press record
- **Mirror text** option for use with a physical teleprompter glass
- **Manual text rotation** — 90° CW or CCW buttons for any orientation
- **Front/back camera toggle** with one tap
- **3-second countdown** before recording starts (adjustable 0–10s)
- **Live recording timer** with warning at 30s before the time limit
- **Camera and microphone selection**
- **Landscape mode** automatically requests HD 1280×720 resolution
- **Recorded clips** viewable and downloadable directly in the app

## Saving Recordings

After stopping a recording, tap **Save** in the Camera panel.

**iPhone:** The video downloads to the Files app as an `.mp4`. To save to your Camera Roll:
1. Open the Files app and find the downloaded clip
2. Long press the file → tap **Share** → tap **Save Video**

The clip will then be available in your Camera Roll for upload to YouTube, Instagram, LinkedIn, Facebook, etc.

**Android:** Video saves as `.webm`. This format is compatible with YouTube and most desktop players. To save, tap Save in the Camera panel and the file will download to your Downloads folder. If it doesn't play in your default gallery app, use VLC or upload directly to a platform.

## Recording Length

Scrollcast has no hard recording limit. How long it records reliably depends on your device and how much memory is available.

**Tested on iPhone 13 with all other apps closed: 10+ minutes recorded successfully.**

For best results before an important take, do a short test recording first to confirm your setup. If you experience freezing or audio-only playback, it means your device has hit its memory ceiling for that session. Close all other apps and browser tabs, reload Scrollcast, and try again.

**Tips for longer recordings:**
- Close all other apps before opening Scrollcast
- Close any unused Safari tabs
- Restart your phone if you haven't recently
- Keep clips under 10 minutes where possible

**For unlimited length:** use a second device running Scrollcast as a teleprompter display, and record with your phone's native Camera app.

## Adding Captions

Captions are not built into this app. Recommended workflow:
1. Save your recording (see above)
2. Import into **CapCut** (free, iOS and Android) for one-tap auto-captions with editing
3. Or upload to **YouTube Studio** which auto-generates editable captions on upload

## Deployment

Hosted on [Vercel](https://vercel.com) via this GitHub repository. Any commit to `main` triggers an automatic redeploy within ~30 seconds.

## Notes

- **For longer recordings:** close all other apps and browser tabs before recording to maximize available memory. Testing on iPhone 13 with no other apps open achieved 7+ minute recordings reliably.
- The teleprompter overlay is a visual guide only — it does not appear in recorded video
- Front camera display is mirrored (like a mirror) — the recorded video is unmirrored
- For best results: Safari on iOS 15+ or Chrome on Android 10+

## Built With

HTML · CSS · JavaScript · MediaRecorder API · getUserMedia API · Screen Orientation API · PWA Manifest
