# Xcode Lingo Privacy Policy

**Effective date: September 5, 2026**  
**Last updated: September 5, 2026**

Xcode Lingo is designed to minimize data collection and keep developer content under the user’s control. This policy explains how information is handled by the Xcode Lingo macOS app and its Xcode Source Editor Extension.

## Summary

Xcode Lingo does not operate an analytics or translation server, does not contain advertising, and does not track users. Processing occurs on device with Apple Intelligence when available. Cloud processing is optional, disabled by default, and uses an endpoint and API key configured by the user.

## Information handled by the app

Xcode Lingo may handle the following information solely to provide features requested by the user:

- Text typed or pasted into the app
- Text or code selected in the Xcode source editor
- Xcode compiler or runtime messages copied by the user
- Translation and explanation results
- API endpoint, model name, processing preferences, and target-language preferences
- An API key supplied by the user when optional cloud processing is configured

This information may contain personal or confidential content if the user includes such content. Users should avoid submitting passwords, private keys, tokens, customer data, or proprietary source code to a cloud provider.

## On-device processing

When Apple Intelligence is available and the applicable processing mode is selected, requests are processed on the user’s Mac through Apple’s Foundation Models framework. Xcode Lingo does not send these requests to a server operated by the developer.

Availability and operation of Apple Intelligence are governed by Apple’s software and privacy terms.

## Optional cloud processing

Cloud processing is disabled by default. It occurs only when the user enables **Allow Cloud Processing**, configures a compatible API endpoint, and supplies an API key.

When enabled, input text, task instructions, and the configured model name are transmitted directly from the user’s Mac to the configured API endpoint. Xcode Lingo does not proxy these requests through a developer-operated server.

The cloud provider may process, retain, or log information according to its own terms and privacy policy. The user is responsible for reviewing the policy of the provider they configure. Disabling cloud processing prevents future cloud requests.

## Clipboard

Xcode Lingo can read text from the macOS clipboard to make copied Xcode diagnostics easier to process. Clipboard text may be placed into the workspace when the app opens or when the user chooses a clipboard action. Loading clipboard text does not by itself send it to Apple Intelligence or a cloud endpoint; processing begins only after the user starts a task.

## Local storage

- API keys are stored in macOS Keychain.
- Preferences and recent history are stored locally using the app’s shared App Group container.
- Recent history is limited by the app and can be cleared from the interface.
- Xcode Lingo does not intentionally synchronize this information to a developer-operated service.

Removing the API key in Settings, clearing history, or uninstalling the app can be used to remove locally stored information. macOS may retain Keychain items after an app is removed; users can delete those items using Keychain Access.

## Data collection, tracking, and advertising

Xcode Lingo does not collect personal information on behalf of the developer, use advertising SDKs, track users across apps or websites, sell personal information, share information with data brokers, or create user accounts.

Direct communication with a user-configured cloud provider is described in the **Optional cloud processing** section above.

## Children

Xcode Lingo is a developer utility and is not directed to children. The developer does not knowingly collect personal information from children.

## Security

Reasonable platform security measures are used, including App Sandbox, macOS Keychain storage for API keys, and encrypted HTTPS connections when the configured endpoint uses HTTPS. No security measure can guarantee absolute protection, particularly when users configure third-party endpoints.

## Changes to this policy

This policy may be updated when Xcode Lingo’s features or legal obligations change. The effective date at the top of this document will be revised when changes are published.

## Contact

For privacy questions, open an issue in this GitHub repository. Do not include API keys, confidential source code, or personal information in a public issue.

---

# Xcode Lingo 隐私政策（中文摘要）

Xcode Lingo 不包含广告或用户追踪，也不运营开发者自己的翻译服务器。支持的 Mac 会优先通过 Apple 智能在设备本地处理内容。

云端处理默认关闭。只有用户主动开启云端处理、配置 API 地址并提供 API Key 后，输入内容才会直接发送至用户选择的 API 服务商。相关数据将按照该服务商的隐私政策处理。

API Key 保存在 macOS 钥匙串中；设置和最近记录保存在本机 App Group 容器中。用户可以在应用中清除历史记录并关闭云端处理。

如有隐私问题，请通过本 GitHub 仓库的 Issues 页面联系。请勿在公开 Issue 中提交 API Key、保密代码或个人信息。
