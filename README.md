# Geminiman WearOS Battery Stats

A lightweight, battery-friendly battery monitoring and history app for Wear OS, with a companion Android phone app.

Track how your watch battery behaves throughout the day or across an entire charge cycle, understand app activity, inspect battery trends, and identify events that may have affected background monitoring.

> Currently available as an **Open Beta**.

---

## ✨ Features

### 🔋 Battery Monitoring

- Current battery percentage and charging state
- Estimated remaining battery time
- Battery health information
- Lightweight background monitoring
- Reliable phone ↔ watch synchronization
- Automatic monitoring recovery after app/process restarts

### 📅 Daily History

View battery activity for each calendar day, including:

- Battery drain
- Charging sessions
- Average drain rate
- Estimated active app time
- App activity rankings
- Battery trend chart

### 🔄 Charge Cycle History

See how long your watch actually lasts from one full charge to the next.

A charge cycle:

- Starts after disconnecting from 100%
- Continues through partial top-ups
- Ends when the watch reaches 100% again
- Can span multiple days
- Supports completed and ongoing cycles

Example:

`31 Dec 26–2 Jan 27`

or:

`5 Aug 26–Ongoing`

### 📊 Interactive Battery Charts

Battery history charts support:

- Expanded chart viewer
- Pinch-to-zoom
- Horizontal panning
- Detailed battery points
- Date and time markers
- Multi-day charge-cycle charts
- Day boundary indicators
- Adaptive time intervals

### 📱 App Activity

See which watch apps were active during the selected period.

- Raw sub-minute activity tracking
- App names and icons
- Package-name fallback when metadata is unavailable
- Daily and charge-cycle rankings
- Improved handling when apps appear or disappear between snapshots

> App activity percentages are estimates based on measured activity and are not exact per-app battery drain measurements.

---

## 🛡 Monitoring Diagnostics

Battery Stats can optionally record events that may explain gaps or changes in monitoring.

### Watch Connection

Records:

- Watch disconnected
- Reconnected nearby
- Connected over network
- Connection route changes

### Battery Saver

Records when Battery Saver is detected as:

- Enabled
- Disabled

When both boundaries are known, the affected period can be highlighted on the battery chart.

If only one boundary is detected, only that event is shown — no missing interval is guessed.

### Background Restrictions

The app can record when background monitoring appears restricted or becomes available again.

These diagnostic options can be individually enabled or disabled from the watch.

---

## 📈 Monitoring Transparency

Battery Stats also reports its own monitoring activity separately from normal app rankings.

Information can include:

- Active monitoring time
- Last snapshot sent
- Monitoring activity percentage
- Estimated monitoring impact

Example:

`Monitoring activity: 0.4% · Very low`

This represents the app's monitoring activity relative to the tracking period. It is **not an exact battery consumption percentage**.

---

## ⌚ Wear OS Features

The watch app also includes:

- Battery information directly on the watch
- Top app activity
- Monitoring settings
- Battery monitoring status
- Tiles
- Battery complication
- Language selection
- About information

---

## 🌍 Languages

Geminiman WearOS Battery Stats currently supports **18 languages**, including Hungarian.

The phone and watch can use different languages independently.

---

## 🔐 Privacy

Battery Stats is designed around local battery monitoring.

Installed application information is used to identify apps appearing in watch usage reports and display their names and icons.

The app does not use installed-app information for advertising.

---

## ⚡ Battery Friendly

The application is designed to keep its own monitoring overhead low.

It avoids:

- Continuous polling
- Permanent foreground services
- Wake locks for monitoring
- Forced network connections

Background monitoring primarily uses scheduled work and system/Wear OS events.

Android Battery Saver, background restrictions, Force Stop, device-specific power management, and connectivity can still delay monitoring.

---

## 🧪 Open Beta

The application is currently being tested through an Open Beta.

During beta testing, battery calculations, charge-cycle detection, device compatibility, and background reliability are being observed across different Wear OS devices.

Feedback is very welcome.

---

## 🐛 Found a Bug?

Please open a GitHub Issue and include, when possible:

- Phone model
- Watch model
- Android version
- Wear OS version
- App version
- What you expected to happen
- What actually happened
- Screenshots or logs if relevant
- Steps to reproduce the problem

Please avoid including personal or sensitive information in reports.

---

## ❤️ Support My Projects

I build these projects as a hobby and because I genuinely enjoy creating useful tools for the community.

My vision has always been simple: **no ads, no paywalls, and no features locked behind a purchase**. If a feature is part of the app, I want everyone to be able to use it.

If you enjoy my work and would like to support what I do, you can:

- ❤️ [Support me through PayPal](https://www.PayPal.me/Dante63)
- 🎗️ [Support me on Patreon](https://www.patreon.com/c/xda_dante63/membership)
- ⭐ Star my projects on GitHub
- ★ Leave a review for the apps you enjoy
- 🐛 Report bugs and issues
- 💡 Share suggestions and ideas
- 📢 Recommend the projects to others who may find them useful

Your support and feedback help keep development going and improve the projects for everyone, and they always motivate me to keep creating, giving back, and doing more for the community.

---

## Disclaimer

Battery estimates and app activity calculations are informational.

Values may differ from manufacturer battery statistics because Android and Wear OS do not expose exact per-app battery consumption data to third-party applications.
