---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AlzEntry metod. Extraherar posten till filsystemet enligt den angivna sökvägen"
type: docs
weight: 60
url: /sv/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Extraherar posten till filsystemet enligt den angivna sökvägen.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till destinationsfilen. Om filen redan finns, kommer den att skrivas över. |
| lösenord | String | Valfritt lösenord för dekryptering. |

### Returvärde

Filinformationen för en sammansatt fil.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| InvalidDataException | Arkivet är skadat. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| FileNotFoundException | Filen hittades inte. |

## Exempel

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Se även

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extraherar posten till den angivna strömmen.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Ström | Destinationsström. Måste vara skrivbar. |
| lösenord | String | Valfritt lösenord för dekryptering. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | *destination* stöder inte skrivning. |
| InvalidOperationException | Arkivet är inte öppnat för extraktion. - eller - Denna post är en katalog. |
| InvalidDataException | Fel data i posten. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |

## Exempel

Extrahera en post från ALZ-arkivet med lösenord.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Se även

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


