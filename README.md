# PaddleScreens QR Redirect

This repository hosts a simple HTML page that handles QR code redirection for the PaddleScreens app. When a user scans a PaddleScreens QR code:

- If they have the app installed, it will open the app directly with the relevant data
- If they don't have the app, it will provide a link to download the app from the App Store

## How It Works

The QR codes contain a custom URL scheme that includes:
1. The PaddleScreens-specific data (club name and court number)
2. A link to the App Store

When scanned, the page attempts to open the app using the custom URL scheme. If that fails (app not installed), it shows the download button.

## Usage

To generate a QR code that works with this system, use the format:

```
https://[your-github-username].github.io/paddle-qr-redirect/?data=PaddleScreens-ClubName-CourtNumber&appstore=https://apps.apple.com/app/6742572918
```

Replace `[your-github-username]` with your actual GitHub username after publishing this repository as GitHub Pages.
