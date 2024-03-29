---
title: LzipArchive.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: LzipArchive metodo. Estrae larchivio lzip in un flusso.
type: docs
weight: 40
url: /it/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

Estrae l'archivio lzip in un flusso.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destination | Stream | Flusso per l'archiviazione dei dati decompressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Le intestazioni dell'archivio e le informazioni di servizio non sono state lette. |
| InvalidDataException | Errore nei dati nell'intestazione o nel checksum. |
| ArgumentNullException | Il flusso di destinazione è nullo. |
| ArgumentException | Il flusso di destinazione non supporta la scrittura. |

### Esempi

```csharp
using (FileStream sourceLzipFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new LzipArchive(sourceLzipFile))
        {
               archive.Extract(extractedFile);
           }
       }
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Estrae l'archivio lzip in un file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo per la memorizzazione di dati decompressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Le intestazioni dell'archivio e le informazioni di servizio non sono state lette. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per aprire il file*fileInfo*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *fileInfo* è zero. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Esempi

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Estrae l'archivio lzip in un file per percorso.

```csharp
public void Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Percorso del file che memorizzerà i dati decompressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Le intestazioni dell'archivio e le informazioni di servizio non sono state lette. |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Esempi

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)


