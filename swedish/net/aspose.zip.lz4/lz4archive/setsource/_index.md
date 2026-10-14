---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Lz4Archive metod. Anger innehållet som ska komprimeras i arkivet"
type: docs
weight: 70
url: /sv/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

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
| InvalidOperationException | Arkivet är förberett för extrahering. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | Arkivet är förberett för extrahering. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

Öppna ett arkiv från en ström och extrahera det till en `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Anger innehållet som ska komprimeras i arkivet.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-arkiv att komprimera. |
| format | TarFormat | Definierar tar-headerformat. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Detta arkiv är förberett för extrahering. |

## Anmärkningar

Använd den här metoden för att komponera ett gemensamt tar.lz4-arkiv.

## Exempel

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Se även

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

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
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för åtkomst |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| InvalidOperationException | Detta arkiv är förberett för extrahering. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

Öppna ett arkiv från fil via sökväg och extrahera det till en `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


