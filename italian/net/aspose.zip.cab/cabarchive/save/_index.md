---
title: "CabArchive.Save"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo CabArchive. Salva l'archivio nello stream fornito"
type: docs
weight: 70
url: /it/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Stream di destinazione. |
| saveOptions | CabSaveOptions | Opzioni per il salvataggio dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *outputStream* non è scrivibile né ricercabile. |
| ObjectDisposedException | L'archivio è stato eliminato. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può essere salvato. |

## Osservazioni

*outputStream* must be writable.

## Esempi

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Vedi anche

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| saveOptions | CabSaveOptions | Opzioni per il salvataggio dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *destinationFileName* è negato. |
| PathTooLongException | Il *destinationFileName* specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Per esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file a 260 caratteri. |
| NotSupportedException | Il file in *destinationFileName* contiene due punti (:) nel mezzo della stringa. |
| FileNotFoundException | Il file non è stato trovato. |
| InvalidOperationException | L'archivio è aperto per l'estrazione. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

È possibile salvare un archivio nello stesso percorso da cui è stato caricato. Tuttavia, non è consigliato perché questo approccio utilizza la copia in un file temporaneo.

## Esempi

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Vedi anche

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


