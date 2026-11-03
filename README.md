# TriggerBot Updates

This public repository contains release metadata and compiled Minecraft mod JARs only. The source code remains in the private `TriggerBot` repository.

## Automatic updates

The mod checks `update.json` for a newer compatible release and can download the JAR into a staging folder. A running Fabric mod cannot safely replace its own loaded JAR; the staged update must be installed after Minecraft exits (or at the next launch by an external updater).

Releases are published by the private source repository's GitHub Actions workflow. The workflow requires a repository secret named `TRIGGERBOT_UPDATES_TOKEN` with **Contents: Read and write** access to this public repository.
