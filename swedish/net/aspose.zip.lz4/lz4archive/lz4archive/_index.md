---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Lz4Archive-konstruktor. Initierar en ny instans av Lz4Archive-klassen som är förberedd för dekomprimering"
type: docs
weight: 10
url: /sv/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Initierar en ny instans av [`Lz4Archive`](../)-klassen som är förberedd för dekomprimering.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. |
| loadOptions | Lz4LoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | Kan inte läsa från *sourceStream* |
| ArgumentNullException | *sourceStream* är null. |
| EndOfStreamException | *sourceStream* är för kort. |
| InvalidDataException | Den *sourceStream* har fel signatur. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

Denna konstruktor dekomprimerar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från en ström och extrahera det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Se även

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Initierar en ny instans av [`Lz4Archive`](../)-klassen.

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |
| loadOptions | Lz4LoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för åtkomst |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| EndOfStreamException | Filen är för kort. |
| InvalidDataException | Data i filen har fel signatur. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| FileNotFoundException | Filen hittades inte. |
| IOException | Filen är redan öppen. |

## Anmärkningar

Denna konstruktor dekomprimerar inte. Se metoden [`Open`](../open/) för dekomprimering.

## Exempel

Öppna ett arkiv från fil via sökväg och extrahera det till en `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Se även

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Initierar en ny instans av [`Lz4Archive`](../)-klassen som är förberedd för komprimering.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inställningar | Lz4ArchiveSetting | Inställningen för det sammansatta arkivet. |

### Se även

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


