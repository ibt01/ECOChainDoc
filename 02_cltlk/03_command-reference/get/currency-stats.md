## Description
Retrieve the stats of for a given currency

## Positional Parameters
`contract` _TEXT_  - The contract that operates the currency

`symbol` _TEXT_ - The symbol for the currency if the contract operates multiple currencies
## Options
There are no options for this subcommand
## Example
Get stats of the TLK token from the tlkio.token contract. 

```sh
cltlk get currency stats tlkio.token TLK
```
```json
{
  "TLK": {
    "supply": "1000000000.0000 TLK",
    "max_supply": "10000000000.0000 TLK",
    "issuer": "tlkio"
  }
}
```
