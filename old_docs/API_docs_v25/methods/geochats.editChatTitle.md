---
title: geochats.editChatTitle
description: Edit geochat title
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/geochats_editChatTitle.html
---
# Method: geochats.editChatTitle  
[Back to methods index](index.md)


Edit geochat title

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[InputGeoChat](../types/InputGeoChat.md) | The geochat | Yes|
|title|[string](../types/string.md) | The new title | Yes|
|address|[string](../types/string.md) | The new address | Yes|


### Return type: [geochats.StatedMessage](../types/geochats.StatedMessage.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$geochats.StatedMessage = $MadelineProto->geochats->editChatTitle(['peer' => InputGeoChat, 'title' => 'string', 'address' => 'string', ]);
```

Or, if you're into Lua:

```lua
geochats.StatedMessage = geochats.editChatTitle({peer=InputGeoChat, title='string', address='string', })
```

