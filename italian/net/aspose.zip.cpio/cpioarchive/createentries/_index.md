---
title: CpioArchive.CreateEntries
second_title: Riferimento API Aspose.ZIP per .NET
description: CpioArchive metodo. Aggiunge allarchivio tutti i file e le directory in modo ricorsivo nella directory data.
type: docs
weight: 30
url: /it/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | String | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

Istanza di ingresso Cpio.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceDirectory* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso*sourceDirectory*. |
| ArgumentException | *sourceDirectory* contiene caratteri non validi come ", &lt;, &gt; o &#x7C;. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. Il percorso specificato, il nome file o entrambi sono troppo lunghi. |
| IOException | *sourceDirectory* sta per un file, non per una directory. |

### Esempi

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Guarda anche

* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | DirectoryInfo | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

Istanza di ingresso Cpio.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *directory* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso*directory*. |
| IOException | *directory* sta per un file, non per una directory. |

### Esempi

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Guarda anche

* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)


