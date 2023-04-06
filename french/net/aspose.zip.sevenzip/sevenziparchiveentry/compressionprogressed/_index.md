---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipArchiveEntry événement. Se déclenche lorsquune partie du flux brut est compressée.
type: docs
weight: 70
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Se déclenche lorsqu'une partie du flux brut est compressée.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### Remarques

L'expéditeur de l'événement est un[`SevenZipArchiveEntry`](../) exemple.

### Exemples

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Voir également

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Assemblée [Aspose.Zip](../../../)


