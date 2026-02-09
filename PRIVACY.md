# Privacy Policy for Google Voice Image Paste Extension

**Last Updated:** February 2025

## Overview

Google Voice Image Paste ("the Extension") is a browser extension that enables users to paste images from their clipboard directly into Google Voice conversations.

## Data Collection

**We do not collect, store, transmit, or share any personal data or user information.**

The Extension operates entirely locally within your browser and does not communicate with any external servers.

## Permissions Explained

The Extension requests the following permissions, used solely for core functionality:

- **clipboardRead**: Required to read image data from your clipboard when you paste. This data is processed locally and immediately passed to Google Voice's upload mechanism. No clipboard data is stored or transmitted.

- **activeTab**: Required to interact with the current Google Voice tab to enable image pasting functionality.

- **host_permissions (voice.google.com)**: Required to run the content script on Google Voice pages only.

## Data Processing

- All image processing (reading from clipboard, compression if needed) happens locally in your browser
- Images are passed directly to Google Voice's existing upload mechanism
- No data is sent to any third-party servers
- No analytics or tracking of any kind

## Third-Party Services

This Extension does not integrate with or send data to any third-party services.

## Changes to This Policy

Any updates to this privacy policy will be reflected in the Extension's GitHub repository and this document will be updated with a new "Last Updated" date.

## Contact

If you have questions about this privacy policy, please open an issue on the GitHub repository:
https://github.com/tomreich/googlevoice-image-paste

## Open Source

This Extension is open source. You can review the complete source code at:
https://github.com/tomreich/googlevoice-image-paste
