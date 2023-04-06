---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchive byggare. Initierar en ny instans avSevenZipArchive klass med valfria inställningar för dess poster.
type: docs
weight: 10
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Initierar en ny instans av[`SevenZipArchive`](../) klass med valfria inställningar för dess poster.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. Om inte specificerat, skulle LZMA-komprimering utan kryptering användas. |

### Exempel

Följande exempel visar hur man komprimerar en enskild fil med standardinställningar: LZMA-komprimering utan kryptering.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Se även

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Initierar en ny instans av[`SevenZipArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *sourceStream* är inte sökbar. |
| ArgumentNullException | *sourceStream* är inget. |
| NotImplementedException | Arkivet innehåller mer än en kodare. Nu stöds endast LZMA-komprimering. |

### Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Ser[`ExtractToDirectory`](../extracttodirectory/) metod för dekomprimering.

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Initierar en ny instans av[`SevenZipArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public SevenZipArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Den fullt kvalificerade eller den relativa sökvägen till arkivfilen. |

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

Denna konstruktor dekomprimerar inte någon post. Ser[`ExtractToDirectory`](../extracttodirectory/) metod för dekomprimering.

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)


