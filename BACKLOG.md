# Add-on backlog

Open add-on packaging work. Earnie product features stay in [JochenTCC/Earnie `backlog/Backlog.md`](https://github.com/JochenTCC/Earnie/blob/main/backlog/Backlog.md).

- [ ] **Stable vs pre-release channel.** Decided 2026-09-26, planned as Earnie **2.6.k** ([Backlog](https://github.com/JochenTCC/Earnie/blob/main/backlog/Backlog.md)): second add-on `earnie_prerelease` („Earnie (Vorabversion)“) next to `earnie`. Stable releases bump both, pre-releases only `earnie_prerelease`. Config moves to `addon_config` (`/config`) so users can copy it between the two; must ship in `earnie` first. Stopgap in **2.6.j**: pre-releases stop bumping `earnie`. Concept: [Earnie-Installation-Haertung-Entwicklungsdokument.md §3.3–3.4](https://github.com/JochenTCC/Earnie-Projekt/blob/main/Entwicklungsplan/Earnie-Installation-Haertung-Entwicklungsdokument.md).
