---
title: ArjArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Reference
description: ArjArchive method. Extracts all entries to the specified directory
type: docs
weight: 60
url: /net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Thrown when the *destinationDirectory* is null. |

## Examples

The following example shows how to extract all entries to a directory:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [ArjArchive](../)
* namespace [Aspose.Zip.ARJ](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


