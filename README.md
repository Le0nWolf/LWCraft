# LWCraft — Vanilla‑Feeling, nur deutlich smoother 🎮

<p align="center">
  <img alt="LWCraft Logo" src="./assets/logo.png" width="140" />
</p>

<p align="center">
  <a href="https://img.shields.io"><img alt="Minecraft" src="https://img.shields.io/badge/Minecraft-1.21.8-34aa2f?logo=minecraft" /></a>
  <a href="#systemanforderungen-🔧"><img alt="Mod‑Loader" src="https://img.shields.io/badge/Loader-Fabric-blue" /></a>
  <a href="https://adoptium.net/"><img alt="Java" src="https://img.shields.io/badge/Java-21-007396?logo=openjdk" /></a>
  <a href="https://github.com/Le0nWolf/LWCraft/releases"><img alt="Releases" src="https://img.shields.io/github/v/release/Le0nWolf/LWCraft?display_name=tag" /></a>
  <a href="https://github.com/Le0nWolf/LWCraft/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/Le0nWolf/LWCraft/total" /></a>
  <a href="./LICENSE"><img alt="Lizenz" src="https://img.shields.io/badge/License-TODO-lightgrey" /></a>
</p>

> **TL;DR:** **LWCraft** ist ein **client‑seitiges** Modpack für **Vanilla‑Gameplay mit besserer Performance und Komfort**. Keine neuen Items oder Rezepte – nur flüssiger, klarer, immersiver.

---

## Inhaltsverzeichnis

