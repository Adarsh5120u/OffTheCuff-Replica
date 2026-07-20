# Off the Cuff — Impromptu Speaking Trainer

A self-contained web app for practicing impromptu speaking. Draw a surprise prompt, get a short prep window, then speak — the app transcribes you live, scores your delivery with no sugar coating, graphs how the speech went, and tells you exactly what to fix.

Everything runs in the browser: speech recognition, audio recording, analysis, and history all stay on your device. No server, no accounts. The optional AI coach uses your own Anthropic API key, stored only in your browser.

## Features

Prompt decks (Table Topics, Debate, Storytelling, Professional, Wildcard) with configurable prep and speaking time, live transcription with an accent selector, strict 0–100 scoring across fillers, pace, dead air, duration and vocabulary, a pace/energy timeline graph with pause markers, prioritized areas-for-improvement with drills, audio playback, session history with streaks, and optional Claude-powered coaching.

## Run it locally

Open `index.html` in Chrome or Edge. Allow microphone access when asked.

## Deploy (GitHub Pages)

1. Create a new repository on GitHub and push this folder to it.
2. In the repo: Settings → Pages → under "Build and deployment", set Source to "Deploy from a branch", pick `main` and `/ (root)`, and save.
3. After a minute your app is live at `https://<your-username>.github.io/<repo-name>/`.

Open that URL in Safari on iPhone and use Share → Add to Home Screen for a full-screen app. HTTPS is required for microphone access, which GitHub Pages provides automatically.

## Browser notes

Live transcription uses the Web Speech API: Chrome/Edge on desktop (Google's recognizer) and Safari on iOS 14.5+ (Apple's on-device recognizer — enable Siri dictation). Pick the accent variant closest to yours in setup; it makes the single biggest difference to transcript accuracy.
