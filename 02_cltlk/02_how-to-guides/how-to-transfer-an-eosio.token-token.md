## Goal

Transfer token created by tlkio.token contract

## Before you begin

* Install the currently supported version of `cltlk`

* You are going to transfer a token created by tlkio.token contract and tlkio.token contract has been deployed on the network which you are connected to

* Understand the following:
  * What is a transaction
  * Token transfers are irrevertable 

## Steps

Assume you would like to transfer `0.0001 TLK` token to an account called `bob` from an account called `alice`, execute the following:

```sh
cltlk transfer alice bob "0.0001 TLK" "Hodl!" -p alice@active
```
