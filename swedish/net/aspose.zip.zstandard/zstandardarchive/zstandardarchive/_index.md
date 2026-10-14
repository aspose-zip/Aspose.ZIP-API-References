---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardArchive konstruktor. Initierar en ny instans av ZstandardArchive‑klassen för komprimering"
type: docs
weight: 10
url: /sv/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Initierar en ny instans av [`ZstandardArchive`](../)‑klassen för komprimering.

```csharp
public ZstandardArchive()
```

## Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Se även

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Initierar en ny instans av [`ZstandardArchive`](../)‑klassen för dekomprimering.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. |
| alternativ | ZstandardLoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| EndOfStreamException | Kastas när slutet på strömmen nås oväntat. |
| IOException | Ett I/O‑fel inträffar. |
| InvalidDataException | Kastas när data är ogiltig eller korrupt. |

## Anmärkningar

Denna konstruktor dekomprimerar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från en ström och extrahera det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Se även

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Initierar en ny instans av [`ZstandardArchive`](../)‑klassen.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |
| alternativ | ZstandardLoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| EndOfStreamException | Kastas när slutet på strömmen nås oväntat. |
| FileNotFoundException | Filen hittades inte. |
| IOException | Filen är redan öppen. |
| InvalidDataException | Kastas när data är ogiltig eller korrupt. |

## Anmärkningar

Denna konstruktor dekomprimerar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från fil via sökväg och extrahera det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Se även

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


