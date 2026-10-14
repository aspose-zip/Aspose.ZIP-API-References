---
title: "EggArchive.EggArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore EggArchive. Inizializza una nuova istanza della classe EggArchive da uno stream"
type: docs
weight: 10
url: /it/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Inizializza una nuova istanza della classe [`EggArchive`](../) da uno stream.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream dell'archivio EGG. Lo stream deve supportare la lettura e la ricerca. |
| loadOptions | EggArchiveLoadOptions | Opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *stream* è nullo. |
| ArgumentException | *stream* non è leggibile né ricercabile. |

### Vedi anche

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`EggArchive`](../) da un percorso di file.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Percorso al file di archivio EGG. |
| loadOptions | EggArchiveLoadOptions | Opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| FileNotFoundException | Il file non esiste. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| FileNotFoundException | Il file non è stato trovato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Vedi anche

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


