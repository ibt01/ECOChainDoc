---
content_title: Nodtlk Troubleshooting
---

### "Database dirty flag set (likely due to unclean shutdown): replay required"

`nodtlk` needs to be shut down cleanly. To ensure this is done, send a `SIGTERM`, `SIGQUIT` or `SIGINT` and wait for the process to shutdown. Failing to do this will result in this error. If you get this error, your only recourse is to replay by starting `nodtlk` with `--replay-blockchain` 

### "Memory does not match data" Error at Restart

If you get an error such as `St9exception: content of memory does not match data expected by executable` when trying to start `nodtlk`, try restarting `nodtlk` with one of the following options (you can use `nodtlk --help` to get a full listing of these).

```
Command Line Options for tlkio::chain_plugin:
    --fix-reversible-blocks               recovers reversible block database if 
                                          that database is in a bad state
    --force-all-checks                    do not skip any checks that can be 
                                          skipped while replaying irreversible 
                                          blocks
    --replay-blockchain                   clear chain state database and replay 
                                          all blocks
    --hard-replay-blockchain              clear chain state database, recover as 
                                          many blocks as possible from the block 
                                          log, and then replay those blocks
    --delete-all-blocks                   clear chain state database and block 
                                          log
```

### "Could not grow database file to requested size." Error

Start `nodtlk` with `--shared-memory-size-mb 1024`. A 1 GB shared memory file allows approximately half a million transactions.

### What version of TLKIO am I running/connecting to?

If defaults can be used, then `cltlk get info` will output a block that contains a field called `server_version`.  If your `nodtlk` is not using the defaults, then you need to know the URL of the `nodtlk`. In that case, use the following with your `nodtlk` URL:

```sh
cltlk --url http://localhost:8888 get info
```

To focus only on the version line within the block:

```sh
cltlk --url http://localhost:8888 get info | grep server_version
```

### Error 3070000: WASM Exception Error

