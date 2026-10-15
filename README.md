<div align="center">

# AdGuard · Personal Configuration

**My privacy and filtering preferences for AdGuard Browser Extension on desktop Chrome**

[![AdGuard](https://img.shields.io/badge/AdGuard-Browser%20Extension-68BC71?style=for-the-badge&logo=adguard&logoColor=white)](https://chromewebstore.google.com/detail/adguard-adblocker/bgnkhhnnamicmpeenaelnjfhikgbkllg)
[![Browser](https://img.shields.io/badge/Browser-Google%20Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.google.com/chrome/)
[![Config](https://img.shields.io/badge/Configuration-JSON-8250DF?style=for-the-badge&logo=json&logoColor=white)](./adguard-extension-settings.json)

</div>

---

## 👋 About

This repository contains my personal configuration for the **AdGuard Browser Extension** on desktop Google Chrome. It reflects my own balance between ad filtering, privacy, tracking protection, and everyday usability.

These settings are personal preferences, not a universal recommendation. Websites may behave differently depending on their own requirements and the installed AdGuard version.

## 📊 At a glance

| Feature | Status | Notes |
|---|:---:|---|
| Acceptable ads | <img alt="Off" src="https://img.shields.io/badge/OFF-gray?style=flat-square"> | Acceptable ads are not allowed |
| Blocked-ads counter | <img alt="On" src="https://img.shields.io/badge/ON-brightgreen?style=flat-square"> | Counter is shown |
| Automatic filter detection | <img alt="On" src="https://img.shields.io/badge/ON-brightgreen?style=flat-square"> | Enabled |
| Safe Browsing | <img alt="Off" src="https://img.shields.io/badge/OFF-gray?style=flat-square"> | AdGuard's browsing-security setting is disabled |
| Anonymous usage data | <img alt="Off" src="https://img.shields.io/badge/OFF-gray?style=flat-square"> | Collection disabled |
| Optimized filters | <img alt="Off" src="https://img.shields.io/badge/OFF-gray?style=flat-square"> | Disabled |
| Stealth mode | <img alt="On" src="https://img.shields.io/badge/ON-brightgreen?style=flat-square"> | Active |
| Third-party cookies | <img alt="Blocked" src="https://img.shields.io/badge/BLOCKED-brightgreen?style=flat-square"> | Configured lifetime: 2,880 minutes (48 hours) |
| First-party cookies | <img alt="Allowed" src="https://img.shields.io/badge/NOT%20BLOCKED-gray?style=flat-square"> | First-party cookie blocking is disabled |
| Custom filter subscriptions | <img alt="None" src="https://img.shields.io/badge/NONE%20CONFIGURED-lightgrey?style=flat-square"> | No custom filter URLs |
| User rules | <img alt="Enabled, empty" src="https://img.shields.io/badge/ENABLED%20%2F%20EMPTY-blue?style=flat-square"> | No rules defined |
| Allowlist | <img alt="Enabled, empty" src="https://img.shields.io/badge/ENABLED%20%2F%20EMPTY-blue?style=flat-square"> | No domains listed |

## 🛡️ Enabled

### Privacy and tracking protection

- **Hide referrer**
- **Hide search queries**
- **Send Do Not Track**
- **Block WebRTC**
- **Remove the `X-Client-Data` header**
- **Block known trackers**
- **Strip tracking parameters from URLs**
- **Block third-party cookies**, with a configured lifetime of 2,880 minutes (48 hours)

### Filtering and interface

- 17 built-in filter IDs are enabled.
- All 7 built-in filter-group IDs represented in the file are enabled.
- Automatic filter detection is enabled.
- The blocked-ads counter is shown.
- The extension context menu is enabled.
- Update notifications are enabled.
- The appearance follows the system theme.
- The user-rules editor has line wrapping disabled.

## 🚫 Disabled

- Acceptable ads
- Safe Browsing / browsing-security protection
- Optimized filters
- Anonymous usage-data collection
- First-party cookie blocking
- AdGuard information notices
- The rate-AdGuard prompt

## 🧩 Built-in filter IDs

The configuration enables these numeric filter IDs:

```text
1, 2, 3, 4, 11, 17, 18, 19, 20, 21, 22, 25, 208, 255, 256, 257, 259
```

Enabled filter-group IDs:

```text
1, 2, 3, 4, 5, 6, 7
```

The JSON stores numeric IDs rather than human-readable filter names. I have intentionally left them as IDs instead of guessing their names; names and availability should be checked against the filter catalog for the installed extension version.

## 📥 Install and apply

### 1. Install AdGuard

Install the official [AdGuard Browser Extension from the Chrome Web Store](https://chromewebstore.google.com/detail/adguard-adblocker/bgnkhhnnamicmpeenaelnjfhikgbkllg).

### 2. Get the configuration file

Download [`adguard-extension-settings.json`](./adguard-extension-settings.json) from this repository.

### 3. Apply the settings

AdGuard's supported settings-sharing/import flow can vary by extension version. In recent versions, AdGuard supports importing configuration through its settings-import links.

1. Open the AdGuard extension and go to **Settings**.
2. Look for the available **Import settings** or settings-sharing option in your installed version.
3. If it accepts a configuration file, select `adguard-extension-settings.json` and confirm.
4. If the extension does not offer direct JSON-file import, do **not** rename the file or paste its raw JSON into an arbitrary field. Use AdGuard's supported configuration-sharing/import flow, or apply the settings manually using the sections above.
5. Review the result after importing.

**Back up your current configuration first.** Importing shared settings may replace existing settings. The JSON in this repository is the configuration file; its presence alone does not guarantee that every extension build can import it directly from a local file.

## ⚠️ Compatibility and privacy notes

- The supplied JSON has `protocol-version` set to `2.0`.
- The file itself does **not** contain an AdGuard extension version field. The version `5.5.3.6` is based on the version information supplied for this configuration, not a version recorded inside the JSON.
- Filter IDs and available options may change across extension versions. Check the settings after applying them.
- Safe Browsing is disabled in this configuration.
- Blocking WebRTC may affect some browser-based calls, chats, or games.
- Blocking third-party cookies may affect sign-in flows or other site functionality.

## 📁 Repository structure

```text
.
├── README.md
└── adguard-extension-settings.json
```

## 🔗 Useful links

- [AdGuard Browser Extension — Chrome Web Store](https://chromewebstore.google.com/detail/adguard-adblocker/bgnkhhnnamicmpeenaelnjfhikgbkllg)
- [AdGuard Browser Extension documentation](https://adguard.com/en/adguard-browser-extension/overview.html)
- [AdGuard Browser Extension version history](https://adguard.com/en/versions/browser-extension/release.html)
- [AdGuard Browser Extension source code and changelog](https://github.com/AdguardTeam/AdguardBrowserExtension)

---

<div align="center">

**Personal configuration · Desktop Chrome · AdGuard Browser Extension**

</div>
