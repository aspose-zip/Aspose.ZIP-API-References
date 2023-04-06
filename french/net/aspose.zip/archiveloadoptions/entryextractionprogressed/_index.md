---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveLoadOptions propriété. Obtient ou définit le délégué appelé lorsque certains octets ont été extraits.
type: docs
weight: 40
url: /fr/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Obtient ou définit le délégué appelé lorsque certains octets ont été extraits.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Remarques

L'expéditeur de l'événement est le[`ArchiveEntry`](../../archiveentry/) instance dont l'extraction est en cours.

### Exemples

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Voir également

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* espace de noms [Aspose.Zip](../../archiveloadoptions/)
* Assemblée [Aspose.Zip](../../../)


