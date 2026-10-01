# Waypoint updates

Personal experimental iPhone app. This repository distributes unsigned builds,
their matching source, and a SideStore feed. No pairing files or Apple credentials
are included. Signing remains on your phone.

## Add once in SideStore

In SideStore, open Sources, tap +, and paste this source address:

```
https://raw.githubusercontent.com/zandstrading1-hash/waypoint-updates/main/source.json
```

Then use Waypoint's Update button in SideStore. This should remove USB and Files
selection from subsequent updates. The first update's adoption of an existing
installation still needs on-phone verification. Do not delete the existing app.

Use Wi-Fi with LocalDevVPN connected. Before updating, Stop & restore in Waypoint
and independently check Maps, Find My, and nearby accessories. Refresh both
Waypoint and SideStore before their seven-day signing countdown expires.

## 0.1.7 (9)

Adds one consent screen before the map with an **OK, I consent** button.
Acceptance is stored only on your phone and remembered after relaunch. No new
account, hosted consent service, telemetry or permissions are added. Light and
dark appearance are supported; recovery controls remain available for a pending
restoration. The device connection and location engine are unchanged.

Compilation, native logic checks and three focused simulator UI tests passed:
consent in both themes, acceptance and relaunch persistence, map/search access,
and pending restoration access. Physical installation and wireless update
adoption still need on-phone verification. Cellular startup/restoration remain
unreliable, and force-quitting the app is not supported for continued holding.

The matching source archive includes build scripts, Swift code and checks,
artwork, dependency pins and license notices. SHA256SUMS.txt identifies all
distribution files. This is not an App Store-signed application.
