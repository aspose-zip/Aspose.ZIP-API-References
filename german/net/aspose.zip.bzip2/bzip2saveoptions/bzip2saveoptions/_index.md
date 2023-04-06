---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2SaveOptions constructeur. Initialisiert eine neue Instanz vonBzip2SaveOptions Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Initialisiert eine neue Instanz von[`Bzip2SaveOptions`](../) Klasse.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | Int32 | Blockgröße in Hunderten von Kilobyte. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Die Blockgröße liegt nicht im gültigen Bereich. |

### Beispiele

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

### Siehe auch

* class [Bzip2SaveOptions](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* Montage [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Initialisiert eine neue Instanz von[`Bzip2SaveOptions`](../) Klasse mit Standardblockgröße, entspricht 900 Kilobyte.

```csharp
public Bzip2SaveOptions()
```

### Beispiele

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

### Siehe auch

* class [Bzip2SaveOptions](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* Montage [Aspose.Zip](../../../)


