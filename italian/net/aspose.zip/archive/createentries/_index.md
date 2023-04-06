---
title: Archive.CreateEntries
second_title: Riferimento API Aspose.ZIP per .NET
description: Archive metodo. Aggiunge allarchivio tutti i file e le directory in modo ricorsivo nella directory data.
type: docs
weight: 40
url: /it/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | DirectoryInfo | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

L'archivio con le voci composte.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| DirectoryNotFoundException | Il percorso verso*directory* non è valido, ad esempio trovarsi su un'unità non mappata. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso*directory*. |

### Esempi

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Guarda anche

* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory data.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | String | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere o meno la directory radice stessa. |

### Valore di ritorno

L'archivio con le voci composte.

### Esempi

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Guarda anche

* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)