* [Überblick](#überblick)
* [Systemanforderungen 🔧](#systemanforderungen-🔧)
* [Features 🚀](#features-🚀)
* [Mod‑Liste 📦](#mod‑liste-📦)
* [Installation (Client) 🛠️](#installation-client-🛠️)
* [Server‑Setup 🖥️](#server-setup-🖥️)
* [Konfiguration ⚙️](#konfiguration-⚙️)
* [Kompatibilität & Performance 🧪](#kompatibilität--performance-🧪)
* [Screenshots / Trailer 🖼️](#screenshots--trailer-🖼️)
* [Roadmap 🧭](#roadmap-🧭)
* [Changelog 🔄](#changelog-🔄)
* [FAQ & Troubleshooting ❓🧯](#faq--troubleshooting-❓🧯)
* [Beitrag & Community 🤝💬](#beitrag--community-🤝💬)
* [Lizenz & Credits 📜🙏](#lizenz--credits-📜🙏)
* [Sicherheit & Telemetrie 🔒📊](#sicherheit--telemetrie-🔒📊)
* [Lokalisierung 🌐](#lokalisierung-🌐)
* [Pre‑Commit Checkliste](#pre-commit-checkliste)

---

## Überblick

**Ziel:** Vanilla‑Erlebnis beibehalten und **spürbar smoother** machen – schnellere Ladezeiten, mehr FPS, feinere UI/Audio‑Details und nützliche Komfortfunktionen (alles **client‑seitig**).

* **Spielgefühl:** Vanilla+, QoL, Immersion, Performance.
* **Keine Content‑Mods:** Fügt **keine** neuen Items/Rezepte hinzu.

## Systemanforderungen 🔧

* **Minecraft:** `1.21.8`
* **Mod‑Loader:** `Fabric` (Version: `TODO`)
* **Java:** `21` (Empfehlung: Temurin/OpenJDK)
* **RAM‑Hinweis:** *Mehr RAM ist in der Regel besser.*
* **Shader‑Support:** Empfohlen via **Iris** (optional)

## Features 🚀

**Performance**

* Moderne Client‑Optimierungen (z. B. *Sodium‑Ökosystem*), schnellere Ladezeiten, weniger Stottern.

**Quality of Life**

* Bessere Tooltips & Anzeigen (z. B. Hunger/HP/Toolhaltbarkeit), clevere Maus‑/Inventar‑Bedienung, übersichtlichere F3‑Infos.

**Immersion**

* Atmosphärische Umgebungs‑Sounds, Raumklang, dezente Partikeleffekte und UI‑Verbesserungen.

## Mod‑Liste 📦

**Top‑Auswahl (Ausschnitt)**

* BetterF3 • AppleSkin • Mouse Tweaks • Sound Physics Remastered • AmbientSounds
* Particular ✨ Reforged (+ CaveDust) • Immersive UI • Pick Up Notifier • Durability Tooltip
* Smooth Scrolling • Client Tweaks • Locator Heads • Detail Armor Reconstructed • Cut Through
* Distant Horizons *(optional; siehe Performance‑Hinweis)*

**Vollständige Liste**

* Siehe [`mods.md`](./docs/mods.md) *(wird automatisch aus `packwiz` generiert)*.


## Installation (Client) 🛠️

**Bevorzugter Launcher:** **Prism Launcher**

### Option A: Import (.zip / .mrpack)

1. Lade das aktuelle Release von der Seite **[Releases](https://github.com/Le0nWolf/LWCraft/releases)** (`.mrpack` **oder** `.zip`).
2. Prism → **Instanzen** → **Importieren** → Datei wählen → **OK**.
3. Starte die Instanz. Erster Start kann etwas länger dauern.


## Server‑Setup 🖥️

> **Status:** Derzeit **kein** separates Server‑Pack; LWCraft ist **client‑seitig** ausgerichtet.

Allgemeines Vorgehen (falls du doch testweise hosten willst):

1. **EULA** akzeptieren (`eula=true`).
2. **Fabric‑Server‑Jar** für die passende MC‑Version bereitstellen.
3. Nur **client‑kompatible** Mods verwenden (keine reinen Server‑Mods nötig).

**Linux (bash)**

```bash
#!/usr/bin/env bash
set -euo pipefail
JAVA=java
ARGS=("-Xms2G" "-Xmx2G" "-XX:+UseG1GC" "-jar" "server.jar" "nogui")
$JAVA "${ARGS[@]}"
```

**Windows (PowerShell)**

```powershell
$java = "java"
$args = "-Xms2G -Xmx2G -XX:+UseG1GC -jar server.jar nogui"
& $java $args
```

## Konfiguration ⚙️

* **Wichtige Pfade:** `config/`, `options.txt`, `shaderpacks/`, `resourcepacks/`
* **Empfohlene Presets:** Sichtweite moderat; Partikel reduziert; Iris‑Profil je nach GPU
* **Keybinds:** Nach Installation auf Konflikte prüfen (In‑Game → *Kontrollen*)

## Kompatibilität & Performance 🧪

* **OptiFine:** Nicht empfohlen → **Sodium** (+ **Iris** für Shader) nutzen.
* **Distant Horizons:** Nur bei stabiler Performance aktivieren; bei FPS‑Drops **deaktivieren**.
* **Treiber/Java:** Java 21 nutzen, Grafiktreiber aktuell halten.

## Screenshots / Trailer 🖼️

| Szene | Bild                                                                   |
| ----: | :--------------------------------------------------------------------- |
| Spawn | ![Spawn‑Screenshot](./assets/screenshots/spawn.png "Spawn‑Ausschnitt") |


## Roadmap 🧭

* [ ] Erste öffentliche Release
* [ ] Automatisierte Mod‑Liste über `packwiz`
* [ ] Discord Community

## Changelog 🔄

* Siehe **[Releases](https://github.com/Le0nWolf/LWCraft/releases)** und Tags.
* (Optional) Später via **commitizen**/Conventional Commits automatisieren.

## FAQ & Troubleshooting ❓🧯

**„Mismatch Mod‑Loader“**

* Prüfe Fabric‑Version und MC‑Version im Launcher.

**„Out of Memory“ / Crash beim Laden**

* *Mehr RAM ist in der Regel besser.* Schließe Browser/Programme; Shader testweise deaktivieren.

**„Ruckler mit Distant Horizons“**

* Feature vorübergehend deaktivieren oder Sichtweite/LoD reduzieren.

**Crash‑Logs einsenden**

* `latest.log` und `crash-reports/*.txt` anhängen. Minimal‑Repro: nur Pflicht‑Mods.

## Beitrag & Community 🤝💬

* PRs willkommen! Siehe [`CONTRIBUTING.md`](./CONTRIBUTING.md) und [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md).
* Issues & Vorschläge: **[Issue‑Tracker](https://github.com/Le0nWolf/LWCraft/issues/new/choose)**
* Discord: *(geplant)*

## Lizenz & Credits 📜🙏

* **Lizenz (Pack):** `TODO: SPDX-ID`
* **Assets:** Logo/Screenshots `TODO`; Lizenzen angeben.
* **Dank an**: Maintainer von Sodium, Iris, BetterF3, AppleSkin & Co.

## Sicherheit & Telemetrie 🔒📊

* **Crash‑Reports:** Lokal gespeichert; Upload nur durch dich.
* **Telemetry:** Nicht vorgesehen (falls doch: Opt‑out dokumentieren).
