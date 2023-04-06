---
title: SharArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: SharArchive metodo. Salva larchivio nel file di destinazione fornito.
type: docs
weight: 70
url: /it/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destinationFileName* è una stringa di lunghezza zero, contiene solo spazi vuoti o contiene uno o più caratteri non validi come definito da System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* è zero. |
| PathTooLongException | Il specificato*destinationFileName*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| DirectoryNotFoundException | Il specificato*destinationFileName* non è valido (ad esempio, si trova su un'unità non mappata). |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| UnauthorizedAccessException | *destinationFileName* specificato un file di sola lettura e l'accesso non è Read.-oppure- percorso specificato una directory.-oppure- Il chiamante non dispone dell'autorizzazione richiesta. |
| NotSupportedException | *destinationFileName* è in un formato non valido. |

### Osservazioni

È possibile salvare un archivio nello stesso percorso da cui è stato caricato. Tuttavia, ciò non è consigliato poiché questo approccio utilizza la copia in un file temporaneo.

### Esempi

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream output)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è zero. |
| ArgumentException | *output* non è scrivibile. - O -*output* è lo stesso flusso da cui estraiamo. |

### Osservazioni

*output*deve essere scrivibile.

### Esempi

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)


