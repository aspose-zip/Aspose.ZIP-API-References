---
title: Class MeteredLicense
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.MeteredLicense class. Provides methods to set metered key
type: docs
weight: 430
url: /net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Provides methods to set metered key.

```csharp
public class MeteredLicense
```

## Constructors

| Name | Description |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | The default constructor. |

## Methods

| Name | Description |
| --- | --- |
| [ResetMeteredKey](../../aspose.zip/meteredlicense/resetmeteredkey/)() | Removes previously setup license. |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Sets metered public and private keys. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Gets consumption credit. |
| static [GetConsumptionQuantity](../../aspose.zip/meteredlicense/getconsumptionquantity/)() | Gets consumption file size. |

## Examples

In this example, an attempt will be made to set metered public and private key

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

the component jar file:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### See Also

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


