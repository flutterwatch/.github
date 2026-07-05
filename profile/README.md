<p align="center">
  <img src="./logo.png" width="116" alt="flutterwatch" />
</p>

<h1 align="center">flutterwatch</h1>

<p align="center">
  <b>Build Flutter apps for Apple&nbsp;Watch.</b><br/>
  A drop-in CLI companion to the Flutter SDK — same commands, same hot reload,
  same DevTools — targeting <b>watchOS</b> instead of iOS.
</p>

<p align="center">
  <a href="https://flutterwatch.dev"><b>Website</b></a> &nbsp;·&nbsp;
  <a href="https://github.com/flutterwatch/flutter-watchos/blob/main/doc/get-started.md">Get started</a> &nbsp;·&nbsp;
  <a href="https://github.com/flutterwatch/flutter-watchos/blob/main/doc/commands.md">Commands</a> &nbsp;·&nbsp;
  <a href="https://pub.dev/packages/flutter_watchos">pub.dev</a> &nbsp;·&nbsp;
  <a href="https://api.flutterwatch.dev/">Join the closed beta</a>
</p>

<p align="center">
  <img alt="Status: closed beta" src="https://img.shields.io/badge/status-closed%20beta-2BA3F2?style=flat-square" />
  <img alt="Platform: macOS" src="https://img.shields.io/badge/host-macOS-3D4E74?style=flat-square" />
  <img alt="Flutter 3.44.4" src="https://img.shields.io/badge/Flutter-3.44.4-1565C0?style=flat-square" />
  <img alt="Target: watchOS" src="https://img.shields.io/badge/target-watchOS-14213A?style=flat-square" />
</p>

---

### What is flutterwatch?

flutterwatch brings the Flutter framework to **Apple Watch**. Write your app in
Dart with the widgets and packages you already use, then build and run it on the
watchOS Simulator or a paired Apple Watch — with hot reload and DevTools, exactly
like Flutter for iOS or Android.

It is a standalone CLI that wraps an unmodified Flutter SDK and a pre-built
watchOS engine, so there's no custom Flutter checkout to maintain. watchOS is a
first-class platform at both build and runtime, which keeps plugins and
cross-platform apps clean.

### Highlights

- 🛠️ **A drop-in CLI** — the `flutter` commands you know (`create`, `run`, `build`, `doctor`), retargeted to watchOS.
- ⚡ **Hot reload & DevTools** — the same inner loop, on the watchOS Simulator.
- ⌚ **Real Apple Watch** — build and run on a paired watch in profile or release.
- 🧩 **watchOS is its own platform** — first-class at build and runtime, so plugins and cross-platform apps stay clean.

### Get started

```sh
# 1. install the toolchain
git clone https://github.com/flutterwatch/flutter-watchos.git
cd flutter-watchos && export PATH="$PATH:$PWD/bin"

# 2. connect your account + fetch the engine
flutter-watchos login
flutter-watchos precache && flutter-watchos doctor

# 3. build your first watch app
flutter-watchos create hello_watch
cd hello_watch && flutter-watchos run
```

Joining the closed beta is self-serve: sign in with GitHub at
**[api.flutterwatch.dev](https://api.flutterwatch.dev/)** and you're in
immediately. Beta accounts build and run in debug and profile modes.

### Repositories

| Repository | What it is |
| --- | --- |
| [**flutter-watchos**](https://github.com/flutterwatch/flutter-watchos) | The CLI, templates, and documentation. |
| [flutter_watchos](https://pub.dev/packages/flutter_watchos) | First-party plugin — platform detection, device info, haptics, and the Digital Crown ([on pub.dev](https://pub.dev/packages/flutter_watchos)). |

<br/>

<p align="center"><sub>
  Not affiliated with or endorsed by Google or Apple. Flutter is a trademark of
  Google&nbsp;LLC; Apple&nbsp;Watch and watchOS are trademarks of Apple&nbsp;Inc.
</sub></p>
