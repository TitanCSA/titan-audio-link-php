# Titan-Audio-Link PHP SDK

> [!IMPORTANT]
> **Get the driver without the one-hour demo limit**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about the full **Titan Audio Link** driver for this SDK. TitanCSA shares purchase details privately.

`composer require titancsa/titan-audio-link`

Windows x64 PHP8.2+; enable FFI extension and `ffi.enable=true`.

```php
require "vendor/autoload.php";
$client=new \TitanCSA\Products\TitanAudioLink\Client();
try {print_r($client->call("list"));} finally {$client->close();}
```

[API and operation schema](docs/API.md). Matching driver installed separately.
