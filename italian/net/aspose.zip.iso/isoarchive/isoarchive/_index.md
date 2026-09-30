---
title: "IsoArchive.IsoArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore IsoArchive. Inizializza una nuova istanza della classe IsoArchive e crea un archivio ISO vuoto per aggiungere nuovi file e directory."
type: docs
weight: 10
url: /it/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Inizializza una nuova istanza della classe [`IsoArchive`](../) e crea un archivio ISO vuoto per aggiungere nuovi file e directory.

```csharp
public IsoArchive()
```

## Esempi

Il seguente esempio mostra come creare un nuovo archivio ISO vuoto e aggiungere file ad esso:

```csharp
// Crea un nuovo archivio ISO vuoto
using(IsoArchive isoArchive = new IsoArchive())
{
    // Aggiungi file all'archivio ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Salva l'archivio ISO in un file
    isoArchive.Save("new_archive.iso");
}
```

### Vedi anche

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`IsoArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. Deve supportare la ricerca. |
| loadOptions | IsoLoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è null. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un archivio ISO valido. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| EndOfStreamException | Generata quando la fine del flusso viene raggiunta inaspettatamente. |
| IOException | Si è verificato un errore di I/O. |
| NotSupportedException | Il flusso non supporta la lettura. |

## Osservazioni

Questo costruttore non estrae alcuna voce.

## Esempi

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Vedi anche

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Inizializza una nuova istanza della classe [`IsoArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |
| loadOptions | IsoLoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| FileNotFoundException | Il file non è stato trovato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| EndOfStreamException | Il file è troppo corto. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

## Osservazioni

Questo costruttore non estrae alcuna voce.

## Esempi

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Vedi anche

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


