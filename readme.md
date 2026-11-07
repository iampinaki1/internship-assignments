#First commit
# HBIntern – React Native (JavaScript/JSX)

A React Native CLI (v0.88) project built using pure JavaScript/JSX and successfully tested on a physical Android device.

## Getting Started

### Prerequisites
Complete the [React Native Environment Setup](https://reactnative.dev/docs/set-up-your-environment) before running the project.

### Run the App

**1. Start Metro**

```bash
npm start
```

**2. Connect your Android device**

Make sure USB debugging is enabled, then run:

```bash
adb reverse tcp:8081 tcp:8081
```

**3. Build and run**

Open another terminal and execute:

```bash
npx react-native run-android --no-packager
```

### Run Tests

```bash
npm test
```

## Issues Fixed

During setup, we encountered and resolved a few issues:

- **TypeScript to JSX:** Migrated the default TypeScript setup to pure JavaScript/JSX and updated Jest configuration.
- **Android SDK:** Installed the required Build-Tools 37.0.0 and CMake 3.22.1 for React Native's New Architecture.
- **Metro Port Conflict:** Used `--no-packager` to reuse the existing Metro server on port 8081.
- **Device Connectivity:** Used `adb reverse` to connect the physical Android device to Metro.
- **Fast Refresh:** Verified that code changes automatically reflect on the connected device.

## Development

React Native's Fast Refresh automatically updates the app whenever you save changes.

For more information, check out the [React Native Documentation](https://reactnative.dev/docs/getting-started).

# colour schema
Colour	HEX Code	Usage
Soft Peach	#F9E0D9	Main background
Warm Coral	#F4B5A3	Primary accent, charts
Light Peach	#F8DFD8	Secondary backgrounds
Pastel Lavender	#DBDBF7	Activity cards
Pure White	#FFFFFF	Cards and containersAX
Off White	#F9F9F9	Secondary surfaces
Charcoal	#252525	Headings and text
Medium Gray	#A7A7A7	Secondary text, icons
Dark Taupe	#5E514D	Graph lines
