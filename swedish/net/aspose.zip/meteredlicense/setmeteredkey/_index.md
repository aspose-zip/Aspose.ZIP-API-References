---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP för .NET API-referens
description: MeteredLicense metod. Ställer in mätt offentlig och privat nyckel.
type: docs
weight: 20
url: /sv/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Ställer in mätt offentlig och privat nyckel.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| publicKey | String | Den offentliga nyckeln. |
| privateKey | String | Den privata nyckeln. |

### Anmärkningar

Om du köper uppmätt licens, när du startar applikationen, bör detta API anropas, normalt räcker detta. Men om alltid misslyckas med att ladda upp förbrukningsdata och överskrider 24 timmar, kommer licensen att ställas in på utvärderingsstatus, för att undvika sådana fall bör du regelbundet kontrollera licensstatusen, om det är utvärderingsstatus, ring detta API igen.

### Se även

* class [MeteredLicense](../)
* namnutrymme [Aspose.Zip](../../meteredlicense/)
* hopsättning [Aspose.Zip](../../../)


