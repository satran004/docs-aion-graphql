---
description: TxnApi is used to get transaction specific details.
---

# txApi - Transaction Apis

### Get last 3 transactions

**Query**

```text
{
  txnApi {
    transactions(first: 3) {
      to
      from
      value
      txHash
      blockNumber
      nrgPrice
      nrgConsumed
      nonce
      data
      contract
    }
  }
}
```

**Result**

```text
{
  "data": {
    "txnApi": {
      "transactions": [
        {
          "to": "a0d2024dca3c505d1a62b663a084dd7570f6f39a690ae981f1d7cb234a5b4f82",
          "from": "a022a68ef27e5febe4570edb2ce5586974cb326f24fce2ebb23012c07dac90e0",
          "value": 1018817512610000000,
          "txHash": "52e5240a975aae7967bd9cc39ea634a6bf51c04f6b0c8c55473c17ffc94aff55",
          "blockNumber": 1483031,
          "nrgPrice": 10000000000,
          "nrgConsumed": 21000,
          "nonce": 6746,
          "data": "",
          "contract": ""
        },
        {
          "to": "a0b017c28ad66e3a94a2618475b26b30b5fb02bb4e1ca0df1b77c10f1e9e0557",
          "from": "a022a68ef27e5febe4570edb2ce5586974cb326f24fce2ebb23012c07dac90e0",
          "value": 1231613758077000000,
          "txHash": "4d205ab6c3470722f659cbd644fa3dd87a3e9d43f354d3afd5388731ec1eef55",
          "blockNumber": 1483031,
          "nrgPrice": 10000000000,
          "nrgConsumed": 21000,
          "nonce": 6747,
          "data": "",
          "contract": ""
        },
        {
          "to": "a031949a9a11d739f82385778cd01395839b362d8f19ec060dc188f515d27201",
          "from": "a022a68ef27e5febe4570edb2ce5586974cb326f24fce2ebb23012c07dac90e0",
          "value": 1082728137311000000,
          "txHash": "c52f9ebb1876fd2fce0a662bf518ab1b3042cefc5444b6d35be47a7d5578db9e",
          "blockNumber": 1483031,
          "nrgPrice": 10000000000,
          "nrgConsumed": 21000,
          "nonce": 6748,
          "data": "",
          "contract": ""
        }
      ]
    }
  }
}
```

