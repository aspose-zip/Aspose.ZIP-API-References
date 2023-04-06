---
title: ArchiveLoadOptions.Encoding
second_title: Riferimento API Aspose.ZIP per .NET
description: ArchiveLoadOptions proprietà. Ottiene o imposta la codifica per i nomi delle voci.
type: docs
weight: 30
url: /it/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Ottiene o imposta la codifica per i nomi delle voci.

```csharp
public Encoding Encoding { get; set; }
```

### Esempi

Nome della voce composto utilizzando la codifica specificata indipendentemente dalle proprietà del file zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Guarda anche

* class [ArchiveLoadOptions](../)
* spazio dei nomi [Aspose.Zip](../../archiveloadoptions/)
* assemblea [Aspose.Zip](../../../)


