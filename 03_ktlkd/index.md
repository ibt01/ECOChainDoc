---
content_title: Ktlkd
---

## Introduction

`ktlkd` is a key manager service daemon for storing private keys and signing digital messages. It provides a secure key storage medium for keys to be encrypted at rest in the associated wallet file. `ktlkd` also defines a secure enclave for signing transaction created by `cltlk` or a third part library.

## Installation

## Operation

When a wallet is unlocked with the corresponding password, `cltlk` can request `ktlkd` to sign a transaction with the appropriate private keys. Also, `ktlkd` provides support for hardware-based wallets such as Secure Encalve and YubiHSM.

[[info | Audience]]
| `ktlkd` is intended to be used by TLKIO developers only.
