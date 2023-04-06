---
title: CpioArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: CpioArchive metodo. Salva larchivio nel file di destinazione fornito.
type: docs
weight: 80
url: /it/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Salva l'archivio nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

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
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Guarda anche

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Salva l'archivio nello stream fornito.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Flusso di destinazione. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è zero. |
| ArgumentException | *output* non è scrivibile. - O -*output* è lo stesso flusso da cui estraiamo. - OR - È impossibile salvare l'archivio in*cpioFormat* a causa di restrizioni di formato. |

### Osservazioni

*output*deve essere scrivibile.

### Esempi

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Guarda anche

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)


