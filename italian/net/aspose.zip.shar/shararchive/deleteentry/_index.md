---
title: SharArchive.DeleteEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: SharArchive metodo. Rimuove la prima occorrenza di una voce specifica dallelenco delle voci.
type: docs
weight: 50
url: /it/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | SharEntry | La voce da rimuovere dall'elenco delle voci. |

### Valore di ritorno

Condividi l'istanza di ingresso.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *entry* è zero. |

### Esempi

Ecco come rimuovere tutte le voci tranne l'ultima:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Guarda anche

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Rimuove la voce dall'elenco delle voci per indice.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entryIndex | Int32 | Indice in base zero della voce da rimuovere. |

### Valore di ritorno

L'archivio con la voce eliminata.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* è minore di 0.-o-*entryIndex* è uguale o maggiore di`Inserimenti` contare. |

### Esempi

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)


