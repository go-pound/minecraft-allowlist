# Go Pound Minecraft Allowlist

This repository contains JSON files that are downloaded by Go Pound's Minecraft servers. They control who can connect to the server, and who has operator privileges.

* [allowlist.json](allowlist.json) follows Minecraft's [`whitelist.json` format](https://minecraft.fandom.com/wiki/Whitelist.json).
* [ops.json](ops.json) follows Minecraft's `ops.json` format.

## Usage

Any server configuration that can download the JSON files from GitHub before starting the Minecraft server can use these files. (Note that the vanilla Minecraft server uses `whitelist.json`, not `allowlist.json`, so you'll need to rename the file as necessary.)

[itzg/docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) can be configured with `OPS_FILE=https://...` and `WHITELIST_FILE=https://...` environment variables.
