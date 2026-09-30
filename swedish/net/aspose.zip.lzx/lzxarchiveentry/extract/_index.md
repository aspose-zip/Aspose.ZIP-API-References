---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LzxArchiveEntry-metoden. Extraherar Lzx-arkivinlägg till ett filsystem via sökväg"
type: docs
weight: 80
url: /sv/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extraherar Lzx-arkivpost till ett filsystem enligt sökväg.

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
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| NotSupportedException | Ogiltig komprimeringsmetod. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| EndOfStreamException | Kastas när slutet på strömmen nås oväntat. |

## Exempel

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Se även

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| ArgumentNullException | Destinationsströmmen är null. |
| NotSupportedException | Ogiltig komprimeringsmetod. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| EndOfStreamException | Kastas när slutet på strömmen nås oväntat. |

### Se även

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


