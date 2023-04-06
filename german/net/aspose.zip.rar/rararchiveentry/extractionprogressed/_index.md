---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: RarArchiveEntry evenement. Wird ausgelöst wenn ein Teil des Rohdatenstroms extrahiert wird.
type: docs
weight: 80
url: /de/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Wird ausgelöst, wenn ein Teil des Rohdatenstroms extrahiert wird.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### Bemerkungen

Ereignissender ist ein[`RarArchiveEntry`](../) Beispiel.

### Beispiele

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namensraum [Aspose.Zip.Rar](../../rararchiveentry/)
* Montage [Aspose.Zip](../../../)


