---
title: IArchiveFileEntry.Extract
second_title: Aspose.ZIP för .NET API-referens
description: IArchiveFileEntry metod. Extraherar posten till filsystemet med den angivna sökvägen.
type: docs
weight: 30
url: /sv/net/aspose.zip/iarchivefileentry/extract/
---
## Extract(string) {#extract}

Extraherar posten till filsystemet med den angivna sökvägen.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

### Returvärde

FileInfo instans som innehåller extraherade data.

### Se även

* interface [IArchiveFileEntry](../)
* namnutrymme [Aspose.Zip](../../iarchivefileentry/)
* hopsättning [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraherar posten till den tillhandahållna strömmen.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destination | Stream | Destinationsström. Måste vara skrivbart. |

### Se även

* interface [IArchiveFileEntry](../)
* namnutrymme [Aspose.Zip](../../iarchivefileentry/)
* hopsättning [Aspose.Zip](../../../)


