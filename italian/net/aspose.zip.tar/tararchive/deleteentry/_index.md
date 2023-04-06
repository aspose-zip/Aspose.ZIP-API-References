---
title: TarArchive.DeleteEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Rimuove la prima occorrenza di una voce specifica dallelenco delle voci.
type: docs
weight: 90
url: /it/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | TarEntry | La voce da rimuovere dall'elenco delle voci. |

### Valore di ritorno

L'archivio con la voce eliminata.

### Esempi

Ecco come rimuovere tutte le voci tranne l'ultima:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Rimuove la voce dall'elenco delle voci per indice.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)


