---
title: SharArchive.SharArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: SharArchive constructeur. Initialiseert een nieuw exemplaar van hetSharArchive klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`SharArchive`](../) klasse.

```csharp
public SharArchive()
```

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een bestand kunt comprimeren.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Zie ook

* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Zie ook

* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)


