---
title: CreateEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Crea una singola voce allinterno dellarchivio.
type: docs
weight: 50
url: /it/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio dell'archivio. |
| newEntrySettings | SevenZipEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`SevenZipArchiveEntry`](../../sevenziparchiveentry) elemento. |

### Valore di ritorno

Istanza di ingresso Seven Zip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* è di sola lettura o è una directory. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately* parametro viene bloccato fino al salvataggio dell'archivio.

### Esempi

Componi l'archivio con voci crittografate con password diverse ciascuna.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |
| newEntrySettings | SevenZipEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`SevenZipArchiveEntry`](../../sevenziparchiveentry) elemento. |
| fileInfo | FileSystemInfo | metadati del file o della cartella da comprimere. |

### Valore di ritorno

Istanza di ingresso SevenZip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Tutti e due*source* e*fileInfo* sono nulli o*source* è nullo e*fileInfo* sta per directory. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimentoDirectoryInfo se la voce è directory.

### Esempi

Componi l'archivio con la voce crittografata compressa LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |
| newEntrySettings | SevenZipEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`SevenZipArchiveEntry`](../../sevenziparchiveentry) elemento. |

### Valore di ritorno

Istanza di immissione zip.

### Esempi

Componi l'archivio 7z con la compressione LZMA2 e la crittografia di tutte le voci.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Crea una singola voce all'interno dell'archivio.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| path | String | Il nome completo del nuovo file o il relativo nome del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio dell'archivio. |
| newEntrySettings | SevenZipEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`SevenZipArchiveEntry`](../../sevenziparchiveentry) elemento. |

### Valore di ritorno

Istanza di immissione zip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere |
| ArgumentException | Il*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso al file*path* è negato. |
| PathTooLongException | Il specificato*path*, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, sulle piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Archivia a*path* contiene due punti (:) al centro della stringa. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*path* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately* parametro viene bloccato fino al salvataggio dell'archivio.

### Esempi

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Guarda anche

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive)
* assemblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
