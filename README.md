# Swashbucklers! — Fabric 26.1.2 Compatibility Port

[![Build](https://github.com/ModPorterMC/swashbucklers-fabric-port/actions/workflows/build.yml/badge.svg)](https://github.com/ModPorterMC/swashbucklers-fabric-port/actions/workflows/build.yml)

An unofficial Fabric compatibility port of **Swashbucklers!** targeting **Minecraft 26.1.2**.

This repository documents the technical work involved in adapting the mod to a modern Fabric environment, including rendering, networking, ship behavior, data resources, and automated validation.

## Target Environment

- Minecraft 26.1.2
- Fabric Loader 0.19.3
- Fabric API 0.155.2+26.1.2
- Java 25
- Fabric Loom 1.17-SNAPSHOT
- Gradle 9.5.1 in CI

## Porting Work

- Fabric project and build configuration
- Ship entity registration
- Client renderer registration and model integration
- Client-to-server ship input networking
- Ship steering and control-state handling
- Buoyancy and ship physics adaptation
- Waterline and visual positioning corrections
- Rider / seat positioning fixes
- Recipes, advancements, tags, and datapack resources
- Automated production client/server validation with GitHub Actions

## Validation

GitHub Actions validates:

- Distributable datapack resources
- Ship entity persistence
- Boat tags
- Ship buoyancy
- Model and renderer registration
- Waterline positioning
- Steering behavior
- Control direction
- Corvette rider-seat alignment

## Building

Requires **Java 25**.

```bash
gradle build
```

The build process retrieves the original **Swashbucklers! 2.6.6B NeoForge 1.21.4** JAR through CurseMaven so original client assets and model data can be prepared during the build.

## Original Project & Rights

**Swashbucklers!** is originally authored by **Halbear**.

The original mod metadata identifies its license as **All Rights Reserved**.

This compatibility-port repository does not grant any additional rights to the original mod's code, textures, models, or other assets.

Because the build process references original Swashbucklers assets, redistribution of compiled builds should only be done when permitted by the original author's terms or with their permission.

## ModPorterMC

Maintained as part of [ModPorterMC](https://github.com/ModPorterMC).

**Minecraft Mod Ports • Version Updates • Loader Conversions**

**Contact:** modportermc@outlook.com
