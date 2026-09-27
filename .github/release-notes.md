> **Unofficial community build.** This is not an official Auxilor release.
> EcoEnchants is a premium plugin; this jar is self-built from source, which is
> permitted under the [GNU GPLv3](https://github.com/f1shsmell/EcoEnchants/blob/master/LICENSE.md)
> license of this repository.

## Provenance (GPLv3 §6 compliance)

- **Corresponding source (exact commit built):** the tagged commit of this fork
- **Upstream project:** https://github.com/Auxilor/EcoEnchants
- **Bundled `libreforge` (also GPLv3):** https://github.com/Auxilor/libreforge

## Changes vs upstream

- Fixed a Gradle task-ordering race (`relocatedLibreforgeJar` vs `clean` →
  `cleanLibreforgeJar`) that silently produced jars without the bundled
  libreforge, causing `LibreforgeNotFoundError` on startup.
- Restored the upstream build configuration (removed a placeholder local jar)
  and made CI build reliably.

## Install

1. Requires the **eco** plugin of the same version on the server
   (https://github.com/Auxilor/eco).
2. Drop the jar into `plugins/` and restart.

Licensed under GPLv3. No additional restrictions are imposed on downstream
recipients.
