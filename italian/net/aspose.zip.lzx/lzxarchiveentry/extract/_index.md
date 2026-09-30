---
title: "LzxArchiveEntry.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo LzxArchiveEntry. Estrae la voce dell'archivio Lzx in un file system per percorso"
type: docs
weight: 80
url: /it/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Estrae la voce dell'archivio Lzx in un file system tramite percorso.

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
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| NotSupportedException | Metodo di compressione non valido. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| EndOfStreamException | Generata quando la fine del flusso viene raggiunta inaspettatamente. |

## Esempi

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Vedi anche

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| ArgumentNullException | Il flusso di destinazione è nullo. |
| NotSupportedException | Metodo di compressione non valido. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| EndOfStreamException | Generata quando la fine del flusso viene raggiunta inaspettatamente. |

### Vedi anche

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


