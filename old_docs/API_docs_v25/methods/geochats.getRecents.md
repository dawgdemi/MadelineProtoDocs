---
title: geochats.getRecents
description: Get recent geochats
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/geochats_getRecents.html
---
# Method: geochats.getRecents  
[Back to methods index](index.md)


Get recent geochats

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|offset|[int](../types/int.md) | Offset | Yes|
|limit|[int](../types/int.md) | Number of results to return | Yes|


### Return type: [geochats.Messages](../types/geochats.Messages.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$geochats.Messages = $MadelineProto->geochats->getRecents(['offset' => int, 'limit' => int, ]);
```

Or, if you're into Lua:

```lua
geochats.Messages = geochats.getRecents({offset=int, limit=int, })
```

