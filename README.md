# Device Sensor Diagnostic Tool

A browser-based diagnostic dashboard for testing **device sensors** and **web platform capabilities** in one place.  
Designed to quickly answer questions like:

- “Are my sensors working?”
- “Is my browser actually allowed to use them?”
- “Is HTTPS / permissions / browser support the problem—or my hardware?”

No build step, no dependencies—just open the page and start testing.

---

## 🎯 Purpose

This tool helps you:

- ✅ **Verify sensors**: Check if motion/orientation events are firing at all
- 🧪 **Test APIs**: DeviceOrientation, DeviceMotion, Permissions, secure context, etc.
- 🐛 **Debug issues**: Distinguish between hardware problems, browser blocks, and bad wiring
- 🔍 **Inspect environment**: Browser, platform, HTTPS status, feature support
- 🛠️ **Prototype & learn**: See live data while experimenting with motion-based features

---

## ✨ Features

Depending on your version, the page typically includes:

- **Environment summary**
  - User agent (browser + OS)
  - Secure context status (HTTPS vs HTTP/file)
  - Platform hints (mobile vs desktop)

- **Capability checks**
  - `DeviceOrientationEvent` support
  - `DeviceMotionEvent` support
  - Permissions API support
  - Orientation/lock API presence (if applicable)

- **Live DeviceOrientation view**
  - Alpha / Beta / Gamma values
  - Absolute vs relative flag
  - Event counters and last-update timestamps
  - Clear indication when *no events* are received

- **Live DeviceMotion view** (if supported)
  - Acceleration (with/without gravity)
  - Rotation rates
  - Event counters and timestamps

- **Permission diagnostics**
  - iOS 13+ motion permission request handling
  - Status messages for granted/denied/blocked
  - Helpful hints when permissions or browser settings are the issue

- **Debug logs**
  - Scrollable log with timestamped entries
  - Notes about errors, permission results, and missing APIs

All in a mobile-friendly, single-page UI that you can hit from any phone, tablet, or desktop.

---

## 🚀 Live Demo

Once you enable GitHub Pages, your URL will look like:

```text
https://yourusername.github.io/Device-Sensor-Diagnostic-Tool/
