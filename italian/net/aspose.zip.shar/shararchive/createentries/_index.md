---
title: SharArchive.CreateEntries
second_title: Riferimento API Aspose.ZIP per .NET
description: SharArchive metodo. Aggiunge allarchivio tutti i file e le directory in modo ricorsivo nella directory data.
type: docs
weight: 30
url: /it/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | String | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

Condividi l'istanza di ingresso.

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
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | DirectoryInfo | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

Condividi l'istanza di ingresso.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *directory* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso*directory*. |
| IOException | *directory* sta per un file, non per una directory. |

### Esempi

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)


