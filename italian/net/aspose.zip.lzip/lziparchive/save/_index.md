---
title: LzipArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: LzipArchive metodo. Salva larchivio lzip nello stream fornito.
type: docs
weight: 50
url: /it/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Salva l'archivio lzip nello stream fornito.

```csharp
public void Save(Stream outputStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *outputStream* non supporta la ricerca. |
| ArgumentNullException | *outputStream* è zero. |

### Osservazioni

*outputStream* deve essere ricercabile.

### Esempi

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Salva l'archivio lzip nel file di destinazione fornito.

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Salva l'archivio lzip nel file di destinazione fornito.

```csharp
public void Save(FileInfo destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destination | FileInfo | FileInfo che verrà aperto come flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per aprire il file*destination*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *destination* è zero. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Esempi

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)


