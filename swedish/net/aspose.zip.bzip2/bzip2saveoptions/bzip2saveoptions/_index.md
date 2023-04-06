---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP för .NET API-referens
description: Bzip2SaveOptions byggare. Initierar en ny instans avBzip2SaveOptions class.
type: docs
weight: 10
url: /sv/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Initierar en ny instans av[`Bzip2SaveOptions`](../) class.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | Int32 | Blockstorlek i hundratals kilobyte. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | Blockstorleken är inte i giltigt intervall. |

### Exempel

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### Se även

* class [Bzip2SaveOptions](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* hopsättning [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Initierar en ny instans av[`Bzip2SaveOptions`](../) klass med standardblockstorlek, lika med 9 hundra kilobyte.

```csharp
public Bzip2SaveOptions()
```

### Exempel

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### Se även

* class [Bzip2SaveOptions](../)
* namnutrymme [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* hopsättning [Aspose.Zip](../../../)


