---
title: ArchiveEntry.CompressionProgressed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveEntry événement. Se déclenche lorsquune partie du flux brut est compressée.
type: docs
weight: 80
url: /fr/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Remarques

L'expéditeur de l'événement est un[`ArchiveEntry`](../) exemple.

### Exemples

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir également

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* espace de noms [Aspose.Zip](../../archiveentry/)
* Assemblée [Aspose.Zip](../../../)


