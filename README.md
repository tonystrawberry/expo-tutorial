# StickerSmash 🎨

A fun photo sticker app built with React Native and Expo. Pick a photo, add emoji stickers, drag them around, and save your creation!

## Features

- **📸 Photo Selection** — Choose photos from your device's library or use the default placeholder
- **😎 Emoji Stickers** — Pick from 6 fun emoji stickers to add to your photo
- **✋ Drag & Drop** — Drag stickers anywhere on your photo with smooth gesture handling
- **🔍 Resize** — Double-tap any sticker to scale it up or down
- **💾 Save** — Export your creation to your device's photo library (or download on web)
- **🌐 Cross-Platform** — Runs on iOS, Android, and Web

## Tech Stack

- [Expo](https://expo.dev) SDK 54
- [React Native](https://reactnative.dev) 0.81
- [Expo Router](https://docs.expo.dev/router/introduction/) for file-based navigation
- [React Native Gesture Handler](https://docs.swmansion.com/react-native-gesture-handler/) for touch interactions
- [React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/) for smooth animations
- [Expo Image Picker](https://docs.expo.dev/versions/latest/sdk/imagepicker/) for photo selection
- [Expo Media Library](https://docs.expo.dev/versions/latest/sdk/media-library/) for saving images

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn
- [Expo Go](https://expo.dev/go) app on your phone (for testing on device)

### Installation

1. Clone the repository and navigate to the project:

   ```bash
   cd StickerSmash
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npx expo start
   ```

4. Open the app:
   - **iOS Simulator** — Press `i` in the terminal
   - **Android Emulator** — Press `a` in the terminal
   - **Physical Device** — Scan the QR code with Expo Go
   - **Web** — Press `w` in the terminal

## Usage

1. **Choose a photo** — Tap "Choose a photo" to pick from your library, or "Use this photo" to use the placeholder
2. **Add a sticker** — Tap the `+` button to open the emoji picker and select a sticker
3. **Position your sticker** — Drag the sticker anywhere on the photo
4. **Resize** — Double-tap the sticker to toggle between normal and 2x size
5. **Save** — Tap "Save" to export your creation
6. **Reset** — Tap "Reset" to start over

## Project Structure

```
StickerSmash/
├── app/                    # App screens (Expo Router)
│   ├── (tabs)/            # Tab-based navigation
│   │   ├── index.tsx      # Main sticker editor screen
│   │   └── about.tsx      # About screen
│   └── _layout.tsx        # Root layout
├── components/            # Reusable components
│   ├── Button.tsx         # Primary/secondary buttons
│   ├── CircleButton.tsx   # Add sticker button
│   ├── EmojiList.tsx      # Horizontal emoji picker list
│   ├── EmojiPicker.tsx    # Modal for emoji selection
│   ├── EmojiSticker.tsx   # Draggable, resizable sticker
│   ├── IconButton.tsx     # Icon buttons (reset, save)
│   └── ImageViewer.tsx    # Photo display component
└── assets/               # Images and emoji assets
```

## Scripts

| Command | Description |
|---------|-------------|
| `npm start` | Start Expo development server |
| `npm run ios` | Start on iOS simulator |
| `npm run android` | Start on Android emulator |
| `npm run web` | Start in web browser |
| `npm run lint` | Run ESLint |

## License

This project is open source and available under the [MIT License](LICENSE).
