---
content_title: Nodtlk
---

## Introduction

`nodtlk` is the core service daemon that runs on every TLKIO node. It can be configured to process smart contracts, validate transactions, produce blocks containing valid transactions, and confirm blocks to record them on the blockchain.

## Installation

## Explore

Navigate the sections below to configure and use `nodtlk`.

* [Usage](02_usage/index.md) - Configuring and using `nodtlk`, node setups/environments.
* [Plugins](03_plugins/index.md) - Using plugins, plugin options, mandatory vs. optional.
* [Replays](04_replays/index.md) - Replaying the chain from a snapshot or a blocks.log file.
* [RPC APIs](05_rpc_apis/index.md) - Remote Procedure Call API reference for plugin HTTP endpoints.
* [Logging](06_logging/index.md) - Logging config/usage, loggers, appenders, logging levels.
* [Upgrade Guides](07_upgrade-guides/index.md) - TLKIO version/consensus upgrade guides.
* [Troubleshooting](08_troubleshooting/index.md) - Common `nodtlk` troubleshooting questions.

[[info | Access Node]]
| A local or remote TLKIO access node running `nodtlk` is required for a client application or smart contract to interact with the blockchain.
