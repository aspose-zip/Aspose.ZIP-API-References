---
title: SevenZipArchiveEntry.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipArchiveEntry metodo. Estrae la voce nel filesystem dal percorso fornito.
type: docs
weight: 80
url: /it/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
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

### Esempi

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
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
| ArgumentException | *destination* non supporta la scrittura. |
| InvalidOperationException | L'archivio non è aperto per l'estrazione. - oppure - Questa voce è una directory. |
| InvalidDataException | Dati errati all'interno della voce. |

### Esempi

Estrarre una voce dell'archivio zip con password.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assemblea [Aspose.Zip](../../../)


