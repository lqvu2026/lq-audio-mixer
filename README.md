# LQ Audio Mixer

A simple web app that puts your voice, or a voice made from your text, over background music. Everything runs in the browser: no uploads, no account.

## Features

- **Background music:** MP3, M4A, WAV, OGG. Volume, fade in, fade out.
- **Voice, three ways:**
  - **Record:** use the microphone. Optionally play the music in your headphones while you record.
  - **Upload:** use an existing voice recording.
  - **Type text:** a voice from your device reads your text. Preview only (see Limitations).
- **Mix settings:** voice volume, start time of the voice, and an option to lower the music while the voice speaks.
- **Preview** the mix, then **save** it as MP3 or WAV. Download or Share.

## Files

- `index.html`: the whole app
- `lq-audio-mixer-icon.png`: 180x180 icon used for the iPhone Home Screen

## Publish on GitHub Pages

1. Put `index.html` and `lq-audio-mixer-icon.png` in the repository root.
2. Commit both files.
3. In the repository, open Settings, then Pages, and publish from the main branch.
4. Wait 1-2 minutes, then open the Pages link.

## Add to iPhone Home Screen

1. Open the page in Safari.
2. Tap Share, then Add to Home Screen.
3. If an old icon shows, delete the old shortcut, quit Safari, reload the page, and add it again.

## Limitations

- Browsers cannot capture the device's text-to-speech voice, so a text voice can be played with the music but not saved to a file. Use Record or Upload to save a mix.
- MP3 saving loads the `lamejs` encoder from cdnjs, so it needs an internet connection. If it fails, the app saves WAV instead.
- Very long music files make large files and take longer to mix.
- On iPhone, the silent switch can mute preview playback.
