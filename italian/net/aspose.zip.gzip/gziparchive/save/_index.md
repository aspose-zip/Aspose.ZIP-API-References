---
title: GzipArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: GzipArchive metodo. Salva larchivio nello stream fornito.
type: docs
weight: 60
url: /it/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *outputStream* non è scrivibile. |
| InvalidOperationException | La fonte non è stata fornita. |

### Osservazioni

*outputStream*deve essere scrivibile.

### Esempi

Scrive dati compressi nel flusso di risposta http.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

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
| ArgumentNullException | *destinationFileName* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*destinationFileName* è negato. |
| PathTooLongException | Il specificato*destinationFileName*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*destinationFileName* contiene i due punti (:) al centro della stringa. |

### Esempi

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)


