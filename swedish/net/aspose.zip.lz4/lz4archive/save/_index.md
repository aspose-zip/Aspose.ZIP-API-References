---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Lz4Archive-metod. Sparar lz4-arkivet till den angivna strömmen"
type: docs
weight: 60
url: /sv/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Sparar lz4‑arkivet till den angivna strömmen.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *output* är null. |
| ArgumentException | *output* är inte skrivbar. |
| InvalidOperationException | Arkivet är förberett för extrahering. - eller - Källan angavs inte. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när komprimeringen avbryts via den tillhandahållna avbokningstoken. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

*output* must be seekable.

## Exempel

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Sparar lz4‑arkivet till den angivna destinationsfilen.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | FileInfo | FileInfo, som kommer att öppnas som destinationsström. |

### Undantag

| undantag | villkor |
| --- | --- |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att öppna *destination*. |
| ArgumentException | Filsökvägen är tom eller innehåller endast blanksteg. |
| FileNotFoundException | Filen hittades inte. |
| UnauthorizedAccessException | Sökvägen till filen är skrivskyddad eller är en katalog. |
| ArgumentNullException | *destination* är null. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| InvalidOperationException | Arkivet är förberett för extrahering. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Sparar arkivet till den angivna destinationsfilen.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *destinationFileName* är null. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för åtkomst |
| ArgumentException | Den *destinationFileName* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *destinationFileName* nekas. |
| PathTooLongException | Den angivna *destinationFileName*, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *destinationFileName* innehåller ett kolon (:) i mitten av strängen. |
| InvalidOperationException | Arkivet är förberett för extrahering. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| FileNotFoundException | Filen som specificerades i *destinationFileName* hittades inte. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |

## Exempel

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


