---
title: "ZstandardArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo ZstandardArchive. Salva l'archivio nello stream fornito"
type: docs
weight: 60
url: /it/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Stream di destinazione. |
| impostazioni | ZstandardSaveOptions | Impostazioni opzionali per la composizione dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentException | *outputStream* non è scrivibile. |
| InvalidOperationException | La sorgente non è stata fornita. |

## Osservazioni

*outputStream* must be writable.

## Esempi

Scrivi dati compressi nello stream di risposta http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Vedi anche

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| impostazioni | ZstandardSaveOptions | Impostazioni opzionali per la composizione dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentNullException | *destinationFileName* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *destinationFileName* è negato. |
| PathTooLongException | Il *destinationFileName* specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Per esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file a 260 caratteri. |
| NotSupportedException | Il file in *destinationFileName* contiene due punti (:) nel mezzo della stringa. |
| Eccezione | Generata quando si verifica un errore di runtime. |
| DirectoryNotFoundException | Il percorso specificato non è valido, (ad esempio, è su un'unità non mappata). |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| InvalidOperationException | La sorgente non è stata fornita. |

## Esempi

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Vedi anche

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | FileInfo | FileInfo, che verrà aperto come stream di destinazione. |
| impostazioni | ZstandardSaveOptions | Impostazioni opzionali per la composizione dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per aprire la *destinazione*. |
| ArgumentException | Il percorso del file è vuoto o contiene solo spazi bianchi. |
| FileNotFoundException | Il file non è stato trovato. |
| UnauthorizedAccessException | Il percorso del file è di sola lettura o è una directory. |
| ArgumentNullException | *destination* è nullo. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| InvalidOperationException | La sorgente non è stata fornita. |

## Esempi

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Vedi anche

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


