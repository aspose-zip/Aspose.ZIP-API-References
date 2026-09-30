---
title: "IsoArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo IsoArchive. Salva l'immagine ISO nel percorso specificato"
type: docs
weight: 70
url: /it/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Salva l'immagine ISO nel percorso specificato.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso in cui l'immagine ISO sarà salvata. |
| saveOptions | IsoSaveOptions | Opzioni con cui salvare l'archivio ISO. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generato quando l'archivio non è in modalità di modifica. |
| ArgumentNullException | Generato quando *path* è nullo. |
| DirectoryNotFoundException | Generato quando il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Generato quando il file è già aperto. |
| UnauthorizedAccessException | Generato quando l'accesso al file *path* è negato. |
| PathTooLongException | Generato quando il *path* specificato supera la lunghezza massima definita dal sistema. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

Il seguente esempio mostra come salvare un archivio ISO in un file:

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

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Salva l'immagine ISO nello stream specificato.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso in cui l'immagine ISO sarà salvata. |
| saveOptions | IsoSaveOptions | Opzioni con cui salvare l'archivio ISO. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generato quando l'archivio non è in modalità di modifica. |
| ArgumentNullException | Generato quando *stream* è nullo. |
| ArgumentException | Generata quando lo *stream* non è scrivibile. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| IOException | Si è verificato un errore di I/O. |

## Esempi

Il seguente esempio mostra come salvare un archivio ISO in uno stream di memoria:

```csharp

 // Crea un nuovo archivio ISO vuoto
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Aggiungi file all'archivio ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Salva l'archivio ISO in uno stream di memoria
     isoArchive.Save(memoryStream);
 }
```

### Vedi anche

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


