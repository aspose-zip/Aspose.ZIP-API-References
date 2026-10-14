---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CabArchive-metod. Skapa en enskild post i arkivet"
type: docs
weight: 40
url: /sv/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Skapa en enskild post i arkivet.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| sökväg | String | Det fullständigt kvalificerade namnet på den nya filen, eller det relativa filnamnet som ska komprimeras. |
| newEntrySettings | CabEntrySettings | Komprimerings- och krypteringsinställningar som används för det tillagda [`CabEntry`](../../cabentry/)‑objektet. |

### Returvärde

Cab‑postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte lägga till poster. |

## Anmärkningar

Postnamnet sätts enbart via parametern *name*. Filnamnet som anges i parametern *path* påverkar inte postnamnet.

## Exempel

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Se även

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Skapa en enskild post i arkivet.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| källa | Ström | Inmatningsströmmen för posten. |
| newEntrySettings | CabEntrySettings | Komprimerings- och krypteringsinställningar som används för det tillagda [`CabEntry`](../../cabentry/)‑objektet. |

### Returvärde

Cab‑postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte lägga till poster. |
| ArgumentNullException | *name* är null. |

## Exempel

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Se även

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Skapa en enskild post i arkivet.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för filen som ska komprimeras. |
| newEntrySettings | CabEntrySettings | Komprimerings- och krypteringsinställningar som används för det tillagda [`CabEntry`](../../cabentry/)‑objektet. |

### Returvärde

CAB‑postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* är skrivskyddad eller är en katalog. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| FileNotFoundException | *fileInfo* representerar en fil som inte kan hittas. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt *fileInfo*. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte lägga till poster. |
| ArgumentNullException | *name* är null. |

## Anmärkningar

Postnamnet sätts enbart via parametern *name*. Filnamnet som anges i parametern *fileInfo* påverkar inte postnamnet.

## Exempel

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Se även

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Skapa en enskild post i arkivet.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| streamProvider | Func`1 | Metoden som tillhandahåller inmatningsström för posten. |
| newEntrySettings | CabEntrySettings | Komprimerings- och krypteringsinställningar som används för det tillagda [`CabEntry`](../../cabentry/)‑objektet. |

### Returvärde

CAB‑postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Arkivet har instansierats för dekomprimering. - eller - Antalet filer har nått gränsen. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentException | *name* är null eller tomt. |

## Exempel

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Se även

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


