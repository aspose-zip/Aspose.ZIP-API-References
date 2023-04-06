---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveLoadOptions fast egendom. Hämtar eller ställer in kodningen för posternas namn.
type: docs
weight: 30
url: /sv/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Hämtar eller ställer in kodningen för posternas namn.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

Postens namn sammansatt med angiven kodning oavsett zip-filens egenskaper.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Se även

* class [ArchiveLoadOptions](../)
* namnutrymme [Aspose.Zip](../../archiveloadoptions/)
* hopsättning [Aspose.Zip](../../../)


