<div align="center">
  <img src="docs/icon.png" width="112" alt="Retra" />
  <h1>Retra</h1>
  <p>
    <b>Instant replay for Windows, with every app on its own audio track.</b><br />
    Game on one track, Discord on another, Spotify on a third, your mic on its own: clips ready to edit, in sync.
  </p>
  <p>
    <img src="https://img.shields.io/badge/Windows-0b0b0d?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" />
    <img src="https://img.shields.io/badge/early%20preview-ffb347?style=for-the-badge" alt="Early preview" />
    <a href="https://github.com/Fialsss/retra-releases/releases/latest"><img src="https://img.shields.io/github/v/release/Fialsss/retra-releases?style=for-the-badge&label=download&color=3ddc97" alt="Download" /></a>
    <a href="https://ko-fi.com/fialss"><img src="https://img.shields.io/badge/Ko--fi-support-ff5e5b?style=for-the-badge&logo=kofi&logoColor=white" alt="Support on Ko-fi" /></a>
  </p>
  <img src="docs/capture.png" width="860" alt="Retra: the Capture page, one channel per track" />
</div>

> [!WARNING]
> Retra is an early preview: expect rough edges. This repository holds only the builds and the updates; the source
> code is not public.

## What it does

- **Instant replay**: the last 5 s to 20 min are always kept, and one hotkey saves them (`Alt+F10`). Turn desktop
  capture off and the buffer runs only while a game is open.
- **Smooth clips at 60 or 120 fps**, following your screen: 120 on a 120 Hz+ display, 60 on a 60 Hz one.
- **Every display at once** if you like, each recording on its own; a save takes the one your mouse is on.
- **1 to 12 audio tracks**, each holding any mix of apps: drag them on, name them, pick their icon. Every clip has
  one named audio stream per track, ready for Premiere, DaVinci Resolve or any editor, and tracks that stayed
  silent aren't in the file at all. The Desktop track holds everything, what your PC plays and your mic, for when
  you just want it all in one.
- **Your microphone, cleaned up live**: noise suppression, gate, EQ, compressor and your own VST3 plugins, already
  in the replay.
- **Quick panel over the game** (`Alt+X`): gallery, record, replay, screenshot, per-track volume and every setting.
- **Clips**: every video in your Videos folder, ShadowPlay's and OBS's too, browsed by folder. Play them with all
  the tracks in sync (Desktop or the separate tracks, never both, so nothing plays twice), turn each track down,
  trim them in several pieces, drop tracks, delete several at once.
- **Hardware encoding** on NVIDIA, AMD or Intel GPUs, in H.264, HEVC or AV1; MP4 or MKV.
- Clips go in a folder per game, named after the game you're playing.
- Updates itself, or checks right away from Settings.

## A look around

<table>
  <tr>
    <td width="50%"><img src="docs/capture-rows.png" alt="Tracks in rows" /></td>
    <td width="50%"><img src="docs/clips.png" alt="Clips" /></td>
  </tr>
  <tr>
    <td><b>Tracks in rows</b>, or as a mixing desk: meters, fader in dB, mute, and the apps on each track.</td>
    <td><b>Clips</b>: your Videos folder by folder, a folder per game, with how much space each takes.</td>
  </tr>
  <tr>
    <td><img src="docs/settings.png" alt="Settings" /></td>
    <td><img src="docs/setup.png" alt="The installer" /></td>
  </tr>
  <tr>
    <td><b>Settings</b> at a glance: every card shows what it holds, the switches work from there.</td>
    <td><b>The installer</b>: pick the folder, and that's it.</td>
  </tr>
</table>

<p align="center">
  <img src="docs/panel.png" width="300" alt="Quick panel" /><br />
  <b>Quick panel</b> over the game, <code>Alt+X</code>.
</p>

## Download

Grab **`Retra-x.y.z-Setup.exe`** from **[Releases](https://github.com/Fialsss/retra-releases/releases/latest)**:
choose where to install it, and Retra is in your Start menu (and on your desktop, if you want).

It updates itself: when a new version is out, a green button shows up at the top right of the window, or
**Settings › App › Check now** looks right away. Windows 10/11 64-bit, with an NVIDIA, AMD or Intel GPU.

Had the portable (0.1.32 or before)? From 0.1.33 there's only the installer: install it once, your settings and
clips carry over.

The builds are not code-signed yet, so Windows SmartScreen may show *"Windows protected your PC"* the first time.
Click **More info → Run anyway**.

## Support

Retra is made by one person in their spare time. If it saves your clips, you can
**[buy me a coffee on Ko-fi](https://ko-fi.com/fialss)**.

## Third-party

Retra ships FFmpeg (the LGPL 2.1 build by BtbN) as a separate, unmodified program, and includes RNNoise, the VST 3 SDK and the WebView2 SDK loader. See [THIRD_PARTY.md](THIRD_PARTY.md).
