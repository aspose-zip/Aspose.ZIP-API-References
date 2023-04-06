---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipLZMA2CompressionSettings costruttore. Crea unistanza delle impostazioni per il metodo di compressione LZMA2 allinterno dellarchivio 7z.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Crea un'istanza delle impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dictionarySize | Int32 | Dimensione del buffer cronologico, deve essere compresa tra 4096 e 1073741824. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* è troppo grande o troppo piccolo. |

### Osservazioni

Più grande è il dizionario, migliore è di solito il rapporto di compressione, ma i dizionari più grandi dei dati non compressi sono uno spreco di RAM.

### Guarda anche

* class [SevenZipLZMA2CompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Crea un'istanza delle impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dictionarySize | Int32 | Dimensione del buffer cronologico, deve essere compresa tra 4096 e 1073741824. |
| fastBytes | Int32 | Controlla il numero di byte veloci utilizzati dai compressori LZMA2. Un numero maggiore di byte veloci può fornire un rapporto di compressione migliore a scapito della velocità di compressione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* è troppo grande o troppo piccolo, o*fastBytes* è troppo grande o troppo piccolo. |

### Osservazioni

Più grande è il dizionario, migliore è di solito il rapporto di compressione, ma i dizionari più grandi dei dati non compressi sono uno spreco di RAM.

### Guarda anche

* class [SevenZipLZMA2CompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assemblea [Aspose.Zip](../../../)


