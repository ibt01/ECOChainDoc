## Goal

Delegate resource for an account or application

## Before you begin

* Install the currently supported version of `cltlk`

* Ensure the reference system contracts from `tlkio.contracts` repository is deployed and used to manage system resources

* Understand the following:
  * What is an account
  * What is network bandwidth
  * What is CPU bandwidth



## Steps

Delegate 0.01 TLK network bandwidth from `bob` to `alice`

```sh
cltlk system delegatebw bob alice "0 TLK" "0.01 TLK"
```

You should see something below:

```console
executed transaction: 5487afafd67bf459a20fcc2dbc5d0c2f0d1f10e33123eaaa07088046fd18e3ae  192 bytes  503 us
#         tlkio <= tlkio::delegatebw            {"from":"bob","receiver":"alice","stake_net_quantity":"0.0100 TLK","stake_cpu_quanti...
#   tlkio.token <= tlkio.token::transfer        {"from":"bob","to":"tlkio.stake","quantity":"0.0010 TLK","memo":"stake bandwidth"}
#  bob <= tlkio.token::transfer        {"from":"bob","to":"tlkio.stake","quantity":"0.0010 TLK","memo":"stake bandwidth"}
#   tlkio.stake <= tlkio.token::transfer        {"from":"bob","to":"tlkio.stake","quantity":"0.0010 TLK","memo":"stake bandwidth"}
```
