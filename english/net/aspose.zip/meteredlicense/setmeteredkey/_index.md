---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP for .NET API Reference
description: MeteredLicense method. Sets metered public and private keys
type: docs
weight: 30
url: /net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Sets metered public and private keys.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | The public key. |
| privateKey | String | The private key. |

## Remarks

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again.

### See Also

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)


