---
title: Bzip2Archive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: Bzip2Archive metodo. Salva larchivio nello stream fornito.
type: docs
weight: 50
url: /it/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Flusso di destinazione. |
| saveOptions | Bzip2SaveOptions | Opzioni per salvare un archivio bzip2. Se non specificato, verrà utilizzata una dimensione del blocco di 900 Kb. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | La fonte dei dati da archiviare non è stata fornita. |
| ArgumentException | *outputStream* non è scrivibile. |
| UnauthorizedAccessException | L'origine del file è di sola lettura o è una directory. |
| DirectoryNotFoundException | Il percorso di origine del file specificato non è valido, ad esempio si trova su un'unità non mappata. |
| IOException | L'origine file è già aperta. |

### Osservazioni

*outputStream*deve essere scrivibile.

### Esempi

Scrive dati compressi nel flusso di risposta http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Guarda anche

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| saveOptions | Bzip2SaveOptions | Opzioni per salvare un archivio bzip2. Se non specificato, verrà utilizzata una dimensione del blocco di 900 Kb. |

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

Scrive dati compressi su file.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Guarda anche

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)


