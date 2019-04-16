---
title: messages.clearAllDrafts
description: Clear all drafts
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.clearAllDrafts  
[Back to methods index](index.md)


Clear all drafts



### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
define('MADELINE_BRANCH', '');
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->clearAllDrafts();
```

Or, if you're into Lua:

```lua
Bool = messages.clearAllDrafts({})
```
