# Step-by-Step: Get This VR Experience Onto a Meta Quest Headset

## What this package is
This folder contains a starter A-Frame/WebXR experience and the exact files needed to begin testing on a Meta Quest headset through Quest Browser first, then as a packaged install later.

## Files in this folder
- `social-anxiety-vr.html` — the VR experience entry file
- `manifest.webmanifest` — required manifest for future PWA packaging on Meta Quest
- `STEP_BY_STEP_QUEST_DEPLOY.md` — this guide

## Fastest route: Browser first
Meta recommends testing WebXR experiences in Meta Quest Browser before packaging them as PWAs because the packaged version uses the same rendering engine as Browser.[cite:319]

### 1. Put the files online over HTTPS
Use one of these:
- Netlify
- Vercel
- GitHub Pages

A-Frame content should be hosted and published as a normal web experience, and Quest Browser requires a secure HTTPS-hosted WebXR site to enter immersive mode reliably.[cite:334][cite:328]

### 2. Upload this folder
Upload `social-anxiety-vr.html` and `manifest.webmanifest` to the root of your site.

### 3. Open the URL on your Meta Quest
- Put on the headset.
- Open **Meta Quest Browser**.
- Type in the full HTTPS URL.
- Start the experience.

### 4. Validate these basics
- The page loads.
- The Start button appears.
- The scene can enter immersive VR mode.
- Text is readable.
- The branch logic works.

## Official install path: Meta Quest Developer Hub
Meta Quest Developer Hub is Meta's official desktop tool for installing and deploying builds to a headset, logging in with a Meta developer account, and connecting a device over USB.[cite:309][cite:308]

### 1. Enable developer mode
Use the same Meta developer account on the headset and in Meta Quest Developer Hub.[cite:308][cite:309]

### 2. Install MQDH on your Mac or Windows PC
Download and install **Meta Quest Developer Hub** from Meta's developer site, then sign in.[cite:309]

### 3. Connect your headset to your computer
Use a USB-C cable and allow the connection prompts on the headset.

### 4. Package later if needed
For an app-like install, create a Quest-compatible WebXR PWA package. Meta's PWA documentation requires a `manifest.webmanifest` with fields such as `name`, `short_name`, `start_url`, and `scope`.[cite:319]

### 5. Sideload and test
Meta's packaging documentation says a generated package can be installed to Quest for testing with Developer Mode enabled and the device connected to your computer.[cite:331]

## What to ask the developer to do next
This starter file is not your final course. The next production tasks are:
1. Replace the placeholder geometry with actual office environments.
2. Add scene-specific audio and captions.
3. Convert the real course brief into structured JSON scene logic.
4. Add analytics, comfort controls, and final branch logic.
5. Test in Quest Browser before any packaging.

## Recommended sequence
1. Approve the content and flow on desktop.
2. Host online over HTTPS.
3. Test in Meta Quest Browser.
4. Fix readability, comfort, and timing.
5. Package only after browser QA passes.
