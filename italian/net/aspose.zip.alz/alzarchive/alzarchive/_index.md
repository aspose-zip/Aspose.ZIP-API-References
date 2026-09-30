---
title: "AlzArchive.AlzArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore AlzArchive. Inizializza una nuova istanza della classe AlzArchive da uno stream"
type: docs
weight: 10
url: /it/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Inizializza una nuova istanza della classe [`AlzArchive`](../) da un flusso.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso dell'archivio ALZ. Il flusso deve supportare la lettura e lo spostamento. |
| loadOptions | AlzArchiveLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Il flusso è nullo. |

### Vedi anche

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`AlzArchive`](../) da un percorso file.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso del file di archivio ALZ. |
| loadOptions | AlzArchiveLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Il percorso del file è nullo. |
| FileNotFoundException | Il file non esiste. |

### Vedi anche

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


