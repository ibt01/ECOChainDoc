## Goal

Connect to a specific `nodtlk` or `ktlkd` host to send COMMAND

`cltlk` and `ktlkd` can connect to a specific node by using the `--url` or `--wallet-url` optional arguments, respectively, followed by the http address and port number these services are listening to.

[[info | Default address:port]]
| If no optional arguments are used (i.e. `--url` or `--wallet-url`), `cltlk` attempts to connect to a local `nodtlk` or `ktlkd` running at localhost `127.0.0.1` and default port `8888`.

## Before you begin

* Install the currently supported version of `cltlk`

## Steps
### Connecting to Nodtlk

```sh
cltlk -url http://nodtlk-host:8888 COMMAND
```

### Connecting to Ktlkd

```sh
cltlk --wallet-url http://ktlkd-host:8888 COMMAND
```
