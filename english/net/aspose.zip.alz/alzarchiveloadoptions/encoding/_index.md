---
title: AlzArchiveLoadOptions.Encoding
second_title: Aspose.ZIP for .NET API Reference
description: AlzArchiveLoadOptions property. Gets or sets the encoding for entries names. Default is Korean Windows code page 949 CP949
type: docs
weight: 40
url: /net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Gets or sets the encoding for entries' names. Default is Korean Windows code page 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Remarks

ALZ archives historically store file names using the Korean Windows ANSI code page.

## Examples

Entry name composed using specified encoding.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### See Also

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


