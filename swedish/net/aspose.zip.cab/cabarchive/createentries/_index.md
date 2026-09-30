---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CabArchive‑metod. Lägger till alla filer rekursivt från den angivna katalogen i arkivet"
type: docs
weight: 30
url: /sv/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Lägger till alla filer, rekursivt, från den angivna katalogen i arkivet.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | DirectoryInfo | Katalog att komprimera. |
| includeRootDirectory | Boolean | Anger om rotkatalogens namn ska inkluderas i postvägar. |

### Returvärde

Den aktuella [`CabArchive`](../)‑instansen.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *directory* är null. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| DirectoryNotFoundException | *directory* kan inte hittas. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt *directory* eller dess innehåll. |
| UnauthorizedAccessException | Åtkomst till *directory* eller någon av dess filer nekas. |
| IOException | Ett I/O-fel uppstår när *directory* nås. |
| PathTooLongException | Den genererade postens sökväg överskrider systemdefinierad maximal längd. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte lägga till poster. |

## Exempel

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Se även

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Lägger till alla filer rekursivt från den angivna katalogsökvägen i arkivet.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceDirectory | String | Katalogsökväg att komprimera. |
| includeRootDirectory | Boolean | Anger om rotkatalogens namn ska inkluderas i postvägar. |

### Returvärde

Den aktuella [`CabArchive`](../)‑instansen.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | *sourceDirectory* är null. |
| DirectoryNotFoundException | *sourceDirectory* kan inte hittas. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt *sourceDirectory*. |
| UnauthorizedAccessException | Åtkomst till *sourceDirectory* nekas. |
| PathTooLongException | Den angivna *sourceDirectory* överskrider systemdefinierad maximal längd. |
| ArgumentException | *sourceDirectory* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| IOException | Ett I/O-fel uppstår när *sourceDirectory* nås. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte lägga till poster. |

## Exempel

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Se även

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


