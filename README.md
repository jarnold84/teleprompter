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
- **Swipe to scroll** — drag the script up or down with your finger at any time, including mid-take. Flick it for momentum. Auto-scroll picks up from wherever you left it, so you can fix your place without stopping the roll
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
- **Live recording timer** showing elapsed time and how large the take has grown
- **Camera and microphone selection**
- **Recording quality setting** — trade image quality against file size for long takes
- **Landscape mode** automatically requests HD 1280×720 resolution
- **Screen stays awake** while recording
- **Recorded clips** viewable, downloadable, and deletable directly in the app
- **Crash recovery** — takes are written to the device as they record, so a take is still there after a crash or a force-quit

## Saving Recordings

After stopping a recording, tap **Save** in the Camera panel.

**iPhone:** The video downloads to the Files app as an `.mp4`. To save to your Camera Roll:
1. Open the Files app and find the downloaded clip
2. Long press the file → tap **Share** → tap **Save Video**

The clip will then be available in your Camera Roll for upload to YouTube, Instagram, LinkedIn, Facebook, etc.

**Android:** Video saves as `.webm`. This format is compatible with YouTube and most desktop players. To save, tap Save in the Camera panel and the file will download to your Downloads folder. If it doesn't play in your default gallery app, use VLC or upload directly to a platform.

## Recording Length

Video is written to the device's storage every few seconds while you record, rather than being held in memory until you stop. Only a second or two of video is ever in memory at once, no matter how long the take runs — so the length you can record is limited by **free storage space**, not by RAM.

The Camera panel shows how much space is free, and the recording timer shows how large the current take has grown.

**Recording quality** (Camera panel) sets how much space a take uses:

| Setting | Approx. size | Good for |
|---|---|---|
| High | ~60 MB / min | Short, image-critical takes |
| Balanced *(default)* | ~30 MB / min | Almost everything |
| Long take | ~15 MB / min | Takes over 15 minutes |

At Balanced, a gigabyte of free space is roughly 30 minutes of video.

**If a take is interrupted** — the app crashes, you get a call, or you force-quit — the video recorded up to that point is already on the device. Reopen Scrollcast and it appears in the Camera panel marked **Recovered**. Save it as normal.

Recovered takes are cleared automatically after 7 days, and you can delete any clip yourself with the Delete button to free space.

**Note:** switching to another app stops the recording and saves it, because iOS suspends the camera when the app is in the background.

## Adding Captions

Captions are not built into this app. Recommended workflow:
1. Save your recording (see above)
2. Import into **CapCut** (free, iOS and Android) for one-tap auto-captions with editing
3. Or upload to **YouTube Studio** which auto-generates editable captions on upload

## Deployment

Hosted on [Vercel](https://vercel.com) via this GitHub repository. Any commit to `main` triggers an automatic redeploy within ~30 seconds.

## Notes

- The teleprompter overlay is a visual guide only — it does not appear in recorded video
- Front camera display is mirrored (like a mirror) — the recorded video is unmirrored
- For best results: Safari on iOS 15+ or Chrome on Android 10+

## Built With

HTML · CSS · JavaScript · MediaRecorder API · getUserMedia API · Screen Orientation API · PWA Manifest
