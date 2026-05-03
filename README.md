# ChromaMix - Mobile Application

## Overview
ChromaMix is a professional-grade art assistant designed to help artists achieve perfect color accuracy. By using the device's camera or uploaded images, it provides precise HEX/RGB values and calculates the ideal mixing ratios for RYB (Red, Yellow, Blue) and White paints.

## Technology Stack
- **Framework**: Capacitor 6.x
- **Build Tool**: Vite
- **Frontend**: Vanilla JS (HTML5/CSS3)
- **Target Platforms**: Android (APK), iOS
- **Design**: Premium Glassmorphism UI

## Features
- **Real-time Color Capture**: Use the back camera to identify colors in the real world.
- **RYB Mixing Engine**: Automatically calculates paint ratios for physical mixing.
- **White Balance Calibration**: Ensuring accuracy across different lighting conditions.
- **Premium UI**: Safe area handling, haptic feedback, and a sleek modern aesthetic.
- **Offline-first**: Works entirely on-device without a backend.

## Local Development

### Prerequisites
- Node.js 20+
- Android SDK (for APK builds)
- Xcode (for iOS builds, macOS only)

### Setup
```bash
# Navigate to the app directory
cd app

# Install dependencies
npm install

# Run development server
npm run dev

# Sync with Capacitor
npx cap sync

# Open in Android Studio
npx cap open android

# Build APK locally
cd android && ./gradlew assembleDebug
```

## GitHub Actions
This project uses automated CI/CD:

| Workflow | Trigger | Output |
|----------|---------|--------|
| Android Build & Release | On push to main | APK artifact |
| Pre-commit Validation | On PR/push | Secret & Gitignore checks |

## License
MIT
