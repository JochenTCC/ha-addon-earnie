# Earnie Add-ons — Home Assistant

Custom Add-on-Repository für [Earnie](https://github.com/JochenTCC/Earnie) (Energiemanagement und Optimierung für Smart Homes), primär für **Home Assistant Green** (HA OS, `aarch64`).

Dieses Repository ist nicht Teil der offiziellen Home-Assistant-Community-Add-on-Liste. Entwicklungsquelle und Issue-Tracker sind das Hauptrepo [JochenTCC/Earnie](https://github.com/JochenTCC/Earnie).

**Auto-publish:** Earnie-Release-Tags triggern `publish_ha_addon`:
- Offiziell (`vX.Y.Z`) → spiegelt `earnie/` **und** `earnie_prerelease/`
- Vorab (`vX.Y.Z-alpha.N` / `-rc.N`) → nur `earnie_prerelease/`

Prebuilt Images: `ghcr.io/jochentcc/earnie-addon-{arch}:<version>` (`image:` in `config.yaml`). Manueller Sync: `sync-to-ha-addon-repo.sh` im Hauptrepo.

## Installation

1. Home Assistant → **Einstellungen → Apps** (bis HA 2026.1: Add-ons) → ⋮ → **Repositories**.
2. URL hinzufügen: `https://github.com/JochenTCC/ha-addon-earnie`.
3. **Earnie** (Stabil) oder **Earnie (Vorabversion)** öffnen → **Installieren**.

Ausführliche Anwenderdokumentation: [docs/einrichtung/homeassistant-addon.md](https://github.com/JochenTCC/Earnie/blob/main/docs/einrichtung/homeassistant-addon.md) — Abschnitt „Stabile Version oder Vorabversion“.

Offene Add-on-Themen: [BACKLOG.md](BACKLOG.md).

## Add-ons in diesem Repository

| Add-on | Beschreibung |
|---|---|
| [Earnie](earnie/) | Stabile Version — offizielle Releases |
| [Earnie (Vorabversion)](earnie_prerelease/) | Community-Test (Alpha/RC); nie parallel zum stabilen Add-on starten |

## CI

Push/PR auf `main`: [`.github/workflows/hassfest.yml`](.github/workflows/hassfest.yml) (Add-on-Lint via `frenck/action-addon-linter`).

## Lizenz

Siehe [LICENSE.md](LICENSE.md) — Source-Available, nicht-kommerzielle Lizenz (identisch zum Hauptrepo).
