# Changelog — Bukkit-Revisited (fork of Bukkit/Bukkit, GPLv3)

All dates 2026. Original code © the Bukkit team and contributors.

## [Unreleased]
### Added
- Fork scaffold: renamed README, this changelog, full audit report
  (`../bukkit-audit-report.md` in the curator's workspace).
- Security audit Round 1 (642 files): YAML loading confirmed SafeConstructor
  everywhere; permission defaults confirmed fail-closed (OP); metadata store
  threading reviewed OK; deserialization sink allow-listed to registered
  aliases; no exec/XXE/raw-deserialization surface found.
### Fixed
- `org.bukkit.util.io.BukkitObjectInputStream.resolveObject`: replaced the
  cryptic trailing `// NPE` comment with an explanation of the intentional
  null-check (see commit). No behavior change — clarity only.

## [Upstream] — everything before this line is original Bukkit history
- Last upstream commit: 2014-08-17 ("Update JavaDocs regarding
  teleportation of entities", BUKKIT-4210). Preserved as-is.
