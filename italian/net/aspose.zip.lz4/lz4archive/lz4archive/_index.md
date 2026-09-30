---
title: "Lz4Archive.Lz4Archive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore Lz4Archive. Inizializza una nuova istanza della classe Lz4Archive preparata per la decompressione"
type: docs
weight: 10
url: /it/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`Lz4Archive`](../) preparata per la decompressione.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. |
| loadOptions | Lz4LoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Impossibile leggere da *sourceStream* |
| ArgumentNullException | *sourceStream* è null. |
| EndOfStreamException | *sourceStream* è troppo corto. |
| InvalidDataException | Il *sourceStream* ha una firma errata. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| IOException | Si è verificato un errore di I/O. |

## Osservazioni

Questo costruttore non decomprime. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da uno stream ed estrailo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Inizializza una nuova istanza della classe [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |
| loadOptions | Lz4LoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| EndOfStreamException | Il file è troppo corto. |
| InvalidDataException | I dati nel file hanno una firma errata. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| FileNotFoundException | Il file non è stato trovato. |
| IOException | Il file è già aperto. |

## Osservazioni

Questo costruttore non decomprime. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da file tramite percorso ed estrailo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Inizializza una nuova istanza della classe [`Lz4Archive`](../) preparata per la compressione.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| impostazioni | Lz4ArchiveSetting | L'impostazione dell'archivio composto. |

### Vedi anche

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


