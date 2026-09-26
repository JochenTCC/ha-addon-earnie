# Earnie Add-ons — Home Assistant

Custom Add-on-Repository für [Earnie](https://github.com/JochenTCC/Earnie) (Energiemanagement und Optimierung für Smart Homes), primär für **Home Assistant Green** (HA OS, `aarch64`).

Dieses Repository ist nicht Teil der offiziellen Home-Assistant-Community-Add-on-Liste. Entwicklungsquelle und Issue-Tracker sind das Hauptrepo [JochenTCC/Earnie](https://github.com/JochenTCC/Earnie).

**Auto-publish:** Offizielle Earnie-Release-Tags (`vX.Y.Z`, ohne alpha/rc) triggern in Earnie den Job `publish_ha_addon`, der `packaging/homeassistant-addon/earnie/` hierher spiegelt. Vorabversionen (alpha/rc) erscheinen auf GHCR, aktualisieren dieses Repository aber **nicht** (Stopgap H12 / Earnie **2.6.j**). Add-on-`version:` entspricht der Earnie-App-Version. Manueller Sync: `sync-to-ha-addon-repo.sh` im Hauptrepo (nur offizielle Versionen).

## Installation

1. Home Assistant → **Einstellungen → Add-ons → Add-on Store**.
2. Oben rechts ⋮ → **Repositories**.
3. URL hinzufügen: `https://github.com/JochenTCC/ha-addon-earnie`.
4. **Earnie** in der Liste öffnen → **Installieren**.

Ausführliche Anwenderdokumentation: [docs/einrichtung/homeassistant-addon.md](https://github.com/JochenTCC/Earnie/blob/main/docs/einrichtung/homeassistant-addon.md) im Hauptrepo.

Offene Add-on-Themen (nicht Earnie-Produktfeatures): [BACKLOG.md](BACKLOG.md).

## Add-ons in diesem Repository

| Add-on | Beschreibung |
|---|---|
| [Earnie](earnie/) | Energiemanagement und Optimierung für Smart Homes — Wrapper um `ghcr.io/jochentcc/earnie-energy` |

## CI

Push/PR auf `main`: [`.github/workflows/hassfest.yml`](.github/workflows/hassfest.yml) (Add-on-Lint via `frenck/action-addon-linter`).

## Lizenz

Siehe [LICENSE.md](LICENSE.md) — Source-Available, nicht-kommerzielle Lizenz (identisch zum Hauptrepo).
