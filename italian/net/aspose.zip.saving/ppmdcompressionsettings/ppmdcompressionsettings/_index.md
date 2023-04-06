---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: PPMdCompressionSettings costruttore. Inizializza una nuova istanza diPPMdCompressionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Inizializza una nuova istanza di[`PPMdCompressionSettings`](../) classe.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| modelOrder | Int32 | Ordine del modello. |
| suballocatorSize | Int32 | La dimensione della memoria in MB suballocator può consumare. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* non è compreso tra 2 e 16. - oppure -*suballocatorSize* non è compreso tra 1 e 256. |

### Osservazioni

Ordini di modelli più grandi si traducono quasi sicuramente in una migliore compressione e sicuramente in un maggiore utilizzo di memoria e CPU.

L'algoritmo PPMd potrebbe richiedere molta memoria, specialmente se utilizzato su file di grandi dimensioni e/o utilizzato con un ordine di modello di grandi dimensioni. Se ppmd richiede più memoria di quella che gli dai, la compressione sarà peggiore.

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Guarda anche

* class [PPMdCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Inizializza una nuova istanza di[`PPMdCompressionSettings`](../) classe con ordine del modello predefinito e dimensione dell'allocatore secondario.

```csharp
public PPMdCompressionSettings()
```

### Osservazioni

L'ordine predefinito del modello è 8 e la dimensione dell'allocatore secondario è 50 MB.

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Guarda anche

* class [PPMdCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assemblea [Aspose.Zip](../../../)


