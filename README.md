# Earnie Add-ons — Home Assistant

Custom Add-on-Repository für [Earnie](https://github.com/JochenTCC/Earnie) (Energiemanagement und Optimierung für Smart Homes), primär für **Home Assistant Green** (HA OS, `aarch64`).

Dieses Repository ist nicht Teil der offiziellen Home-Assistant-Community-Add-on-Liste. Entwicklungsquelle und Issue-Tracker sind das Hauptrepo [JochenTCC/Earnie](https://github.com/JochenTCC/Earnie) — dieses Repo wird bei Releases aus `packaging/homeassistant-addon/earnie/` dort synchronisiert (`sync-to-ha-addon-repo.sh`).

## Installation

1. Home Assistant → **Einstellungen → Add-ons → Add-on Store**.
2. Oben rechts ⋮ → **Repositories**.
3. URL hinzufügen: `https://github.com/JochenTCC/ha-addon-earnie`.
4. **Earnie** in der Liste öffnen → **Installieren**.

Ausführliche Anwenderdokumentation: [docs/einrichtung/homeassistant-addon.md](https://github.com/JochenTCC/Earnie/blob/main/docs/einrichtung/homeassistant-addon.md) im Hauptrepo.

## Add-ons in diesem Repository

| Add-on | Beschreibung |
|---|---|
| [Earnie](earnie/) | Energiemanagement und Optimierung für Smart Homes — Wrapper um `ghcr.io/jochentcc/earnie-energy` |

## Lizenz

Siehe [LICENSE.md](LICENSE.md) — Source-Available, nicht-kommerzielle Lizenz (identisch zum Hauptrepo).
