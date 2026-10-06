# Dobber Home Assistant Wallmount Dashboard

A custom Home Assistant wallmount dashboard with a modern glass-style interface for lighting, climate, media, cameras, energy, calendar, waste collection and security.

## Features

- Responsive wallmount layout
- Glass-style interface
- Lighting control with scenes and popups
- Climate / air-conditioning controls
- Live camera views
- Sonos / media controls
- Energy and solar information
- Calendar overview
- Waste collection cards
- Alarm / security overview
- Custom bottom navigation
- Screensaver support

## Installation

1. Install the required custom cards through HACS.
2. Create a new Home Assistant dashboard.
3. Open the Raw Configuration Editor.
4. Copy the contents of `dashboard.yaml` into the dashboard.
5. Replace the example entity IDs with your own Home Assistant entities.
6. Add your own dashboard background at `/config/www/dashboard-background.png` or change the background path in the YAML.

## Required custom cards / integrations

This dashboard uses custom Home Assistant frontend components such as:

- Button Card
- Mushroom
- Layout Card
- Mini Graph Card
- Mini Media Player
- Stack In Card
- Auto Entities
- Atomic Calendar Revive
- Advanced Camera Card
- Card Mod
- Browser Mod

Depending on your setup, additional integrations may be required for specific entities such as SolarEdge, Alarmo, cameras, waste collection, climate devices or media players.

## Entity IDs

The published configuration contains example entity IDs. Replace them with the corresponding entities from your own Home Assistant installation.

Common examples include:

```yaml
light.woonkamer
light.keuken
climate.airco_beneden
camera.oprit
calendar.personal
sensor.p1_actueel_vermogen
sensor.afval_gft
```

## Spotify playlists

The YAML contains placeholder Spotify playlist IDs:

```text
YOUR_PARTY_PLAYLIST_ID
YOUR_CHILL_PLAYLIST_ID
YOUR_LOUNGE_PLAYLIST_ID
```

Replace these with your own playlist IDs if you use those controls.

## Background image

The public version expects a background image at:

```text
/config/www/dashboard-background.png
```

which is referenced from Lovelace as:

```text
/local/dashboard-background.png
```

The original personal background image is intentionally not included.

## Privacy

This repository is intended to contain dashboard configuration only. Do not commit passwords, API keys, access tokens, webhook secrets, private URLs, MQTT credentials or personal camera snapshots.

## Notes

This dashboard was built for a specific Home Assistant environment, so some configuration changes will always be necessary before it works in another installation.

## License

MIT License. See `LICENSE`.