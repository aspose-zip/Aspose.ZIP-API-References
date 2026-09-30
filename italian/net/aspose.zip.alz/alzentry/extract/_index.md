---
title: "AlzEntry.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo AlzEntry. Estrae la voce nel file system nel percorso fornito"
type: docs
weight: 60
url: /it/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Estrae la voce nel file system usando il percorso fornito.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |
| password | String | Password opzionale per la decrittazione. |

### Valore restituito

Le informazioni file di un file composto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| InvalidDataException | L'archivio è corrotto. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| FileNotFoundException | Il file non è stato trovato. |

## Esempi

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Vedi anche

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Estrae la voce nello stream fornito.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |
| password | String | Password opzionale per la decrittazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |
| InvalidOperationException | L'archivio non è aperto per l'estrazione. - oppure - Questa voce è una directory. |
| InvalidDataException | Dati errati nella voce. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |

## Esempi

Estrai una voce dell'archivio ALZ con password.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Vedi anche

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


