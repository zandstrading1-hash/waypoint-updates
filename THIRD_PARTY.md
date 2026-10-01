# Native dependency notices

The native Waypoint prototype in this directory is provided under AGPL-3.0-only; see `LICENSE`. This does not change the licensing of unrelated dependencies or automatically relicense the separate Python controller.

The connection/ownership sequence in `WaypointPhone/DeviceBridge.swift` is adapted from StikDebug's `StikDebug/Device/IdeviceFFIBridge.swift`, tag **3.1.13**, commit **4bdfc92aa7cebd7a534f1e1ef56415f5727402de**. Copyright remains with the StikDebug contributors; upstream is AGPL-3.0. This file was modified to use a private instance, a single serial command queue, an explicit restore-without-set path, and sanitized failures.

- [Pinned StikDebug source](https://github.com/StikDebug/StikDebug/tree/4bdfc92aa7cebd7a534f1e1ef56415f5727402de)
- [Upstream license](https://github.com/StikDebug/StikDebug/blob/4bdfc92aa7cebd7a534f1e1ef56415f5727402de/LICENSE)
- [idevice source and MIT license](https://github.com/jkcoxson/idevice)

`build.py` retrieves the `idevice.h`, `module.modulemap`, and `libidevice_ffi.a` artifacts committed in that exact StikDebug revision and checks their SHA-256 hashes. The library implements the underlying Apple protocols; these were not independently reinvented. The native build uses Apple's SwiftUI, MapKit, Core Location and system SDK frameworks.

If distributing this derivative, retain these notices and the license and provide the corresponding source and build materials as required by applicable licenses. No signed app, Apple certificate, or pairing record is included in this source tree.
