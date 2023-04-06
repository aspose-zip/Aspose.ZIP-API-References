---
title: ArchiveEntry.ExtractionProgressed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveEntry événement. Se déclenche lorsquune partie du flux brut est extraite.
type: docs
weight: 90
url: /fr/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Se déclenche lorsqu'une partie du flux brut est extraite.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Remarques

L'expéditeur de l'événement est un[`ArchiveEntry`](../) exemple.

### Exemples

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### Voir également

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* espace de noms [Aspose.Zip](../../archiveentry/)
* Assemblée [Aspose.Zip](../../../)


