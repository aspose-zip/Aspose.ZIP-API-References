---
title: IsoArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive method. Extracts all entries to the specified directory
type: docs
weight: 70
url: /net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Extracts all entries to the specified directory.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The directory to extract the entries to. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Thrown when the archive is in editing mode. |
| ArgumentNullException | Thrown when the *destinationDirectory* is null. |

## Examples

The following example shows how to extract all entries to a directory:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


