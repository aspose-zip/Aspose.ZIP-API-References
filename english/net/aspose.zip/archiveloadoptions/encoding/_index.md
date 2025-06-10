---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveLoadOptions property. Gets or sets the encoding for entries names
type: docs
weight: 40
url: /net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Gets or sets the encoding for entries' names.

```csharp
public Encoding Encoding { get; set; }
```

## Examples

Entry name composed using specified encoding regardless of zip file properties.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (var archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### See Also

* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


