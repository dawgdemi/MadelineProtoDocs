---
title: req_pq
description: Requests PQ for factorization
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: req\_pq  
[Back to methods index](index.md)


Requests PQ for factorization

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|nonce|[int128](../types/int128.md) | Random number for cryptographic security | Yes|


### Return type: [ResPQ](../types/ResPQ.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$ResPQ = $MadelineProto->req_pq(['nonce' => int128, ]);
```

Or, if you're into Lua:

```lua
ResPQ = req_pq({nonce=int128, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|INPUT_METHOD_INVALID_1615239032_X|Invalid method, use req_pq_multi instead|


