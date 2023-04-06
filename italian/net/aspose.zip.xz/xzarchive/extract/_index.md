---
title: XzArchive.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: XzArchive metodo. Estrae larchivio xz in un flusso.
type: docs
weight: 30
url: /it/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Estrae l'archivio xz in un flusso.

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

### Esempi

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Guarda anche

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Estrae l'archivio xz in un file.

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
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Guarda anche

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Estrae l'archivio xz in un file per percorso.

```csharp
public FileInfo Extract(string path)
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
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Guarda anche

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)


