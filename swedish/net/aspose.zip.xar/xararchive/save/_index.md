---
title: "XarArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarArchive-metod. Sparar arkivet till den angivna destinationsfilen."
type: docs
weight: 80
url: /sv/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Sparar arkivet till den angivna destinationsfilen.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| saveOptions | XarSaveOptions | Alternativ för att spara xar-arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *destinationFileName* är null. |
| InvalidOperationException | Omöjligt att modifiera xar-arkivet. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemdefinierad maximal längd. |
| UnauthorizedAccessException | *destinationFileName* angav en fil som är skrivskyddad. -eller- *destinationFileName* angav en katalog. -eller- Anroparen har inte den nödvändiga behörigheten. |

### Se även

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Sparar arkivet till den angivna strömmen.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |
| saveOptions | XarSaveOptions | Alternativ för att spara xar-arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *output* är null. |
| ArgumentException | *output* är inte skrivbar/läsbar eller sökbar. |
| InvalidOperationException | Omöjligt att modifiera xar-arkivet. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

### Se även

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


