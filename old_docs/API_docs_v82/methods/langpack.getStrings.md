---
title: langpack.getStrings
description: Get strings from a language pack
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/langpack_getStrings.html
---
# Method: langpack.getStrings  
[Back to methods index](index.md)


Get strings from a language pack

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|lang\_code|[string](../types/string.md) | Language code | Yes|
|keys|Array of [string](../types/string.md) | Keys | Yes|


### Return type: [Vector\_of\_LangPackString](../types/LangPackString.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Vector_of_LangPackString = $MadelineProto->langpack->getStrings(['lang_code' => 'string', 'keys' => ['string', 'string'], ]);
```

Or, if you're into Lua:

```lua
Vector_of_LangPackString = langpack.getStrings({lang_code='string', keys={'string'}, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|LANG_PACK_INVALID|The provided language pack is invalid|


