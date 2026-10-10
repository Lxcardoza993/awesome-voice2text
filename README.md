# Awesome Voice2Text

> A curated list of open-source voice input / dictation software — fully open, extensible, and lightweight. Benchmarked against Typeless, Lazytype, and Shandianshuo (闪电说), all of which are closed-source.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*If this list is useful, please ⭐ the repo — it helps others find it.*

**Languages**: [English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Contents

- [Benchmarks (Closed-Source)](#benchmarks-closed-source)
- [Why this list](#why-this-list)
- [Inclusion criteria](#inclusion-criteria)
- [Top Picks](#top-picks)
- [All Projects](#all-projects)
- [Categorized List](#categorized-list)
  - [Cross-Platform Desktop Real-Time Dictation](#cross-platform-desktop-real-time-dictation)
  - [Native macOS Dictation](#native-macos-dictation)
  - [AI Speech Cleanup / LLM Post-Processing](#ai-speech-cleanup-llm-post-processing)
  - [Local/Offline STT Engines and Toolkits](#localoffline-stt-engines-and-toolkits)
  - [System-Level Voice Input / IME](#system-level-voice-input-ime)
  - [Chinese Speech Input / IME](#chinese-speech-input-ime)
  - [Browser & Web Voice Input](#browser-web-voice-input)
  - [Mobile Voice Input (Non-IME)](#mobile-voice-input-non-ime)
  - [Lightweight Scripts, CLI & Voice Control](#lightweight-scripts-cli-voice-control)
  - [Other](#other)
- [Open-source vs. Benchmarks](#open-source-vs-benchmarks)
- [How to Choose](#how-to-choose)
- [Contributing 贡献](#contributing-贡献)
- [Star History](#star-history)
- [License](#license)

## Benchmarks (Closed-Source)

| Product | Pricing | Platforms | Model/Engine | Open Source |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Why this list

Typeless, Lazytype, and Shandianshuo (闪电说) are powerful but closed-source. This list collects open-source alternatives that meet three criteria: the code is fully public, the tool can be extended, and it stays light enough to run on a personal machine. It currently covers **75 projects across 9 categories**, all verified to be fully open source.

## Inclusion criteria

- ✅ **Fully open source** — all code on a public forge (GitHub, GitLab, Codeberg).
- 🔌 **Extensible** — you can add the features, models, or integrations you want.
- ⚡ **Lightweight** — minimal bloat, fast startup, small footprint.

## Top Picks

🏆 **[Handy](https://github.com/cjpais/Handy)** — Cross-platform offline voice-to-text tool using Whisper or Parakeet, with global hotkeys and clipboard paste. *Community flagship — 25,281 stars, the most polished offering.*

**Fit-5 picks** (meet all three criteria):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — High-performance C/C++ port of OpenAI Whisper with CPU/GPU inference, quantization and cross-platform support.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linux offline speech-to-text tool using Vosk that simulates keyboard input into any application.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux and Wayland push-to-talk voice-to-text with seven local ASR engines, GPU support, and meeting mode.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash script for offline voice typing via Whisper for TTY, X11, Wayland, and WSL with optional LLM editing.

## All Projects

| Name | ⭐ Stars | License | Language | Fit | Open | Ext | LW | Chinese |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 51,163 | MIT | C/C++, CMake, Python/Java/C# bindings | 5 | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | 1,882 | GPL-3.0 | Python | 5 | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | 909 | MIT | Rust | 5 | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | 155 | GPL-2.0 | Bash | 5 | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | 25,281 | MIT | Rust, Tauri, React, TypeScript, Tailwind | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | 19,906 | MIT | Python, PyQt6, Whisper, PyTorch, ONNX Runtime | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [FunASR](https://github.com/modelscope/FunASR) | 18,745 | MIT | Python (PyTorch) | 4 | ⚠️ | ✅ | ⚠️ | ✅ |
| [vosk-api](https://github.com/alphacep/vosk-api) | 14,889 | Apache-2.0 | C++ with Python, Java, C#, Node.js, Rust, Go | 4 | ⚠️ | ✅ | ✅ | ✅ |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | 13,280 | Apache-2.0 | C++, Python, Go, Java, Rust, C#, Swift, JS, Dart | 4 | ✅ | ✅ | ⚠️ | ✅ |
| [Vibe](https://github.com/thewh1teagle/vibe) | 6,635 | MIT | Rust, Tauri, TypeScript, React, whisper.cpp | 4 | ✅ | ✅ | ✅ | ✅ |
| [Epicenter](https://github.com/EpicenterHQ/epicenter) | 4,663 | MIT + AGPL-3.0-or-later | — | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) | 2,821 | Apache-2.0 | Python, PyTorch, Gradio, FFmpeg | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) | 1,541 | GPL-3.0 | Swift | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) | 1,474 | MIT | Swift, Shell, CMake, C, Ruby | 4 | ✅ | ⚠️ | ⚠️ | ✅ |
| [Amical](https://github.com/amicalhq/amical) | 1,388 | MIT | TypeScript, Electron, Next.js, React | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr) | 1,074 | MIT | Python, C/C++, GTK4, Astro | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [whisper-writer](https://github.com/savbell/whisper-writer) | 1,071 | GPL-3.0 | Python | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Transcribro](https://github.com/soupslurpr/Transcribro) | 723 | ISC | Kotlin, Android, C++, Jetpack Compose | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [Whisper IME](https://github.com/woheller69/whisperIME) | 603 | MIT | Java, Android, TensorFlow Lite | 4 | ✅ | ✅ | ✅ | ◐ |
| [Vocalinux](https://github.com/jatinkrmalik/vocalinux) | 404 | GPL-3.0 | Python, GTK, whisper.cpp, VOSK | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [VoiceTypr](https://github.com/moinulmoin/voicetypr) | 389 | AGPL-3.0 | Rust, Tauri, TypeScript, React, Vite, Whisper | 4 | ✅ | ✅ | ✅ | ◐ |
| [HoldSpeak](https://github.com/karolswdev/HoldSpeak) | 277 | Apache-2.0 | Python, FastAPI, Astro, Swift, SQLite | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Chirp](https://github.com/Whamp/chirp-stt) | 191 | MIT | Python | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) | 163 | GPL-3.0 | Python, C++, Shell | 4 | ✅ | ✅ | ✅ | ✅ |
| [Dabri](https://github.com/AshBuk/dabri) | 110 | MIT | Go, whisper.cpp (CGO), YAML | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [hns](https://github.com/primaprashant/hns) | 107 | MIT | Python 3.10+ | 4 | ✅ | ✅ | ✅ | ◐ |
| [Elograf](https://github.com/papoteur-mga/elograf) | 82 | GPL-3.0 | Python 3.7+, PyQt6, Vosk, ujson | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) | 1 | MIT | Swift | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [Voicisst](https://github.com/lucyfromnaarm/voicisst) | 0 | MIT | Python | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Cadenza](https://github.com/DragonKingIO/Cadenza-voice) | 3 | MIT | Swift | 4 | ✅ | ✅ | ✅ | ✅ |
| [dsnote (Speech Note)](https://github.com/mkiol/dsnote) | 1,525 | MPL-2.0 | C++17, Qt5/QML, CMake, Python | 3.5 | ✅ | ⚠️ | ⚠️ | ✅ || [VoiceFlow](https://github.com/infiniV/VoiceFlow) | 393 | MIT | Python, React, Vite, faster-whisper | 3.5 | ✅ | ⚠️ | ✅ | ◐ |
| [voice-input-method](https://github.com/pofice/voice-input-method) | 38 | GPL-3.0-or-later | Python 3.10+ | 3.5 | ✅ | ✅ | ✅ | ✅ |
| [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) | 0 | MIT | JavaScript (Manifest V3), Python | 3.5 | ⚠️ | ✅ | ✅ | ⚠️ |
| [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) | 12,636 | Apache-2.0 | Python, C++ | 3 | ✅ | ✅ | ⚠️ | ✅ |
| [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) | 8,731 | MIT | Python, C/C++ | 3 | ⚠️ | ✅ | ✅ | ✅ |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) | 5,387 | GPL-3.0 | Swift, whisper.cpp | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) | 5,013 | GPL-3.0 | Swift | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) | 4,143 | MIT | TypeScript, React, Electron, Vite, Tailwind CSS | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [Ghost Pepper](https://github.com/matthartman/ghost-pepper) | 2,800 | MIT | Swift | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [WhisperBoard](https://github.com/Saik0s/Whisperboard) | 1,040 | GPL-3.0 | Swift, SwiftUI, TCA, whisper.cpp, Tuist | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [Voquill](https://github.com/voquill/voquill) | 977 | AGPL-3.0 | TypeScript, Rust, React, Vite | 3 | ⚠️ | ✅ | ⚠️ | ⚠️ |
| [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) | 695 | Apache-2.0 | Kotlin, Android SDK 36, Compose | 3 | ⚠️ | ✅ | ⚠️ | ✅ |
| [Pindrop](https://github.com/watzon/pindrop) | 546 | MIT | Swift, SwiftUI, WhisperKit, SwiftData, Sparkle | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [vosk-browser](https://github.com/ccoreilly/vosk-browser) | 520 | Apache-2.0 | TypeScript, JavaScript, WebAssembly | 3 | ✅ | ✅ | ✅ | ◐ |
| [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) | 366 | AGPL-3.0 | Rust, TypeScript, React, Python | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [OpenTypeless](https://github.com/tover0314-w/opentypeless) | 308 | MIT | TypeScript, Rust, React, Tauri | 3 | ✅ | ⚠️ | ✅ | ✅ |
| [voxd](https://github.com/jakovius/voxd) | 266 | MIT | Python | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [whisper-dictation](https://github.com/foges/whisper-dictation) | 219 | MIT | Python | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [Speed of Sound](https://github.com/zugaldia/speedofsound) | 171 | MIT | Kotlin, JVM, GTK, Sherpa ONNX | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [blurt](https://github.com/QuantiusBenignus/blurt) | 107 | GPL-3.0 | JavaScript, Shell, CSS | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) | 77 | MIT | Python 3.10-3.12, tkinter, LiteLLM | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [Aria](https://github.com/Xingxun7777/Aria) | 71 | Apache-2.0 | Python 3.12, PyTorch, CUDA, PySide6 | 3 | ✅ | ✅ | ⚠️ | ✅ |
| [Vosk Android Service](https://github.com/alphacep/vosk-android-service) | 64 | Apache-2.0 | Java, Android SDK, Gradle, Vosk, JNA, RxJava2 | 3 | ✅ | ✅ | ✅ | ◐ |
| [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) | 59 | MIT | Python, PyTorch, customtkinter | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [TalkType](https://github.com/lmacan1/talktype) | 54 | MIT | Python | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [FnKey](https://github.com/evoleinik/fnkey) | 45 | GPL-3.0 | Rust | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) | 29 | MIT | Python, faster-whisper, CTranslate2, pyaudio | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [Speechfire](https://github.com/Jejkobb/Speechfire) | 27 | None | JavaScript, Python | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
| [Osprey](https://github.com/osprey-voice/osprey) | 26 | MIT | Python | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [whisper-dictation](https://github.com/jacopone/whisper-dictation) | 18 | MIT | Python, Nix | 3 | ✅ | ✅ | ✅ | — |
| [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) | 15 | MIT | Electron, React, TypeScript | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) | 13 | MIT | JavaScript (React) | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [Dictus](https://github.com/getdictus/dictus-ios) | 12 | MIT | Swift, SwiftUI, WhisperKit, CoreML | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) | 11 | MIT | Python | 3 | ⚠️ | ✅ | ⚠️ | ⚠️ |
| [hush](https://github.com/djmunro/hush) | 6 | MIT | Rust | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [freespeak](https://github.com/Zetaphor/freespeak) | 6 | MIT | Python, PyQt6, JavaScript, HTML, CSS | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [WhisperDictation](https://github.com/sam-pop/WhisperDictation) | 1 | MIT | Swift, C/C++ | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [voico](https://github.com/Kirera-Wainaina/voico) | 1 | MIT | TypeScript, JavaScript, Node.js, Chrome MV3 | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [localflow](https://github.com/sidharth-n/localflow) | 0 | Apache-2.0 | Python | 3 | ⚠️ | ✅ | ✅ | ◐ |
| [yammer](https://github.com/andynu/yammer) | 0 | MIT | Rust, Tauri, TypeScript, Node.js | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [whisper_dictation](https://github.com/themanyone/whisper_dictation) | 291 | GPL-2.0 | Python, C/C++, GStreamer | 2 | ✅ | ✅ | ⚠️ | ◐ |
| [OmniDictate](https://github.com/gurjar1/OmniDictate) | 141 | CC BY-NC 4.0 | Python, PySide6, faster-whisper | 2 | ⚠️ | ⚠️ | ⚠️ | ◐ |
| [seamless](https://github.com/woheller69/seamless) | 84 | MIT | Java, Kotlin, Android | 2 | ⚠️ | ⚠️ | ⚠️ | ⚠️ |
| [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) | 25 | MIT | Python | 2 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) | 9 | GPL-3.0 | Python | 2 | ✅ | ⚠️ | ⚠️ | ◐ |

## Categorized List

### Cross-Platform Desktop Real-Time Dictation

Whisper-based desktop dictation apps for Linux, Windows, or cross-platform, with push-to-talk, local transcription, and auto-input.

- [Handy](https://github.com/cjpais/Handy) — Cross-platform offline voice-to-text tool using Whisper or Parakeet, with global hotkeys and clipboard paste.
- [Buzz](https://github.com/chidiwilliams/buzz) — Cross-platform desktop GUI for offline Whisper transcription and translation with GPU acceleration, live mic.
- [Vibe](https://github.com/thewh1teagle/vibe) — Cross-platform desktop app for offline audio and video transcription using Whisper, with GPU acceleration.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Local-first app toolkit with Markdown/SQLite storage, Yjs CRDT sync, and a desktop speech-to-text utility.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux-native speech-to-text with local Whisper and ONNX models, cloud APIs, Waybar integration, visualizer.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Desktop dictation app using Whisper locally or via API, triggered by global hotkey to type into active window.
- [Chirp](https://github.com/Whamp/chirp-stt) — Windows CPU-only dictation app using ParakeetV3, with hotkey toggle, clipboard paste, and word overrides.
- [Dabri](https://github.com/AshBuk/dabri) — Linux offline STT app using whisper.cpp with daemon, CLI, and WebSocket modes for X11/Wayland desktops.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux and Sailfish OS offline note-taking app with local STT, TTS, and translation using multiple engines.
- [voxd](https://github.com/jakovius/voxd) — Linux desktop voice dictation using whisper.cpp for offline ASR with ydotool typing and AI post-processing.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linux offline voice typing via Whisper, Parakeet, or Canary ONNX, with X11/Wayland support and LLM polish.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windows voice-typing assistant using Caps Lock hotkey, with multi-provider STT and optional LLM refinement.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Cross-platform offline dictation app with distil-whisper, hotkey control, and optional local LLM assistant.
- [TalkType](https://github.com/lmacan1/talktype) — Cross-platform push-to-talk voice typing using faster-whisper, with global hotkeys and smart paste.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Offline multilingual dictation app using Faster-Whisper, triggered by hotkey to transcribe into active field.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — NixOS/Wayland local voice dictation using whisper.cpp with GTK4 feedback and 99-language support.
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux Wayland voice dictation app with STT, grammar correction via LanguageTool, and ydotool text input.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Local AI desktop agent combining voice dictation, LLM chat, image generation, and voice-driven automation.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows desktop speech-to-text using faster-whisper with keyboard simulation, VAD, PTT, and punctuation.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Whisper voice dictation for KDE Wayland with background daemon, systemd service, and clipboard paste.

### Native macOS Dictation

Native macOS dictation apps built with Swift and WhisperKit, supporting global hotkeys, menu bar, and Neural Engine acceleration.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — A macOS speech transcription app with Whisper and Parakeet engines, global hotkeys, and batch processing.
- [Pindrop](https://github.com/watzon/pindrop) — Native macOS menu-bar dictation app using WhisperKit for offline STT, with hotkeys and optional AI cleanup.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Offline multilingual dictation tool using Whisper, triggered by hotkey to transcribe into any input field.
- [FnKey](https://github.com/evoleinik/fnkey) — A macOS menu-bar app that transcribes speech via Deepgram Nova-3 while Fn is held and pastes the result.
- [hush](https://github.com/djmunro/hush) — A macOS push-to-talk dictation app using local Whisper/Parakeet ONNX with auto-paste via hotkey.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — A macOS menu-bar dictation app using offline Whisper with Metal GPU acceleration and cursor text injection.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS menu-bar app records on Globe/Fn release, transcribes via faster-whisper, and pastes at cursor.
- [Cadenza](https://github.com/DragonKingIO/Cadenza-voice) — Local-first macOS voice input: hold a hotkey, speak, text appears at cursor; SenseVoice/Parakeet on-device.

### AI Speech Cleanup / LLM Post-Processing

Dictation tools using local or cloud LLMs to polish, format, summarize, and restyle speech recognition output into clean, formal text.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — A macOS dictation app with on-device and cloud STT, global hotkeys, AI workflows, plugins, REST API, and CLI.
- [Amical](https://github.com/amicalhq/amical) — Local-first AI dictation app using Whisper for offline transcription and Ollama for smart note processing.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Offline voice dictation tool for macOS/Windows using Whisper, with global hotkeys and optional AI enhancement.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Local-first voice assistant for macOS and Linux with push-to-talk, transcription, and plugin extraction.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — A macOS push-to-talk dictation app using Whisper and LLM cleanup, pasting polished text via Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Local voice dictation with Whisper and LLM polishing, push-to-talk, dictionary, and client-server split.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Local voice dictation and meeting recorder with faster-whisper, LLM summaries, and dual-track audio capture.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Native macOS voice-to-text app using local whisper.cpp models, with global shortcuts and context-aware modes.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — A macOS dictation app with on-device speech recognition and optional AI post-processing for formatting.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Desktop voice transcription app with hotkeys, AI assistant, meeting diarization, and semantic search.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — A macOS menu-bar app for offline speech-to-text and meeting summaries using Whisper and Qwen on Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Cross-platform Tauri voice typing app with local Whisper or Groq, AI cleanup, glossary, and voice assistant.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Cross-platform voice dictation assistant with LLM formatting, supporting local Whisper, Ollama or cloud APIs.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Cross-platform Tauri app for AI voice typing, text rewriting, and voice Q&A with global hotkeys.
- [Aria](https://github.com/Xingxun7777/Aria) — Windows AI voice input using offline Qwen3-ASR with OCR context, hot word correction, and voice commands.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windows voice dictation using whisper.cpp, Groq or llama.cpp, multiple styles, auto-paste to active window.
- [localflow](https://github.com/sidharth-n/localflow) — Local cross-platform voice dictation using Moonshine STT, Qwen3-4B polisher, push-to-talk, and skip-gate.
- [yammer](https://github.com/andynu/yammer) — Linux local speech-to-text with Whisper and LLM cleanup, plus Tauri overlay UI and xdotool input injection.

### Local/Offline STT Engines and Toolkits

Offline ASR engines and speech toolkits for app integration: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech, and SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — High-performance C/C++ port of OpenAI Whisper with CPU/GPU inference, quantization and cross-platform support.
- [FunASR](https://github.com/modelscope/FunASR) — Industrial ASR toolkit with Paraformer, SenseVoice, VAD, diarization, streaming, and OpenAI-compatible API.
- [vosk-api](https://github.com/alphacep/vosk-api) — Offline speech recognition toolkit with small CPU-only models for 20+ languages and multi-language bindings.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Offline speech toolkit using next-gen Kaldi and ONNX Runtime for STT, TTS, speaker ID, VAD, and more.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Comprehensive speech toolkit with ASR, TTS, voiceprint, diarization, translation, and streaming services.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Speech model with ASR for 50+ languages, emotion, audio events, and fast non-autoregressive inference.

### System-Level Voice Input / IME

Voice input solutions integrated at the system level, including input methods, IBus/Fcitx extensions, Android IME, and iOS keyboards.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME and voice input service using Whisper for offline speech recognition and English translation.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Offline Linux voice dictation app with whisper.cpp, Whisper, and VOSK engines, Vulkan GPU, and GTK GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — GNOME Shell extension for offline voice input via whisper.cpp with hotkey trigger, supporting X11 and Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Android offline speech recognition service using Vosk with standard RecognitionService API support.
- [Dictus](https://github.com/getdictus/dictus-ios) — Open-source iOS keyboard for on-device voice dictation using WhisperKit and CoreML, works in any app.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linux IBus speech-to-text input method with streaming STT, optional Whisper refinement, and GPU acceleration.

### Chinese Speech Input / IME

Projects optimized for Chinese speech recognition and input, including FunASR, Paraformer, and SenseVoice-based Chinese IMEs and keyboards.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Offline Linux Chinese voice input using FunASR Paraformer, IBus/Fcitx5, PTT hotkey, and sentence polishing.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Cross-platform offline voice input method using FunASR, with hotword correction, auto-paste and GUI/CLI modes.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android voice input keyboard with 11 ASR engines, LLM post-processing, floating ball, and Material3 UI.

### Browser & Web Voice Input

Browser-based voice input via extensions, WebAssembly wrappers, or Web UIs, typically requiring a local or cloud STT backend.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI for subtitles from files, YouTube, or mic, with VAD, BGM separation, and diarization.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Browser extension for real-time offline speech-to-text via Vosk, with Arabic and English voice commands.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Browser-based offline speech recognition library packaging Vosk as WebAssembly running in a WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Browser extension and local Whisper server for offline speech-to-text in Firefox and Chrome via Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Chrome extension that records voice via hotkey, transcribes with OpenAI Whisper API, and auto-pastes text.
- [voico](https://github.com/Kirera-Wainaina/voico) — Chrome extension for voice-to-text input into web fields, with a Node.js backend using Google and OpenAI STT.

### Mobile Voice Input (Non-IME)

Standalone voice transcription apps on Android or iOS, rather than input method keyboards.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Private on-device speech recognition keyboard for Android using Whisper via whisper.cpp and Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Open-source iOS app for offline voice transcription using Whisper.cpp, with recording and audio export.
- [seamless](https://github.com/woheller69/seamless) — Android offline speech-to-text translation app using Meta Seamless M4T Lite for 5 languages with TTS output.

### Lightweight Scripts, CLI & Voice Control

Lightweight scripts, CLI tools, tray triggers, or utilities suited for developer integration or as supplements to existing toolchains.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linux offline speech-to-text tool using Vosk that simulates keyboard input into any application.
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash script for offline voice typing via Whisper for TTY, X11, Wayland, and WSL with optional LLM editing.
- [hns](https://github.com/primaprashant/hns) — CLI tool for local microphone speech-to-text using faster-whisper, with clipboard copy and stdout piping.
- [Elograf](https://github.com/papoteur-mga/elograf) — PyQt6 GUI manager for nerd-dictation with system tray, Vosk models, input simulation, and KDE hotkeys.
- [Osprey](https://github.com/osprey-voice/osprey) — Command-based voice control and typing tool using Kaldi and Dragonfly for fully local speech recognition.

### Other

Projects not yet assigned to a category.

- [VoxType](https://github.com/peteonrails/voxtype) — Linux and Wayland push-to-talk voice-to-text with seven local ASR engines, GPU support, and meeting mode.

## Open-source vs. Benchmarks

| Project | Price | Open Source | Extensible | Offline | Chinese |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Free (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Free (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## How to Choose

- **Polished cross-platform desktop app** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 stars, Whisper/Parakeet offline.
- **Minimal Linux offline, scriptable** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simulates keyboard input into any app.
- **Embed STT in your own app** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, embeddable.
- **Chinese-first input** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; Offline Linux Chinese voice input using FunASR Paraformer, IBus/Fcitx5, PTT hotkey, and sentence polishing.
- **Self-host a transcription API/server** → [FunASR](https://github.com/modelscope/FunASR) — Industrial ASR toolkit with Paraformer, SenseVoice, VAD, diarization, streaming, and OpenAI-compatible API.

## Contributing 贡献

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md). Projects must be fully open source, extensible, and lightweight; please follow the description style guide (English, one line, factual, no marketing fluff).

欢迎投稿——请参阅 [CONTRIBUTING.md](CONTRIBUTING.md)。项目必须完全开源、可扩展、轻量级；请遵循描述风格指南（英文、一行、实事求是、无营销花哨）。

## Star History

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Star growth over time for the most-starred projects in this list, including this repository.

## License

[MIT](LICENSE).
