# "Scrollcast" - iOS Video Teleprompter App

A mobile-first teleprompter + video recording web app designed for musicians, speakers, and creators. Works in both portrait and landscape orientation. No app store required — runs in Safari and installs directly to your iPhone home screen.

## Installing to Your iPhone Home Screen

This is the recommended way to use the app. Installing it gives you a fullscreen experience with no browser chrome, and enables orientation locking features.

1. Open Safari on your iPhone and navigate to your Vercel URL
2. Tap the **Share** button at the bottom of Safari (box with arrow pointing up)
3. Scroll down and tap **"Add to Home Screen"**
4. Give it a name (e.g. "Prompter") and tap **Add**

The app will appear as an icon on your home screen. Open it from there — not from Safari — for the full experience. Future updates deploy automatically; no need to reinstall.

## Features

- **Scrolling teleprompter overlay** on top of a live camera feed
- **Portrait and landscape support** — orientation detected automatically
- **Prompter box repositions automatically** when you rotate the phone, always staying near the front-facing camera
- **9-point text positioning** — override placement at any corner, edge, or side
- **Adjustable text size, box width, box height, opacity, and scroll speed**
- **Easy script editing** — paste or type directly in the app, tap Apply to load
- **Mirror text** option for use with a physical teleprompter glass
- **Manual text rotation** — 90° CW or CCW buttons for reading in any orientation
- **Front/back camera toggle** with one tap
- **3-second countdown** before recording starts (adjustable 0–10s)
- **Live recording timer** with blinking REC indicator
- **Camera and microphone selection**
- **Landscape mode** automatically requests HD 1280×720 resolution
- **Recorded clips** viewable and downloadable directly in the app

## Saving Recordings to Your Camera Roll

After stopping a recording, tap **Save** in the Camera panel. The video downloads to the **Files app** as an `.mp4`.

To save it to your Camera Roll for easy sharing:

1. Open the **Files app** and find the downloaded clip
2. Long press the file to bring up the context menu
3. Tap **Share**
4. Tap **Save Video**

The clip will now appear in your Camera Roll and can be uploaded directly from any app — YouTube, Instagram, LinkedIn, Facebook, etc.

## Adding Captions

Captions are not built into this app. The recommended workflow is:

1. Save your recording to the Camera Roll (see above)
2. Import into **CapCut** (free iOS app) for one-tap auto-captions with editing
3. Or upload to **YouTube Studio** which auto-generates editable captions on upload

## Deployment

Hosted on [Vercel](https://vercel.com) via this GitHub repository. Any commit to `main` triggers an automatic redeploy within ~30 seconds. The home screen icon always loads the latest version automatically.

## Notes

- Must be opened from the **home screen icon** (not Safari) for full PWA behavior
- Camera and microphone permissions must be granted in Safari Settings on first launch
- Recorded video saves as `.mp4` — compatible with iOS Photos, Instagram, YouTube, LinkedIn, and Facebook
- The teleprompter overlay appears on screen as a guide only and does not appear in recorded video footage
- Front camera display is mirrored (like a mirror) — recorded video is unmirrored (natural orientation)
- For best results use Safari on iOS 15+

## Built With

HTML · CSS · JavaScript · MediaRecorder API · getUserMedia API · Screen Orientation API
