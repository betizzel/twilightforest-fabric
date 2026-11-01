Twilight Forest Unofficial
==============

This repository preserves the existing [Twilight Forest Unofficial Fabric port](https://github.com/marlester-dev/twilightforest-unofficial), not a new port. Its source is based on upstream `1.20.1-fabric` commit `df09491a18afc5cf4c6f2aa26536896afe2670cf`, whose version is 1.4.7 for Minecraft 1.20.1. This January 2025 revision postdates the December 2024 published 1.4.7 binary and includes later changes; it is not verified as the source of that binary or a bit-identical rebuild.

### Building this fork

Use JDK 17 and the included Gradle 8.8 wrapper: `./gradlew build` (Windows: `gradlew.bat build`). The build downloads Minecraft, mappings, Loom and dependencies from the repositories configured in the upstream build; it also consults Maven Local, so local artifacts can affect reproducibility. The expected remapped mod is `build/libs/twilightforest-fabric-1.20.1-1.4.7.jar`. The upstream data-generation run is `./gradlew runDatagen` and writes to `src/generated/resources`. No build or binary equivalence is claimed here.

The fork's mapping configuration uses official Mojang mappings as the base followed by Parchment. Upstream's Quilt/Parchment/official ordering produced an invalid mapped Minecraft compile jar with Loom 1.7.4; this change has not yet been build-verified.

The upstream LICENSE distinguishes LGPL-2.1 code from CC BY-NC-SA 4.0 non-code assets and describes sound-specific exceptions and uncertainty. Preserve its notices, attribution, noncommercial and share-alike conditions where applicable; do not assume every sound has the same license.

This is the github page of the Twilight Forest Unofficial mod

## Licensing
See the LICENSE file

## Downloads
Releases will be available on [CurseForge](https://www.curseforge.com/minecraft/mc-mods/the-twilight-forest-unofficial/files) when ready.

## Community
Keep in touch with development on our [Discord server](https://discord.gg/qySFRKMzkY).

## Translating
Submitting translations for Twilight Forest Unofficial can be done via creating a pull request. All translations are in [this](https://github.com/marlester-dev/twilightforest-fabric-1201/tree/HEAD/src/main/resources/assets/twilightforest/lang) folder.
