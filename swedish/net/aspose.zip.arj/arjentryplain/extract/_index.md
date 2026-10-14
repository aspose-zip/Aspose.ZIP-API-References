---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ArjEntryPlain-metod. Extraherar posten till filsystemet med den angivna sökvägen"
type: docs
weight: 40
url: /sv/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Extraherar posten till filsystemet enligt den angivna sökvägen.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till destinationsfilen. Om filen redan finns, kommer den att skrivas över. |

### Returvärde

Filinformationen för en sammansatt fil.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null eller tom. |
| ObjectDisposedException | Kastas om arkivet har disponerats. |
| FileNotFoundException | Filen hittades inte. |
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemdefinierad maximal längd. |
| NotImplementedException | Post komprimerad med metod 4. |

## Exempel

Extrahera två poster från rar-arkivet.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Se även

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extraherar ARJ-arkivpost till en fil.

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
| ObjectDisposedException | Kastas om arkivet har disponerats. |
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| NotImplementedException | Post komprimerad med metod 4. |

## Exempel

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Se även

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | Kontrollsumman matchar inte för header eller data. - eller - Arkivet är korrupt. |
| NotImplementedException | Post komprimerad med metod 4. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om arkivet har disponerats. |

### Se även

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


