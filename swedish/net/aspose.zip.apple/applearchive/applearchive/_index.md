---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AppleArchive konstruktor. Initierar en ny instans av AppleArchive‑klassen med inställningar som används för sammansatta poster."
type: docs
weight: 10
url: /sv/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Initierar en ny instans av [`AppleArchive`](../)‑klassen med inställningar som används för sammansatta poster.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Inställningar som används när ett nytt Apple‑arkiv komponeras. |

### Se även

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Initierar en ny instans av [`AppleArchive`](../)‑klassen och komponera en postlista som kan extraheras från arkivet.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. |
| loadOptions | AppleArchiveLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *sourceStream* är null. |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | *sourceStream* är inte ett giltigt Apple‑arkiv. |
| EndOfStreamException | Strömmen avslutas oväntat under parsning av arkivposterna. |

## Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Se metoderna [`ExtractToDirectory`](../extracttodirectory/) och [`Open`](../../applearchiveentry/open/) för dekomprimering.

### Se även

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Initierar en ny instans av [`AppleArchive`](../)‑klassen och komponera en postlista som kan extraheras från arkivet.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Den fullständigt kvalificerade eller relativa sökvägen till arkivfilen. |
| loadOptions | AppleArchiveLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| FileNotFoundException | Filen hittades inte. |
| InvalidDataException | *path* är inte ett giltigt Apple‑arkiv. |
| EndOfStreamException | Strömmen avslutas oväntat under parsning av arkivposterna. |

## Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Se metoderna [`ExtractToDirectory`](../extracttodirectory/) och [`Open`](../../applearchiveentry/open/) för dekomprimering.

### Se även

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


