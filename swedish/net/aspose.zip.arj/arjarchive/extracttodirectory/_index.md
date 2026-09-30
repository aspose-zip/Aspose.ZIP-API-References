---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ArjArchive metod. Extraherar alla poster till den angivna katalogen"
type: docs
weight: 60
url: /sv/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

Extraherar alla poster till den angivna katalogen.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | String | Katalogen som posterna ska extraheras till. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | Kastas när *destinationDirectory* är null. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| NotImplementedException | Post komprimerad med metod 4. |

## Exempel

Följande exempel visar hur man extraherar alla poster till en katalog:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


