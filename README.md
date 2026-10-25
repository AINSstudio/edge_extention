# AINS Studio Glasswing for Microsoft Edge

Microsoft Edge build of AINS Studio **v5.0.0**, codename **Glasswing**. Edge is Chromium-based, so this package uses the same Manifest V3 extension APIs as the Chrome build, with Edge-specific product metadata.

## Install locally

1. Extract `ains-studio-glasswing-edge-v5.0.0.zip`.
2. Open `edge://extensions`.
3. Turn on **Developer mode**.
4. Choose **Load unpacked** and select the extracted folder containing `manifest.json`.
5. Open AINS at `https://ains.moe.gov.my/web/` and refresh the page. Use the extension toolbar icon or the AINS navbar shortcut to open Studio settings.

## Included

- AINS Studio full settings center, global and per-feature controls, and custom Studio 404 page.
- Reading overview, local activity view, translation, themes, and Excel/CSV record assistant.
- Manifest V3 service worker with permissions restricted to AINS web pages and local extension storage.

To publish in Microsoft Edge Add-ons, create a publisher listing and submit the package through Microsoft Partner Center. This folder is unpacked source; it has not been submitted or approved by Microsoft.
