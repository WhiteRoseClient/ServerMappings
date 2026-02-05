# ServerMappings

### Anforderungen für neue Server

3. Erstelle einen Pull Request
2. Füge deinen Server zur `servers.json` hinzu
1. Forke dieses Repository

## Server hinzufügen

| `discord_state_format` | Format für den State-Text. Platzhalter: `{players}`, `{max}` | Nein (Standard: `{players}/{max}`) |
| `discord_details` | Text für die Discord-Details | Nein (Standard: `name`) |
| `discord_small_image` | Asset-Name für das kleine Discord-Bild | Nein (Standard: `multiplayer`) |
| `discord_large_image` | Asset-Name für das große Discord-Bild | Nein (Standard: `large`) |
| `addresses` | Liste von Server-Adressen (unterstützt Wildcards mit `*`) | Ja |
| `name` | Name des Servers | Ja |
|------|--------------|--------------|
| Feld | Beschreibung | Erforderlich |

## Felder

```
]
  }
    "discord_state_format": "{players}/{max} Spieler"
    "discord_details": "ServerName",
    "discord_small_image": "large",
    "discord_large_image": "server_logo",
    "addresses": ["server.de", "play.server.de", "*.server.de"],
    "name": "ServerName",
  {
[
```json

Die Datei `servers.json` enthält alle unterstützten Server im folgenden Format:

## Struktur

Dieses Repository enthält Server-Informationen für die Discord Rich Presence des WhiteRose Clients.


