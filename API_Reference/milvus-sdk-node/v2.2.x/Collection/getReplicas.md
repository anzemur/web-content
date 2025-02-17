# getReplicas()

This method returns replica information.

## Invocation

```javascript
new milvusClient(MILUVS_ADDRESS).indexManager.getReplicas(
  GetReplicaReq
);
```

## Parameter

### GetIndexStateReq

| Parameter | Description | Type   | Required |
| -- | --  | -- | -- |
| collectionID | Collection ID | Number | True |
| timeout | An optional duration of time in millisecond to allow for the RPC. Default is undefined | Number | False |

## Example

```javascript
new milvusClient(MILUVS_ADDRESS).indexManager.getReplicas({
  collectionID: 123,
});
```

## Return

```javascript
// getIndexState return
{
  replicas: [
    {
      partition_ids: [Array],
      shard_replicas: [Array],
      node_ids: [Array],
      replicaID: '436724291187770258',
      collectionID: '436777253933154305'
    }
  ],
  status: { error_code: 'Success', reason: '' }
}
```


