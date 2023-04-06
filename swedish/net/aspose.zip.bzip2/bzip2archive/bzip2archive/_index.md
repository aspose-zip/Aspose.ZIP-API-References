---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP för .NET API-referens
description: Bzip2Archive byggare. Initierar en ny instans avBzip2Archive klass förberedd för komprimering.
type: docs
weight: 10
url: /sv/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Initierar en ny instans av[`Bzip2Archive`](../) klass förberedd för komprimering.

```csharp
public Bzip2Archive()
```

### Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Se även

* class [Bzip2Archive](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2archive/)
* hopsättning [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Initierar en ny instans av[`Bzip2Archive`](../) klass förberedd för dekomprimering.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Open`](../open/) metod för dekomprimering.

### Exempel

Öppna ett arkiv från en ström och extrahera det till en`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Se även

* class [Bzip2Archive](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2archive/)
* hopsättning [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Initierar en ny instans av[`Bzip2Archive`](../) klass förberedd för dekomprimering.

```csharp
public Bzip2Archive(string path)
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

Denna konstruktor dekomprimerar inte. Ser[`Open`](../open/) metod för dekomprimering.

### Exempel

Öppna ett arkiv från fil för sökväg och extrahera det till en`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Se även

* class [Bzip2Archive](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2archive/)
* hopsättning [Aspose.Zip](../../../)


