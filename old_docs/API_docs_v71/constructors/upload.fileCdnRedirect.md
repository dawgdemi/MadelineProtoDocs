---
title: upload.fileCdnRedirect
description: The file must be downloaded from a [CDN DC](https://core.telegram.org/cdn).
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/upload_fileCdnRedirect.html
---
# Constructor: upload.fileCdnRedirect  
[Back to constructors index](index.md)



The file must be downloaded from a [CDN DC](https://core.telegram.org/cdn).

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|dc\_id|[int](../types/int.md) | Yes|[CDN DC](https://core.telegram.org/cdn) ID|
|file\_token|[bytes](../types/bytes.md) | Yes|File token (see [CDN files](https://core.telegram.org/cdn)|
|encryption\_key|[bytes](../types/bytes.md) | Yes|Encryption key (see [CDN files](https://core.telegram.org/cdn)|
|encryption\_iv|[bytes](../types/bytes.md) | Yes|Encryption IV (see [CDN files](https://core.telegram.org/cdn)|
|cdn\_file\_hashes|Array of [CdnFileHash](../types/CdnFileHash.md) | Yes|Cdn file hashes|



### Type: [upload.File](../types/upload.File.md)


### Example:

```php
$upload.fileCdnRedirect = ['_' => 'upload.fileCdnRedirect', 'dc_id' => int, 'file_token' => 'bytes', 'encryption_key' => 'bytes', 'encryption_iv' => 'bytes', 'cdn_file_hashes' => [CdnFileHash, CdnFileHash]];
```  


Or, if you're into Lua:

```lua
upload.fileCdnRedirect={_='upload.fileCdnRedirect', dc_id=int, file_token='bytes', encryption_key='bytes', encryption_iv='bytes', cdn_file_hashes={CdnFileHash}}

```


