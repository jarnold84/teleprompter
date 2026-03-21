# iOS Mobile Browser-Based Video Teleprompter

A mobile-first teleprompter + video recording web app designed for musicians, speakers, and creators. Works in both landscape and portrait orientation. No app store required — runs in Safari and can be added to your iPhone home screen.

## Features

- **Scrolling teleprompter overlay** on top of a live camera feed
- **Landscape and portrait support** with automatic orientation detection
- **9-point text positioning** — place the prompter at any corner, edge, or side
- **Adjustable text size, box width, box height, opacity, and scroll speed**
- **Easy script editing** — paste or type directly in the app
- **Mirror text** option for use with a physical teleprompter glass
- **Front/back camera toggle** (defaults to front-facing)
- **5-second countdown** before recording starts (adjustable 0–10s)
- **Live recording timer** with blinking REC indicator
- **Camera, microphone, and resolution settings**
- **Recorded clips downloadable** directly from the app

## Usage

Open the live URL in **Safari on iPhone**. To install as a home screen app:

1. Tap the **Share** button in Safari
2. Tap **"Add to Home Screen"**
3. Tap **Add**

The app will open fullscreen like a native app.

## Saving & Sharing Recordings

After stopping a recording, tap **Save** in the Camera panel. The video will download to the **Files app** as an `.mp4`.

To get it into your Camera Roll for easy sharing:

1. Open the **Files app** and locate the downloaded clip
2. Tap and hold the file to bring up the context menu
3. Tap **Share**
4. Tap **Save Video**

The clip will now appear in your Camera Roll and can be uploaded directly from any app — YouTube, Instagram, LinkedIn, Facebook, etc.



Hosted on [Vercel](https://vercel.com) via this GitHub repository. Any commit to `main` triggers an automatic redeploy.

## Notes

- The teleprompter overlay is a UI guide only and does not appear in recorded video footage
- Camera and microphone permissions must be granted in Safari Settings
- Recorded video saves as `.mp4` on iOS or `.webm` on desktop browsers
- For best results, use in Safari on iOS 15+

## Built With

HTML · CSS · JavaScript · MediaRecorder API · getUserMedia API
