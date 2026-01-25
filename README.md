# Google Voice Image Paste Extension

A Chrome extension that enables pasting images directly into Google Voice conversations using Ctrl+V (or Cmd+V on Mac).

## Features

- Paste images from clipboard directly into Google Voice
- Works with screenshots, copied images from web pages, or any image in clipboard
- Shows confirmation notification when image is pasted
- Seamlessly integrates with Google Voice's existing upload mechanism

## Installation

### Developer Mode (Unpacked Extension)

1. Open Chrome and navigate to `chrome://extensions/`
2. Enable **Developer mode** (toggle in top-right corner)
3. Click **Load unpacked**
4. Select the `GoogleVoicePasteImage` folder
5. The extension is now active!

## Usage

1. Go to [Google Voice](https://voice.google.com)
2. Open a conversation
3. Copy an image to your clipboard (screenshot, right-click copy, etc.)
4. Press **Ctrl+V** (Windows/Linux) or **Cmd+V** (Mac)
5. The image will be uploaded to the conversation

## Troubleshooting

### Image paste not working?

1. Open Chrome DevTools (F12) and check the Console for messages starting with `[GV Image Paste]`
2. The extension may need selector updates if Google Voice changed their DOM structure
3. Ensure you have an image (not text) in your clipboard

### Updating selectors

If Google Voice updates their interface, you may need to update the selectors in `content.js`:

1. Open Google Voice in Chrome
2. Right-click on the message input field → Inspect
3. Note the element's attributes (class, aria-label, etc.)
4. Update the `CONFIG` object in `content.js`

## Files

- `manifest.json` - Extension configuration
- `content.js` - Main script that handles paste events

## Permissions

- `activeTab` - Access to the current tab
- `clipboardRead` - Read images from clipboard
- `host_permissions` for `voice.google.com` - Run on Google Voice pages

## Version History

- **1.0.0** - Initial release
