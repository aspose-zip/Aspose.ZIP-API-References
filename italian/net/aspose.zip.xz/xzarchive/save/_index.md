---
title: XzArchive.Save
second_title: Riferimento API Aspose.ZIP per .NET
description: XzArchive metodo. Salva larchivio xz nello stream fornito.
type: docs
weight: 40
url: /it/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

Salva l'archivio xz nello stream fornito.

```csharp
public void Save(Stream output)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Flusso di destinazione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *output* non supporta la ricerca. |
| ArgumentNullException | *output* è zero. |

### Osservazioni

*output* deve essere ricercabile.

### Esempi

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Guarda anche

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Salva l'archivio xz nel file di destinazione fornito.

```csharp
public void Save(string destinationFileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destinationFileName* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*destinationFileName* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*destinationFileName* è negato. |
| PathTooLongException | Il specificato*destinationFileName*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*destinationFileName* contiene i due punti (:) al centro della stringa. |

### Esempi

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Guarda anche

* class [XzArchive](../)
* spazio dei nomi [Aspose.Zip.Xz](../../xzarchive/)
* assemblea [Aspose.Zip](../../../)


