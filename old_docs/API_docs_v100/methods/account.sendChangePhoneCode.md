---
title: account.sendChangePhoneCode
description: Verify a new phone number to associate to the current account
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_sendChangePhoneCode.html
---
# Method: account.sendChangePhoneCode  
[Back to methods index](index.md)


Verify a new phone number to associate to the current account

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|phone\_number|[string](../types/string.md) | New phone number | Yes|
|settings|[CodeSettings](../types/CodeSettings.md) | Phone code settings | Yes|


### Return type: [auth.SentCode](../types/auth.SentCode.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$auth.SentCode = $MadelineProto->account->sendChangePhoneCode(['phone_number' => 'string', 'settings' => CodeSettings, ]);
```

Or, if you're into Lua:

```lua
auth.SentCode = account.sendChangePhoneCode({phone_number='string', settings=CodeSettings, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|PHONE_NUMBER_INVALID|The phone number is invalid|


