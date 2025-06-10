---
title: IsoArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive method. Extracts all entries to the specified directory
type: docs
weight: 60
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
| OperationCanceledException | In .NET Framework 4.0 and above: Thrown when the extraction is canceled via the provided cancellation token. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

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


