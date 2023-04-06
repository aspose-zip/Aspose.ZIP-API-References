---
title: ArchiveEntry.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveEntry metodo. Estrae la voce nel filesystem dal percorso fornito.
type: docs
weight: 100
url: /it/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

Estrae la voce nel filesystem dal percorso fornito.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |
| password | String | Password facoltativa per la decrittazione. |

### Valore di ritorno

Le informazioni sul file del file composto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |
| InvalidDataException | Verifica CRC o MAC non riuscita per la voce. |

### Esempi

Estrarre due voci dell'archivio zip, ciascuna con la propria password

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Guarda anche

* class [ArchiveEntry](../)
* spazio dei nomi [Aspose.Zip](../../archiveentry/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Estrae la voce nel flusso fornito.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destination | Stream | Flusso di destinazione. Deve essere scrivibile. |
| password | String | Password facoltativa per la decrittazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidDataException | Verifica CRC o MAC non riuscita per la voce. |
| ArgumentException | *destination* non supporta la scrittura. |

### Esempi

Estrarre una voce dell'archivio zip con password.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Guarda anche

* class [ArchiveEntry](../)
* spazio dei nomi [Aspose.Zip](../../archiveentry/)
* assemblea [Aspose.Zip](../../../)


