---
title: "UueArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo UueArchive. Salva l'archivio nello stream fornito"
type: docs
weight: 70
url: /it/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Stream di destinazione. |
| saveOptions | UueSaveOptions | Opzioni per il salvataggio dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | La sorgente dei dati da archiviare non è stata fornita. |
| ArgumentException | *outputStream* non è scrivibile. |
| UnauthorizedAccessException | La sorgente del file è di sola lettura o è una directory. |
| DirectoryNotFoundException | Il percorso della sorgente file specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | La sorgente del file è già aperta. |

## Osservazioni

*outputStream* must be writable.

## Esempi

Scrivi dati compressi nello stream di risposta http.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Vedi anche

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Salva l'archivio in un file di destinazione fornito.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| saveOptions | UueSaveOptions | Opzioni per il salvataggio dell'archivio. |

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
| InvalidOperationException | La sorgente dei dati da archiviare non è stata fornita. |

## Esempi

Scrivi dati codificati su file.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Vedi anche

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


