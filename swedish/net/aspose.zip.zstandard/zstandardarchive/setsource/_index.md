---
title: "ZstandardArchive.SetSource"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardArchive-metod. Anger innehållet som ska komprimeras i arkivet"
type: docs
weight: 70
url: /sv/net/aspose.zip.zstandard/zstandardarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Anger innehållet som ska komprimeras i arkivet.

```csharp
public void SetSource(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Ström | Inmatningsströmmen för arkivet. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new ZstandardArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.zst");
}
```

### Se även

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Anger innehållet som ska komprimeras i arkivet.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileInfo | FileInfo | Referensen till en fil som ska komprimeras. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.zst");
}
```

### Se även

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Anger innehållet som ska komprimeras i arkivet.

```csharp
public void SetSource(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökväg till filen som ska komprimeras. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |

## Exempel

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Se även

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


