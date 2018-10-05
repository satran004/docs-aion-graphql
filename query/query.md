# Query

This type of APIs are __used for read-only operations. __

_Example:_ Get Transaction, Get Blocks, Get Balance etc.

If you are accessing a Query type API, you can optionally start your request data with "query" keyword.

Both of the following queries are valid.

```javascript
query {
  blockApi {
    blocks(first: 20) {
      number
      hash
      parentHash
      timestamp
      nrgConsumed
      nrgLimit
    }
  }
}
```

```javascript
{
  blockApi {
    blocks(first: 20) {
      number
      hash
      parentHash
      timestamp
      nrgConsumed
      nrgLimit
    }
  }
}
```

