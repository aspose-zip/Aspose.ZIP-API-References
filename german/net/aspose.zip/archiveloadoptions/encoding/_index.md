---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveLoadOptions eigendom. Ruft die Codierung für die Namen der Einträge ab oder legt sie fest.
type: docs
weight: 30
url: /de/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Ruft die Codierung für die Namen der Einträge ab oder legt sie fest.

```csharp
public Encoding Encoding { get; set; }
```

### Beispiele

Eintragsname, der unabhängig von den Eigenschaften der ZIP-Datei unter Verwendung der angegebenen Codierung zusammengesetzt ist.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Siehe auch

* class [ArchiveLoadOptions](../)
* namensraum [Aspose.Zip](../../archiveloadoptions/)
* Montage [Aspose.Zip](../../../)


