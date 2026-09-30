---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "FastLZStream-methode. Schrijft een reeks bytes naar de comprimerende stream en verplaatst de huidige positie binnen deze stream met het aantal geschreven bytes"
type: docs
weight: 120
url: /nl/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Schrijft een reeks bytes naar de comprimerende stream en schuift de huidige positie binnen deze stream vooruit met het aantal geschreven bytes.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| buffer | Byte[] | Een array van bytes. Deze methode kopieert count bytes van buffer naar de huidige stream. |
| offset | Int32 | De nulgebaseerde byte-offset in buffer waarop begonnen moet worden met het kopiëren van bytes naar de huidige stream. |
| count | Int32 | Het aantal bytes dat naar de huidige stream moet worden geschreven. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Wordt gegooid als de stream is vrijgegeven. |
| ArgumentNullException | *buffer* is `null`. |

### Zie ook

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


