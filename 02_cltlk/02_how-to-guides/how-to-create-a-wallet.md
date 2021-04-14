## Goal

Create a `ktlkd` wallet

## Before you begin

* Install the currently supported version of `cltlk`

* Understand the following:
  * What is an account
  * What is a public and private key pair

## Steps

Create a wallet and save the password to a file:

```sh
cltlk wallet create --file password.pwd
```

This should produce similar output as below. Note the wallet is named `default` if no name is provided.

```console
Creating wallet: default
Save password to use in the future to unlock this wallet.
Without password imported keys will not be retrievable.
saving password to password.pwd
```

Alternatively, you can name a wallet with `-n` option:

```sh
cltlk wallet create -n named_wallet -f passwd
```

You should see something like the output below:

```console
Creating wallet: named_wallet
Save password to use in the future to unlock this wallet.
Without password imported keys will not be retrievable.
saving password to passwd
```
