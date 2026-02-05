# ServerMappings

Dieses Repository enthält Server-Informationen für die Discord Rich Presence des WhiteRose Clients.

## Struktur

```json
[
  {
    "name": "ServerName",
    "addresses": ["server.de", "play.server.de", "*.server.de"],
    "discord_large_image": "server_logo",
    "discord_small_image": "large",
    "discord_details": "ServerName",
    "discord_state_format": "{players}/{max} Spieler"
  }
]
```

## Felder

| Feld | Beschreibung | Erforderlich |
|------|--------------|--------------|
| `name` | Name des Servers | Ja |
| `addresses` | Liste von Server-Adressen (unterstützt Wildcards mit `*`) | Ja |
| `discord_large_image` | Asset-Name für das große Discord-Bild | Nein (Standard: `large`) |
| `discord_small_image` | Asset-Name für das kleine Discord-Bild | Nein (Standard: `multiplayer`) |
| `discord_details` | Text für die Discord-Details | Nein (Standard: `name`) |
| `discord_state_format` | Format für den State-Text. Platzhalter: `{players}`, `{max}` | Nein (Standard: `{players}/{max}`) |

## Server hinzufügen

### Anforderungen für neue Server

1. Forke dieses Repository
2. Füge deinen Server zur `servers.json` hinzu
3. Erstelle einen Pull Request
