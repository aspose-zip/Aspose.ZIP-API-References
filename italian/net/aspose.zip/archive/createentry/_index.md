---
title: Archive.CreateEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Archive metodo. Crea una singola voce allinterno dellarchivio.
type: docs
weight: 50
url: /it/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Crea una singola voce all'interno dell'archivio.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| path | String | Il nome completo del nuovo file o il relativo nome del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`ArchiveEntry`](../../archiveentry/) articolo. |

### Valore di ritorno

Istanza di ingresso zip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*path* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately* parametro diventa bloccato fino al salvataggio dell'archivio.

### Esempi

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Guarda anche

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`ArchiveEntry`](../../archiveentry/) articolo. |

### Valore di ritorno

Istanza di ingresso zip.

### Esempi

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Guarda anche

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`ArchiveEntry`](../../archiveentry/) articolo. |

### Valore di ritorno

Istanza di ingresso zip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* è di sola lettura o è una directory. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately* parametro diventa bloccato fino al salvataggio dell'archivio.

### Esempi

Componi un archivio con voci crittografate con diversi metodi di crittografia e password ciascuno.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Guarda anche

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'aggiunta[`ArchiveEntry`](../../archiveentry/) articolo. |
| fileInfo | FileSystemInfo | I metadati del file o della cartella da comprimere. |

### Valore di ritorno

Istanza di ingresso zip.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Entrambi*source* E*fileInfo* sono nulli o*source*è nullo e*fileInfo* sta per directory. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimento aDirectoryInfo se la voce è directory.

### Esempi

Componi archivio con voce crittografata.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Guarda anche

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)


