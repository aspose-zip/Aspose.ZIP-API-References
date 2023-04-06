---
title: TarArchive.TarArchive
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive byggare. Initierar en ny instans avTarArchive class.
type: docs
weight: 10
url: /sv/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Initierar en ny instans av[`TarArchive`](../) class.

```csharp
public TarArchive()
```

### Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Initierar en ny instans av[`Archive`](../../../aspose.zip/archive/) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public TarArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. Det måste vara sökbart. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidDataException | *sourceStream* är inte sökbar. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../tarentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Initierar en ny instans av[`TarArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public TarArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivfilen. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../tarentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


