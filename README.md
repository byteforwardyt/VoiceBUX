# VoiceBUX

Free local speech studio for Apple Silicon Macs. VoiceBUX is a fork of [Voicebox](https://github.com/jamiepine/voicebox) with extra engines and a side-by-side compare tool.

<p align="center">
  <a href="https://github.com/byteforwardyt/VoiceBUX/releases/download/v0.0.3/VoiceBUX-0.0.3-macOS-arm64.dmg">
    <img alt="Download VoiceBUX for Mac" src="https://img.shields.io/badge/Download-VoiceBUX%20for%20Mac-111111?style=for-the-badge&logo=apple&logoColor=white">
  </a>
</p>

The button downloads the compiled Mac app. It is free. No account is required.

## Download

This build is for Apple Silicon only, on macOS 11 or later. It will not run on an Intel Mac.

The file is signed with Developer ID Application: Leo Torres (NU9KNGPZDQ) and notarized by Apple, so Gatekeeper can open it.

- Version: 0.0.3
- File: VoiceBUX-0.0.3-macOS-arm64.dmg (592 MB)
- Direct link: https://github.com/byteforwardyt/VoiceBUX/releases/download/v0.0.3/VoiceBUX-0.0.3-macOS-arm64.dmg
- SHA-256: `5d6d2d11dfecc421b945ade27ef544626cc1235872551129fd76ce4430950f42`

1. Click the download button.
2. Open the disk image.
3. Drag Voicebux into Applications.
4. Open Voicebux from Applications.

macOS may ask once to confirm an app downloaded from the internet. That prompt is normal.

Speech models are not inside this download. The first time you use an engine, VoiceBUX downloads that model onto your Mac. Large models, especially MOSS, need a lot of disk space and memory.

Your voices and history stay on this Mac, in `~/Library/Application Support/local.voicebux.desktop`.

## What it does

Open Voicebux, pick a voice and an engine, type a script, and generate speech. You can clone a voice from your own recording, narrate a longer script as separate takes, transcribe audio, and export the result.

Compare plays the same script and reference voice across engines. You can listen before the engine names are shown. The original recording is kept. The listening copies are matched for loudness only: no compression, pitch change, or profile effects.

## What changed from Voicebox

VoiceBUX started from Voicebox and added engines the original build did not have:

| | Voicebox | VoiceBUX 0.0.3 |
| --- | --- | --- |
| Qwen TTS | Yes | Yes, 0.6B and 1.7B |
| Qwen CustomVoice | Yes | Yes, 0.6B and 1.7B |
| LuxTTS | Yes | Yes |
| Chatterbox and Chatterbox Turbo | Yes | Yes |
| TADA | Yes | Yes, 1B and 3B multilingual |
| Kokoro | Yes | Yes |
| VoxCPM2 | No | Yes, 48 kHz |
| MOSS-TTS v1.5 8B | No | Yes, 31 languages |
| MOSS Voice Acting v1.5 8B | No | Yes |
| Side-by-side compare | No | Yes |
| Qwen VoiceDesign | Yes, in the current original | Not in this build |
| OmniVoice | Yes, in the current original | Not in this build |

The current original project is [jamiepine/voicebox](https://github.com/jamiepine/voicebox). It has moved on since this fork. VoiceBUX does not include Qwen VoiceDesign or OmniVoice. Those two are in today's Voicebox, not in this download.

Compare in VoiceBUX can render one line on Qwen3-TTS 1.7B, VoxCPM2, MOSS-TTS, and MOSS Voice Acting, then reveal which engine made each take.

## License

MIT. VoiceBUX is free to download and use. The original Voicebox copyright is in [LICENSE](LICENSE). Model and third-party licenses still apply to the engines you download. Do not clone a person's voice without their permission.
