# Google Voice Image Paste Extension

A Chrome extension that enables pasting images directly into Google Voice conversations using Ctrl+V (or Cmd+V on Mac).

## Features

- Paste images from clipboard directly into Google Voice
- Works with screenshots, copied images from web pages, or any image in clipboard
- Shows confirmation notification when image is pasted
- Seamlessly integrates with Google Voice's existing upload mechanism

## Installation

### Developer Mode (Unpacked Extension)

1. Download the package from github (click Code > Download ZIP).  Unzip it and remember the folder name.  We'll use `GoogleVoiceImagePaste` as an example
2. Open Chrome/Edge and navigate to `chrome://extensions/`
3. Enable **Developer mode** toggle
4. Click **Load unpacked**
5. Select the `googlevoice-image-paste-main` folder inside the `GoogleVoiceImagePaste` folder.  It's the one with the manifest.json file in it.
6. The extension is now active!  You will need to reload any Google Voice tabs.

## Usage

1. Go to [Google Voice](https://voice.google.com)
2. Open a conversation
3. Copy an image to your clipboard (screenshot, right-click copy, etc.)
4. Press **Ctrl+V** (Windows/Linux) or **Cmd+V** (Mac)
5. The image will be uploaded to the conversation

## Troubleshooting

### Image paste not working?

1. Open Chrome DevTools (F12) and check the Console for messages starting with `[GV Image Paste]`
2. Ensure you have an image (not text) in your clipboard

## Files

- `manifest.json` - Extension configuration
- `content.js` - Main script that handles paste events

## Permissions

- `activeTab` - Access to the current tab
- `clipboardRead` - Read images from clipboard
- `host_permissions` for `voice.google.com` - Run on Google Voice pages

## Version History

- **1.0.0** - Initial release


