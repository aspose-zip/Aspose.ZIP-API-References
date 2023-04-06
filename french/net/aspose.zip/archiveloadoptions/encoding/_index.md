---
title: ArchiveLoadOptions.Encoding
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveLoadOptions propriété. Obtient ou définit lencodage des noms des entrées.
type: docs
weight: 30
url: /fr/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Obtient ou définit l'encodage des noms des entrées.

```csharp
public Encoding Encoding { get; set; }
```

### Exemples

Nom d'entrée composé à l'aide de l'encodage spécifié, quelles que soient les propriétés du fichier zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Voir également

* class [ArchiveLoadOptions](../)
* espace de noms [Aspose.Zip](../../archiveloadoptions/)
* Assemblée [Aspose.Zip](../../../)


