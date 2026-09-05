# Xcode Lingo

> Understand Xcode. Keep coding. 读懂 Xcode，继续创造。

Xcode Lingo is a privacy-first macOS assistant and Xcode Source Editor Extension for developers who work in Simplified Chinese, Japanese, or Korean. It translates English developer content, explains Xcode errors, and generates useful code comments without interrupting your coding flow.

Xcode Lingo 是一款面向中文、日文和韩文开发者的 macOS 工具，帮助你快速翻译英文技术内容、解读 Xcode 错误并生成代码注释。

## Features

- Translate English into Simplified Chinese, Japanese, or Korean
- Explain compiler and runtime errors with likely causes and actionable fixes
- Understand the purpose and important behavior of selected code
- Generate concise comments while preserving identifiers and formatting
- Use Xcode commands directly from the Editor menu
- Paste and process copied Xcode diagnostics in the standalone workspace
- Search and reuse up to 30 recent results
- Localized interface in English, Simplified Chinese, Japanese, and Korean
- Use Apple Intelligence on device when available
- Optionally use a user-configured Responses-compatible cloud API

## Privacy

Cloud processing is disabled by default. On supported Macs, Xcode Lingo prioritizes Apple Intelligence for on-device processing. Text is sent to a cloud endpoint only after the user explicitly enables cloud processing and supplies an API key.

- No advertising or tracking
- No developer-operated analytics or backend service
- API keys are stored in macOS Keychain
- Settings and history are stored locally in the App Group container
- Clipboard text may be loaded into the workspace, but is not processed or transmitted until the user starts a task

Read the complete [Privacy Policy](PRIVACY.md).

## Requirements

- macOS 14 or later
- Xcode with Source Editor Extension support
- Apple Intelligence requires a supported Apple silicon Mac, macOS 26 or later, and Apple Intelligence enabled
- A compatible API endpoint and personal API key are optional

## Enable the Xcode extension

1. Install and open Xcode Lingo once.
2. Open **System Settings → General → Login Items & Extensions**.
3. Open **Xcode Source Editor** extensions and enable **XcodeLingoExtension**.
4. Restart Xcode.
5. Select text or code in the source editor.
6. Choose a Xcode Lingo command from Xcode’s **Editor** menu.

XcodeKit can read and modify the current source editor selection, but it cannot directly read items from Xcode’s Issue Navigator. Copy those diagnostics and process them in the Xcode Lingo workspace.

## Build from source

1. Open `XcodeLingo.xcodeproj` in Xcode.
2. Select the `XcodeLingo` scheme.
3. Choose your development team under Signing & Capabilities.
4. Build and run the macOS app.
5. Enable the extension using the steps above.

## Processing modes

- **Automatic:** Apple Intelligence first; cloud fallback only when cloud processing is authorized and configured
- **Apple Intelligence Only:** always process on device
- **Cloud API Only:** use the endpoint and API key supplied by the user

## Security

Do not paste passwords, private keys, access tokens, or other secrets into any translation service. When cloud processing is enabled, review the privacy and retention policy of the API provider you configure.

## Support

Use the repository’s **Issues** page to report a bug or request a feature. Remove source code, API keys, and other confidential information before attaching logs or screenshots.

## Disclaimer

Xcode Lingo is an independent developer tool and is not affiliated with or endorsed by Apple Inc. or OpenAI. Xcode, macOS, Apple Intelligence, and related marks are trademarks of Apple Inc.

