---
title: "XarArchive.DeleteEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo XarArchive. Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci"
type: docs
weight: 50
url: /it/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| voce | XarEntry | La voce da rimuovere dall'elenco delle voci. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *entry* è nullo. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | L'archivio non è aperto per l'estrazione. |

## Esempi

Ecco come è possibile rimuovere tutte le voci tranne l'ultima:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Vedi anche

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


