# REDREAM — Minecraft Java Launcher for Android

REDREAM is being developed as an Android launcher for Minecraft: Java Edition with a custom black/red interface.

## Current repository status

- The app/ directory contains the REDREAM UI prototype (WebView-based).
- .github/workflows/build-engine.yml builds an arm64 debug APK from the upstream ZalithLauncher2/PojavLauncher engine with REDREAM app-name configuration.
- The engine APK is an intermediate build: the custom REDREAM interface is not yet integrated into the game engine. The existing WebView prototype does not launch Minecraft by itself.
- Modrinth catalog, actual installation into a game profile, Microsoft/Ely.by account flow, and skin synchronization still need to be connected to the engine before they can be called complete.

## Build the engine APK

1. Open the repository's Actions tab.
2. Select Build REDREAM game engine.
3. Press Run workflow and wait for the job to finish.
4. Download the artifact REDREAM-engine-arm64-debug from the completed run.

This artifact is built from the upstream ZalithLauncher2 project and is an unofficial modified build. Upstream source and license: https://github.com/ZalithLauncher/ZalithLauncher2

## Planned integration work

1. Bring the engine source into this repository while preserving its upstream notices and GPL-3.0 obligations.
2. Replace the engine's launcher screens with the REDREAM black/red UI.
3. Connect real version installation and launch, profiles, mod/modpack downloads, and supported authentication.
4. Build and test the integrated APK on an Android device.

The engine workflow is a build step, not a claim that all planned REDREAM features are already implemented.
