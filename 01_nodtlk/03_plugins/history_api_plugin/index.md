## Description

The `history_api_plugin` exposes functionality from the [`history_plugin`](../history_plugin/index.md) to the RPC API interface managed by the [`http_plugin`](../http_plugin/index.md), providing read-only access to blockchain data.

It provides four RPC API endpoints:

* get_actions
* get_transaction
* get_key_accounts
* get_controlled_accounts

[[info | More Info]]

The four actions listed above are used by the following `cltlk` commands (matching order):

* get actions
* get transaction
* get accounts
* get servants

## Usage

```console
# config.ini
plugin = tlkio::history_api_plugin
```
```sh
# command-line
nodtlk ... --plugin tlkio::history_api_plugin
```

## Options

None

## Dependencies

* [`history_plugin`](../history_plugin/index.md)
* [`chain_plugin`](../chain_plugin/index.md)
* [`http_plugin`](../http_plugin/index.md)

### Load Dependency Examples

```console
# config.ini
plugin = tlkio::history_plugin
[options]
plugin = tlkio::chain_plugin
[options]
plugin = tlkio::http_plugin
[options]
```
```sh
# command-line
nodtlk ... --plugin tlkio::history_plugin [options]  \
           --plugin tlkio::chain_plugin [operations] [options]  \
           --plugin tlkio::http_plugin [options]
```
