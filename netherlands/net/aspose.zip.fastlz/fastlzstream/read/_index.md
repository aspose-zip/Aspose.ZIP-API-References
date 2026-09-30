---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "FastLZStream-methode. Leest een reeks bytes uit de stream en verplaatst de positie binnen de stream met het aantal gelezen bytes. Niet ondersteund"
type: docs
weight: 90
url: /nl/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Leest een reeks bytes uit de stream en schuift de positie binnen de stream vooruit met het aantal gelezen bytes. Niet ondersteund.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| buffer | Byte[] | Een array van bytes. Wanneer deze methode terugkeert, bevat de buffer de opgegeven byte-array met de waarden tussen offset en (offset + count - 1) vervangen door de bytes die van de huidige bron zijn gelezen. |
| offset | Int32 | De nulgebaseerde byte-offset in buffer waarop begonnen moet worden met het opslaan van de gegevens die uit de huidige stream zijn gelezen. |
| count | Int32 | Het maximale aantal bytes dat uit de huidige stream moet worden gelezen. |

### Retourwaarde

Het totale aantal bytes dat in de buffer is gelezen. Dit kan minder zijn dan het aangevraagde aantal bytes als dat aantal momenteel niet beschikbaar is, of nul (0) als het einde van de stream is bereikt.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| NotSupportedException | De bewerking wordt niet ondersteund. |

### Zie ook

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


