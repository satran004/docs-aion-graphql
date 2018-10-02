# Test Your First API

If you want to try AION GraphQL API without deploying your own instance, you can do so.

The following URL can be accessed to try out GraphQL queries on the browser. This instanace is connected to AION Mainnet.

This instance is available for the community to quickly test and develop application. But don't use this instance for your production deployment.

Following url shows an editor in the browser where you can test any GraphQL API provided by this project directly in the browser :

[https://api.aion-graphql.com/playground.html](https://api.aion-graphql.com/playground.html)

If you want to invoke GraphQL API from your application, use the following url :

[https://api.aion-graphql.com/](https://api.aion-graphql.com/playground.html)graphql

## First API Call

### Get Latest Transactions

Let's get the latest 20 transactions.

Run the following query in the GraphQL Playground's editor.

_**Query:**_

```javascript
{
  txnApi {
    transactions(first:3) {
      from
      to
      value
      blockHash
      blockNumber
      nrgConsumed
    }
  }
}
```

_**Output:**_

```javascript
{
  "data": {
    "txnApi": {
      "transactions": [
        {
          "from": "a0f2daa8de60d0e911fb468492242d604e1e11ec6f142bfee15757408aff2902",
          "to": "a0f499fe8fc35c31b0c8a802d947744d765f7c555d01b2b69ef7a9d894bbbfd4",
          "value": 1764539184830000000,
          "blockHash": "7a3945f5f9efa86d0fd61feb2d0e099bbddbea0151aaa369546177734526541b",
          "blockNumber": 1327310,
          "nrgConsumed": 21000
        },
        {
          "from": "a0a1e55cbbffc99d9dcaf56e5350847267471cd6d69d4dead14953e5e82d97bf",
          "to": "a09b42055863ae7b85c9c73b3d295927e64935edd1d11341bdd991533ecc6e4b",
          "value": 1613059522337000000,
          "blockHash": "2cc936f93331e9123fbeda8831790a836f4c792324fa7359b93b7b9eeb3ccb51",
          "blockNumber": 1327304,
          "nrgConsumed": 21000
        },
        {
          "from": "a0a1e55cbbffc99d9dcaf56e5350847267471cd6d69d4dead14953e5e82d97bf",
          "to": "a0937619ca96b490baa44eac64c82b5c1fba5f6a1e19809bb9c4099449074d85",
          "value": 1507893876082000000,
          "blockHash": "2cc936f93331e9123fbeda8831790a836f4c792324fa7359b93b7b9eeb3ccb51",
          "blockNumber": 1327304,
          "nrgConsumed": 21000
        }
      ]
    }
  }
}
```

**Congratulations !!!** You just accessed AION mainnet to get transactions.

