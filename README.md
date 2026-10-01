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

## 0.1.6 (8)

Adds a four-second local connection check without changing location. Includes
continuous area walking, a full-height scrolling options panel, and corrected
Light/Dark appearance. Compilation and native logic checks passed. Seven existing simulator flows passed
on the first diagnostic candidate; the corrected candidate passed its focused
connection cancellation/result test. The pending Cancel control was visually
reviewed. Physical performance and cellular operation still need testing.
This build does not fix cellular startup or cellular restoration. Force-quitting
the app is not supported for continued holding.

The matching source archive includes build scripts, Swift code and checks,
artwork, dependency pins and license notices. SHA256SUMS.txt identifies all
distribution files. This is not an App Store-signed application.
