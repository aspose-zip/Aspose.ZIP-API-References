---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP voor .NET API-referentie
description: MeteredLicense methode. Stelt gemeten publieke en private sleutel in.
type: docs
weight: 20
url: /nl/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Stelt gemeten publieke en private sleutel in.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| publicKey | String | De openbare sleutel. |
| privateKey | String | De privésleutel. |

### Opmerkingen

Als u een gemeten licentie aanschaft, moet deze API bij het starten van de applicatie worden aangeroepen, normaal gesproken is dit voldoende. Als het echter altijd niet lukt om verbruiksgegevens te uploaden en de 24 uur overschrijdt, wordt de licentie ingesteld op de evaluatiestatus, om een dergelijk geval te voorkomen, moet u regelmatig de licentiestatus controleren. Als het de evaluatiestatus is, roept u deze API opnieuw op.

### Zie ook

* class [MeteredLicense](../)
* naamruimte [Aspose.Zip](../../meteredlicense/)
* montage [Aspose.Zip](../../../)


