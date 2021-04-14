## Goal

Stake resource for your account

## Before you begin

* Install the currently supported version of `cltlk`

* Ensure the reference system contracts from `tlkio.contracts` repository is deployed and used to manage system resources

* Understand the following:
  * What is an account
  * What is network bandwidth
  * What is CPU bandwidth

## Steps

Stake 0.01 TLK network bandwidth for `alice`

```sh
cltlk system delegatebw alice alice "0 TLK" "0.01 TLK"
```

Stake 0.01 TLK CPU bandwidth for `alice`:

```sh
cltlk system delegatebw alice alice "0.01 TLK" "0 TLK"
```
