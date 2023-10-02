---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP for .NET API Reference
description: MeteredLicense method. Sets metered public and private key
type: docs
weight: 20
url: /net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Sets metered public and private key.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | The public key. |
| privateKey | String | The private key. |

## Remarks

If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

### See Also

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)


