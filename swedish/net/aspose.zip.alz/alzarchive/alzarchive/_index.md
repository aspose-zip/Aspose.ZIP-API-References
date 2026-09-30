---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AlzArchive konstruktor. Initierar en ny instans av klassen AlzArchive från en ström"
type: docs
weight: 10
url: /sv/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Initierar en ny instans av klassen [`AlzArchive`](../) från en ström.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | ALZ-arkivströmmen. Strömmen måste stödja läsning och sökning. |
| loadOptions | AlzArchiveLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | stream är null. |

### Se även

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Initierar en ny instans av klassen [`AlzArchive`](../) från en filsökväg.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till ALZ-arkivfilen. |
| loadOptions | AlzArchiveLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | filePath är null. |
| FileNotFoundException | Filen finns inte. |

### Se även

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


