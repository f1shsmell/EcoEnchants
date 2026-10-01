> **Unofficial community build / 非官方社区构建.** This is not an official Auxilor release.
> EcoEnchants is a premium plugin; this jar is self-built from source, which is
> permitted under the [GNU GPLv3](https://github.com/f1shsmell/EcoEnchants/blob/master/LICENSE.md)
> license of this repository.

## Provenance (GPLv3 §6 compliance)

- **Corresponding source (exact commit built):** the tagged commit of this fork
- **Upstream project:** https://github.com/Auxilor/EcoEnchants
- **Bundled `libreforge` (also GPLv3):** https://github.com/Auxilor/libreforge

## Changes vs upstream

- **Full Simplified Chinese (zh-CN) localization:**
  - 102 custom enchant names & descriptions (incl. EcoJobs/EcoPets/EcoSkills integrations)
  - 44 vanilla enchant names & descriptions (official Minecraft zh-CN terms)
  - Rarity names, applicable-item names, `/enchant` GUI, `/enchantinfo`, group menu, command messages
- README rewritten with a full EN-ZH name reference and effect summaries
- `lumberjack`: added pale oak wood/log to mineable blocks
- Fixed a Gradle task-ordering race (`relocatedLibreforgeJar` vs `clean` →
  `cleanLibreforgeJar`) that silently produced jars without the bundled
  libreforge, causing `LibreforgeNotFoundError` on startup.

## Install

1. Requires the **eco** plugin of the same version on the server
   (https://github.com/Auxilor/eco).
2. Drop the jar into `plugins/` and restart.

## 安装说明(简体中文)

1. 服务端需安装同版本的前置插件 **eco**(Paper 1.21.8+ / Folia,Java 21+)。
2. 将 jar 放入 `plugins/` 目录并重启即可。
3. 所有译名均为配置文本,可在 `plugins/EcoEnchants/` 对应 yml 中自行修改后执行 `/ecoenchants reload` 热重载。

Licensed under GPLv3. No additional restrictions are imposed on downstream
recipients.
