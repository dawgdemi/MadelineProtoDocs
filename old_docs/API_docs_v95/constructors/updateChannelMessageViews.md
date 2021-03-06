---
title: updateChannelMessageViews
description: The view counter of a message in a channel has changed
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateChannelMessageViews  
[Back to constructors index](index.md)



The view counter of a message in a channel has changed

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|channel\_id|[int](../types/int.md) | Yes|Channel ID|
|id|[int](../types/int.md) | Yes|ID of the message|
|views|[int](../types/int.md) | Yes|New view counter|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateChannelMessageViews = ['_' => 'updateChannelMessageViews', 'channel_id' => int, 'id' => int, 'views' => int];
```  


Or, if you're into Lua:

```lua
updateChannelMessageViews={_='updateChannelMessageViews', channel_id=int, id=int, views=int}

```


