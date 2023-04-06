---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipPPMdCompressionSettings costruttore. Crea unistanza delle impostazioni per il metodo di compressione PPMd allinterno dellarchivio 7z.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Crea un'istanza delle impostazioni per il metodo di compressione PPMd all'interno dell'archivio 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| maxOrder | Byte | Ordine massimo. |
| suballocatorSize | Int32 | La dimensione della memoria in MB suballocator può consumare. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* non è compreso tra 2 e 32, o*suballocatorSize* non è compreso tra 1 e 1024. |

### Osservazioni

Ordini di modelli più grandi si traducono quasi sicuramente in una migliore compressione e sicuramente in un maggiore utilizzo di memoria e CPU.

L'algoritmo PPMd potrebbe richiedere molta memoria, specialmente se utilizzato su file di grandi dimensioni e/o utilizzato con un ordine di modello di grandi dimensioni. Se ppmd richiede più memoria di quella che gli dai, la compressione sarà peggiore.

### Esempi

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Guarda anche

* class [SevenZipPPMdCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Crea un'istanza delle impostazioni per il metodo di compressione PPMd all'interno dell'archivio 7z con l'ordine del modello predefinito e la dimensione dell'allocatore secondario.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Osservazioni

L'ordine predefinito del modello è 6 e la dimensione dell'allocatore secondario è 16 MB.

### Esempi

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Guarda anche

* class [SevenZipPPMdCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assemblea [Aspose.Zip](../../../)


