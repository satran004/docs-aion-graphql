# Mutation

Mutation apis are used whenever there is any state change on the blockchain.

_Example_: Send Transaction, Contract Deploy, Account Create etc.

Mutation query should always starts with "mutation" keyword.

```javascript
mutation sendTransaction {
  txnApi {
    sendTransaction(
      txArgs: {
        from: "a0xxxxxxxxx",
        to: "a0xxxxxxxxxxxxxx",
        value: 40000
      }){
        status
        msgHash
        txHash
        txResult
        txDeploy
        error
    }
  }
}
```

