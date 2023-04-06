---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveLoadOptions eigendom. Haalt de codering voor de namen van ingangen op of stelt deze in.
type: docs
weight: 30
url: /nl/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Haalt de codering voor de namen van ingangen op of stelt deze in.

```csharp
public Encoding Encoding { get; set; }
```

### Voorbeelden

Itemnaam samengesteld met behulp van opgegeven codering, ongeacht de eigenschappen van het zipbestand.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Zie ook

* class [ArchiveLoadOptions](../)
* naamruimte [Aspose.Zip](../../archiveloadoptions/)
* montage [Aspose.Zip](../../../)


