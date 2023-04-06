---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP för .NET API-referens
description: CpioArchive byggare. Initierar en ny instans avCpioArchive class.
type: docs
weight: 10
url: /sv/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Initierar en ny instans av[`CpioArchive`](../) class.

```csharp
public CpioArchive()
```

### Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Se även

* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Initierar en ny instans av[`CpioArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. Det måste vara sökbart. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *sourceStream* är inget. |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | *sourceStream* är inte giltigt cpio-arkiv. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../cpioentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Initierar en ny instans av[`CpioArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public CpioArchive(string path)
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

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../cpioentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)


