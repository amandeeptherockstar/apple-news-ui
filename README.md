# Apple Music Sheet UI Demo with Expo

This project demonstrates an implementation of the Apple Music player UI in React Native using Expo, with a focus on replicating the smooth sheet transitions and scaling animations.

![Demo](assets/gifs/demo1.gif)

## Features

- 🎵 Full-screen music player modal with gesture controls
- 🔄 Smooth scaling animations of the root content
- 👆 Interactive pan gesture handling
- 📱 iOS-style sheet presentation
- 🎨 Dynamic border radius animations
- 🌟 Visual audio visualizer
- 💫 Haptic feedback on modal interactions
- 🖼️ Blur effects and backdrop filters
- 📱 Sticky mini-player navigation
- 📋 Apple Music style track listing
- ⚡ Gesture handling with drag thresholds
- 🔄 Horizontal swipe to dismiss

## Tech Stack

- [Expo](https://expo.dev) - React Native development platform
- [Expo Router](https://docs.expo.dev/router/introduction) - File-based routing
- [React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/) - Smooth animations
- [React Native Gesture Handler](https://docs.swmansion.com/react-native-gesture-handler/) - Native-driven gesture handling

## Getting Started

1. Install dependencies:

   ```bash
   npm install
   ```

2. Start the development server:

   ```bash
   npx expo start
   ```

3. Open in iOS Simulator or Android Emulator:
   - Press `i` for iOS
   - Press `a` for Android

## Implementation Details

The project showcases several key features of modern React Native development:

- Shared element transitions between mini and full player
- Gesture-based interactions with multi-axis support
- Context-based animation state management
- Worklet-based animations for optimal performance

### Known Issues

- Horizontal drag gesture conflicts with content scrolling when the modal is partially scrolled, causing flickering. This needs to be addressed by properly managing gesture priorities and scroll state.

## Project Structure

```
project-root/
├── app/
│   ├── (tabs)/
│   │   ├── search/            # Search and library screens
│   │   │   ├── _layout.tsx
│   │   │   ├── library.tsx
│   │   │   ├── new.tsx
│   │   │   └── radio.tsx
│   │   ├── music/             # Music player routes
│   │   │   ├── [id].tsx
│   │   │   └── _layout.tsx
│   │   └── _layout.tsx        # Tab navigation layout
├── components/
│   ├── navigation/
│   │   └── TabBarIcon.tsx     # Tab bar icons
│   ├── Overlay/               # Sheet UI components
│   │   ├── OverlayContext.tsx
│   │   ├── OverlayProvider.tsx
│   │   └── ThemedView.tsx
│   └── ThemedText.tsx
├── contexts/
│   ├── AudioContext.tsx       # Audio playback state
│   └── RootScaleContext.tsx   # Scale animation state
├── constants/
│   └── Colors.ts             # Theme colors
└── hooks/                    # Custom React hooks
    ├── useColorScheme.ts
    ├── useThemeColor.ts
    └── useColorScheme.web.ts
```

## Contributing

Feel free to contribute to this project by:

1. Forking the repository
2. Creating a feature branch
3. Submitting a pull request

## License

This project is open source and available under the MIT License.


## Dummy data scraped:
1. Podcast: https://podcasts.apple.com/us/room/1589753370 (#serialized-server-data)
fyi: 
i. replace: {w}x{h}
with : /376x376bb.webp

ii.