---
title: "LhaArchiveEntry.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "LhaArchiveEntry metodo. Estrae la voce dell'archivio Lha in un file system per percorso"
type: docs
weight: 60
url: /it/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Estrae la voce dell'archivio Lha in un file system tramite percorso.

```csharp
public FileSystemInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Percorso del file che conterrà i dati decompressi. |

### Valore restituito

FileSystemInfoInstance contenente i dati estratti.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Intestazioni dell'archivio e informazioni di servizio non sono state lette. |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

## Esempi

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Vedi anche

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Estrae la voce nello stream fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

## Osservazioni

Non fa nulla per la voce della directory.

### Vedi anche

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Estrae la voce dell'archivio Lha in un file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo per memorizzare i dati decompressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Intestazioni dell'archivio e informazioni di servizio non sono state lette. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per aprire il *fileInfo*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *fileInfo* è nullo. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |

## Osservazioni

Non fa nulla per la voce della directory.

## Esempi

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Vedi anche

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


