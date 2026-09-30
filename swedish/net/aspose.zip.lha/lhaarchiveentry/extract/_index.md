---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LhaArchiveEntry-metoden. Extraherar Lha-arkivinlägg till ett filsystem enligt sökväg"
type: docs
weight: 60
url: /sv/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Extraherar Lha-arkivpost till ett filsystem enligt sökväg.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökväg till fil som kommer att lagra dekomprimerad data. |

### Returvärde

FileSystemInfoInstance som innehåller extraherad data.

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Arkivhuvuden och serviceinformation lästes inte. |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| InvalidDataException | Kastas när data är ogiltig eller korrupt. |

## Exempel

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Se även

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Extraherar posten till den angivna strömmen.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Ström | Destinationsström. Måste vara skrivbar. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | *destination* stöder inte skrivning. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| InvalidDataException | Kastas när data är ogiltig eller korrupt. |

## Anmärkningar

Gör ingenting för kataloginlägg.

### Se även

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extraherar Lha-arkivpost till en fil.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo för att lagra dekomprimerad data. |

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Arkivhuvuden och serviceinformation lästes inte. |
| SecurityException | Anroparen har inte den erforderliga behörigheten att öppna *fileInfo*. |
| ArgumentException | Filsökvägen är tom eller innehåller endast blanksteg. |
| FileNotFoundException | Filen hittades inte. |
| UnauthorizedAccessException | Sökvägen till filen är skrivskyddad eller är en katalog. |
| ArgumentNullException | *fileInfo* är null. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |

## Anmärkningar

Gör ingenting för kataloginlägg.

## Exempel

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Se även

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


