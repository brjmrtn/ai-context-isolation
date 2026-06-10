# Privacy Policy — AI Context Isolation

**Last updated: June 10, 2026**

## Overview

AI Context Isolation is a Chrome extension that allows users to save reusable context blocks and inject them into AI chat platforms. This privacy policy explains how the extension handles user data.

## Data Collection

**AI Context Isolation does not collect any personal data.**

The extension does not:
- Collect, transmit, or share any user data
- Send any information to external servers
- Track user behavior or usage patterns
- Use analytics or telemetry services
- Access any data beyond what is strictly necessary to function

## Data Storage

The only data stored by this extension are the context blocks (title and content) created by the user. This data is:

- Stored **locally on the user's device** using the Chrome `storage.local` API
- Never transmitted outside the user's browser
- Fully controlled by the user — they can edit or delete it at any time

## Permissions Used

| Permission | Reason |
|---|---|
| `sidePanel` | Display the extension's UI as a side panel |
| `storage` | Save context blocks locally on the user's device |
| `activeTab` | Identify the active tab to inject context into it |
| `scripting` | Inject selected context text into the AI chat input area |
| Host permissions | Restrict injection exclusively to supported AI platforms |

## Third-Party Services

This extension does not use any third-party services, APIs, or SDKs.

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
