# AINS Studio Glasswing for Microsoft Edge v5.0.0

**Codename: Glasswing**

Glasswing brings AINS Studio’s v5 settings center and reading tools to Microsoft Edge. This package is based on the Chromium Manifest V3 build and targets AINS pages only.

## Highlights

- Full settings page inside AINS with a global switch and controls for visual design, translation, reading dashboard, local activity collection, Excel import, and clipboard behavior.
- iOS-inspired Studio navigation and appearance controls.
- Reading dashboard with date filtering, record counts, local snapshots, and CSV export.
- Localized AINS announcement “Don’t show again” preference, with a reset control in settings.
- Custom Studio not-found page and navbar shortcut to settings.
- Admin-only Excel/CSV reading-record helper with selectable starting row, mapped columns, paced form filling, review, and retry timing.
- Safari is a separate upcoming target; this is the Edge package.

## Developer notes

This release uses Manifest V3, a service worker, Chromium’s `chrome.*` extension APIs, and the same scoped AINS host access as the Chrome edition (`https://ains.moe.gov.my/web/*`). It requests `storage` and `scripting` permissions. No broad all-sites permission is requested.

Configuration, reading snapshots, and importer state are kept in extension local storage. The importer’s local salted PBKDF2-SHA-256 verifier is a UI lock only; it does not grant server-side AINS administrative privileges. The browser package has not been reviewed or published by Microsoft.

## Install for development

1. Download and extract `ains-studio-glasswing-edge-v5.0.0.zip`.
2. Open `edge://extensions`, enable **Developer mode**, and select **Load unpacked**.
3. Choose the folder containing `manifest.json`, then refresh AINS.

For store distribution, prepare a Microsoft Edge Add-ons listing and submit it through Microsoft Partner Center.
