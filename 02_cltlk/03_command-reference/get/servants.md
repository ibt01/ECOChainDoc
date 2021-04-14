## Description
Retrieve accounts which are servants of a given account 

## Info

**Command**

```sh
cltlk get servants
```
**Output**

```console
Usage: cltlk get servants account

Positionals:
  account TEXT                The name of the controlling account
```

## Command

```sh
cltlk get servants inita
```

## Output

```json
{
  "controlled_accounts": [
    "tester"
  ]
}
```
