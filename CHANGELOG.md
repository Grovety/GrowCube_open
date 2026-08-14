# Changelog

## 4.3 — 2026-08-14

- Fixed the static humidity reading on the graph screen. The current value now updates correctly.
- Removed manual “air watering.” If watering is attempted while the tank is empty, GrowCube now performs an emergency stop.
- Added channel letters to the plant graph screen.
- Fixed graph caching. The latest received state is now stored correctly and is no longer replaced by an outdated graph with gaps after reopening the screen.
- Added local IP addresses for GrowCube devices. They are currently always visible; conditional display is being considered, for example after tapping the device name three times.
- Ruled out a software cause for unusually stable humidity readings. If this behavior is an issue, it is hardware-related.
- Fixed the tank level not decreasing correctly. An `unknown` value sent before GrowCube determines the water level is now handled properly instead of being replaced with the previously saved value.
