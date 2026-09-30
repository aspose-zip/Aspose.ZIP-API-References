---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "UueArchive‑konstruktor. Initierar en ny instans av UueArchive‑klassen för kodning"
type: docs
weight: 10
url: /sv/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Initierar en ny instans av klassen [`UueArchive`](../) för kodning.

```csharp
public UueArchive()
```

## Exempel

Följande exempel visar hur man uuencodar en fil.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Se även

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Initierar en ny instans av klassen [`UueArchive`](../) för avkodning.

```csharp
public UueArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. |

## Anmärkningar

Denna konstruktor avkodar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från en ström och extrahera det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Se även

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Initierar en ny instans av klassen [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |

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
| FileNotFoundException | Filen hittades inte. |
| IOException | Filen är redan öppen. |

## Anmärkningar

Denna konstruktor dekomprimerar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från fil via sökväg och avkoda det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Se även

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


