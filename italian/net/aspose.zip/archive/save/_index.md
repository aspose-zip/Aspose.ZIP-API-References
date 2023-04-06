---
title: Archive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: Archive metodo. Salva larchivio nello stream fornito.
type: docs
weight: 90
url: /it/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | Stream | Flusso di destinazione. |
| saveOptions | ArchiveSaveOptions | Opzioni per il salvataggio in archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *outputStream* non è scrivibile. |

### Osservazioni

*outputStream*deve essere scrivibile.

### Esempi

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Guarda anche

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| saveOptions | ArchiveSaveOptions | Opzioni per il salvataggio in archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*destinationFileName* è negato. |
| PathTooLongException | Il specificato*destinationFileName*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*destinationFileName* contiene i due punti (:) al centro della stringa. |

### Osservazioni

È possibile salvare un archivio nello stesso percorso da cui è stato caricato. Tuttavia, ciò non è consigliato poiché questo approccio utilizza la copia in un file temporaneo.

### Esempi

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Guarda anche

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)


