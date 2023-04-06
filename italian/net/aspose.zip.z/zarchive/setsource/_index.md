---
title: ZArchive.SetSource
second_title: Riferimento API Aspose.ZIP per .NET
description: ZArchive metodo. Imposta il contenuto da comprimere allinterno dellarchivio.
type: docs
weight: 50
url: /it/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | Il flusso di input per l'archivio. |

### Esempi

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo che verrà aperto come flusso di input. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per aprire il file*fileInfo*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *fileInfo* è zero. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |

### Esempi

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Imposta il contenuto da comprimere all'interno dell'archivio.

```csharp
public void SetSource(string sourcePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourcePath | String | Percorso del file che verrà aperto come flusso di input. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourcePath* è una stringa nulla o vuota. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a una risorsa. |
| ArgumentException | IL*sourcePath* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*sourcePath* è negato. |
| PathTooLongException | Il specificato*sourcePath*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*sourcePath* contiene i due punti (:) al centro della stringa. |

### Esempi

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### Guarda anche

* class [ZArchive](../)
* spazio dei nomi [Aspose.Zip.Z](../../zarchive/)
* assemblea [Aspose.Zip](../../../)


