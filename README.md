
# Endless Runner Game

This endless runner game was developed by me as part of my Computer Graphics Lab exam project. The game is built using Flutter and Flame, and showcases various computer graphics concepts and game development techniques. Below are some of the features I implemented:


## Features

**Flutter:**
- Custom FlameGame base
- Main menu and navigation
- Themed UI and settings
- Sound and music integration

**Flame:**
- Player movement and steering
- Collision detection
- Parallax backgrounds
- Visual effects
- Enemy and object spawning

You can find the main game logic in `lib/flame_game/`.

This project demonstrates my understanding of computer graphics principles, game loops, collision detection, and UI/UX in Flutter.



## Getting Started

To run the game, make sure you have the [Flutter SDK installed](https://docs.flutter.dev/get-started/install). Clone this repository and run the following command in the project root:

```shell
flutter pub get
```

Then you can launch the game on your preferred device or emulator:

```shell
flutter run
```



The game supports multiple platforms including Android, iOS, Windows, macOS, and web.



## Development Notes

I developed and tested the game using Visual Studio Code and Android Studio. The code is organized in a feature-first fashion for clarity and maintainability.



### Code Structure

```
lib
├── app_lifecycle
├── audio
├── flame_game
├── level_selection
├── main_menu
├── player_progress
├── settings
├── style
└── main.dart
└── router.dart
```

I kept state management simple to focus on graphics and gameplay logic.



## Building for Production

You can build the game for iOS, Android, web, and desktop using standard Flutter commands. See the official [Flutter documentation](https://docs.flutter.dev/) for details.



## Integrations

The game is ready for further integrations such as ads, in-app purchases, analytics, and more. For my lab exam, I focused on core gameplay and graphics features.



## Audio

Audio is enabled by default. Music tracks in `assets/music` are Creative Commons Attribution (CC-BY) licensed by [Mr Smith](https://freemusicarchive.org/music/mr-smith). Sound effects in `assets/sfx` are public domain (CC0).



## Logging

The template uses the [`logging`](https://pub.dev/packages/logging) package
to log messages to the console. This makes it very easy to log messages
from anywhere with something like the following:

```dart
import 'package:logging/logging.dart';

final _log = Logger('Foo');

void foo() {
  _log.info('Hello, world!');
}
```

This will show up in the console as:

```text
[Foo] Hello, world!
```

When using Flutter DevTools, all the metadata of the log message is preserved,
so you can filter by logger name, log level, and so on.

Later, when you're closer to production, you can gather these log messages
(see `lib/main.dart`) and send them to a service like Firebase Crashlytics
when appropriate.
See [`firebase_crashlytics`](https://pub.dev/packages/firebase_crashlytics)
for more information.


## Settings

The game includes a settings page, accessible from the main menu and in-game. Preferences are saved locally using [`shared_preferences`](https://pub.dev/packages/shared_preferences).



## Icon

To update the launcher icon, replace `assets/icon-adaptive-foreground.png` and `assets/icon.png`, then run:

```shell
flutter pub run flutter_launcher_icons:main
```



# Troubleshooting

Refer to the official Flutter documentation for troubleshooting build or platform issues. Most warnings from plugins can be safely ignored during development.
