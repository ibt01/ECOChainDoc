Configure the directories where cltlk, ktlkd, and nodtlk are located in the Linux environment variable PATH, and the system runs on the ubuntu 18.04 x64 server

Client tool:
```
cltlk
```


Private key management tool, need to be used with cltlk:
```
ktlkd
```


Blockchain node:
```
nodtlk
```

Start Node:
```
./nodtlk --disable-replay-opts --access-control-allow-origin='*'  --contracts-console --data-dir ./data --config-dir /yinni/config  --genesis-json  /yinni/config/genesis.json --verbose-http-errors >> configmodenodtlk.log 2>&1 &
```
