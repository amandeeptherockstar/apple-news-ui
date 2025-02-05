# Apple News Clone with Expo

A universal iOS News app clone built with React Native and Expo, delivering a native experience across iOS, Android, and Web platforms.

## 🚀 Live Demo

- Web: https://applenews.expo.app
- iOS/Android: Instruction below

## ✨ Key Features

- 💣 Works on Android, iOS, and Web
- 🔄 Native gestures and transitions
- 🎵 Podcast Player with full playback controls
- 📲 iOS-specific features:
  - Live Activities for sports scores
  - Home Screen Widgets
  - Watch support
  - Context menus and peek previews
- 🤏 Swipe actions like 𝕏 (Twitter)
- 🔍 Smart search with keyword highlighting
- ⚡️ Example Server Components (RSC) integration
- ↕️ Drag & sort favorites

## 🛠 Tech Stack

### Core
- [Expo](https://expo.dev) - Universal app development platform
- [React Native](https://reactnative.dev) - Cross-platform native UI
- [TypeScript](https://www.typescriptlang.org) - Type-safe JavaScript
- [Tailwind CSS](https://tailwindcss.com) - Utility-first styling

### Navigation & Routing
- [Expo Router](https://docs.expo.dev/router/introduction) - File-based universal routing
- [React Navigation](https://reactnavigation.org) - Native navigation primitives

### Animation & Gestures
- [Reanimated 4](https://docs.swmansion.com/react-native-reanimated/) - Native animations
- [Gesture Handler](https://docs.swmansion.com/react-native-gesture-handler/) - Native gestures

### Data & State
- [MMKV](https://github.com/mrousavy/react-native-mmkv) - Ultra-fast storage

### UI Components
- [Zeego](https://zeego.dev) - Native context menus
- [Radix UI](https://www.radix-ui.com) - Web components

### Native Features
- [WidgetKit](https://developer.apple.com/documentation/widgetkit) - iOS widgets
- [ActivityKit](https://developer.apple.com/documentation/activitykit) - Live Activities
- [Expo AV](https://docs.expo.dev/versions/latest/sdk/av/) - Audio playback

## 📱 Installation

1. Clone the repository:
```bash
git clone https://github.com/saulamsal/apple-news-ui
```

2. Install dependencies (using bun or npm):
```bash
cd apple-news-ui
bun install
# or
npm install
```

3. Start the development server:
```bash
bun run start
# or
npm start
```

4. Run on your preferred platform:
```bash
# iOS
bun run ios
# Android
bun run android
# Web
bun run web
```


## 🧪 Experimental Features

Some features are in development and may be unstable:
- React Server Components integration
- Watch app support
- Background audio controls
- Enhanced Live Activities

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is MIT licensed.

## 🙏 Acknowledgments

- [@baconbrix](https://github.com/baconbrix) for `create-target`
- [@mrousavy](https://github.com/mrousavy) for `react-native-mmkv`
- [@fernandotherojo](https://github.com/fernandotherojo) for Zeego
- [Expo team](https://expo.dev) for the amazing tooling

## Data Sources

### Podcast Data
- Source: Apple Podcasts API
- Example URL: https://podcasts.apple.com/us/room/1589753370
- Image URL format: Replace `{w}x{h}` with `/376x376bb.webp`

## TODO

### Audio 
- [ ] Replace expo-av with expo-audio
- [ ] Lock screen player implementation
- [ ] Lock screen controls
  - Pending react-native-track-player support for new architecture
  - Alternative: Wait for expo-audio lock screen control support

### UI/UX 
- [ ] Shared transitions (Currently broken in Expo 52)
- [ ] Fix long press behavior - Details view and context menu conflict
- [ ] Optimize navigation performance during audio playback (25% complete)
- [ ] Fix /audio/[id] not playing on web when not loaded via MiniPlayer click

### Other
- [ ] More robust RSC examples
