---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: Bzip2CompressionSettings costruttore. Inizializza una nuova istanza diBzip2CompressionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Inizializza una nuova istanza di[`Bzip2CompressionSettings`](../) classe.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | Int32 | Dimensione del blocco in centinaia di kilobyte. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | La dimensione del blocco non è compresa tra 1 e 9. |

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [Bzip2CompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Inizializza una nuova istanza di[`Bzip2CompressionSettings`](../) classe con dimensione del blocco predefinita, pari a 9 centinaia di kilobyte.

```csharp
public Bzip2CompressionSettings()
```

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [Bzip2CompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assemblea [Aspose.Zip](../../../)


