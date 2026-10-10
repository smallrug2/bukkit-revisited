# Bukkit-Revisited

A maintained revival fork of the classic Bukkit Minecraft server API —
preserved, audited, and fixed, with full credit to the original creators.

## Why this exists (not a copy — a revival)

The original Bukkit project (2011–2014) changed Minecraft server history
and then went quiet; its repository is archival and its old issue tracker
is gone. This fork exists to **keep that code alive and maintained**:
preserving it exactly as it was, documenting a real security audit of it,
and landing small, careful fixes on top. Every original file, credit, and
license term is preserved untouched — see "Credits & license" below. What
changes here is tracked line-by-line in `CHANGELOG.md`, newest first.

If you want to *play or host*, use a living implementation (Spigot, Paper,
Purpur) — an API without an engine runs nothing, and version support lives
in implementations, not here. If you want to *study, audit, or preserve*
the API that started it all, you're home.

## The original README, preserved verbatim

> Bukkit
> ======
>
> A Minecraft Server API.
>
> Website: [http://bukkit.org](http://bukkit.org)
> Bugs/Suggestions: [http://leaky.bukkit.org](http://leaky.bukkit.org)
> Contributing Guidelines: [CONTRIBUTING.md](https://github.com/Bukkit/Bukkit/blob/master/CONTRIBUTING.md)
>
> Compilation
> -----------
>
> We use maven to handle our dependencies.
>
> * Install [Maven 3](http://maven.apache.org/download.html)
> * Check out this repo and: `mvn clean install`

(Full original also kept as `README-ORIGINAL.md`. Note: bukkit.org and
leaky.bukkit.org are historical links from 2014 and may no longer resolve.)

## What this fork adds

- `CHANGELOG.md` — every fork change, newest first (currently: fork
  scaffold + security audit Round 1 + one clarity fix, zero behavior change).
- A documented 642-file security audit: YAML loading confirmed safe,
  permission defaults fail-closed, metadata threading reviewed OK,
  deserialization allow-listed, no exec/XXE/raw-deserialization surface.
- Ongoing small fixes, one commit each, never touching credits or license.

## Credits & license — read this, it matters

- **All source code: the original Bukkit team and contributors.** Every
  copyright notice, author credit, CONTRIBUTING.md term, and file history
  is preserved exactly as published. Nothing was stripped or rebranded.
- **License: GPLv3 (`LICENCE.txt`), unchanged as the license requires.**
  This fork — like any lawful fork — stays GPLv3, so anyone may use, study,
  share, and further fork it under the same terms.
- **Fork maintenance & audit:** smallrug2, with audit work by Muse Spark.
  New work only; no claim on the original code.
- Not affiliated with or endorsed by the original Bukkit project, SpigotMC,
  or Mojang. Not an official Bukkit release.

## Contents & building

- `src/` — original API sources, credits intact
- `CHANGELOG.md`, `README-ORIGINAL.md`, `PUSH-GUIDE.txt`
- Standard Maven layout (`pom.xml`); period dependencies may need
  mirroring on modern setups.
