# Barbie Android APK

Android mobile application for Barbie project built with React Native.

## Features
- Cross-platform development with React Native
- Native Android performance
- Seamless UI/UX

## Prerequisites

- Node.js (v16 or higher)
- Java Development Kit (JDK 11 or higher)
- Android SDK
- Android Studio (recommended)
- React Native CLI

## Installation

### 1. Install dependencies
```bash
npm install
```

### 2. Install Android dependencies
```bash
cd android && ./gradlew build
cd ..
```

### 3. Run on Android device/emulator
```bash
npm run android
```

## Build APK

### Debug APK
```bash
cd android
./gradlew assembleDebug
cd ..
```
APK will be located at: `android/app/build/outputs/apk/debug/app-debug.apk`

### Release APK
```bash
cd android
./gradlew assembleRelease
cd ..
```
APK will be located at: `android/app/build/outputs/apk/release/app-release.apk`

## Project Structure

```
Barbie-Android/
├── android/                 # Native Android code
├── ios/                     # iOS code (optional)
├── src/
│   ├── components/         # React components
│   ├── screens/            # Screen components
│   ├── navigation/         # Navigation setup
│   ├── services/           # API services
│   └── assets/             # Images, fonts, etc.
├── App.tsx                 # Main App component
├── index.js                # Entry point
├── package.json
└── tsconfig.json
```

## Available Scripts

- `npm start` - Start Metro bundler
- `npm run android` - Run on Android device/emulator
- `npm run build:android` - Build APK
- `npm run lint` - Run ESLint
- `npm run test` - Run tests

## Troubleshooting

### Port 8081 already in use
```bash
lsof -i :8081
kill -9 <PID>
```

### Build issues
```bash
cd android
./gradlew clean
cd ..
npm install
```

## Contributing
Feel free to submit issues and enhancement requests!

## License
MIT
