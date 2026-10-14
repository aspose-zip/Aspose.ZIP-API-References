---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoArchive-metod. Lägger till en fil i ISO-avbilden"
type: docs
weight: 40
url: /sv/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Lägger till en fil i ISO-avbilden.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Sökväg till filen i ISO. |
| filePath | String | Sökväg till filen. |

### Returvärde

ISO‑posten har sammansatts.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *filePath* är null. |
| ArgumentException | *filePath* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *filePath* nekas. |
| PathTooLongException | Den angivna *filePath* överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *filePath* innehåller ett kolon (:) i mitten av strängen. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| FileNotFoundException | Filen som angavs i *filePath* hittades inte. |
| InvalidOperationException | Arkivet är inte i redigeringsläge. |

### Se även

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Lägger till en fil i ISO-avbilden.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Sökväg till filen i ISO. |
| källa | Ström | Ström som innehåller filens data. |

### Returvärde

ISO‑posten har sammansatts.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | Kastas när ett *name* eller *source* är null. |
| InvalidOperationException | Arkivet är inte i redigeringsläge. |

### Se även

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Lägger till en fil i ISO-avbilden.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Sökväg till katalogen i ISO:n. |

### Returvärde

ISO‑posten har sammansatts.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | `name` är null eller tom. |
| InvalidOperationException | Arkivet är öppnat för extraktion. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

### Se även

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


