---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoArchive‑metod. Extraherar alla poster till den angivna katalogen"
type: docs
weight: 60
url: /sv/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

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
| InvalidOperationException | Kastas när arkivet är i redigeringsläge. |
| ArgumentNullException | Kastas när *destinationDirectory* är null. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

Följande exempel visar hur man extraherar alla poster till en katalog:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


