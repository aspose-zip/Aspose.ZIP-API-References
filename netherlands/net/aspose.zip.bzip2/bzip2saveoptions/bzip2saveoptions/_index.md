---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2SaveOptions constructeur. Initialiseert een nieuw exemplaar van hetBzip2SaveOptions klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Bzip2SaveOptions`](../) klasse.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | Int32 | Blokgrootte in honderden kilobytes. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | Blokgrootte valt niet binnen het geldige bereik. |

### Voorbeelden

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

### Zie ook

* class [Bzip2SaveOptions](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* montage [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Initialiseert een nieuw exemplaar van het[`Bzip2SaveOptions`](../) klasse met standaard blokgrootte, gelijk aan 9 honderd kilobytes.

```csharp
public Bzip2SaveOptions()
```

### Voorbeelden

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

### Zie ook

* class [Bzip2SaveOptions](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* montage [Aspose.Zip](../../../)


