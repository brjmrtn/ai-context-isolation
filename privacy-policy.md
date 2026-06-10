# Privacy Policy — AI Context Isolation

**Last updated: June 10, 2026**

## Overview

AI Context Isolation is a Chrome extension that allows users to save reusable context blocks and inject them into AI chat platforms. This privacy policy explains how the extension handles user data.

## Data Collection

The extension itself does not collect any personal data. The only exception is the license validation process described below.

The extension does not:
- Collect, transmit, or share browsing data
- Track user behavior or usage patterns
- Use analytics or telemetry services
- Access any data beyond what is strictly necessary to function

## Data Storage

The only data stored by this extension are the context blocks (title and content) created by the user. This data is:

- Stored **locally on the user's device** using the Chrome `storage.local` API
- Never transmitted outside the user's browser
- Fully controlled by the user — they can edit or delete it at any time

The Pro license key entered by the user is also stored locally using `chrome.storage.local` solely to avoid requiring re-entry on every browser restart.

## License Validation

AI Context Isolation Pro uses **Lemon Squeezy** to process payments and validate license keys. When a user enters a license key, the extension sends that key to the Lemon Squeezy API (`api.lemonsqueezy.com`) to verify its validity.

No other data is sent during this process. Lemon Squeezy's privacy policy applies to the purchase process: https://www.lemonsqueezy.com/privacy

## Permissions Used

| Permission | Reason |
|---|---|
| `sidePanel` | Display the extension's UI as a side panel |
| `storage` | Save context blocks and license status locally on the user's device |
| `activeTab` | Identify the currently active tab to inject context into it |
| `scripting` | Inject the selected context text into the AI chat input area |
| Host permissions (AI platforms) | Restrict injection exclusively to the 8 supported AI platforms |
| Host permissions (api.lemonsqueezy.com) | Validate Pro license keys against the Lemon Squeezy API |

## Third-Party Services

| Service | Purpose | Privacy Policy |
|---|---|---|
| Lemon Squeezy | Payment processing and license validation | https://www.lemonsqueezy.com/privacy |

## Supported Platforms

The extension only operates on the following domains when explicitly triggered by the user:
- chatgpt.com
- claude.ai
- gemini.google.com
- grok.com
- copilot.microsoft.com
- perplexity.ai
- chat.deepseek.com
- chat.mistral.ai

## Changes to This Policy

If this policy changes in the future, the updated version will be published at this URL with a new "Last updated" date.

## Contact

For questions about this privacy policy, open an issue at:
https://github.com/brjmrtn/ai-context-isolation/issues
