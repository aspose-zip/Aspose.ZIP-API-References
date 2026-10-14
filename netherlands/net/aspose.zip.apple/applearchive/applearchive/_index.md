---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AppleArchive constructor. Initialiseert een nieuw exemplaar van de AppleArchive-klasse met instellingen die worden gebruikt voor samengestelde items."
type: docs
weight: 10
url: /nl/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Initialiseert een nieuw exemplaar van de [`AppleArchive`](../)-klasse met instellingen die worden gebruikt voor samengestelde items.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Instellingen die worden gebruikt bij het samenstellen van een nieuw Apple Archive. |

### Zie ook

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`AppleArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| loadOptions | AppleArchiveLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is niet doorzoekbaar. |
| InvalidDataException | *sourceStream* is geen geldig Apple Archive. |
| EndOfStreamException | De stroom eindigt onverwacht tijdens het parseren van de archiefvermeldingen. |

## Opmerkingen

Deze constructor decompresseert geen enkele vermelding. Zie de methoden [`ExtractToDirectory`](../extracttodirectory/) en [`Open`](../../applearchiveentry/open/) voor decompressie.

### Zie ook

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`AppleArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |
| loadOptions | AppleArchiveLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| FileNotFoundException | Het bestand is niet gevonden. |
| InvalidDataException | *path* is geen geldig Apple Archive. |
| EndOfStreamException | De stroom eindigt onverwacht tijdens het parseren van de archiefvermeldingen. |

## Opmerkingen

Deze constructor decompresseert geen enkele vermelding. Zie de methoden [`ExtractToDirectory`](../extracttodirectory/) en [`Open`](../../applearchiveentry/open/) voor decompressie.

### Zie ook

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


