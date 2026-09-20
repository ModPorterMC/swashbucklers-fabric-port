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

- distributable datapack resources
- ship entity persistence
- boat tags
- ship buoyancy
- model and renderer registration
- waterline positioning
- steering behavior
- control direction
- Corvette rider-seat alignment

## Building

Requires Java 25.

```bash
gradle build
