---
title: "Lz4Archive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo Lz4Archive. Salva l'archivio lz4 nello stream fornito"
type: docs
weight: 60
url: /it/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Salva l'archivio lz4 nello stream fornito.

```csharp
public void Save(Stream output)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Stream di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è nullo. |
| ArgumentException | *output* non è scrivibile. |
| InvalidOperationException | L'archivio è pronto per l'estrazione. - oppure - La sorgente non è stata fornita. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generato quando la compressione viene annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

*output* must be seekable.

## Esempi

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Salva l'archivio lz4 nel file di destinazione fornito.

```csharp
public void Save(FileInfo destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | FileInfo | FileInfo, che verrà aperto come stream di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per aprire la *destinazione*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *destination* è nullo. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| InvalidOperationException | L'archivio è pronto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere |
| ArgumentException | Il *destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *destinationFileName* è negato. |
| PathTooLongException | Il *destinationFileName* specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Per esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file a 260 caratteri. |
| NotSupportedException | Il file in *destinationFileName* contiene due punti (:) nel mezzo della stringa. |
| InvalidOperationException | L'archivio è pronto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, (ad esempio, è su un'unità non mappata). |
| FileNotFoundException | Il file specificato in *destinationFileName* non è stato trovato. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |

## Esempi

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


