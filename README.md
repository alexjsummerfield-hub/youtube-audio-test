# YouTube Audio Library

A lightweight personal web app for organising YouTube links and listening with simple, large controls, especially on an iPhone.

**[Launch the app](https://alexjsummerfield-hub.github.io/youtube-audio-test/)**

## Features

- YouTube link library with full-title, text-first browsing.
- Folders and manual ordering of videos and folders.
- **Video**, **Audio**, and **Library** views.
- Automatically saved playback positions for resuming later.
- Play/pause, a seek slider, ±30-second controls, and playback speed selection.
- Sleep timer that pauses playback after 10, 20, 30, or 60 minutes.
- Audio idle/pocket lock: after 30 seconds without interaction, a dark overlay protects against accidental touches.

## How to use

1. Open the app, paste a YouTube video link into **Library**, and tap **Add**.
2. Select a title and tap **Play**. Use **Audio** for listening controls or **Video** to see the player or interact with an ad.
3. Select a library item and use **↑ / ↓** to reorder it, or **Move → New folder** to create a folder. Tap a folder to open it; press and hold a folder to select it for ordering, renaming, or removal.
4. Set playback speed or a sleep timer as needed. When Audio locks, tap to wake, then tap **Unlock controls**.

Keep the page open while listening. The pocket lock protects the app's controls; playback with the phone locked or the browser in the background is not guaranteed.

## Technical and local-data notes

The app is a single client-side HTML/JavaScript page using the official YouTube embedded/IFrame player and browser `localStorage`. No build step or app-specific server is required.

Your library, folders, and playback progress are stored locally in that browser, with no app account or cross-device sync. Clearing the site's browser data removes them; another browser or device has its own library. Video titles and playback still use YouTube's online services, so an internet connection is required.
